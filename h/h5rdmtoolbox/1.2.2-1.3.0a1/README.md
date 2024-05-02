# Comparing `tmp/h5rdmtoolbox-1.2.2.tar.gz` & `tmp/h5rdmtoolbox-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5rdmtoolbox-1.2.2.tar", last modified: Thu Jan  4 12:52:28 2024, max compression
+gzip compressed data, was "h5rdmtoolbox-1.3.0a1.tar", last modified: Thu May  2 12:07:38 2024, max compression
```

## Comparing `h5rdmtoolbox-1.2.2.tar` & `h5rdmtoolbox-1.3.0a1.tar`

### file list

```diff
@@ -1,167 +1,165 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.585860 h5rdmtoolbox-1.2.2/
--rw-rw-rw-   0        0        0     1090 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/LICENSE
--rw-rw-rw-   0        0        0    14016 2024-01-04 12:52:28.583861 h5rdmtoolbox-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     8874 2024-01-04 12:29:17.000000 h5rdmtoolbox-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.264491 h5rdmtoolbox-1.2.2/h5rdmtoolbox/
--rw-rw-rw-   0        0        0     6013 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/__init__.py
--rw-rw-rw-   0        0        0     3784 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/_cfg.py
--rw-rw-rw-   0        0        0    21219 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/_repr.py
--rw-rw-rw-   0        0        0     4045 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/_user.py
--rw-rw-rw-   0        0        0      232 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/_version.py
--rw-rw-rw-   0        0        0      129 2023-04-05 11:22:04.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/cache.py
--rw-rw-rw-   0        0        0      274 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/consts.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.319062 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/
--rw-rw-rw-   0        0        0      991 2024-01-02 07:36:55.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/__init__.py
--rw-rw-rw-   0        0        0     1234 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/_h5tbx.py
--rw-rw-rw-   0        0        0    12879 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/_m4i_namespace.py
--rw-rw-rw-   0        0        0     2848 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/_obo_namespace.py
--rw-rw-rw-   0        0        0       56 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/cfg.py
--rw-rw-rw-   0        0        0      775 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/consts.py
--rw-rw-rw-   0        0        0    31920 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/core.py
--rw-rw-rw-   0        0        0     1026 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/errors.py
--rw-rw-rw-   0        0        0    17617 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/generate.py
--rw-rw-rw-   0        0        0      417 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/references.py
--rw-rw-rw-   0        0        0    17103 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_attributes.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.339875 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/
--rw-rw-rw-   0        0        0     2084 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/__init__.py
--rw-rw-rw-   0        0        0     4726 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/accessor.py
--rw-rw-rw-   0        0        0    13103 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/affixes.py
--rw-rw-rw-   0        0        0       51 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/cache.py
--rw-rw-rw-   0        0        0      469 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/consts.py
--rw-rw-rw-   0        0        0     6665 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/h5interface.py
--rw-rw-rw-   0        0        0     4808 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/name.py
--rw-rw-rw-   0        0        0    36812 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/table.py
--rw-rw-rw-   0        0        0    10035 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/transformation.py
--rw-rw-rw-   0        0        0     2315 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/utils.py
--rw-rw-rw-   0        0        0     8863 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/toolbox_validators.py
--rw-rw-rw-   0        0        0     7428 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/utils.py
--rw-rw-rw-   0        0        0      146 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/warnings.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.354533 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/
--rw-rw-rw-   0        0        0      291 2023-03-31 12:21:41.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/fluid-v1.yml
--rw-rw-rw-   0        0        0      717 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/h5tbx.yaml
--rw-rw-rw-   0        0        0     1064 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/piv-v1.yml
--rw-rw-rw-   0        0        0     3135 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/style.css
--rw-rw-rw-   0        0        0     2532 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/tutorial_convention.yaml
--rw-rw-rw-   0        0        0     2558 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/tutorial_standard_name_table.yaml
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.361536 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/
--rw-rw-rw-   0        0        0      283 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.375926 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/
--rw-rw-rw-   0        0        0      197 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/__init__.py
--rw-rw-rw-   0        0        0     4053 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/filedb.py
--rw-rw-rw-   0        0        0      554 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/nonsearchable.py
--rw-rw-rw-   0        0        0    17495 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/objdb.py
--rw-rw-rw-   0        0        0     2576 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/query.py
--rw-rw-rw-   0        0        0     1745 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/utils.py
--rw-rw-rw-   0        0        0     7371 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/lazy.py
--rw-rw-rw-   0        0        0    14721 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/mongo.py
--rw-rw-rw-   0        0        0     1589 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/template.py
--rw-rw-rw-   0        0        0      123 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/errors.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.403952 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/
--rw-rw-rw-   0        0        0        0 2023-03-27 13:37:37.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/__init__.py
--rw-rw-rw-   0        0        0        0 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/dataset.py
--rw-rw-rw-   0        0        0     6054 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/ipyvolume.py
--rw-rw-rw-   0        0        0     3169 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/magnitude.py
--rw-rw-rw-   0        0        0     7774 2023-12-24 12:29:36.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/normalize.py
--rw-rw-rw-   0        0        0     3305 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/scatterhist.py
--rw-rw-rw-   0        0        0      911 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/units.py
--rw-rw-rw-   0        0        0     3177 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/extensions/vector.py
--rw-rw-rw-   0        0        0     1245 2023-03-09 20:20:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/hdfgui.py
--rw-rw-rw-   0        0        0     8597 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/identifiers.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.406863 h5rdmtoolbox-1.2.2/h5rdmtoolbox/layout/
--rw-rw-rw-   0        0        0       50 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/layout/__init__.py
--rw-rw-rw-   0        0        0    11939 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/layout/core.py
--rw-rw-rw-   0        0        0      384 2024-01-04 12:29:17.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/namespace.py
--rw-rw-rw-   0        0        0     6546 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/plotting.py
--rw-rw-rw-   0        0        0      290 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/protected_attributes.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.421114 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/
--rw-rw-rw-   0        0        0      337 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/h5metamapper.py
--rw-rw-rw-   0        0        0     1656 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/interface.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.432231 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/
--rw-rw-rw-   0        0        0      222 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/__init__.py
--rw-rw-rw-   0        0        0    12313 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/core.py
--rw-rw-rw-   0        0        0     5921 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/metadata.py
--rw-rw-rw-   0        0        0     2380 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/tokens.py
--rw-rw-rw-   0        0        0      610 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/utils.py
--rw-rw-rw-   0        0        0    15640 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/tutorial.py
--rw-rw-rw-   0        0        0    20001 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/utils.py
--rw-rw-rw-   0        0        0      101 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/warnings.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.453335 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/
--rw-rw-rw-   0        0        0      170 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/__init__.py
--rw-rw-rw-   0        0        0     2347 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/accessory.py
--rw-rw-rw-   0        0        0    94313 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/core.py
--rw-rw-rw-   0        0        0     3981 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/ds_decoder.py
--rw-rw-rw-   0        0        0    11810 2024-01-04 12:45:23.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/h5attr.py
--rw-rw-rw-   0        0        0      465 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/h5ext.py
--rw-rw-rw-   0        0        0      903 2023-12-29 13:39:56.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/h5utils.py
--rw-rw-rw-   0        0        0     2566 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/h5yaml.py
--rw-rw-rw-   0        0        0     5972 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/iri.py
--rw-rw-rw-   0        0        0     4298 2024-01-04 12:46:47.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/jsonld.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.470755 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/
--rw-rw-rw-   0        0        0       24 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/__init__.py
--rw-rw-rw-   0        0        0     6276 2024-01-04 12:29:17.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/_build.py
--rw-rw-rw-   0        0        0     4634 2024-01-04 12:29:17.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/_codemeta_namespace.py
--rw-rw-rw-   0        0        0    13013 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/_m4i_namespace.py
--rw-rw-rw-   0        0        0     2880 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/_obo_namespace.py
--rw-rw-rw-   0        0        0  1912672 2024-01-03 15:22:46.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/_qudt_quantitykind_namespace.py
--rw-rw-rw-   0        0        0  1840786 2024-01-03 15:22:42.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/namespaces/_qudt_unit_namespace.py
--rw-rw-rw-   0        0        0     4620 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/xr2hdf.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.575339 h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/
--rw-rw-rw-   0        0        0    14016 2024-01-04 12:52:28.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5089 2024-01-04 12:52:28.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 12:52:28.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      896 2024-01-04 12:52:28.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-01-04 12:52:28.000000 h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-03-08 18:17:38.000000 h5rdmtoolbox-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0     2454 2024-01-04 12:52:28.587863 h5rdmtoolbox-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-09-27 08:03:12.000000 h5rdmtoolbox-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.501330 h5rdmtoolbox-1.2.2/tests/
--rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.2.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1107 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/clean_zenodo_sandbox.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.509814 h5rdmtoolbox-1.2.2/tests/conventions/
--rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.2.2/tests/conventions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.517330 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/
--rw-rw-rw-   0        0        0        0 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.526879 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/
--rw-rw-rw-   0        0        0        0 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/__init__.py
--rw-rw-rw-   0        0        0     6467 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_interface.py
--rw-rw-rw-   0        0        0     6827 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_provenance.py
--rw-rw-rw-   0        0        0    11980 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_snt.py
--rw-rw-rw-   0        0        0    13236 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py
--rw-rw-rw-   0        0        0     1224 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/test_standard_attributes.py
--rw-rw-rw-   0        0        0    13045 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/test_standard_names.py
--rw-rw-rw-   0        0        0    32242 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/tests/conventions/test_conventions.py
--rw-rw-rw-   0        0        0      548 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/test_references.py
--rw-rw-rw-   0        0        0     4786 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/test_toolbox_validators.py
--rw-rw-rw-   0        0        0     5060 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/conventions/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.537565 h5rdmtoolbox-1.2.2/tests/database/
--rw-rw-rw-   0        0        0        0 2023-12-12 15:09:30.000000 h5rdmtoolbox-1.2.2/tests/database/__init__.py
--rw-rw-rw-   0        0        0    13567 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/database/notest_mongo_old.py
--rw-rw-rw-   0        0        0    12049 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/database/test_hdfDB.py
--rw-rw-rw-   0        0        0     4632 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/database/test_mongo.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.540603 h5rdmtoolbox-1.2.2/tests/layouts/
--rw-rw-rw-   0        0        0        0 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/layouts/__init__.py
--rw-rw-rw-   0        0        0     4192 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/layouts/test_core.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.548159 h5rdmtoolbox-1.2.2/tests/repository/
--rw-rw-rw-   0        0        0        0 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/repository/__init__.py
--rw-rw-rw-   0        0        0     2720 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/repository/test_metadatamapper.py
--rw-rw-rw-   0        0        0    16454 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/tests/repository/test_zenodo.py
--rw-rw-rw-   0        0        0     2679 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/tests/test_config.py
--rw-rw-rw-   0        0        0    11786 2023-12-24 12:29:36.000000 h5rdmtoolbox-1.2.2/tests/test_extensions.py
--rw-rw-rw-   0        0        0     3389 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/test_identifiers.py
--rw-rw-rw-   0        0        0      829 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/test_logger.py
--rw-rw-rw-   0        0        0     6930 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/test_plotting.py
--rw-rw-rw-   0        0        0     3311 2023-12-17 17:23:56.000000 h5rdmtoolbox-1.2.2/tests/test_repr.py
--rw-rw-rw-   0        0        0     2001 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/test_user.py
--rw-rw-rw-   0        0        0     4499 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/tests/test_utils.py
--rw-rw-rw-   0        0        0      868 2023-12-26 18:15:20.000000 h5rdmtoolbox-1.2.2/tests/test_version.py
--rw-rw-rw-   0        0        0     1169 2023-12-24 12:29:36.000000 h5rdmtoolbox-1.2.2/tests/test_xarray_export.py
-drwxrwxrwx   0        0        0        0 2024-01-04 12:52:28.573331 h5rdmtoolbox-1.2.2/tests/wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.2.2/tests/wrapper/__init__.py
--rw-rw-rw-   0        0        0    35658 2024-01-02 16:53:25.000000 h5rdmtoolbox-1.2.2/tests/wrapper/test_core.py
--rw-rw-rw-   0        0        0      615 2023-04-05 11:22:04.000000 h5rdmtoolbox-1.2.2/tests/wrapper/test_dump.py
--rw-rw-rw-   0        0        0    22734 2024-01-04 12:42:15.000000 h5rdmtoolbox-1.2.2/tests/wrapper/test_file.py
--rw-rw-rw-   0        0        0      829 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/tests/wrapper/test_h5ext.py
--rw-rw-rw-   0        0        0     4251 2024-01-04 12:29:17.000000 h5rdmtoolbox-1.2.2/tests/wrapper/test_namespaces.py
--rw-rw-rw-   0        0        0     1360 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.2.2/tests/wrapper/test_xr2df.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.722196 h5rdmtoolbox-1.3.0a1/
+-rw-rw-rw-   0        0        0     1090 2024-04-22 14:41:40.000000 h5rdmtoolbox-1.3.0a1/LICENSE
+-rw-rw-rw-   0        0        0    14625 2024-05-02 12:07:38.721208 h5rdmtoolbox-1.3.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     9172 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.300527 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/
+-rw-rw-rw-   0        0        0     9533 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/__init__.py
+-rw-rw-rw-   0        0        0     3913 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_cfg.py
+-rw-rw-rw-   0        0        0    26542 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_repr.py
+-rw-rw-rw-   0        0        0     5257 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_user.py
+-rw-rw-rw-   0        0        0      232 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_version.py
+-rw-rw-rw-   0        0        0     1621 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/cli.py
+-rw-rw-rw-   0        0        0       94 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/consts.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.345535 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/
+-rw-rw-rw-   0        0        0     1402 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/__init__.py
+-rw-rw-rw-   0        0        0       56 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/cfg.py
+-rw-rw-rw-   0        0        0      775 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/consts.py
+-rw-rw-rw-   0        0        0    31958 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/core.py
+-rw-rw-rw-   0        0        0      988 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/definition.py
+-rw-rw-rw-   0        0        0     1026 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/errors.py
+-rw-rw-rw-   0        0        0    17349 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/generate.py
+-rw-rw-rw-   0        0        0     2724 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/hdf_ontology.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.352535 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/
+-rw-rw-rw-   0        0        0      150 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/__init__.py
+-rw-rw-rw-   0        0        0     1308 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/h5namespace.py
+-rw-rw-rw-   0        0        0     1445 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/h5ontocls.py
+-rw-rw-rw-   0        0        0      417 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/references.py
+-rw-rw-rw-   0        0        0    17167 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_attributes.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.405058 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/
+-rw-rw-rw-   0        0        0     2125 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/__init__.py
+-rw-rw-rw-   0        0        0     4726 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/accessor.py
+-rw-rw-rw-   0        0        0    13103 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/affixes.py
+-rw-rw-rw-   0        0        0       51 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/cache.py
+-rw-rw-rw-   0        0        0      469 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/consts.py
+-rw-rw-rw-   0        0        0     6662 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/h5interface.py
+-rw-rw-rw-   0        0        0     4808 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/name.py
+-rw-rw-rw-   0        0        0    35542 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/table.py
+-rw-rw-rw-   0        0        0    10035 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/transformation.py
+-rw-rw-rw-   0        0        0     2354 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/utils.py
+-rw-rw-rw-   0        0        0     8680 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/toolbox_validators.py
+-rw-rw-rw-   0        0        0     7428 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/utils.py
+-rw-rw-rw-   0        0        0      146 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/warnings.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.471603 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/
+-rw-rw-rw-   0        0        0     1084 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/def_icon.png
+-rw-rw-rw-   0        0        0     1070 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/fluid-v1.yml
+-rw-rw-rw-   0        0        0      717 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/h5tbx.yaml
+-rw-rw-rw-   0        0        0     2587 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/id_icon.png
+-rw-rw-rw-   0        0        0     3340 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/iri_icon.png
+-rw-rw-rw-   0        0        0     1064 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/piv-v1.yml
+-rw-rw-rw-   0        0        0     3651 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/style.css
+-rw-rw-rw-   0        0        0     2532 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_convention.yaml
+-rw-rw-rw-   0        0        0     2558 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_standard_name_table.yaml
+-rw-rw-rw-   0        0        0     3287 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/type_icon.png
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.499606 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/
+-rw-rw-rw-   0        0        0     3170 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.513607 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/
+-rw-rw-rw-   0        0        0      107 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/__init__.py
+-rw-rw-rw-   0        0        0     4727 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/filedb.py
+-rw-rw-rw-   0        0        0    21521 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/objdb.py
+-rw-rw-rw-   0        0        0     2697 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/query.py
+-rw-rw-rw-   0        0        0     1933 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/utils.py
+-rw-rw-rw-   0        0        0     2156 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/interface.py
+-rw-rw-rw-   0        0        0    14802 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/mongo.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/dev.py
+-rw-rw-rw-   0        0        0      123 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.525612 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/
+-rw-rw-rw-   0        0        0        0 2023-03-27 13:37:37.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2507 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/magnitude.py
+-rw-rw-rw-   0        0        0     4045 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/normalize.py
+-rw-rw-rw-   0        0        0     1903 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/units.py
+-rw-rw-rw-   0        0        0     4872 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/vector.py
+-rw-rw-rw-   0        0        0     8675 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/identifiers.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.530609 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/layout/
+-rw-rw-rw-   0        0        0       50 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/layout/__init__.py
+-rw-rw-rw-   0        0        0    24988 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/layout/core.py
+-rw-rw-rw-   0        0        0     6546 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/plotting.py
+-rw-rw-rw-   0        0        0      290 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/protected_attributes.py
+-rw-rw-rw-   0        0        0     5282 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/protocols.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.533609 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/
+-rw-rw-rw-   0        0        0      337 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/__init__.py
+-rw-rw-rw-   0        0        0     2039 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/interface.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.545621 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/
+-rw-rw-rw-   0        0        0      222 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/__init__.py
+-rw-rw-rw-   0        0        0    16277 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/core.py
+-rw-rw-rw-   0        0        0     7647 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/metadata.py
+-rw-rw-rw-   0        0        0     3533 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/tokens.py
+-rw-rw-rw-   0        0        0      610 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/utils.py
+-rw-rw-rw-   0        0        0    15780 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/tutorial.py
+-rw-rw-rw-   0        0        0    21187 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/utils.py
+-rw-rw-rw-   0        0        0      101 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/warnings.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.572663 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/
+-rw-rw-rw-   0        0        0       99 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     3106 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/accessor.py
+-rw-rw-rw-   0        0        0    96947 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/core.py
+-rw-rw-rw-   0        0        0     4027 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/ds_decoder.py
+-rw-rw-rw-   0        0        0    18622 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5attr.py
+-rw-rw-rw-   0        0        0      465 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5ext.py
+-rw-rw-rw-   0        0        0      899 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5utils.py
+-rw-rw-rw-   0        0        0     4047 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5yaml.py
+-rw-rw-rw-   0        0        0    42227 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/jsonld.py
+-rw-rw-rw-   0        0        0     6241 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/lazy.py
+-rw-rw-rw-   0        0        0    17291 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/rdf.py
+-rw-rw-rw-   0        0        0     4582 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/xr2hdf.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.710194 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/
+-rw-rw-rw-   0        0        0    14625 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4872 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      976 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-03-08 18:17:38.000000 h5rdmtoolbox-1.3.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0     2271 2024-05-02 12:07:38.724196 h5rdmtoolbox-1.3.0a1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-09-27 08:03:12.000000 h5rdmtoolbox-1.3.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.595663 h5rdmtoolbox-1.3.0a1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1013 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/clean_zenodo_sandbox.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.616660 h5rdmtoolbox-1.3.0a1/tests/conventions/
+-rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.624662 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/
+-rw-rw-rw-   0        0        0        0 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.660187 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/
+-rw-rw-rw-   0        0        0        0 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/__init__.py
+-rw-rw-rw-   0        0        0     6464 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_interface.py
+-rw-rw-rw-   0        0        0     6827 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_provenance.py
+-rw-rw-rw-   0        0        0    13348 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_snt.py
+-rw-rw-rw-   0        0        0    13236 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py
+-rw-rw-rw-   0        0        0     2503 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_attributes.py
+-rw-rw-rw-   0        0        0    13045 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_names.py
+-rw-rw-rw-   0        0        0    30934 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_conventions.py
+-rw-rw-rw-   0        0        0     2051 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_engmeta.py
+-rw-rw-rw-   0        0        0     8450 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_ontology.py
+-rw-rw-rw-   0        0        0      548 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_references.py
+-rw-rw-rw-   0        0        0     5094 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_toolbox_validators.py
+-rw-rw-rw-   0        0        0     5060 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.670187 h5rdmtoolbox-1.3.0a1/tests/database/
+-rw-rw-rw-   0        0        0        0 2023-12-12 15:09:30.000000 h5rdmtoolbox-1.3.0a1/tests/database/__init__.py
+-rw-rw-rw-   0        0        0     1252 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/database/test_find_rdf.py
+-rw-rw-rw-   0        0        0    25285 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/database/test_hdfDB.py
+-rw-rw-rw-   0        0        0     9625 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/database/test_mongo.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.677187 h5rdmtoolbox-1.3.0a1/tests/layouts/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/layouts/__init__.py
+-rw-rw-rw-   0        0        0    12712 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/layouts/test_core.py
+-rw-rw-rw-   0        0        0     2282 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/layouts/test_docs.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.681208 h5rdmtoolbox-1.3.0a1/tests/repository/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/repository/__init__.py
+-rw-rw-rw-   0        0        0    18963 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/repository/test_zenodo.py
+-rw-rw-rw-   0        0        0     2679 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/tests/test_config.py
+-rw-rw-rw-   0        0        0     6015 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_extensions.py
+-rw-rw-rw-   0        0        0     4243 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_identifiers.py
+-rw-rw-rw-   0        0        0     6930 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     5035 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_repr.py
+-rw-rw-rw-   0        0        0     4079 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_user.py
+-rw-rw-rw-   0        0        0     4604 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_utils.py
+-rw-rw-rw-   0        0        0      798 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/test_version.py
+-rw-rw-rw-   0        0        0     1169 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/tests/test_xarray_export.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.707191 h5rdmtoolbox-1.3.0a1/tests/wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/__init__.py
+-rw-rw-rw-   0        0        0    43471 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_core.py
+-rw-rw-rw-   0        0        0     2020 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_dump.py
+-rw-rw-rw-   0        0        0    16978 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_file.py
+-rw-rw-rw-   0        0        0      829 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_h5ext.py
+-rw-rw-rw-   0        0        0    20791 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_jsonld.py
+-rw-rw-rw-   0        0        0     1930 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_lazy.py
+-rw-rw-rw-   0        0        0     1629 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_namespaces.py
+-rw-rw-rw-   0        0        0    18383 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_rdf.py
+-rw-rw-rw-   0        0        0     1360 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_xr2df.py
```

### Comparing `h5rdmtoolbox-1.2.2/LICENSE` & `h5rdmtoolbox-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/PKG-INFO` & `h5rdmtoolbox-1.3.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5rdmtoolbox
-Version: 1.2.2
+Version: 1.3.0a1
 Summary: Supporting a FAIR Research Data lifecycle using Python and HDF5.
 Home-page: https://h5rdmtoolbox.readthedocs.io/en/latest/
 Author: Matthias Probst
 Author-email: matthias.probst@kit.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,27 +25,32 @@
 Requires-Dist: IPython>=7.34.0
 Requires-Dist: pyyaml>6.0
 Requires-Dist: xarray>=2022.3.0
 Requires-Dist: pint==0.21.1
 Requires-Dist: pint_xarray
 Requires-Dist: regex
 Requires-Dist: packaging
+Requires-Dist: ontolutils>=0.2.20
 Requires-Dist: python-forge
 Requires-Dist: requests
 Requires-Dist: pydantic>=2.3.0
 Requires-Dist: rdflib
 Provides-Extra: database
 Requires-Dist: pymongo; extra == "database"
+Provides-Extra: layout-validation
+Requires-Dist: tabulate; extra == "layout-validation"
 Provides-Extra: csv
 Requires-Dist: pandas; extra == "csv"
 Provides-Extra: snt
 Requires-Dist: xmltodict; extra == "snt"
 Requires-Dist: tabulate; extra == "snt"
 Requires-Dist: python-gitlab; extra == "snt"
 Requires-Dist: pypandoc; extra == "snt"
+Provides-Extra: gui
+Requires-Dist: PyQt5; extra == "gui"
 Provides-Extra: test
 Requires-Dist: pytest>=7.1.2; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: xmltodict; extra == "test"
 Requires-Dist: scipy; extra == "test"
 Requires-Dist: pandas; extra == "test"
@@ -78,15 +83,17 @@
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: scikit-image; extra == "docs"
 Requires-Dist: scikit-learn; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: simplejson; extra == "docs"
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: kglab; extra == "docs"
 Provides-Extra: complete
+Requires-Dist: PyQt5; extra == "complete"
 Requires-Dist: pytest>=7.1.2; extra == "complete"
 Requires-Dist: pytest-cov; extra == "complete"
 Requires-Dist: pylint; extra == "complete"
 Requires-Dist: xmltodict; extra == "complete"
 Requires-Dist: scipy; extra == "complete"
 Requires-Dist: pandas; extra == "complete"
 Requires-Dist: xmltodict; extra == "complete"
@@ -117,36 +124,37 @@
 Requires-Dist: sphinx-copybutton; extra == "complete"
 Requires-Dist: scikit-image; extra == "complete"
 Requires-Dist: scikit-learn; extra == "complete"
 Requires-Dist: sphinx-design; extra == "complete"
 Requires-Dist: simplejson; extra == "complete"
 Requires-Dist: myst-nb; extra == "complete"
 Requires-Dist: sphinxcontrib-bibtex; extra == "complete"
+Requires-Dist: kglab; extra == "complete"
 
 # HDF5 Research Data Management Toolbox
 
 ![Tests](https://github.com/matthiasprobst/h5RDMtoolbox/actions/workflows/tests.yml/badge.svg)
 ![DOCS](https://codecov.io/gh/matthiasprobst/h5RDMtoolbox/branch/dev/graph/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/h5rdmtoolbox/badge/?version=latest)](https://h5rdmtoolbox.readthedocs.io/en/latest/?badge=latest)
 ![pyvers](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 
 *Note, that the project is still under development!*
 
-The "HDF5 Research Data Management Toolbox" (h5RDMtoolbox) is a python package supporting everybody who is working with
+The "HDF5 Research Data Management Toolbox" (h5RDMtoolbox) is a Python package supporting everybody who is working with
 HDF5 to achieve a sustainable data lifecycle which follows
 the [FAIR (Findable, Accessible, Interoperable, Reusable)](https://www.nature.com/articles/sdata201618)
 principles. It specifically supports the five main steps of *planning*, *collecting*, *analyzing*, *sharing* and
 *reusing* data. Please visit the [documentation](https://h5rdmtoolbox.readthedocs.io/en/latest/) for detailed
 information of try the [quickstart using colab](#quickstart).
 
 ## Highlights
 
 - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to allow easy access to metadata and data during
   analysis and processing (
-  see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface).
+  see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface)).
 - Assigning [metadata with "globally unique and persistent identifiers"]() as required
   by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/)
   . This "remove[s] ambiguity in the meaning of your published data...".
 - Define standard attributes through
   [conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/convention/index.html) and enforce users to use
   them
 - Upload HDF5 files directly
@@ -254,17 +262,21 @@
 - `h5py=3.7.0`: HDF5 file interface
 - `xarray>=2022.3.0`: Working with scientific arrays in combination with attributes. Allows carrying metadata from HDF5
   to user
 - `pint>=0.19.2`: Allows working with units
 - `pint_xarray>=0.2.1`: Working with units for usage with xarray
 - `python-forge==18.6.0`: Used to update function signatures when using
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
+- `pydantic`: Used to validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
 - `pyyaml>6.0.0`: Reading and writing of yaml files, e.g. metadata definitions (conventions). Note, lower versions
   collide with python 3.11
 - `requests`: Used to download files from the internet or validate URLs, e.g. metadata definitions (conventions)
+- `rdflib`: Used to enable working with RDF
+- `ontolutils`: Required to work with RDF and derive semantic description of HDF5 file content
+
 
 #### Optional dependencies
 
 To run unit tests or to enable certain features, additional dependencies must be installed.
 
 Install optional dependencies by specifying them in square brackets after the package name, e.g.:
```

### Comparing `h5rdmtoolbox-1.2.2/README.md` & `h5rdmtoolbox-1.3.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 ![Tests](https://github.com/matthiasprobst/h5RDMtoolbox/actions/workflows/tests.yml/badge.svg)
 ![DOCS](https://codecov.io/gh/matthiasprobst/h5RDMtoolbox/branch/dev/graph/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/h5rdmtoolbox/badge/?version=latest)](https://h5rdmtoolbox.readthedocs.io/en/latest/?badge=latest)
 ![pyvers](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 
 *Note, that the project is still under development!*
 
-The "HDF5 Research Data Management Toolbox" (h5RDMtoolbox) is a python package supporting everybody who is working with
+The "HDF5 Research Data Management Toolbox" (h5RDMtoolbox) is a Python package supporting everybody who is working with
 HDF5 to achieve a sustainable data lifecycle which follows
 the [FAIR (Findable, Accessible, Interoperable, Reusable)](https://www.nature.com/articles/sdata201618)
 principles. It specifically supports the five main steps of *planning*, *collecting*, *analyzing*, *sharing* and
 *reusing* data. Please visit the [documentation](https://h5rdmtoolbox.readthedocs.io/en/latest/) for detailed
 information of try the [quickstart using colab](#quickstart).
 
 ## Highlights
 
 - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to allow easy access to metadata and data during
   analysis and processing (
-  see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface).
+  see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface)).
 - Assigning [metadata with "globally unique and persistent identifiers"]() as required
   by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/)
   . This "remove[s] ambiguity in the meaning of your published data...".
 - Define standard attributes through
   [conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/convention/index.html) and enforce users to use
   them
 - Upload HDF5 files directly
@@ -130,17 +130,21 @@
 - `h5py=3.7.0`: HDF5 file interface
 - `xarray>=2022.3.0`: Working with scientific arrays in combination with attributes. Allows carrying metadata from HDF5
   to user
 - `pint>=0.19.2`: Allows working with units
 - `pint_xarray>=0.2.1`: Working with units for usage with xarray
 - `python-forge==18.6.0`: Used to update function signatures when using
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
+- `pydantic`: Used to validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
 - `pyyaml>6.0.0`: Reading and writing of yaml files, e.g. metadata definitions (conventions). Note, lower versions
   collide with python 3.11
 - `requests`: Used to download files from the internet or validate URLs, e.g. metadata definitions (conventions)
+- `rdflib`: Used to enable working with RDF
+- `ontolutils`: Required to work with RDF and derive semantic description of HDF5 file content
+
 
 #### Optional dependencies
 
 To run unit tests or to enable certain features, additional dependencies must be installed.
 
 Install optional dependencies by specifying them in square brackets after the package name, e.g.:
```

#### html2text {}

```diff
@@ -2,25 +2,25 @@
 matthiasprobst/h5RDMtoolbox/actions/workflows/tests.yml/badge.svg) ![DOCS]
 (https://codecov.io/gh/matthiasprobst/h5RDMtoolbox/branch/dev/graph/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/h5rdmtoolbox/badge/
 ?version=latest)](https://h5rdmtoolbox.readthedocs.io/en/latest/?badge=latest)
 ![pyvers](https://img.shields.io/badge/python-
 3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue) *Note, that the
 project is still under development!* The "HDF5 Research Data Management
-Toolbox" (h5RDMtoolbox) is a python package supporting everybody who is working
+Toolbox" (h5RDMtoolbox) is a Python package supporting everybody who is working
 with HDF5 to achieve a sustainable data lifecycle which follows the [FAIR
 (Findable, Accessible, Interoperable, Reusable)](https://www.nature.com/
 articles/sdata201618) principles. It specifically supports the five main steps
 of *planning*, *collecting*, *analyzing*, *sharing* and *reusing* data. Please
 visit the [documentation](https://h5rdmtoolbox.readthedocs.io/en/latest/) for
 detailed information of try the [quickstart using colab](#quickstart). ##
 Highlights - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to
 allow easy access to metadata and data during analysis and processing ( see
 [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/
-quickoverview.html#datasets-xarray-interface). - Assigning [metadata with
+quickoverview.html#datasets-xarray-interface)). - Assigning [metadata with
 "globally unique and persistent identifiers"]() as required by [F1 of the FAIR
 principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-
 globally-unique-persistent-identifiers/) . This "remove[s] ambiguity in the
 meaning of your published data...". - Define standard attributes through
 [conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/
 convention/index.html) and enforce users to use them - Upload HDF5 files
 directly to [repositories](https://h5rdmtoolbox.readthedocs.io/en/latest/
@@ -80,33 +80,37 @@
 Working with regular expressions **Specific to the package are ...** -
 `h5py=3.7.0`: HDF5 file interface - `xarray>=2022.3.0`: Working with scientific
 arrays in combination with attributes. Allows carrying metadata from HDF5 to
 user - `pint>=0.19.2`: Allows working with units - `pint_xarray>=0.2.1`:
 Working with units for usage with xarray - `python-forge==18.6.0`: Used to
 update function signatures when using the [standard attributes](https://
 h5rdmtoolbox.readthedocs.io/en/latest/conventions/
-standard_attributes_and_conventions.html) - `pyyaml>6.0.0`: Reading and writing
-of yaml files, e.g. metadata definitions (conventions). Note, lower versions
-collide with python 3.11 - `requests`: Used to download files from the internet
-or validate URLs, e.g. metadata definitions (conventions) #### Optional
-dependencies To run unit tests or to enable certain features, additional
-dependencies must be installed. Install optional dependencies by specifying
-them in square brackets after the package name, e.g.: pip install h5RDMtoolbox
-[mongodb] [mongodb] - `pymongo>=4.2.0`: Database solution for HDF5 files [csv]
-- `pandas>=1.4.3`: Mainly used for reading csv and pretty printing [snt] -
-`xmltodict`: Reading of xml files - `tabulate>=0.8.10`: Pretty printing of
-tables - `python-gitlab`: Access to gitlab repositories - `pypandoc>=2.3`:
-Conversion of markdown files to html ## Citing the package If you intend to use
-the package in your work, you may cite the paper in the journal [inggrid]
-(https://preprints.inggrid.org/repository/view/23/) Here's the bibtext to it:
-``` @article{probst2023h5rdmtoolbox, title={h5RDMtoolbox-A Python Toolbox for
-FAIR Data Management around HDF5}, author={Probst, Matthias and Pritz, Balazs},
-year={2023}, publisher={ing. grid Preprint Repository} } ``` ## Contribution
-Feel free to contribute. Make sure to write `docstrings` to your methods and
-classes and please write tests and use PEP 8 (https://peps.python.org/pep-0008/
-) Please write tests for your code and put them into the `test/` folder. Visit
-the [README file](./tests/README.md) in the test-folder for more information.
-Pleas also add a jupyter notebook in the `docs/` folder in order to document
-your code. Please visit the [README file](./docs/README.md) in the docs-folder
-for more information on how to compile the documentation. Please use the
-**numpy style for the docstrings**: https://sphinxcontrib-
-napoleon.readthedocs.io/en/latest/example_numpy.html#example-numpy
+standard_attributes_and_conventions.html) - `pydantic`: Used to validate
+[standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/
+conventions/standard_attributes_and_conventions.html) - `pyyaml>6.0.0`: Reading
+and writing of yaml files, e.g. metadata definitions (conventions). Note, lower
+versions collide with python 3.11 - `requests`: Used to download files from the
+internet or validate URLs, e.g. metadata definitions (conventions) - `rdflib`:
+Used to enable working with RDF - `ontolutils`: Required to work with RDF and
+derive semantic description of HDF5 file content #### Optional dependencies To
+run unit tests or to enable certain features, additional dependencies must be
+installed. Install optional dependencies by specifying them in square brackets
+after the package name, e.g.: pip install h5RDMtoolbox[mongodb] [mongodb] -
+`pymongo>=4.2.0`: Database solution for HDF5 files [csv] - `pandas>=1.4.3`:
+Mainly used for reading csv and pretty printing [snt] - `xmltodict`: Reading of
+xml files - `tabulate>=0.8.10`: Pretty printing of tables - `python-gitlab`:
+Access to gitlab repositories - `pypandoc>=2.3`: Conversion of markdown files
+to html ## Citing the package If you intend to use the package in your work,
+you may cite the paper in the journal [inggrid](https://preprints.inggrid.org/
+repository/view/23/) Here's the bibtext to it: ``` @article
+{probst2023h5rdmtoolbox, title={h5RDMtoolbox-A Python Toolbox for FAIR Data
+Management around HDF5}, author={Probst, Matthias and Pritz, Balazs}, year=
+{2023}, publisher={ing. grid Preprint Repository} } ``` ## Contribution Feel
+free to contribute. Make sure to write `docstrings` to your methods and classes
+and please write tests and use PEP 8 (https://peps.python.org/pep-0008/) Please
+write tests for your code and put them into the `test/` folder. Visit the
+[README file](./tests/README.md) in the test-folder for more information. Pleas
+also add a jupyter notebook in the `docs/` folder in order to document your
+code. Please visit the [README file](./docs/README.md) in the docs-folder for
+more information on how to compile the documentation. Please use the **numpy
+style for the docstrings**: https://sphinxcontrib-napoleon.readthedocs.io/en/
+latest/example_numpy.html#example-numpy
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/_cfg.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_cfg.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,34 +13,36 @@
     if isinstance(level, str):
         return level.lower() in ('error', 'debug', 'critical', 'warning', 'info', 'fatal', 'warning', 'warn')
     # 0: NOTSET, 10: DEBUG, 20: INFO, 30: WARNING, 40: ERROR, 50: CRITICAL
     return level in (0, 10, 20, 30, 40, 50)
 
 
 CONFIG = {
-          'return_xarray': True,
-          'advanced_shape_repr': True,
-          'natural_naming': True,
-          'hdf_compression': None,  # 'gzip',
-          'hdf_compression_opts': None,  # 5,
-          'adjusting_plotting_labels': True,
-          'xarray_unit_repr_in_plots': 'in',
-          'plotting_name_order': ('plot_name', 'long_name', 'standard_name'),
-          'require_unit': True,  # datasets require units
-          'ureg_format': 'C~',
-          'init_logger_level': 'ERROR',
-          'dtime_fmt': '%Y%m%d%H%M%S%f',
-          'expose_user_prop_to_attrs': True,
-          'add_provenance': False,
-          'ignore_set_std_attr_err': False,
-
-          # if a standard attribute is defined and cannot be retrieved because the value is invalid, ignore it:
-          'ignore_get_std_attr_err': False,
-          'allow_deleting_standard_attributes': False,
-          }
+    'return_xarray': True,
+    'advanced_shape_repr': True,
+    'natural_naming': True,
+    'hdf_compression': None,  # 'gzip',
+    'hdf_compression_opts': None,  # 5,
+    'adjusting_plotting_labels': True,
+    'xarray_unit_repr_in_plots': 'in',
+    'plotting_name_order': ('plot_name', 'long_name', 'standard_name'),
+    'require_unit': True,  # datasets require units
+    'ureg_format': 'C~',
+    'init_logger_level': 'ERROR',
+    'dtime_fmt': '%Y%m%d%H%M%S%f',
+    'expose_user_prop_to_attrs': True,
+    'add_provenance': False,
+    'ignore_set_std_attr_err': False,
+    'auto_create_h5tbx_version': False,  # automatically creates the group h5rdmtoolbox with the version attribute
+    'uuid_name': 'uuid',  # attribute name used for UUIDs
+    # if a standard attribute is defined and cannot be retrieved because the value is invalid, ignore it:
+    'ignore_get_std_attr_err': False,
+    'allow_deleting_standard_attributes': False,
+    'ignore_none': False
+}
 
 _VALIDATORS = {
     'return_xarray': lambda x: isinstance(x, bool),
     'advanced_shape_repr': lambda x: isinstance(x, bool),
     'natural_naming': lambda x: isinstance(x, bool),
     'hdf_compression': lambda x: isinstance(x, str),
     'hdf_compression_opts': lambda x: isinstance(x, int),
@@ -50,16 +52,16 @@
     'require_unit': lambda x: isinstance(x, bool),
     'ureg_format': lambda x: isinstance(x, str),
     'init_logger_level': lambda x: is_valid_logger_level(x),
     'dtime_fmt': lambda x: isinstance(x, str),
     'expose_user_prop_to_attrs': lambda x: isinstance(x, bool),
     'add_provenance': lambda x: isinstance(x, bool),
     'ignore_set_std_attr_err': lambda x: isinstance(x, bool),
-
     'ignore_get_std_attr_err': lambda x: isinstance(x, bool),
+    'ignore_none': lambda x: isinstance(x, bool)
 }
 
 
 class set_config:
     """Set the configuration parameters."""
 
     def __init__(self, **kwargs):
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/_repr.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_repr.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,1319 +9,1651 @@
 00000080: 2061 7320 7872 0d0a 6672 6f6d 2049 5079   as xr..from IPy
 00000090: 7468 6f6e 2e64 6973 706c 6179 2069 6d70  thon.display imp
 000000a0: 6f72 7420 4854 4d4c 2c20 6469 7370 6c61  ort HTML, displa
 000000b0: 790d 0a66 726f 6d20 6162 6320 696d 706f  y..from abc impo
 000000c0: 7274 2061 6273 7472 6163 746d 6574 686f  rt abstractmetho
 000000d0: 640d 0a66 726f 6d20 6e75 6d70 7920 696d  d..from numpy im
 000000e0: 706f 7274 206e 6461 7272 6179 0d0a 6672  port ndarray..fr
-000000f0: 6f6d 2074 696d 6520 696d 706f 7274 2070  om time import p
-00000100: 6572 665f 636f 756e 7465 725f 6e73 0d0a  erf_counter_ns..
-00000110: 0d0a 6672 6f6d 202e 2069 6d70 6f72 7420  ..from . import 
-00000120: 6765 745f 636f 6e66 6967 0d0a 6672 6f6d  get_config..from
-00000130: 202e 2069 6d70 6f72 7420 6964 656e 7469   . import identi
-00000140: 6669 6572 730d 0a66 726f 6d20 2e20 696d  fiers..from . im
-00000150: 706f 7274 2070 726f 7465 6374 6564 5f61  port protected_a
-00000160: 7474 7269 6275 7465 730d 0a0d 0a48 3550  ttributes....H5P
-00000170: 595f 5350 4543 4941 4c5f 4154 5452 4942  Y_SPECIAL_ATTRIB
-00000180: 5554 4553 203d 2028 2744 494d 454e 5349  UTES = ('DIMENSI
-00000190: 4f4e 5f4c 4953 5427 2c20 2752 4546 4552  ON_LIST', 'REFER
-000001a0: 454e 4345 5f4c 4953 5427 2c20 274e 414d  ENCE_LIST', 'NAM
-000001b0: 4527 2c20 2743 4c41 5353 272c 2070 726f  E', 'CLASS', pro
-000001c0: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-000001d0: 732e 434f 4f52 4449 4e41 5445 5329 0d0a  s.COORDINATES)..
-000001e0: 7472 793a 0d0a 2020 2020 4353 535f 5354  try:..    CSS_ST
-000001f0: 5220 3d20 696d 706f 7274 6c69 625f 7265  R = importlib_re
-00000200: 736f 7572 6365 732e 6669 6c65 7328 2768  sources.files('h
-00000210: 3572 646d 746f 6f6c 626f 7827 292e 6a6f  5rdmtoolbox').jo
-00000220: 696e 7061 7468 2827 6461 7461 2f73 7479  inpath('data/sty
-00000230: 6c65 2e63 7373 2729 2e72 6561 645f 6279  le.css').read_by
-00000240: 7465 7328 292e 6465 636f 6465 2822 7574  tes().decode("ut
-00000250: 6638 2229 0d0a 6578 6365 7074 2046 696c  f8")..except Fil
-00000260: 654e 6f74 466f 756e 6445 7272 6f72 3a0d  eNotFoundError:.
-00000270: 0a20 2020 2069 6d70 6f72 7420 7061 7468  .    import path
-00000280: 6c69 620d 0a0d 0a20 2020 2077 6974 6820  lib....    with 
-00000290: 6f70 656e 2870 6174 686c 6962 2e50 6174  open(pathlib.Pat
-000002a0: 6828 5f5f 6669 6c65 5f5f 292e 7061 7265  h(__file__).pare
-000002b0: 6e74 202f 2027 6461 7461 2f73 7479 6c65  nt / 'data/style
-000002c0: 2e63 7373 2729 2061 7320 663a 0d0a 2020  .css') as f:..  
-000002d0: 2020 2020 2020 4353 535f 5354 5220 3d20        CSS_STR = 
-000002e0: 662e 7265 6164 2829 2e72 7374 7269 7028  f.read().rstrip(
-000002f0: 290d 0a0d 0a22 2222 0d0a 6469 7363 6c61  )...."""..discla
-00000300: 696d 6572 3a0d 0a0d 0a64 726f 7064 6f77  imer:....dropdow
-00000310: 6e20 5f68 746d 6c20 7265 7072 6573 656e  n _html represen
-00000320: 7461 7469 6f6e 2072 6561 6c69 7a65 6420  tation realized 
-00000330: 7769 7468 2022 6835 6669 6c65 5f68 746d  with "h5file_htm
-00000340: 6c5f 7265 7072 220d 0a69 7320 696e 7370  l_repr"..is insp
-00000350: 6972 6564 2061 6e64 206d 6f73 746c 7920  ired and mostly 
-00000360: 7461 6b65 6e20 6672 6f6d 3a0d 0a68 7474  taken from:..htt
-00000370: 7073 3a2f 2f6a 7366 6964 646c 652e 6e65  ps://jsfiddle.ne
-00000380: 742f 7461 7930 3863 6e39 2f34 2f20 2878  t/tay08cn9/4/ (x
-00000390: 6172 7261 7920 7061 636b 6167 6529 0d0a  array package)..
-000003a0: 0d0a 2222 220d 0a0d 0a53 4455 4d50 5f54  .."""....SDUMP_T
-000003b0: 4142 4c45 5f53 5041 4349 4e47 203d 2033  ABLE_SPACING = 3
-000003c0: 302c 2032 302c 2038 2c20 3330 0d0a 0d0a  0, 20, 8, 30....
-000003d0: 0d0a 636c 6173 7320 4243 6f6c 6f72 733a  ..class BColors:
-000003e0: 0d0a 2020 2020 2222 2243 6f6c 6f72 2063  ..    """Color c
-000003f0: 6c61 7373 2074 6f20 636f 6c6f 7220 7465  lass to color te
-00000400: 7874 2222 220d 0a20 2020 2048 4541 4445  xt"""..    HEADE
-00000410: 5220 3d20 275c 3033 335b 3935 6d27 0d0a  R = '\033[95m'..
-00000420: 2020 2020 4f4b 424c 5545 203d 2027 5c30      OKBLUE = '\0
-00000430: 3333 5b39 346d 270d 0a20 2020 204f 4b43  33[94m'..    OKC
-00000440: 5941 4e20 3d20 275c 3033 335b 3936 6d27  YAN = '\033[96m'
-00000450: 0d0a 2020 2020 4f4b 4752 4545 4e20 3d20  ..    OKGREEN = 
-00000460: 275c 3033 335b 3932 6d27 0d0a 2020 2020  '\033[92m'..    
-00000470: 5741 524e 494e 4720 3d20 275c 3033 335b  WARNING = '\033[
-00000480: 3933 6d27 0d0a 2020 2020 4641 494c 203d  93m'..    FAIL =
-00000490: 2027 5c30 3333 5b39 316d 270d 0a20 2020   '\033[91m'..   
-000004a0: 2045 4e44 4320 3d20 275c 3033 335b 306d   ENDC = '\033[0m
-000004b0: 270d 0a20 2020 2042 4f4c 4420 3d20 275c  '..    BOLD = '\
-000004c0: 3033 335b 316d 270d 0a20 2020 2055 4e44  033[1m'..    UND
-000004d0: 4552 4c49 4e45 203d 2027 5c30 3333 5b34  ERLINE = '\033[4
-000004e0: 6d27 0d0a 2020 2020 4954 414c 4943 203d  m'..    ITALIC =
-000004f0: 2027 5c30 3333 5b33 6d27 0d0a 0d0a 0d0a   '\033[3m'......
-00000500: 6465 6620 6d61 6b65 5f69 7461 6c69 6328  def make_italic(
-00000510: 7374 7269 6e67 293a 0d0a 2020 2020 2222  string):..    ""
-00000520: 226d 616b 6520 7374 7269 6e67 2069 7461  "make string ita
-00000530: 6c69 6322 2222 0d0a 2020 2020 7265 7475  lic"""..    retu
-00000540: 726e 2066 227b 4243 6f6c 6f72 732e 4954  rn f"{BColors.IT
-00000550: 414c 4943 7d7b 7374 7269 6e67 7d7b 4243  ALIC}{string}{BC
-00000560: 6f6c 6f72 732e 454e 4443 7d22 0d0a 0d0a  olors.ENDC}"....
-00000570: 0d0a 6465 6620 6d61 6b65 5f62 6f6c 6428  ..def make_bold(
-00000580: 7374 7269 6e67 293a 0d0a 2020 2020 2222  string):..    ""
-00000590: 226d 616b 6520 7374 7269 6e67 2062 6f6c  "make string bol
-000005a0: 6422 2222 0d0a 2020 2020 7265 7475 726e  d"""..    return
-000005b0: 2066 227b 4243 6f6c 6f72 732e 424f 4c44   f"{BColors.BOLD
-000005c0: 7d7b 7374 7269 6e67 7d7b 4243 6f6c 6f72  }{string}{BColor
-000005d0: 732e 454e 4443 7d22 0d0a 0d0a 0d0a 6465  s.ENDC}"......de
-000005e0: 6620 7761 726e 696e 6774 6578 7428 7374  f warningtext(st
-000005f0: 7269 6e67 293a 0d0a 2020 2020 2222 226d  ring):..    """m
-00000600: 616b 6520 7374 7269 6e67 206f 7261 6e67  ake string orang
-00000610: 6522 2222 0d0a 2020 2020 7265 7475 726e  e"""..    return
-00000620: 2066 227b 4243 6f6c 6f72 732e 5741 524e   f"{BColors.WARN
-00000630: 494e 477d 7b73 7472 696e 677d 7b42 436f  ING}{string}{BCo
-00000640: 6c6f 7273 2e45 4e44 437d 220d 0a0d 0a0d  lors.ENDC}".....
-00000650: 0a64 6566 2066 6169 6c74 6578 7428 7374  .def failtext(st
-00000660: 7269 6e67 293a 0d0a 2020 2020 2222 226d  ring):..    """m
-00000670: 616b 6520 7374 7269 6e67 2072 6564 2222  ake string red""
-00000680: 220d 0a20 2020 2072 6574 7572 6e20 6622  "..    return f"
-00000690: 7b42 436f 6c6f 7273 2e46 4149 4c7d 7b73  {BColors.FAIL}{s
-000006a0: 7472 696e 677d 7b42 436f 6c6f 7273 2e45  tring}{BColors.E
-000006b0: 4e44 437d 220d 0a0d 0a0d 0a64 6566 2066  NDC}"......def f
-000006c0: 6169 6c70 7269 6e74 2873 7472 696e 6729  ailprint(string)
-000006d0: 3a0d 0a20 2020 2022 2222 7072 696e 7420  :..    """print 
-000006e0: 7374 7269 6e67 2069 6e20 7265 6422 2222  string in red"""
-000006f0: 0d0a 2020 2020 7072 696e 7428 6661 696c  ..    print(fail
-00000700: 7465 7874 2873 7472 696e 6729 290d 0a0d  text(string))...
-00000710: 0a0d 0a64 6566 206f 6b74 6578 7428 7374  ...def oktext(st
-00000720: 7269 6e67 293a 0d0a 2020 2020 2222 226d  ring):..    """m
-00000730: 616b 6520 7374 7269 6e67 2067 7265 656e  ake string green
-00000740: 2222 220d 0a20 2020 2072 6574 7572 6e20  """..    return 
-00000750: 6622 7b42 436f 6c6f 7273 2e4f 4b47 5245  f"{BColors.OKGRE
-00000760: 454e 7d7b 7374 7269 6e67 7d7b 4243 6f6c  EN}{string}{BCol
-00000770: 6f72 732e 454e 4443 7d22 0d0a 0d0a 0d0a  ors.ENDC}"......
-00000780: 6465 6620 6f6b 7072 696e 7428 7374 7269  def okprint(stri
-00000790: 6e67 293a 0d0a 2020 2020 2222 2270 7269  ng):..    """pri
-000007a0: 6e74 2073 7472 696e 6720 696e 2072 6564  nt string in red
-000007b0: 2222 220d 0a20 2020 2070 7269 6e74 286f  """..    print(o
-000007c0: 6b74 6578 7428 7374 7269 6e67 2929 0d0a  ktext(string))..
-000007d0: 0d0a 0d0a 6465 6620 6d61 6b65 5f68 7265  ....def make_hre
-000007e0: 6628 7572 6c2c 2074 6578 7429 202d 3e20  f(url, text) -> 
-000007f0: 7374 723a 0d0a 2020 2020 6966 206e 6f74  str:..    if not
-00000800: 2075 726c 2e73 7461 7274 7377 6974 6828   url.startswith(
-00000810: 2768 7474 7027 293a 0d0a 2020 2020 2020  'http'):..      
-00000820: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00000830: 6f72 2866 2749 6e76 616c 6964 2055 524c  or(f'Invalid URL
-00000840: 3a20 227b 7572 6c7d 222e 204d 7573 7420  : "{url}". Must 
-00000850: 7374 6172 7420 7769 7468 2022 6874 7470  start with "http
-00000860: 2227 290d 0a20 2020 2072 6574 7572 6e20  "')..    return 
-00000870: 6627 3c61 2068 7265 663d 227b 7572 6c7d  f'<a href="{url}
-00000880: 223e 7b74 6578 747d 3c2f 613e 270d 0a0d  ">{text}</a>'...
-00000890: 0a0d 0a64 6566 2070 726f 6365 7373 5f73  ...def process_s
-000008a0: 7472 696e 675f 666f 725f 6c69 6e6b 2873  tring_for_link(s
-000008b0: 7472 696e 673a 2073 7472 2920 2d3e 2074  tring: str) -> t
-000008c0: 7970 696e 672e 5475 706c 655b 7374 722c  yping.Tuple[str,
-000008d0: 2062 6f6f 6c5d 3a0d 0a20 2020 2022 2222   bool]:..    """
-000008e0: 7072 6f63 6573 7320 7374 7269 6e67 2074  process string t
-000008f0: 6f20 6d61 6b65 206c 696e 6b73 2061 6374  o make links act
-00000900: 7561 6c6c 7920 636c 6963 6b61 626c 6520  ually clickable 
-00000910: 696e 2068 746d 6c0d 0a0d 0a20 2020 2050  in html....    P
-00000920: 6172 616d 6574 6572 730d 0a20 2020 202d  arameters..    -
-00000930: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2073  ---------..    s
-00000940: 7472 696e 673a 2073 7472 0d0a 2020 2020  tring: str..    
-00000950: 2020 2020 7374 7269 6e67 2074 6f20 7072      string to pr
-00000960: 6f63 6573 730d 0a0d 0a20 2020 2052 6574  ocess....    Ret
-00000970: 7572 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d  urns..    ------
-00000980: 2d0d 0a20 2020 2073 7472 0d0a 2020 2020  -..    str..    
-00000990: 2020 2020 7072 6f63 6573 7365 6420 7374      processed st
-000009a0: 7269 6e67 0d0a 2020 2020 626f 6f6c 0d0a  ring..    bool..
-000009b0: 2020 2020 2020 2020 5472 7565 2069 6620          True if 
-000009c0: 7374 7269 6e67 2061 6374 7561 6c6c 7920  string actually 
-000009d0: 636f 6e74 6169 6e73 2061 206c 696e 6b0d  contains a link.
-000009e0: 0a0d 0a20 2020 2022 2222 0d0a 2020 2020  ...    """..    
-000009f0: 6966 2027 7a65 6e6f 646f 2e27 2069 6e20  if 'zenodo.' in 
-00000a00: 7374 7269 6e67 3a0d 0a20 2020 2020 2020  string:..       
-00000a10: 2069 6620 7265 2e6d 6174 6368 2872 2731   if re.match(r'1
-00000a20: 305c 2e5c 647b 342c 397d 2f7a 656e 6f64  0\.\d{4,9}/zenod
-00000a30: 6f5c 2e5c 647b 342c 397d 272c 2073 7472  o\.\d{4,9}', str
-00000a40: 696e 6729 3a0d 0a20 2020 2020 2020 2020  ing):..         
-00000a50: 2020 207a 656e 6f64 6f5f 7572 6c20 3d20     zenodo_url = 
-00000a60: 6627 6874 7470 733a 2f2f 646f 692e 6f72  f'https://doi.or
-00000a70: 672f 7b73 7472 696e 677d 270d 0a20 2020  g/{string}'..   
-00000a80: 2020 2020 2020 2020 2069 6d67 5f75 726c           img_url
-00000a90: 203d 2066 2768 7474 7073 3a2f 2f7a 656e   = f'https://zen
-00000aa0: 6f64 6f2e 6f72 672f 6261 6467 652f 444f  odo.org/badge/DO
-00000ab0: 492f 7b73 7472 696e 677d 2e73 7667 270d  I/{string}.svg'.
-00000ac0: 0a20 2020 2020 2020 2069 6620 7374 7269  .        if stri
-00000ad0: 6e67 2e73 7461 7274 7377 6974 6828 2768  ng.startswith('h
-00000ae0: 7474 7073 3a2f 2f7a 656e 6f64 6f2e 6f72  ttps://zenodo.or
-00000af0: 672f 7265 636f 7264 2f27 293a 0d0a 2020  g/record/'):..  
-00000b00: 2020 2020 2020 2020 2020 7a65 6e6f 646f            zenodo
-00000b10: 5f75 726c 203d 2073 7472 696e 670d 0a20  _url = string.. 
-00000b20: 2020 2020 2020 2020 2020 2069 6d67 5f75             img_u
-00000b30: 726c 203d 2066 2768 7474 7073 3a2f 2f7a  rl = f'https://z
-00000b40: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
-00000b50: 444f 492f 3130 2e35 3238 312f 7a65 6e6f  DOI/10.5281/zeno
-00000b60: 646f 2e7b 7374 7269 6e67 2e73 706c 6974  do.{string.split
-00000b70: 2822 2f22 295b 2d31 5d7d 2e73 7667 270d  ("/")[-1]}.svg'.
-00000b80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000b90: 6d61 6b65 5f68 7265 6628 7572 6c3d 7a65  make_href(url=ze
-00000ba0: 6e6f 646f 5f75 726c 2c20 7465 7874 3d66  nodo_url, text=f
-00000bb0: 273c 696d 6720 7372 633d 227b 696d 675f  '<img src="{img_
-00000bc0: 7572 6c7d 2220 616c 743d 2244 4f49 223e  url}" alt="DOI">
-00000bd0: 2729 2c20 5472 7565 0d0a 2020 2020 666f  '), True..    fo
-00000be0: 7220 7020 696e 2028 7222 2868 7474 7073  r p in (r"(https
-00000bf0: 3f3a 2f2f 5c53 2b29 222c 2072 2228 6674  ?://\S+)", r"(ft
-00000c00: 703a 2f2f 5c53 2b29 222c 2072 2228 7777  p://\S+)", r"(ww
-00000c10: 775c 2e5c 532b 2922 293a 0d0a 2020 2020  w\.\S+)"):..    
-00000c20: 2020 2020 7572 6c73 203d 2072 652e 6669      urls = re.fi
-00000c30: 6e64 616c 6c28 702c 2073 7472 696e 6729  ndall(p, string)
-00000c40: 0d0a 2020 2020 2020 2020 6966 2075 726c  ..        if url
-00000c50: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000c60: 666f 7220 7572 6c20 696e 2075 726c 733a  for url in urls:
-00000c70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c80: 2020 6964 656e 7469 6669 6572 203d 2069    identifier = i
-00000c90: 6465 6e74 6966 6965 7273 2e66 726f 6d5f  dentifiers.from_
-00000ca0: 7572 6c28 7572 6c29 0d0a 2020 2020 2020  url(url)..      
-00000cb0: 2020 2020 2020 2020 2020 6966 2069 6465            if ide
-00000cc0: 6e74 6966 6965 723a 0d0a 2020 2020 2020  ntifier:..      
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00000ce0: 6369 645f 7572 6c5f 7265 7072 203d 2069  cid_url_repr = i
-00000cf0: 6465 6e74 6966 6965 722e 5f72 6570 725f  dentifier._repr_
-00000d00: 6874 6d6c 5f28 290d 0a20 2020 2020 2020  html_()..       
-00000d10: 2020 2020 2020 2020 2020 2020 2073 7472               str
-00000d20: 696e 6720 3d20 7374 7269 6e67 2e72 6570  ing = string.rep
-00000d30: 6c61 6365 2875 726c 2c20 6f72 6369 645f  lace(url, orcid_
-00000d40: 7572 6c5f 7265 7072 290d 0a20 2020 2020  url_repr)..     
-00000d50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00000d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d70: 2020 2020 2020 7374 7269 6e67 203d 2073        string = s
-00000d80: 7472 696e 672e 7265 706c 6163 6528 7572  tring.replace(ur
-00000d90: 6c2c 206d 616b 655f 6872 6566 2875 726c  l, make_href(url
-00000da0: 2c20 7572 6c29 290d 0a20 2020 2020 2020  , url))..       
-00000db0: 2020 2020 2072 6574 7572 6e20 7374 7269       return stri
-00000dc0: 6e67 2c20 5472 7565 0d0a 0d0a 2020 2020  ng, True....    
-00000dd0: 7265 7475 726e 2073 7472 696e 672c 2046  return string, F
-00000de0: 616c 7365 0d0a 0d0a 0d0a 6465 6620 6765  alse......def ge
-00000df0: 745f 6972 695f 6963 6f6e 5f68 7265 6628  t_iri_icon_href(
-00000e00: 6972 693a 2073 7472 2920 2d3e 2073 7472  iri: str) -> str
-00000e10: 3a0d 0a20 2020 2022 2222 6765 7420 6874  :..    """get ht
-00000e20: 6d6c 2072 6570 7265 7365 6e74 6174 696f  ml representatio
-00000e30: 6e20 6f66 2061 6e20 4952 4920 7769 7468  n of an IRI with
-00000e40: 2069 636f 6e22 2222 0d0a 2020 2020 7265   icon"""..    re
-00000e50: 7475 726e 2066 273c 6120 6872 6566 3d22  turn f'<a href="
-00000e60: 7b69 7269 7d22 3e3c 696d 6720 7372 633d  {iri}"><img src=
-00000e70: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000e80: 636f 6d2f 6d61 7474 6869 6173 7072 6f62  com/matthiasprob
-00000e90: 7374 2f68 3552 444d 746f 6f6c 626f 782f  st/h5RDMtoolbox/
-00000ea0: 626c 6f62 2f64 6576 2f68 3572 646d 746f  blob/dev/h5rdmto
-00000eb0: 6f6c 626f 782f 6461 7461 2f69 7269 5f69  olbox/data/iri_i
-00000ec0: 636f 6e2e 706e 673f 7261 773d 7472 7565  con.png?raw=true
-00000ed0: 2220 616c 743d 2220 5b49 5249 5d22 2077  " alt=" [IRI]" w
-00000ee0: 6964 7468 3d22 3136 2220 6865 6967 6874  idth="16" height
-00000ef0: 3d22 3136 2220 2f3e 3c2f 613e 270d 0a0d  ="16" /></a>'...
-00000f00: 0a0d 0a63 6c61 7373 205f 4844 4635 5374  ...class _HDF5St
-00000f10: 7275 6374 7572 6552 6570 723a 0d0a 0d0a  ructureRepr:....
-00000f20: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000f30: 2873 656c 662c 2069 676e 6f72 655f 6174  (self, ignore_at
-00000f40: 7472 733d 4e6f 6e65 293a 0d0a 2020 2020  trs=None):..    
-00000f50: 2020 2020 7365 6c66 2e62 6173 655f 696e      self.base_in
-00000f60: 7465 6e74 203d 2027 2020 270d 0a20 2020  tent = '  '..   
-00000f70: 2020 2020 2073 656c 662e 6d61 785f 6174       self.max_at
-00000f80: 7472 5f6c 656e 6774 6820 3d20 3130 300d  tr_length = 100.
-00000f90: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00000fa0: 6c6c 6170 7365 6420 3d20 4e6f 6e65 0d0a  llapsed = None..
-00000fb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000fc0: 6f62 6a5f 6366 6720 3d20 7b7d 0d0a 2020  obj_cfg = {}..  
-00000fd0: 2020 2020 2020 6966 2069 676e 6f72 655f        if ignore_
-00000fe0: 6174 7472 7320 6973 204e 6f6e 653a 0d0a  attrs is None:..
-00000ff0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001000: 2e69 676e 6f72 655f 6174 7472 7320 3d20  .ignore_attrs = 
-00001010: 4835 5059 5f53 5045 4349 414c 5f41 5454  H5PY_SPECIAL_ATT
-00001020: 5249 4255 5445 530d 0a20 2020 2020 2020  RIBUTES..       
-00001030: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001040: 2020 2020 7365 6c66 2e69 676e 6f72 655f      self.ignore_
-00001050: 6174 7472 7320 3d20 6967 6e6f 7265 5f61  attrs = ignore_a
-00001060: 7474 7273 0d0a 0d0a 2020 2020 4070 726f  ttrs....    @pro
-00001070: 7065 7274 790d 0a20 2020 2064 6566 2063  perty..    def c
-00001080: 6865 636b 626f 785f 7374 6174 6528 7365  heckbox_state(se
-00001090: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
-000010a0: 2020 2020 2072 6574 7572 6e20 2727 2069       return '' i
-000010b0: 6620 7365 6c66 2e63 6f6c 6c61 7073 6564  f self.collapsed
-000010c0: 2065 6c73 6520 2763 6865 636b 6564 270d   else 'checked'.
-000010d0: 0a0d 0a20 2020 2064 6566 205f 5f64 6174  ...    def __dat
-000010e0: 6173 6574 5f5f 2873 656c 662c 206e 616d  aset__(self, nam
-000010f0: 652c 2068 356f 626a 2920 2d3e 2073 7472  e, h5obj) -> str
-00001100: 3a0d 0a20 2020 2020 2020 2022 2222 6f76  :..        """ov
-00001110: 6572 7772 6974 6520 7468 6520 4835 5265  erwrite the H5Re
-00001120: 7072 2070 6172 656e 7420 6d65 7468 6f64  pr parent method
-00001130: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-00001140: 6835 6f62 6a2e 6474 7970 652e 6368 6172  h5obj.dtype.char
-00001150: 203d 3d20 2753 273a 0d0a 2020 2020 2020   == 'S':..      
-00001160: 2020 2020 2020 2320 6861 6e64 656c 2073        # handel s
-00001170: 7472 696e 6720 6461 7461 7365 7473 3a0d  tring datasets:.
-00001180: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001190: 7572 6e20 7365 6c66 2e5f 5f73 7472 696e  urn self.__strin
-000011a0: 6764 6174 6173 6574 5f5f 286e 616d 652c  gdataset__(name,
-000011b0: 2068 356f 626a 290d 0a20 2020 2020 2020   h5obj)..       
-000011c0: 2069 6620 6835 6f62 6a2e 6e64 696d 203d   if h5obj.ndim =
-000011d0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-000011e0: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-000011f0: 3044 6461 7461 7365 745f 5f28 6e61 6d65  0Ddataset__(name
-00001200: 2c20 6835 6f62 6a29 0d0a 2020 2020 2020  , h5obj)..      
-00001210: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-00001220: 4e44 6461 7461 7365 745f 5f28 6e61 6d65  NDdataset__(name
-00001230: 2c20 6835 6f62 6a29 0d0a 0d0a 2020 2020  , h5obj)....    
-00001240: 4061 6273 7472 6163 746d 6574 686f 640d  @abstractmethod.
-00001250: 0a20 2020 2064 6566 205f 5f73 7472 696e  .    def __strin
-00001260: 6764 6174 6173 6574 5f5f 2873 656c 662c  gdataset__(self,
-00001270: 206e 616d 652c 2068 356f 626a 293a 0d0a   name, h5obj):..
-00001280: 2020 2020 2020 2020 2222 2264 6174 6173          """datas
-00001290: 6574 2072 6570 7265 7365 6e74 6174 696f  et representatio
-000012a0: 6e22 2222 0d0a 0d0a 2020 2020 4061 6273  n"""....    @abs
-000012b0: 7472 6163 746d 6574 686f 640d 0a20 2020  tractmethod..   
-000012c0: 2064 6566 205f 5f30 4464 6174 6173 6574   def __0Ddataset
-000012d0: 5f5f 2873 656c 662c 206e 616d 652c 2068  __(self, name, h
-000012e0: 356f 626a 293a 0d0a 2020 2020 2020 2020  5obj):..        
-000012f0: 2222 2264 6174 6173 6574 2072 6570 7265  """dataset repre
-00001300: 7365 6e74 6174 696f 6e22 2222 0d0a 0d0a  sentation"""....
-00001310: 2020 2020 4061 6273 7472 6163 746d 6574      @abstractmet
-00001320: 686f 640d 0a20 2020 2064 6566 205f 5f4e  hod..    def __N
-00001330: 4464 6174 6173 6574 5f5f 2873 656c 662c  Ddataset__(self,
-00001340: 206e 616d 652c 2068 356f 626a 293a 0d0a   name, h5obj):..
-00001350: 2020 2020 2020 2020 2222 2264 6174 6173          """datas
-00001360: 6574 2072 6570 7265 7365 6e74 6174 696f  et representatio
-00001370: 6e22 2222 0d0a 0d0a 2020 2020 4061 6273  n"""....    @abs
-00001380: 7472 6163 746d 6574 686f 640d 0a20 2020  tractmethod..   
-00001390: 2064 6566 205f 5f67 726f 7570 5f5f 2873   def __group__(s
-000013a0: 656c 662c 206e 616d 652c 2068 356f 626a  elf, name, h5obj
-000013b0: 293a 0d0a 2020 2020 2020 2020 2222 2264  ):..        """d
-000013c0: 6174 6173 6574 2072 6570 7265 7365 6e74  ataset represent
-000013d0: 6174 696f 6e22 2222 0d0a 0d0a 2020 2020  ation"""....    
-000013e0: 4061 6273 7472 6163 746d 6574 686f 640d  @abstractmethod.
-000013f0: 0a20 2020 2064 6566 205f 5f61 7474 7273  .    def __attrs
-00001400: 5f5f 2873 656c 662c 206e 616d 652c 2068  __(self, name, h
-00001410: 356f 626a 293a 0d0a 2020 2020 2020 2020  5obj):..        
-00001420: 2222 2264 6174 6173 6574 2072 6570 7265  """dataset repre
-00001430: 7365 6e74 6174 696f 6e22 2222 0d0a 0d0a  sentation"""....
-00001440: 0d0a 636c 6173 7320 4844 4635 5374 7275  ..class HDF5Stru
-00001450: 6374 7572 6553 7472 5265 7072 285f 4844  ctureStrRepr(_HD
-00001460: 4635 5374 7275 6374 7572 6552 6570 7229  F5StructureRepr)
-00001470: 3a0d 0a0d 0a20 2020 2064 6566 205f 5f63  :....    def __c
-00001480: 616c 6c5f 5f28 7365 6c66 2c20 6772 6f75  all__(self, grou
-00001490: 702c 2069 6e64 656e 743d 302c 2070 7265  p, indent=0, pre
-000014a0: 616d 626c 653d 4e6f 6e65 293a 0d0a 2020  amble=None):..  
-000014b0: 2020 2020 2020 6966 2070 7265 616d 626c        if preambl
-000014c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000014d0: 7072 696e 7428 7072 6561 6d62 6c65 290d  print(preamble).
-000014e0: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
-000014f0: 725f 6e61 6d65 2069 6e20 6772 6f75 702e  r_name in group.
-00001500: 6174 7472 732e 7261 772e 6b65 7973 2829  attrs.raw.keys()
-00001510: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00001520: 6620 6e6f 7420 6174 7472 5f6e 616d 652e  f not attr_name.
-00001530: 6973 7570 7065 7228 293a 0d0a 2020 2020  isupper():..    
-00001540: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00001550: 7428 7365 6c66 2e62 6173 655f 696e 7465  t(self.base_inte
-00001560: 6e74 202a 2069 6e64 656e 7420 2b20 7365  nt * indent + se
-00001570: 6c66 2e5f 5f61 7474 7273 5f5f 2861 7474  lf.__attrs__(att
-00001580: 725f 6e61 6d65 2c20 6772 6f75 7029 290d  r_name, group)).
-00001590: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-000015a0: 2c20 6974 656d 2069 6e20 6772 6f75 702e  , item in group.
-000015b0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
-000015c0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000015d0: 6e63 6528 6974 656d 2c20 6835 7079 2e44  nce(item, h5py.D
-000015e0: 6174 6173 6574 293a 0d0a 2020 2020 2020  ataset):..      
-000015f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00001600: 7365 6c66 2e62 6173 655f 696e 7465 6e74  self.base_intent
-00001610: 202a 2069 6e64 656e 7420 2b20 7365 6c66   * indent + self
-00001620: 2e5f 5f64 6174 6173 6574 5f5f 286b 6579  .__dataset__(key
-00001630: 2c20 6974 656d 2929 0d0a 2020 2020 2020  , item))..      
-00001640: 2020 2020 2020 2020 2020 666f 7220 6174            for at
-00001650: 7472 5f6e 616d 6520 696e 2069 7465 6d2e  tr_name in item.
-00001660: 6174 7472 732e 7261 772e 6b65 7973 2829  attrs.raw.keys()
-00001670: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001680: 2020 2020 2020 2069 6620 6e6f 7420 6174         if not at
-00001690: 7472 5f6e 616d 652e 6973 7570 7065 7228  tr_name.isupper(
-000016a0: 2920 616e 6420 6174 7472 5f6e 616d 6520  ) and attr_name 
-000016b0: 6e6f 7420 696e 2073 656c 662e 6967 6e6f  not in self.igno
-000016c0: 7265 5f61 7474 7273 3a0d 0a20 2020 2020  re_attrs:..     
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2070 7269 6e74 2873 656c 662e 6261     print(self.ba
-000016f0: 7365 5f69 6e74 656e 7420 2a20 2869 6e64  se_intent * (ind
-00001700: 656e 7420 2b20 3229 202b 2073 656c 662e  ent + 2) + self.
-00001710: 5f5f 6174 7472 735f 5f28 6174 7472 5f6e  __attrs__(attr_n
-00001720: 616d 652c 2069 7465 6d29 290d 0a20 2020  ame, item))..   
-00001730: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-00001740: 696e 7374 616e 6365 2869 7465 6d2c 2068  instance(item, h
-00001750: 3570 792e 4772 6f75 7029 3a0d 0a20 2020  5py.Group):..   
-00001760: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00001770: 6e74 2873 656c 662e 6261 7365 5f69 6e74  nt(self.base_int
-00001780: 656e 7420 2a20 696e 6465 6e74 202b 2073  ent * indent + s
-00001790: 656c 662e 5f5f 6772 6f75 705f 5f28 6b65  elf.__group__(ke
-000017a0: 792c 2069 7465 6d29 290d 0a20 2020 2020  y, item))..     
-000017b0: 2020 2020 2020 2020 2020 2073 656c 6628             self(
-000017c0: 6974 656d 2c20 696e 6465 6e74 202b 2031  item, indent + 1
-000017d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000017e0: 2020 2023 2066 6f72 2061 7474 725f 6e61     # for attr_na
-000017f0: 6d65 2c20 6174 7472 5f76 616c 7565 2069  me, attr_value i
-00001800: 6e20 6974 656d 2e61 7474 7273 2e69 7465  n item.attrs.ite
-00001810: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00001820: 2020 2020 2020 2023 2020 2020 2069 6620         #     if 
-00001830: 6e6f 7420 6174 7472 5f6e 616d 652e 6973  not attr_name.is
-00001840: 7570 7065 7228 2920 616e 6420 6174 7472  upper() and attr
-00001850: 5f6e 616d 6520 6e6f 7420 696e 2073 656c  _name not in sel
-00001860: 662e 6967 6e6f 7265 5f61 7474 7273 3a0d  f.ignore_attrs:.
-00001870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001880: 2023 2020 2020 2020 2020 2070 7269 6e74   #         print
-00001890: 2873 656c 662e 6261 7365 5f69 6e74 656e  (self.base_inten
-000018a0: 7420 2a20 2869 6e64 656e 7420 2b20 3229  t * (indent + 2)
-000018b0: 202b 2073 656c 662e 5f5f 6174 7472 5f73   + self.__attr_s
-000018c0: 7472 5f5f 2861 7474 725f 6e61 6d65 2c20  tr__(attr_name, 
-000018d0: 6174 7472 5f76 616c 7565 2929 0d0a 0d0a  attr_value))....
-000018e0: 2020 2020 6465 6620 5f5f 6461 7461 7365      def __datase
-000018f0: 745f 5f28 7365 6c66 2c20 6e61 6d65 3a20  t__(self, name: 
-00001900: 7374 722c 2068 356f 626a 3a20 6835 7079  str, h5obj: h5py
-00001910: 2e44 6174 6173 6574 2920 2d3e 2073 7472  .Dataset) -> str
-00001920: 3a0d 0a20 2020 2020 2020 2069 6620 6835  :..        if h5
-00001930: 6f62 6a2e 6474 7970 652e 6368 6172 203d  obj.dtype.char =
-00001940: 3d20 2753 273a 0d0a 2020 2020 2020 2020  = 'S':..        
-00001950: 2020 2020 2320 6861 6e64 656c 2073 7472      # handel str
-00001960: 696e 6720 6461 7461 7365 7473 3a0d 0a20  ing datasets:.. 
-00001970: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001980: 6e20 7365 6c66 2e5f 5f73 7472 696e 6764  n self.__stringd
-00001990: 6174 6173 6574 5f5f 286e 616d 652c 2068  ataset__(name, h
-000019a0: 356f 626a 290d 0a20 2020 2020 2020 2069  5obj)..        i
-000019b0: 6620 6835 6f62 6a2e 6e64 696d 203d 3d20  f h5obj.ndim == 
-000019c0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000019d0: 7265 7475 726e 2073 656c 662e 5f5f 3044  return self.__0D
-000019e0: 6461 7461 7365 745f 5f28 6e61 6d65 2c20  dataset__(name, 
-000019f0: 6835 6f62 6a29 0d0a 2020 2020 2020 2020  h5obj)..        
-00001a00: 7265 7475 726e 2073 656c 662e 5f5f 4e44  return self.__ND
-00001a10: 6461 7461 7365 745f 5f28 6e61 6d65 2c20  dataset__(name, 
-00001a20: 6835 6f62 6a29 0d0a 0d0a 2020 2020 6465  h5obj)....    de
-00001a30: 6620 5f5f 7374 7269 6e67 6461 7461 7365  f __stringdatase
-00001a40: 745f 5f28 7365 6c66 2c20 6e61 6d65 3a20  t__(self, name: 
-00001a50: 7374 722c 2068 356f 626a 3a20 6835 7079  str, h5obj: h5py
-00001a60: 2e44 6174 6173 6574 2920 2d3e 2073 7472  .Dataset) -> str
-00001a70: 3a0d 0a20 2020 2020 2020 2022 2222 7374  :..        """st
-00001a80: 7269 6e67 2072 6570 7265 7365 6e74 6174  ring representat
-00001a90: 696f 6e20 6f66 2061 2073 7472 696e 6720  ion of a string 
-00001aa0: 6461 7461 7365 7422 2222 0d0a 2020 2020  dataset"""..    
-00001ab0: 2020 2020 6966 2068 356f 626a 2e6e 6469      if h5obj.ndi
-00001ac0: 6d20 3d3d 2030 3a0d 0a20 2020 2020 2020  m == 0:..       
-00001ad0: 2020 2020 2072 6574 7572 6e20 6622 5c30       return f"\0
-00001ae0: 3333 5b31 6d7b 6e61 6d65 7d5c 3033 335b  33[1m{name}\033[
-00001af0: 306d 3a20 7b68 356f 626a 2e76 616c 7565  0m: {h5obj.value
-00001b00: 735b 2829 5d7d 220d 0a20 2020 2020 2020  s[()]}"..       
-00001b10: 2072 6574 7572 6e20 6622 5c30 3333 5b31   return f"\033[1
-00001b20: 6d7b 6e61 6d65 7d5c 3033 335b 306d 3a20  m{name}\033[0m: 
-00001b30: 7b68 356f 626a 2e73 6861 7065 7d2c 2064  {h5obj.shape}, d
-00001b40: 7479 7065 3a20 7b68 356f 626a 2e64 7479  type: {h5obj.dty
-00001b50: 7065 7d22 0d0a 0d0a 2020 2020 6465 6620  pe}"....    def 
-00001b60: 5f5f 3044 6461 7461 7365 745f 5f28 7365  __0Ddataset__(se
-00001b70: 6c66 2c20 6e61 6d65 3a20 7374 722c 2068  lf, name: str, h
-00001b80: 356f 626a 3a20 6835 7079 2e44 6174 6173  5obj: h5py.Datas
-00001b90: 6574 2920 2d3e 2073 7472 3a0d 0a20 2020  et) -> str:..   
-00001ba0: 2020 2020 2022 2222 7374 7269 6e67 2072       """string r
-00001bb0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00001bc0: 2061 2030 4420 6461 7461 7365 7422 2222   a 0D dataset"""
-00001bd0: 0d0a 2020 2020 2020 2020 7661 6c75 6520  ..        value 
-00001be0: 3d20 6835 6f62 6a2e 7661 6c75 6573 5b28  = h5obj.values[(
-00001bf0: 295d 0d0a 2020 2020 2020 2020 6966 2069  )]..        if i
-00001c00: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
-00001c10: 2066 6c6f 6174 293a 0d0a 2020 2020 2020   float):..      
-00001c20: 2020 2020 2020 7661 6c75 6520 3d20 6627        value = f'
-00001c30: 7b76 616c 7565 3a66 7d27 0d0a 2020 2020  {value:f}'..    
-00001c40: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00001c50: 6e63 6528 7661 6c75 652c 2028 696e 742c  nce(value, (int,
-00001c60: 206e 702e 696e 7465 6765 7229 293a 0d0a   np.integer)):..
-00001c70: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00001c80: 6520 3d20 6627 7b69 6e74 2876 616c 7565  e = f'{int(value
-00001c90: 293a 647d 270d 0a20 2020 2020 2020 2065  ):d}'..        e
-00001ca0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00001cb0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-00001cc0: 7228 6627 556e 6578 7065 6374 6564 2074  r(f'Unexpected t
-00001cd0: 7970 6520 7b74 7970 6528 7661 6c75 6529  ype {type(value)
-00001ce0: 7d27 290d 0a20 2020 2020 2020 2072 6574  }')..        ret
-00001cf0: 7572 6e20 6622 5c30 3333 5b31 6d7b 6e61  urn f"\033[1m{na
-00001d00: 6d65 7d5c 3033 335b 306d 207b 7661 6c75  me}\033[0m {valu
-00001d10: 657d 2c20 6474 7970 653a 207b 6835 6f62  e}, dtype: {h5ob
-00001d20: 6a2e 6474 7970 657d 220d 0a0d 0a20 2020  j.dtype}"....   
-00001d30: 2064 6566 205f 5f4e 4464 6174 6173 6574   def __NDdataset
-00001d40: 5f5f 2873 656c 662c 206e 616d 652c 2068  __(self, name, h
-00001d50: 356f 626a 3a20 6835 7079 2e44 6174 6173  5obj: h5py.Datas
-00001d60: 6574 293a 0d0a 2020 2020 2020 2020 2222  et):..        ""
-00001d70: 2273 7472 696e 6720 7265 7072 6573 656e  "string represen
-00001d80: 7461 7469 6f6e 206f 6620 6120 4e44 2064  tation of a ND d
-00001d90: 6174 6173 6574 2222 220d 0a20 2020 2020  ataset"""..     
-00001da0: 2020 2072 6574 7572 6e20 6622 5c30 3333     return f"\033
-00001db0: 5b31 6d7b 6e61 6d65 7d5c 3033 335b 306d  [1m{name}\033[0m
-00001dc0: 3a20 7b68 356f 626a 2e73 6861 7065 7d2c  : {h5obj.shape},
-00001dd0: 2064 7479 7065 3a20 7b68 356f 626a 2e64   dtype: {h5obj.d
-00001de0: 7479 7065 7d22 0d0a 0d0a 2020 2020 6465  type}"....    de
-00001df0: 6620 5f5f 6772 6f75 705f 5f28 7365 6c66  f __group__(self
-00001e00: 2c20 6e61 6d65 2c20 6974 656d 2920 2d3e  , name, item) ->
-00001e10: 2073 7472 3a0d 0a20 2020 2020 2020 2072   str:..        r
-00001e20: 6574 7572 6e20 6622 2f5c 3033 335b 316d  eturn f"/\033[1m
-00001e30: 7b6e 616d 657d 5c30 3333 5b30 6d22 0d0a  {name}\033[0m"..
-00001e40: 0d0a 2020 2020 6465 6620 5f5f 6174 7472  ..    def __attr
-00001e50: 735f 5f28 7365 6c66 2c20 6e61 6d65 2c20  s__(self, name, 
-00001e60: 7661 6c75 6529 202d 3e20 7374 723a 0d0a  value) -> str:..
-00001e70: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00001e80: 275c 3033 335b 336d 613a 207b 6e61 6d65  '\033[3ma: {name
-00001e90: 7d5c 3033 335b 306d 3a20 7b76 616c 7565  }\033[0m: {value
-00001ea0: 7d27 0d0a 0d0a 0d0a 636c 6173 7320 4844  }'......class HD
-00001eb0: 4635 5374 7275 6374 7572 6548 544d 4c52  F5StructureHTMLR
-00001ec0: 6570 7228 5f48 4446 3553 7472 7563 7475  epr(_HDF5Structu
-00001ed0: 7265 5265 7072 293a 0d0a 0d0a 2020 2020  reRepr):....    
-00001ee0: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-00001ef0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-00001f00: 2020 2020 2067 726f 7570 2c0d 0a20 2020       group,..   
-00001f10: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001f20: 6c6c 6170 7365 643a 2062 6f6f 6c20 3d20  llapsed: bool = 
-00001f30: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00001f40: 2020 2020 2020 2020 7072 6561 6d62 6c65          preamble
-00001f50: 3a20 7374 7220 3d20 4e6f 6e65 2c0d 0a20  : str = None,.. 
-00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f70: 696e 6465 6e74 3a20 696e 7420 3d20 302c  indent: int = 0,
-00001f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001f90: 2020 2063 6875 6e6b 733a 2062 6f6f 6c20     chunks: bool 
-00001fa0: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-00001fb0: 2020 2020 2020 2020 2020 206d 6178 7368             maxsh
-00001fc0: 6170 653a 2062 6f6f 6c20 3d20 4661 6c73  ape: bool = Fals
-00001fd0: 6529 3a0d 0a20 2020 2020 2020 2069 6620  e):..        if 
-00001fe0: 6973 696e 7374 616e 6365 2867 726f 7570  isinstance(group
-00001ff0: 2c20 6835 7079 2e47 726f 7570 293a 0d0a  , h5py.Group):..
-00002000: 2020 2020 2020 2020 2020 2020 6835 6772              h5gr
-00002010: 6f75 7020 3d20 6772 6f75 700d 0a20 2020  oup = group..   
-00002020: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00002030: 2020 2020 2020 2020 6835 6772 6f75 7020          h5group 
-00002040: 3d20 6772 6f75 705b 272f 275d 0d0a 0d0a  = group['/']....
-00002050: 2020 2020 2020 2020 7365 6c66 2e63 6f6c          self.col
-00002060: 6c61 7073 6564 203d 2063 6f6c 6c61 7073  lapsed = collaps
-00002070: 6564 0d0a 0d0a 2020 2020 2020 2020 7365  ed....        se
-00002080: 6c66 2e5f 6f62 6a5f 6366 672e 7570 6461  lf._obj_cfg.upda
-00002090: 7465 287b 2763 6875 6e6b 7327 3a20 6368  te({'chunks': ch
-000020a0: 756e 6b73 2c0d 0a20 2020 2020 2020 2020  unks,..         
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2020 2027 6d61 7873 6861 7065 273a       'maxshape':
-000020d0: 206d 6178 7368 6170 657d 290d 0a0d 0a20   maxshape}).... 
-000020e0: 2020 2020 2020 205f 6964 203d 2068 3567         _id = h5g
-000020f0: 726f 7570 2e6e 616d 6520 2b20 7065 7266  roup.name + perf
-00002100: 5f63 6f75 6e74 6572 5f6e 7328 292e 5f5f  _counter_ns().__
-00002110: 7374 725f 5f28 290d 0a0d 0a20 2020 2020  str__()....     
-00002120: 2020 205f 6874 6d6c 203d 2066 273c 6865     _html = f'<he
-00002130: 6164 3e3c 7374 796c 653e 7b43 5353 5f53  ad><style>{CSS_S
-00002140: 5452 7d3c 2f73 7479 6c65 3e3c 2f68 6561  TR}</style></hea
-00002150: 643e 270d 0a20 2020 2020 2020 2069 6620  d>'..        if 
-00002160: 7072 6561 6d62 6c65 3a0d 0a20 2020 2020  preamble:..     
-00002170: 2020 2020 2020 205f 6874 6d6c 202b 3d20         _html += 
-00002180: 6627 5c6e 7b70 7265 616d 626c 657d 5c6e  f'\n{preamble}\n
-00002190: 270d 0a20 2020 2020 2020 205f 6874 6d6c  '..        _html
-000021a0: 202b 3d20 225c 6e3c 6469 7620 636c 6173   += "\n<div clas
-000021b0: 733d 2768 3574 622d 7761 7270 273e 220d  s='h5tb-warp'>".
-000021c0: 0a20 2020 2020 2020 205f 6874 6d6c 202b  .        _html +
-000021d0: 3d20 7365 6c66 2e5f 5f67 726f 7570 5f5f  = self.__group__
-000021e0: 2868 3567 726f 7570 2e6e 616d 652e 7273  (h5group.name.rs
-000021f0: 706c 6974 2827 2f27 2c20 3129 5b31 5d2c  plit('/', 1)[1],
-00002200: 2068 3567 726f 7570 290d 0a20 2020 2020   h5group)..     
-00002210: 2020 205f 6874 6d6c 202b 3d20 225c 6e3c     _html += "\n<
-00002220: 2f64 6976 3e22 0d0a 2020 2020 2020 2020  /div>"..        
-00002230: 7265 7475 726e 205f 6874 6d6c 0d0a 0d0a  return _html....
-00002240: 2020 2020 6465 6620 5f5f 7374 7269 6e67      def __string
-00002250: 6461 7461 7365 745f 5f28 7365 6c66 2c20  dataset__(self, 
-00002260: 6e61 6d65 2c20 6835 6f62 6a29 202d 3e20  name, h5obj) -> 
-00002270: 7374 723a 0d0a 2020 2020 2020 2020 6966  str:..        if
-00002280: 2068 356f 626a 2e6e 6469 6d20 3d3d 2030   h5obj.ndim == 0
-00002290: 3a0d 0a20 2020 2020 2020 2020 2020 205f  :..            _
-000022a0: 7063 6e73 203d 2070 6572 665f 636f 756e  pcns = perf_coun
-000022b0: 7465 725f 6e73 2829 2e5f 5f73 7472 5f5f  ter_ns().__str__
-000022c0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000022d0: 5f69 6431 203d 2066 2764 732d 312d 7b68  _id1 = f'ds-1-{h
-000022e0: 356f 626a 2e6e 616d 657d 2d7b 5f70 636e  5obj.name}-{_pcn
-000022f0: 737d 3127 0d0a 2020 2020 2020 2020 2020  s}1'..          
-00002300: 2020 5f69 6432 203d 2066 2764 732d 322d    _id2 = f'ds-2-
-00002310: 7b68 356f 626a 2e6e 616d 657d 2d7b 5f70  {h5obj.name}-{_p
-00002320: 636e 737d 3227 0d0a 2020 2020 2020 2020  cns}2'..        
-00002330: 2020 2020 7265 7475 726e 2066 2222 225c      return f"""\
-00002340: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00002350: 2020 2020 2020 203c 756c 2069 643d 227b         <ul id="{
-00002360: 5f69 6431 7d22 2063 6c61 7373 3d22 6835  _id1}" class="h5
-00002370: 7462 2d76 6172 2d6c 6973 7422 3e0d 0a20  tb-var-list">.. 
-00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002390: 2020 203c 696e 7075 7420 6964 3d22 7b5f     <input id="{_
-000023a0: 6964 327d 2220 636c 6173 733d 2268 3574  id2}" class="h5t
-000023b0: 622d 7661 726e 616d 652d 696e 2220 7479  b-varname-in" ty
-000023c0: 7065 3d22 6368 6563 6b62 6f78 2220 7b73  pe="checkbox" {s
-000023d0: 656c 662e 6368 6563 6b62 6f78 5f73 7461  elf.checkbox_sta
-000023e0: 7465 7d3e 0d0a 2020 2020 2020 2020 2020  te}>..          
-000023f0: 2020 2020 2020 2020 2020 3c6c 6162 656c            <label
-00002400: 2063 6c61 7373 3d27 6835 7462 2d76 6172   class='h5tb-var
-00002410: 6e61 6d65 2720 0d0a 2020 2020 2020 2020  name' ..        
-00002420: 2020 2020 2020 2020 2020 2020 666f 723d              for=
-00002430: 227b 5f69 6432 7d22 3e7b 6e61 6d65 7d3c  "{_id2}">{name}<
-00002440: 2f6c 6162 656c 3e3a 205b 7b68 356f 626a  /label>: [{h5obj
-00002450: 2e64 7479 7065 7d5d 2064 6174 613d 7b68  .dtype}] data={h
-00002460: 356f 626a 2e76 616c 7565 735b 2829 5d7d  5obj.values[()]}
-00002470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002480: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00002490: 2020 2065 6c69 6620 6835 6f62 6a2e 6e64     elif h5obj.nd
-000024a0: 696d 203d 3d20 313a 0d0a 2020 2020 2020  im == 1:..      
-000024b0: 2020 2020 2020 5f70 636e 7320 3d20 7065        _pcns = pe
-000024c0: 7266 5f63 6f75 6e74 6572 5f6e 7328 292e  rf_counter_ns().
-000024d0: 5f5f 7374 725f 5f28 290d 0a20 2020 2020  __str__()..     
-000024e0: 2020 2020 2020 205f 6964 3120 3d20 6627         _id1 = f'
-000024f0: 6473 2d31 2d7b 6835 6f62 6a2e 6e61 6d65  ds-1-{h5obj.name
-00002500: 7d2d 7b5f 7063 6e73 7d31 270d 0a20 2020  }-{_pcns}1'..   
-00002510: 2020 2020 2020 2020 205f 6964 3220 3d20           _id2 = 
-00002520: 6627 6473 2d32 2d7b 6835 6f62 6a2e 6e61  f'ds-2-{h5obj.na
-00002530: 6d65 7d2d 7b5f 7063 6e73 7d32 270d 0a20  me}-{_pcns}2'.. 
-00002540: 2020 2020 2020 2020 2020 205f 7374 7264             _strd
-00002550: 6174 6120 3d20 6835 6f62 6a5b 2829 5d0d  ata = h5obj[()].
-00002560: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002570: 6973 696e 7374 616e 6365 285f 7374 7264  isinstance(_strd
-00002580: 6174 612c 2078 722e 4461 7461 4172 7261  ata, xr.DataArra
-00002590: 7929 3a0d 0a20 2020 2020 2020 2020 2020  y):..           
-000025a0: 2020 2020 2072 6574 7572 6e20 6622 2222       return f"""
-000025b0: 5c6e 0d0a 2020 2020 2020 2020 2020 2020  \n..            
-000025c0: 2020 2020 2020 2020 2020 2020 3c75 6c20              <ul 
-000025d0: 6964 3d22 7b5f 6964 317d 2220 636c 6173  id="{_id1}" clas
-000025e0: 733d 2268 3574 622d 7661 722d 6c69 7374  s="h5tb-var-list
-000025f0: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-00002600: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-00002610: 7574 2069 643d 227b 5f69 6432 7d22 2063  ut id="{_id2}" c
-00002620: 6c61 7373 3d22 6835 7462 2d76 6172 6e61  lass="h5tb-varna
-00002630: 6d65 2d69 6e22 2074 7970 653d 2263 6865  me-in" type="che
-00002640: 636b 626f 7822 207b 7365 6c66 2e63 6865  ckbox" {self.che
-00002650: 636b 626f 785f 7374 6174 657d 3e0d 0a20  ckbox_state}>.. 
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 2020 2020 203c 6c61 6265 6c20 636c         <label cl
-00002680: 6173 733d 2768 3574 622d 7661 726e 616d  ass='h5tb-varnam
-00002690: 6527 0d0a 2020 2020 2020 2020 2020 2020  e'..            
-000026a0: 2020 2020 2020 2020 2020 2020 666f 723d              for=
-000026b0: 227b 5f69 6432 7d22 3e7b 6e61 6d65 7d3c  "{_id2}">{name}<
-000026c0: 2f6c 6162 656c 3e3a 205b 7b68 356f 626a  /label>: [{h5obj
-000026d0: 2e64 7479 7065 7d5d 0d0a 2020 2020 2020  .dtype}]..      
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2222 220d 0a20 2020 2020 2020 2020    """..         
-00002700: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00002710: 2020 2020 2020 2020 2073 7472 5f76 616c           str_val
-00002720: 7565 7320 3d20 272c 2027 2e6a 6f69 6e28  ues = ', '.join(
-00002730: 5f73 7472 6461 7461 290d 0a20 2020 2020  _strdata)..     
-00002740: 2020 2020 2020 2065 7863 6570 7420 556e         except Un
-00002750: 6963 6f64 6544 6563 6f64 6545 7272 6f72  icodeDecodeError
-00002760: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002770: 2020 2073 7472 5f76 616c 7565 7320 3d20     str_values = 
-00002780: 273c 693e 556e 6963 6f64 6544 6563 6f64  '<i>UnicodeDecod
-00002790: 6545 7272 6f72 3c2f 693e 270d 0a20 2020  eError</i>'..   
-000027a0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-000027b0: 5479 7065 4572 726f 723a 0d0a 2020 2020  TypeError:..    
-000027c0: 2020 2020 2020 2020 2020 2020 7374 725f              str_
-000027d0: 7661 6c75 6573 203d 2066 273c 693e 5479  values = f'<i>Ty
-000027e0: 7065 4572 726f 723a 207b 7479 7065 285f  peError: {type(_
-000027f0: 7374 7264 6174 6129 7d3c 2f69 3e27 0d0a  strdata)}</i>'..
-00002800: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002810: 726e 2066 2222 225c 6e0d 0a20 2020 2020  rn f"""\n..     
-00002820: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002830: 756c 2069 643d 227b 5f69 6431 7d22 2063  ul id="{_id1}" c
-00002840: 6c61 7373 3d22 6835 7462 2d76 6172 2d6c  lass="h5tb-var-l
-00002850: 6973 7422 3e0d 0a20 2020 2020 2020 2020  ist">..         
-00002860: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
-00002870: 7420 6964 3d22 7b5f 6964 327d 2220 636c  t id="{_id2}" cl
-00002880: 6173 733d 2268 3574 622d 7661 726e 616d  ass="h5tb-varnam
-00002890: 652d 696e 2220 7479 7065 3d22 6368 6563  e-in" type="chec
-000028a0: 6b62 6f78 2220 7b73 656c 662e 6368 6563  kbox" {self.chec
-000028b0: 6b62 6f78 5f73 7461 7465 7d3e 0d0a 2020  kbox_state}>..  
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028d0: 2020 3c6c 6162 656c 2063 6c61 7373 3d27    <label class='
-000028e0: 6835 7462 2d76 6172 6e61 6d65 270d 0a20  h5tb-varname'.. 
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2066 6f72 3d22 7b5f 6964 327d 223e     for="{_id2}">
-00002910: 7b6e 616d 657d 3c2f 6c61 6265 6c3e 3a20  {name}</label>: 
-00002920: 5b7b 6835 6f62 6a2e 6474 7970 657d 5d20  [{h5obj.dtype}] 
-00002930: 6461 7461 3d22 7b73 7472 5f76 616c 7565  data="{str_value
-00002940: 737d 220d 0a20 2020 2020 2020 2020 2020  s}"..           
-00002950: 2020 2020 2020 2020 2022 2222 0d0a 2020           """..  
-00002960: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002970: 662e 5f5f 4e44 6461 7461 7365 745f 5f28  f.__NDdataset__(
-00002980: 6e61 6d65 2c20 6835 6f62 6a29 0d0a 0d0a  name, h5obj)....
-00002990: 2020 2020 6465 6620 5f5f 3044 6461 7461      def __0Ddata
-000029a0: 7365 745f 5f28 7365 6c66 2c20 6e61 6d65  set__(self, name
-000029b0: 3a20 7374 722c 2068 356f 626a 3a20 6835  : str, h5obj: h5
-000029c0: 7079 2e44 6174 6173 6574 2920 2d3e 2073  py.Dataset) -> s
-000029d0: 7472 3a0d 0a20 2020 2020 2020 205f 6964  tr:..        _id
-000029e0: 3120 3d20 6627 6473 2d31 2d7b 6835 6f62  1 = f'ds-1-{h5ob
-000029f0: 6a2e 6e61 6d65 7d2d 7b70 6572 665f 636f  j.name}-{perf_co
-00002a00: 756e 7465 725f 6e73 2829 2e5f 5f73 7472  unter_ns().__str
-00002a10: 5f5f 2829 7d27 0d0a 2020 2020 2020 2020  __()}'..        
-00002a20: 5f69 6432 203d 2066 2764 732d 322d 7b68  _id2 = f'ds-2-{h
-00002a30: 356f 626a 2e6e 616d 657d 2d7b 7065 7266  5obj.name}-{perf
-00002a40: 5f63 6f75 6e74 6572 5f6e 7328 292e 5f5f  _counter_ns().__
-00002a50: 7374 725f 5f28 297d 270d 0a20 2020 2020  str__()}'..     
-00002a60: 2020 2075 6e69 7473 203d 2068 356f 626a     units = h5obj
-00002a70: 2e61 7474 7273 2e67 6574 2827 756e 6974  .attrs.get('unit
-00002a80: 7327 2c20 2727 290d 0a20 2020 2020 2020  s', '')..       
-00002a90: 205f 6874 6d6c 203d 2066 2222 225c 6e0d   _html = f"""\n.
-00002aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ab0: 203c 756c 2069 643d 227b 5f69 6431 7d22   <ul id="{_id1}"
-00002ac0: 2063 6c61 7373 3d22 6835 7462 2d76 6172   class="h5tb-var
-00002ad0: 2d6c 6973 7422 3e0d 0a20 2020 2020 2020  -list">..       
-00002ae0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00002af0: 6964 3d22 7b5f 6964 327d 2220 636c 6173  id="{_id2}" clas
-00002b00: 733d 2268 3574 622d 7661 726e 616d 652d  s="h5tb-varname-
-00002b10: 696e 2220 7479 7065 3d22 6368 6563 6b62  in" type="checkb
-00002b20: 6f78 2220 7b73 656c 662e 6368 6563 6b62  ox" {self.checkb
-00002b30: 6f78 5f73 7461 7465 7d3e 0d0a 2020 2020  ox_state}>..    
-00002b40: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
-00002b50: 656c 2063 6c61 7373 3d27 6835 7462 2d76  el class='h5tb-v
-00002b60: 6172 6e61 6d65 2720 666f 723d 227b 5f69  arname' for="{_i
-00002b70: 6432 7d22 3e7b 6e61 6d65 7d3c 2f6c 6162  d2}">{name}</lab
-00002b80: 656c 3e0d 0a20 2020 2020 2020 2020 2020  el>..           
-00002b90: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-00002ba0: 3d22 6835 7462 2d64 696d 7322 3e7b 6835  ="h5tb-dims">{h5
-00002bb0: 6f62 6a2e 7661 6c75 6573 5b28 295d 7d20  obj.values[()]} 
-00002bc0: 5b7b 756e 6974 737d 5d20 287b 6835 6f62  [{units}] ({h5ob
-00002bd0: 6a2e 6474 7970 657d 293c 2f73 7061 6e3e  j.dtype})</span>
-00002be0: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-00002bf0: 7572 6e20 5f68 746d 6c0d 0a0d 0a20 2020  urn _html....   
-00002c00: 2064 6566 205f 5f4e 4464 6174 6173 6574   def __NDdataset
-00002c10: 5f5f 2873 656c 662c 206e 616d 652c 2068  __(self, name, h
-00002c20: 356f 626a 3a20 6835 7079 2e44 6174 6173  5obj: h5py.Datas
-00002c30: 6574 293a 0d0a 2020 2020 2020 2020 6473  et):..        ds
-00002c40: 5f64 6972 6e61 6d65 203d 206f 732e 7061  _dirname = os.pa
-00002c50: 7468 2e64 6972 6e61 6d65 2868 356f 626a  th.dirname(h5obj
-00002c60: 2e6e 616d 6529 0d0a 2020 2020 2020 2020  .name)..        
-00002c70: 5f73 6861 7065 203d 2068 356f 626a 2e73  _shape = h5obj.s
-00002c80: 6861 7065 0d0a 2020 2020 2020 2020 6966  hape..        if
-00002c90: 2067 6574 5f63 6f6e 6669 6728 2761 6476   get_config('adv
-00002ca0: 616e 6365 645f 7368 6170 655f 7265 7072  anced_shape_repr
-00002cb0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-00002cc0: 205f 7368 6170 655f 7265 7072 203d 2027   _shape_repr = '
-00002cd0: 2827 0d0a 2020 2020 2020 2020 2020 2020  ('..            
-00002ce0: 6e64 696d 203d 2068 356f 626a 2e6e 6469  ndim = h5obj.ndi
-00002cf0: 6d0d 0a20 2020 2020 2020 2020 2020 2066  m..            f
-00002d00: 6f72 2069 2069 6e20 7261 6e67 6528 6e64  or i in range(nd
-00002d10: 696d 293a 0d0a 2020 2020 2020 2020 2020  im):..          
-00002d20: 2020 2020 2020 6f72 6967 5f64 696d 5f6e        orig_dim_n
-00002d30: 616d 6520 3d20 4e6f 6e65 0d0a 2020 2020  ame = None..    
-00002d40: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00002d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002d60: 2020 2020 2020 6f72 6967 5f64 696d 5f6e        orig_dim_n
-00002d70: 616d 6520 3d20 6835 6f62 6a2e 6469 6d73  ame = h5obj.dims
-00002d80: 5b69 5d5b 305d 2e6e 616d 650d 0a20 2020  [i][0].name..   
-00002d90: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00002da0: 6570 7420 5275 6e74 696d 6545 7272 6f72  ept RuntimeError
-00002db0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002dc0: 2020 2020 2020 2070 6173 7320 2023 206e         pass  # n
-00002dd0: 6f20 6469 6d65 6e73 696f 6e20 7363 616c  o dimension scal
-00002de0: 6520 636f 756c 6420 6265 2066 6f75 6e64  e could be found
-00002df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e00: 2020 6966 206f 7269 675f 6469 6d5f 6e61    if orig_dim_na
-00002e10: 6d65 3a0d 0a20 2020 2020 2020 2020 2020  me:..           
-00002e20: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
-00002e30: 6174 682e 6469 726e 616d 6528 6f72 6967  ath.dirname(orig
-00002e40: 5f64 696d 5f6e 616d 6529 203d 3d20 6473  _dim_name) == ds
-00002e50: 5f64 6972 6e61 6d65 3a0d 0a20 2020 2020  _dirname:..     
-00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e70: 2020 2064 696d 5f6e 616d 6520 3d20 6f73     dim_name = os
-00002e80: 2e70 6174 682e 6261 7365 6e61 6d65 286f  .path.basename(o
-00002e90: 7269 675f 6469 6d5f 6e61 6d65 290d 0a20  rig_dim_name).. 
-00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002eb0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 6469 6d5f 6e61 6d65 203d 206f 7269    dim_name = ori
-00002ee0: 675f 6469 6d5f 6e61 6d65 0d0a 2020 2020  g_dim_name..    
-00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f00: 6966 2069 203d 3d20 303a 0d0a 2020 2020  if i == 0:..    
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 5f73 6861 7065 5f72 6570 7220      _shape_repr 
-00002f30: 2b3d 2066 277b 6469 6d5f 6e61 6d65 7d3a  += f'{dim_name}:
-00002f40: 207b 5f73 6861 7065 5b69 5d7d 270d 0a20   {_shape[i]}'.. 
-00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f60: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f80: 2020 5f73 6861 7065 5f72 6570 7220 2b3d    _shape_repr +=
-00002f90: 2066 272c 207b 6469 6d5f 6e61 6d65 7d3a   f', {dim_name}:
-00002fa0: 207b 5f73 6861 7065 5b69 5d7d 270d 0a20   {_shape[i]}'.. 
-00002fb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002fc0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00002fd0: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
-00002fe0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-00002ff0: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
-00003000: 6861 7065 5f72 6570 7220 2b3d 2066 277b  hape_repr += f'{
-00003010: 5f73 6861 7065 5b69 5d7d 270d 0a20 2020  _shape[i]}'..   
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 5f73 6861 7065 5f72 6570 7220 2b3d 2066  _shape_repr += f
-00003060: 272c 207b 5f73 6861 7065 5b69 5d7d 270d  ', {_shape[i]}'.
-00003070: 0a20 2020 2020 2020 2020 2020 205f 7368  .            _sh
-00003080: 6170 655f 7265 7072 202b 3d20 2729 270d  ape_repr += ')'.
-00003090: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000030a0: 5f73 6861 7065 5f72 6570 7220 3d3d 2027  _shape_repr == '
-000030b0: 2829 2720 616e 6420 6e64 696d 203e 2030  ()' and ndim > 0
-000030c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000030d0: 2020 205f 7368 6170 655f 7265 7072 203d     _shape_repr =
-000030e0: 205f 7368 6170 650d 0a20 2020 2020 2020   _shape..       
-000030f0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00003100: 2020 2020 5f73 6861 7065 5f72 6570 7220      _shape_repr 
-00003110: 3d20 5f73 6861 7065 0d0a 0d0a 2020 2020  = _shape....    
-00003120: 2020 2020 6966 2073 656c 662e 5f6f 626a      if self._obj
-00003130: 5f63 6667 5b27 6368 756e 6b73 275d 3a0d  _cfg['chunks']:.
-00003140: 0a20 2020 2020 2020 2020 2020 2063 6875  .            chu
-00003150: 6e6b 735f 7374 7220 3d20 6627 2063 6875  nks_str = f' chu
-00003160: 6e6b 733d 7b68 356f 626a 2e63 6875 6e6b  nks={h5obj.chunk
-00003170: 737d 270d 0a20 2020 2020 2020 2065 6c73  s}'..        els
-00003180: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00003190: 6368 756e 6b73 5f73 7472 203d 2027 270d  chunks_str = ''.
-000031a0: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
-000031b0: 6c66 2e5f 6f62 6a5f 6366 675b 276d 6178  lf._obj_cfg['max
-000031c0: 7368 6170 6527 5d3a 0d0a 2020 2020 2020  shape']:..      
-000031d0: 2020 2020 2020 6d61 7873 6861 7065 5f73        maxshape_s
-000031e0: 7472 203d 2066 2720 6d61 7873 6861 7065  tr = f' maxshape
-000031f0: 3d7b 6835 6f62 6a2e 6d61 7873 6861 7065  ={h5obj.maxshape
-00003200: 7d27 0d0a 2020 2020 2020 2020 656c 7365  }'..        else
-00003210: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
-00003220: 6178 7368 6170 655f 7374 7220 3d20 2727  axshape_str = ''
-00003230: 0d0a 0d0a 2020 2020 2020 2020 5f69 6431  ....        _id1
-00003240: 203d 2066 2764 732d 312d 7b68 356f 626a   = f'ds-1-{h5obj
-00003250: 2e6e 616d 657d 2d7b 7065 7266 5f63 6f75  .name}-{perf_cou
-00003260: 6e74 6572 5f6e 7328 292e 5f5f 7374 725f  nter_ns().__str_
-00003270: 5f28 297d 270d 0a20 2020 2020 2020 205f  _()}'..        _
-00003280: 6964 3220 3d20 6627 6473 2d32 2d7b 6835  id2 = f'ds-2-{h5
-00003290: 6f62 6a2e 6e61 6d65 7d2d 7b70 6572 665f  obj.name}-{perf_
-000032a0: 636f 756e 7465 725f 6e73 2829 2e5f 5f73  counter_ns().__s
-000032b0: 7472 5f5f 2829 7d27 0d0a 0d0a 2020 2020  tr__()}'....    
-000032c0: 2020 2020 5f68 746d 6c20 3d20 6622 2222      _html = f"""
-000032d0: 5c6e 0d0a 2020 2020 2020 2020 2020 2020  \n..            
-000032e0: 2020 2020 3c75 6c20 6964 3d22 7b5f 6964      <ul id="{_id
-000032f0: 317d 2220 636c 6173 733d 2268 3574 622d  1}" class="h5tb-
-00003300: 7661 722d 6c69 7374 223e 0d0a 2020 2020  var-list">..    
-00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003320: 3c69 6e70 7574 2069 643d 227b 5f69 6432  <input id="{_id2
-00003330: 7d22 2063 6c61 7373 3d22 6835 7462 2d76  }" class="h5tb-v
-00003340: 6172 6e61 6d65 2d69 6e22 2074 7970 653d  arname-in" type=
-00003350: 2263 6865 636b 626f 7822 207b 7365 6c66  "checkbox" {self
-00003360: 2e63 6865 636b 626f 785f 7374 6174 657d  .checkbox_state}
-00003370: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00003380: 2020 2020 2020 203c 6c61 6265 6c20 636c         <label cl
-00003390: 6173 733d 2768 3574 622d 7661 726e 616d  ass='h5tb-varnam
-000033a0: 6527 2066 6f72 3d22 7b5f 6964 327d 223e  e' for="{_id2}">
-000033b0: 7b6e 616d 657d 3c2f 6c61 6265 6c3e 0d0a  {name}</label>..
-000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033d0: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-000033e0: 2268 3574 622d 6469 6d73 223e 7b5f 7368  "h5tb-dims">{_sh
-000033f0: 6170 655f 7265 7072 7d20 5b7b 6835 6f62  ape_repr} [{h5ob
-00003400: 6a2e 6474 7970 657d 5d7b 6368 756e 6b73  j.dtype}]{chunks
-00003410: 5f73 7472 7d7b 6d61 7873 6861 7065 5f73  _str}{maxshape_s
-00003420: 7472 7d3c 2f73 7061 6e3e 2222 220d 0a20  tr}</span>""".. 
-00003430: 2020 2020 2020 2072 6574 7572 6e20 5f68         return _h
-00003440: 746d 6c0d 0a0d 0a20 2020 2064 6566 205f  tml....    def _
-00003450: 5f64 6174 6173 6574 5f5f 2873 656c 662c  _dataset__(self,
-00003460: 206e 616d 652c 2068 356f 626a 2920 2d3e   name, h5obj) ->
-00003470: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
-00003480: 2222 6765 6e65 7261 7465 2068 746d 6c20  ""generate html 
-00003490: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-000034a0: 6620 6120 6461 7461 7365 7422 2222 0d0a  f a dataset"""..
-000034b0: 0d0a 2020 2020 2020 2020 6972 6920 3d20  ..        iri = 
-000034c0: 6835 6f62 6a2e 6972 692e 7375 626a 6563  h5obj.iri.subjec
-000034d0: 740d 0a20 2020 2020 2020 2069 6620 6972  t..        if ir
-000034e0: 6920 6973 206e 6f74 204e 6f6e 653a 0d0a  i is not None:..
-000034f0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00003500: 202b 3d20 6765 745f 6972 695f 6963 6f6e   += get_iri_icon
-00003510: 5f68 7265 6628 6972 6929 0d0a 0d0a 2020  _href(iri)....  
-00003520: 2020 2020 2020 6973 5f73 7472 696e 675f        is_string_
-00003530: 6461 7461 7365 7420 3d20 6835 6f62 6a2e  dataset = h5obj.
-00003540: 6474 7970 652e 6368 6172 203d 3d20 2753  dtype.char == 'S
-00003550: 270d 0a20 2020 2020 2020 2069 6620 6973  '..        if is
-00003560: 5f73 7472 696e 675f 6461 7461 7365 743a  _string_dataset:
-00003570: 0d0a 2020 2020 2020 2020 2020 2020 5f68  ..            _h
-00003580: 746d 6c5f 7072 6520 3d20 7365 6c66 2e5f  tml_pre = self._
-00003590: 5f73 7472 696e 6764 6174 6173 6574 5f5f  _stringdataset__
-000035a0: 286e 616d 652c 2068 356f 626a 290d 0a20  (name, h5obj).. 
-000035b0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000035c0: 2020 2020 2020 2020 2020 6966 2068 356f            if h5o
-000035d0: 626a 2e6e 6469 6d20 3d3d 2030 3a0d 0a20  bj.ndim == 0:.. 
-000035e0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-000035f0: 6874 6d6c 5f70 7265 203d 2073 656c 662e  html_pre = self.
-00003600: 5f5f 3044 6461 7461 7365 745f 5f28 6e61  __0Ddataset__(na
-00003610: 6d65 2c20 6835 6f62 6a29 0d0a 2020 2020  me, h5obj)..    
-00003620: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00003630: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00003640: 6874 6d6c 5f70 7265 203d 2073 656c 662e  html_pre = self.
-00003650: 5f5f 4e44 6461 7461 7365 745f 5f28 6e61  __NDdataset__(na
-00003660: 6d65 2c20 6835 6f62 6a29 0d0a 0d0a 2020  me, h5obj)....  
-00003670: 2020 2020 2020 2320 6e6f 7720 616c 6c20        # now all 
-00003680: 6174 7472 6962 7574 6573 206f 6620 7468  attributes of th
-00003690: 6520 6461 7461 7365 743a 0d0a 2020 2020  e dataset:..    
-000036a0: 2020 2020 2320 6f70 656e 2061 7474 7269      # open attri
-000036b0: 6275 7465 2073 6563 7469 6f6e 3a0d 0a20  bute section:.. 
-000036c0: 2020 2020 2020 205f 6874 6d6c 5f64 735f         _html_ds_
-000036d0: 6174 7472 7320 3d20 2222 225c 6e20 2020  attrs = """\n   
-000036e0: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
-000036f0: 2063 6c61 7373 3d22 6835 7462 2d61 7474   class="h5tb-att
-00003700: 722d 6c69 7374 223e 2222 220d 0a0d 0a20  r-list">""".... 
-00003710: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-00003720: 6835 6f62 6a2e 6174 7472 732e 6b65 7973  h5obj.attrs.keys
-00003730: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00003740: 2069 6620 6b20 6e6f 7420 696e 2073 656c   if k not in sel
-00003750: 662e 6967 6e6f 7265 5f61 7474 7273 2061  f.ignore_attrs a
-00003760: 6e64 206e 6f74 206b 2e69 7375 7070 6572  nd not k.isupper
-00003770: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00003780: 2020 2020 205f 6874 6d6c 5f64 735f 6174       _html_ds_at
-00003790: 7472 7320 2b3d 2073 656c 662e 5f5f 6174  trs += self.__at
-000037a0: 7472 735f 5f28 6b2c 2068 356f 626a 290d  trs__(k, h5obj).
-000037b0: 0a0d 0a20 2020 2020 2020 2023 2063 6c6f  ...        # clo
-000037c0: 7365 2061 7474 7269 6275 7465 2073 6563  se attribute sec
-000037d0: 7469 6f6e 0d0a 2020 2020 2020 2020 5f68  tion..        _h
-000037e0: 746d 6c5f 6473 5f61 7474 7273 202b 3d20  tml_ds_attrs += 
-000037f0: 2222 225c 6e20 2020 2020 2020 2020 2020  """\n           
-00003800: 2020 2020 203c 2f75 6c3e 2222 220d 0a0d       </ul>"""...
-00003810: 0a20 2020 2020 2020 2023 2063 6c6f 7365  .        # close
-00003820: 2064 6174 6173 6574 2073 6563 7469 6f6e   dataset section
-00003830: 0d0a 2020 2020 2020 2020 5f68 746d 6c5f  ..        _html_
-00003840: 706f 7374 203d 2022 2222 5c6e 2020 2020  post = """\n    
-00003850: 2020 2020 2020 2020 2020 2020 3c2f 756c              </ul
-00003860: 3e22 2222 0d0a 2020 2020 2020 2020 5f68  >"""..        _h
-00003870: 746d 6c5f 6473 203d 205f 6874 6d6c 5f70  tml_ds = _html_p
-00003880: 7265 202b 205f 6874 6d6c 5f64 735f 6174  re + _html_ds_at
-00003890: 7472 7320 2b20 5f68 746d 6c5f 706f 7374  trs + _html_post
-000038a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000038b0: 205f 6874 6d6c 5f64 730d 0a0d 0a20 2020   _html_ds....   
-000038c0: 2064 6566 205f 5f67 726f 7570 5f5f 2873   def __group__(s
-000038d0: 656c 662c 206e 616d 652c 2068 356f 626a  elf, name, h5obj
-000038e0: 3a20 6835 7079 2e47 726f 7570 293a 0d0a  : h5py.Group):..
-000038f0: 2020 2020 2020 2020 6e6b 6579 7320 3d20          nkeys = 
-00003900: 6c65 6e28 6835 6f62 6a2e 6b65 7973 2829  len(h5obj.keys()
-00003910: 290d 0a20 2020 2020 2020 205f 6964 203d  )..        _id =
-00003920: 2066 2764 732d 7b6e 616d 657d 2d7b 7065   f'ds-{name}-{pe
-00003930: 7266 5f63 6f75 6e74 6572 5f6e 7328 292e  rf_counter_ns().
-00003940: 5f5f 7374 725f 5f28 297d 270d 0a20 2020  __str__()}'..   
-00003950: 2020 2020 205f 6772 6f75 706e 616d 6520       _groupname 
-00003960: 3d20 6f73 2e70 6174 682e 6261 7365 6e61  = os.path.basena
-00003970: 6d65 2868 356f 626a 2e6e 616d 6529 0d0a  me(h5obj.name)..
-00003980: 0d0a 2020 2020 2020 2020 6966 205f 6772  ..        if _gr
-00003990: 6f75 706e 616d 6520 3d3d 2027 273a 0d0a  oupname == '':..
-000039a0: 2020 2020 2020 2020 2020 2020 5f67 726f              _gro
-000039b0: 7570 6e61 6d65 203d 2027 2f27 2020 2320  upname = '/'  # 
-000039c0: 7265 636f 7665 7220 726f 6f74 206e 616d  recover root nam
-000039d0: 650d 0a20 2020 2020 2020 2020 2020 2063  e..            c
-000039e0: 6865 636b 626f 785f 7374 6174 6520 3d20  heckbox_state = 
-000039f0: 2763 6865 636b 6564 270d 0a20 2020 2020  'checked'..     
-00003a00: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00003a10: 2020 2020 2020 6368 6563 6b62 6f78 5f73        checkbox_s
-00003a20: 7461 7465 203d 2073 656c 662e 6368 6563  tate = self.chec
-00003a30: 6b62 6f78 5f73 7461 7465 0d0a 0d0a 2020  kbox_state....  
-00003a40: 2020 2020 2020 6972 6920 3d20 6835 6f62        iri = h5ob
-00003a50: 6a2e 6972 692e 7375 626a 6563 740d 0a20  j.iri.subject.. 
-00003a60: 2020 2020 2020 2069 6620 6972 6920 6973         if iri is
-00003a70: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00003a80: 2020 2020 2020 2020 5f67 726f 7570 6e61          _groupna
-00003a90: 6d65 202b 3d20 6765 745f 6972 695f 6963  me += get_iri_ic
-00003aa0: 6f6e 5f68 7265 6628 6972 6929 0d0a 2020  on_href(iri)..  
-00003ab0: 2020 2020 2020 5f68 746d 6c20 3d20 6622        _html = f"
-00003ac0: 2222 5c6e 0d0a 2020 2020 2020 2020 2020  ""\n..          
-00003ad0: 2020 2020 3c75 6c20 7374 796c 653d 226c      <ul style="l
-00003ae0: 6973 742d 7374 796c 652d 7479 7065 3a20  ist-style-type: 
-00003af0: 6e6f 6e65 3b22 2063 6c61 7373 3d22 6835  none;" class="h5
-00003b00: 6772 702d 7365 6374 696f 6e73 223e 0d0a  grp-sections">..
-00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b20: 2020 2020 3c6c 693e 0d0a 2020 2020 2020      <li>..      
-00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b40: 2020 3c69 6e70 7574 2069 643d 2267 726f    <input id="gro
-00003b50: 7570 2d7b 5f69 647d 2220 7479 7065 3d22  up-{_id}" type="
-00003b60: 6368 6563 6b62 6f78 2220 7b63 6865 636b  checkbox" {check
-00003b70: 626f 785f 7374 6174 657d 3e0d 0a20 2020  box_state}>..   
-00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b90: 2020 2020 203c 6c61 6265 6c20 7374 796c       <label styl
-00003ba0: 653d 2266 6f6e 742d 7765 6967 6874 3a20  e="font-weight: 
-00003bb0: 626f 6c64 2220 666f 723d 2267 726f 7570  bold" for="group
-00003bc0: 2d7b 5f69 647d 223e 0d0a 2020 2020 2020  -{_id}">..      
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003be0: 2020 7b5f 6772 6f75 706e 616d 657d 3c73    {_groupname}<s
-00003bf0: 7061 6e3e 287b 6e6b 6579 737d 293c 2f73  pan>({nkeys})</s
-00003c00: 7061 6e3e 3c2f 6c61 6265 6c3e 0d0a 2020  pan></label>..  
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2222 220d 0a0d 0a20 2020 2020 2020 205f  """....        _
-00003c30: 6874 6d6c 202b 3d20 2222 225c 6e0d 0a20  html += """\n.. 
-00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 2020 203c 756c 2063 6c61 7373 3d22 6835     <ul class="h5
-00003c60: 7462 2d61 7474 722d 6c69 7374 223e 2222  tb-attr-list">""
-00003c70: 220d 0a20 2020 2020 2020 2023 2077 7269  "..        # wri
-00003c80: 7465 2061 7474 7269 6275 7465 733a 0d0a  te attributes:..
-00003c90: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00003ca0: 2068 356f 626a 2e61 7474 7273 2e6b 6579   h5obj.attrs.key
-00003cb0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00003cc0: 2020 6966 206e 6f74 206b 2e69 7375 7070    if not k.isupp
-00003cd0: 6572 2829 3a0d 0a20 2020 2020 2020 2020  er():..         
-00003ce0: 2020 2020 2020 205f 6874 6d6c 202b 3d20         _html += 
-00003cf0: 7365 6c66 2e5f 5f61 7474 7273 5f5f 286b  self.__attrs__(k
-00003d00: 2c20 6835 6f62 6a29 0d0a 2020 2020 2020  , h5obj)..      
-00003d10: 2020 2320 636c 6f73 6520 6174 7472 6962    # close attrib
-00003d20: 7574 6520 7365 6374 696f 6e0d 0a20 2020  ute section..   
-00003d30: 2020 2020 205f 6874 6d6c 202b 3d20 2222       _html += ""
-00003d40: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00003d50: 2020 2020 2020 203c 2f75 6c3e 2222 220d         </ul>""".
-00003d60: 0a0d 0a20 2020 2020 2020 2064 6174 6173  ...        datas
-00003d70: 6574 7320 3d20 5b28 6b2c 2076 2920 666f  ets = [(k, v) fo
-00003d80: 7220 6b2c 2076 2069 6e20 6835 6f62 6a2e  r k, v in h5obj.
-00003d90: 6974 656d 7328 2920 6966 2069 7369 6e73  items() if isins
-00003da0: 7461 6e63 6528 762c 2068 3570 792e 4461  tance(v, h5py.Da
-00003db0: 7461 7365 7429 5d0d 0a20 2020 2020 2020  taset)]..       
-00003dc0: 2067 726f 7570 7320 3d20 5b28 6b2c 2076   groups = [(k, v
-00003dd0: 2920 666f 7220 6b2c 2076 2069 6e20 6835  ) for k, v in h5
-00003de0: 6f62 6a2e 6974 656d 7328 2920 6966 2069  obj.items() if i
-00003df0: 7369 6e73 7461 6e63 6528 762c 2068 3570  sinstance(v, h5p
-00003e00: 792e 4772 6f75 7029 5d0d 0a0d 0a20 2020  y.Group)]....   
-00003e10: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
-00003e20: 2064 6174 6173 6574 733a 0d0a 2020 2020   datasets:..    
-00003e30: 2020 2020 2020 2020 5f68 746d 6c20 2b3d          _html +=
-00003e40: 2073 656c 662e 5f5f 6461 7461 7365 745f   self.__dataset_
-00003e50: 5f28 6b2c 2076 290d 0a0d 0a20 2020 2020  _(k, v)....     
-00003e60: 2020 2066 6f72 206b 2c20 7620 696e 2067     for k, v in g
-00003e70: 726f 7570 733a 0d0a 2020 2020 2020 2020  roups:..        
-00003e80: 2020 2020 5f68 746d 6c20 2b3d 2073 656c      _html += sel
-00003e90: 662e 5f5f 6772 6f75 705f 5f28 6b2c 2076  f.__group__(k, v
-00003ea0: 290d 0a20 2020 2020 2020 205f 6874 6d6c  )..        _html
-00003eb0: 202b 3d20 275c 6e3c 2f6c 693e 270d 0a20   += '\n</li>'.. 
-00003ec0: 2020 2020 2020 205f 6874 6d6c 202b 3d20         _html += 
-00003ed0: 275c 6e3c 2f75 6c3e 270d 0a20 2020 2020  '\n</ul>'..     
-00003ee0: 2020 2072 6574 7572 6e20 5f68 746d 6c0d     return _html.
-00003ef0: 0a0d 0a20 2020 2064 6566 205f 5f61 7474  ...    def __att
-00003f00: 7273 5f5f 2873 656c 662c 206e 616d 652c  rs__(self, name,
-00003f10: 2068 356f 626a 293a 0d0a 2020 2020 2020   h5obj):..      
-00003f20: 2020 6174 7472 5f76 616c 7565 203d 2068    attr_value = h
-00003f30: 356f 626a 2e61 7474 7273 2e72 6177 5b6e  5obj.attrs.raw[n
-00003f40: 616d 655d 0d0a 0d0a 2020 2020 2020 2020  ame]....        
-00003f50: 6966 2069 7369 6e73 7461 6e63 6528 6174  if isinstance(at
-00003f60: 7472 5f76 616c 7565 2c20 6e70 2e62 7974  tr_value, np.byt
-00003f70: 6573 5f29 3a0d 0a20 2020 2020 2020 2020  es_):..         
-00003f80: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00003f90: 2020 2020 2020 2020 2061 7474 725f 7661           attr_va
-00003fa0: 6c75 6520 3d20 6174 7472 5f76 616c 7565  lue = attr_value
-00003fb0: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-00003fc0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00003fd0: 6365 7074 2055 6e69 636f 6465 4465 636f  cept UnicodeDeco
-00003fe0: 6465 4572 726f 723a 0d0a 2020 2020 2020  deError:..      
-00003ff0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00004000: 6773 2e77 6172 6e28 6627 4361 6e6e 6f74  gs.warn(f'Cannot
-00004010: 2064 6563 6f64 6520 6174 7472 6962 7574   decode attribut
-00004020: 6520 7661 6c75 6520 666f 7220 7b6e 616d  e value for {nam
-00004030: 657d 272c 2052 756e 7469 6d65 5761 726e  e}', RuntimeWarn
-00004040: 696e 6729 0d0a 2020 2020 2020 2020 6972  ing)..        ir
-00004050: 6920 3d20 6835 6f62 6a2e 6972 692e 6765  i = h5obj.iri.ge
-00004060: 7428 6e61 6d65 290d 0a0d 0a20 2020 2020  t(name)....     
-00004070: 2020 2069 7269 5f70 7265 6469 6361 7465     iri_predicate
-00004080: 203d 2069 7269 2e70 7265 6469 6361 7465   = iri.predicate
-00004090: 0d0a 2020 2020 2020 2020 6966 2069 7269  ..        if iri
-000040a0: 5f70 7265 6469 6361 7465 2069 7320 6e6f  _predicate is no
-000040b0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000040c0: 2020 2020 206e 616d 6520 2b3d 2067 6574       name += get
-000040d0: 5f69 7269 5f69 636f 6e5f 6872 6566 2869  _iri_icon_href(i
-000040e0: 7269 5f70 7265 6469 6361 7465 290d 0a0d  ri_predicate)...
-000040f0: 0a20 2020 2020 2020 2069 7269 5f6f 626a  .        iri_obj
-00004100: 6563 7420 3d20 6972 692e 6f62 6a65 6374  ect = iri.object
-00004110: 0d0a 0d0a 2020 2020 2020 2020 6966 2069  ....        if i
-00004120: 7369 6e73 7461 6e63 6528 6174 7472 5f76  sinstance(attr_v
-00004130: 616c 7565 2c20 6e64 6172 7261 7929 3a0d  alue, ndarray):.
-00004140: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00004150: 6620 616c 6c28 6973 696e 7374 616e 6365  f all(isinstance
-00004160: 2869 7465 6d2c 2073 7472 2920 666f 7220  (item, str) for 
-00004170: 6974 656d 2069 6e20 6174 7472 5f76 616c  item in attr_val
-00004180: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
-00004190: 2020 2020 2020 5f73 7472 696e 675f 7661        _string_va
-000041a0: 6c75 655f 6c69 7374 203d 205b 5d0d 0a20  lue_list = [].. 
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000041c0: 6f72 2069 7465 6d20 696e 2061 7474 725f  or item in attr_
-000041d0: 7661 6c75 653a 0d0a 2020 2020 2020 2020  value:..        
-000041e0: 2020 2020 2020 2020 2020 2020 5f76 616c              _val
-000041f0: 7565 2c20 6973 5f75 726c 203d 2070 726f  ue, is_url = pro
-00004200: 6365 7373 5f73 7472 696e 675f 666f 725f  cess_string_for_
-00004210: 6c69 6e6b 2869 7465 6d29 0d0a 2020 2020  link(item)..    
-00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004230: 6966 2069 735f 7572 6c3a 0d0a 2020 2020  if is_url:..    
-00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004250: 2020 2020 5f73 7472 696e 675f 7661 6c75      _string_valu
-00004260: 655f 6c69 7374 2e61 7070 656e 6428 5f76  e_list.append(_v
-00004270: 616c 7565 290d 0a20 2020 2020 2020 2020  alue)..         
-00004280: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00004290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000042a0: 2020 2020 2020 2020 2020 5f73 7472 696e            _strin
-000042b0: 675f 7661 6c75 655f 6c69 7374 2e61 7070  g_value_list.app
-000042c0: 656e 6428 6974 656d 290d 0a20 2020 2020  end(item)..     
-000042d0: 2020 2020 2020 2020 2020 205f 7661 6c75             _valu
-000042e0: 655f 7374 7220 3d20 222c 2022 2e6a 6f69  e_str = ", ".joi
-000042f0: 6e28 5f73 7472 696e 675f 7661 6c75 655f  n(_string_value_
-00004300: 6c69 7374 290d 0a0d 0a20 2020 2020 2020  list)....       
-00004310: 2020 2020 2020 2020 2069 6620 6972 695f           if iri_
-00004320: 6f62 6a65 6374 2069 7320 6e6f 7420 4e6f  object is not No
-00004330: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00004340: 2020 2020 2020 2020 205f 7661 6c75 655f           _value_
-00004350: 7374 7220 2b3d 2067 6574 5f69 7269 5f69  str += get_iri_i
-00004360: 636f 6e5f 6872 6566 2869 7269 5f6f 626a  con_href(iri_obj
-00004370: 6563 7429 0d0a 2020 2020 2020 2020 2020  ect)..          
-00004380: 2020 2020 2020 7265 7475 726e 2027 3c6c        return '<l
-00004390: 6920 7374 796c 653d 226c 6973 742d 7374  i style="list-st
-000043a0: 796c 652d 7479 7065 3a20 6e6f 6e65 3b20  yle-type: none; 
-000043b0: 2720 5c0d 0a20 2020 2020 2020 2020 2020  ' \..           
-000043c0: 2020 2020 2020 2020 2020 2020 6627 666f              f'fo
-000043d0: 6e74 2d73 7479 6c65 3a20 6974 616c 6963  nt-style: italic
-000043e0: 223e 7b6e 616d 657d 203a 207b 5f76 616c  ">{name} : {_val
-000043f0: 7565 5f73 7472 7d3c 2f6c 693e 270d 0a20  ue_str}</li>'.. 
-00004400: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00004410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004420: 2020 5f76 616c 7565 203d 2061 7474 725f    _value = attr_
-00004430: 7661 6c75 652e 5f5f 7265 7072 5f5f 2829  value.__repr__()
-00004440: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00004450: 2020 2020 6966 206c 656e 285f 7661 6c75      if len(_valu
-00004460: 6529 203e 2073 656c 662e 6d61 785f 6174  e) > self.max_at
-00004470: 7472 5f6c 656e 6774 683a 0d0a 2020 2020  tr_length:..    
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 5f76 616c 7565 203d 2066 277b 5f76 616c  _value = f'{_val
-000044a0: 7565 5b30 3a73 656c 662e 6d61 785f 6174  ue[0:self.max_at
-000044b0: 7472 5f6c 656e 6774 685d 7d2e 2e2e 270d  tr_length]}...'.
-000044c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000044d0: 2020 2069 6620 6972 695f 6f62 6a65 6374     if iri_object
-000044e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 205f 7661 6c75 6520 2b3d 2067 6574     _value += get
-00004510: 5f69 7269 5f69 636f 6e5f 6872 6566 2869  _iri_icon_href(i
-00004520: 7269 5f70 7265 6469 6361 7465 290d 0a0d  ri_predicate)...
-00004530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004540: 2072 6574 7572 6e20 6627 3c6c 6920 7374   return f'<li st
-00004550: 796c 653d 226c 6973 742d 7374 796c 652d  yle="list-style-
-00004560: 7479 7065 3a20 6e6f 6e65 3b20 666f 6e74  type: none; font
-00004570: 2d73 7479 6c65 3a20 6974 616c 6963 223e  -style: italic">
-00004580: 7b6e 616d 657d 203a 207b 5f76 616c 7565  {name} : {_value
-00004590: 7d3c 2f6c 693e 270d 0a0d 0a20 2020 2020  }</li>'....     
-000045a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000045b0: 2861 7474 725f 7661 6c75 652c 2073 7472  (attr_value, str
-000045c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000045d0: 5f76 616c 7565 5f73 7472 203d 2066 277b  _value_str = f'{
-000045e0: 6174 7472 5f76 616c 7565 7d27 0d0a 2020  attr_value}'..  
-000045f0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00004600: 285f 7661 6c75 655f 7374 7229 203e 2031  (_value_str) > 1
-00004610: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004620: 2020 2069 6620 5f76 616c 7565 5f73 7472     if _value_str
-00004630: 5b30 5d20 3d3d 2027 3c27 2061 6e64 205f  [0] == '<' and _
-00004640: 7661 6c75 655f 7374 725b 2d31 5d20 3d3d  value_str[-1] ==
-00004650: 2027 3e27 3a0d 0a20 2020 2020 2020 2020   '>':..         
-00004660: 2020 2020 2020 2020 2020 205f 7661 6c75             _valu
-00004670: 655f 7374 7220 3d20 5f76 616c 7565 5f73  e_str = _value_s
-00004680: 7472 5b31 3a2d 315d 0d0a 0d0a 2020 2020  tr[1:-1]....    
-00004690: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-000046a0: 6966 2069 7420 6973 2061 2069 6465 6e74  if it is a ident
-000046b0: 6966 6965 723a 0d0a 2020 2020 2020 2020  ifier:..        
-000046c0: 2020 2020 6964 656e 7469 6669 6572 203d      identifier =
-000046d0: 2069 6465 6e74 6966 6965 7273 2e66 726f   identifiers.fro
-000046e0: 6d5f 7572 6c28 5f76 616c 7565 5f73 7472  m_url(_value_str
-000046f0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00004700: 6620 6964 656e 7469 6669 6572 2069 7320  f identifier is 
-00004710: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00004720: 2020 2020 2020 2020 2020 205f 7661 6c75             _valu
-00004730: 655f 6874 6d6c 203d 2069 6465 6e74 6966  e_html = identif
-00004740: 6965 722e 5f72 6570 725f 6874 6d6c 5f28  ier._repr_html_(
-00004750: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004760: 2020 2069 735f 7572 6c20 3d20 5472 7565     is_url = True
-00004770: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00004780: 7365 3a20 2023 206d 6179 6265 2073 6f6d  se:  # maybe som
-00004790: 6520 6f74 6865 7220 7572 6c3a 0d0a 2020  e other url:..  
-000047a0: 2020 2020 2020 2020 2020 2020 2020 5f76                _v
-000047b0: 616c 7565 5f68 746d 6c2c 2069 735f 7572  alue_html, is_ur
-000047c0: 6c20 3d20 7072 6f63 6573 735f 7374 7269  l = process_stri
-000047d0: 6e67 5f66 6f72 5f6c 696e 6b28 5f76 616c  ng_for_link(_val
-000047e0: 7565 5f73 7472 290d 0a20 2020 2020 2020  ue_str)..       
-000047f0: 2020 2020 2020 2020 2023 2069 6620 6973           # if is
-00004800: 5f75 726c 2061 6e64 206e 6f74 205f 7661  _url and not _va
-00004810: 6c75 655f 6874 6d6c 2e73 7461 7274 7377  lue_html.startsw
-00004820: 6974 6828 277b 2729 3a0d 0a0d 0a20 2020  ith('{'):....   
-00004830: 2020 2020 2020 2020 2023 2061 6464 2069           # add i
-00004840: 7269 2069 636f 6e20 6966 2061 7661 696c  ri icon if avail
-00004850: 6162 6c65 3a0d 0a20 2020 2020 2020 2020  able:..         
-00004860: 2020 2069 6620 6972 695f 6f62 6a65 6374     if iri_object
-00004870: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00004880: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00004890: 7661 6c75 655f 6874 6d6c 202b 3d20 6765  value_html += ge
-000048a0: 745f 6972 695f 6963 6f6e 5f68 7265 6628  t_iri_icon_href(
-000048b0: 6972 695f 6f62 6a65 6374 290d 0a0d 0a20  iri_object).... 
-000048c0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000048d0: 5f75 726c 2061 6e64 206e 6f74 205f 7661  _url and not _va
-000048e0: 6c75 655f 6874 6d6c 2e73 7461 7274 7377  lue_html.startsw
-000048f0: 6974 6828 277b 2729 3a20 2023 2054 4f44  ith('{'):  # TOD
-00004900: 4f3a 2077 6879 2074 6865 2073 6563 6f6e  O: why the secon
-00004910: 6420 636f 6e64 6974 696f 6e3f 0d0a 2020  d condition?..  
-00004920: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004930: 7475 726e 2066 273c 6c69 2073 7479 6c65  turn f'<li style
-00004940: 3d22 6c69 7374 2d73 7479 6c65 2d74 7970  ="list-style-typ
-00004950: 653a 206e 6f6e 653b 2066 6f6e 742d 7374  e: none; font-st
-00004960: 796c 653a 2069 7461 6c69 6322 3e7b 6e61  yle: italic">{na
-00004970: 6d65 7d20 3a20 7b5f 7661 6c75 655f 6874  me} : {_value_ht
-00004980: 6d6c 7d3c 2f6c 693e 270d 0a20 2020 2020  ml}</li>'..     
-00004990: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000049a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000049b0: 2073 656c 662e 6d61 785f 6174 7472 5f6c   self.max_attr_l
-000049c0: 656e 6774 683a 0d0a 2020 2020 2020 2020  ength:..        
-000049d0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000049e0: 656e 285f 7661 6c75 655f 7374 7229 203e  en(_value_str) >
-000049f0: 2073 656c 662e 6d61 785f 6174 7472 5f6c   self.max_attr_l
-00004a00: 656e 6774 683a 0d0a 2020 2020 2020 2020  ength:..        
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a20: 5f76 616c 7565 5f73 7472 203d 2066 277b  _value_str = f'{
-00004a30: 5f76 616c 7565 5f73 7472 5b30 3a73 656c  _value_str[0:sel
-00004a40: 662e 6d61 785f 6174 7472 5f6c 656e 6774  f.max_attr_lengt
-00004a50: 6820 2d20 335d 7d2e 2e2e 270d 0a20 2020  h - 3]}...'..   
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 5f76 616c 7565 5f73 7472 203d 2061 7474  _value_str = att
-00004aa0: 725f 7661 6c75 650d 0a20 2020 2020 2020  r_value..       
-00004ab0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 2020 2020 5f76 616c 7565 5f73 7472 203d      _value_str =
-00004ae0: 2061 7474 725f 7661 6c75 650d 0a20 2020   attr_value..   
-00004af0: 2020 2020 2020 2020 2069 6620 6972 695f           if iri_
-00004b00: 6f62 6a65 6374 2069 7320 6e6f 7420 4e6f  object is not No
-00004b10: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00004b20: 2020 2020 205f 7661 6c75 655f 7374 7220       _value_str 
-00004b30: 2b3d 2067 6574 5f69 7269 5f69 636f 6e5f  += get_iri_icon_
-00004b40: 6872 6566 2869 7269 5f6f 626a 6563 7429  href(iri_object)
-00004b50: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00004b60: 7475 726e 2066 273c 6c69 2073 7479 6c65  turn f'<li style
-00004b70: 3d22 6c69 7374 2d73 7479 6c65 2d74 7970  ="list-style-typ
-00004b80: 653a 206e 6f6e 653b 2066 6f6e 742d 7374  e: none; font-st
-00004b90: 796c 653a 2069 7461 6c69 6322 3e7b 6e61  yle: italic">{na
-00004ba0: 6d65 7d20 3a20 7b5f 7661 6c75 655f 7374  me} : {_value_st
-00004bb0: 727d 3c2f 6c69 3e27 0d0a 0d0a 2020 2020  r}</li>'....    
-00004bc0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00004bd0: 7461 6e63 6528 6174 7472 5f76 616c 7565  tance(attr_value
-00004be0: 2c20 6e64 6172 7261 7929 3a0d 0a20 2020  , ndarray):..   
-00004bf0: 2020 2020 2020 2020 2069 6620 6765 7461           if geta
-00004c00: 7474 7228 6174 7472 5f76 616c 7565 2c20  ttr(attr_value, 
-00004c10: 275f 7265 7072 5f68 746d 6c5f 272c 204e  '_repr_html_', N
-00004c20: 6f6e 6529 3a0d 0a20 2020 2020 2020 2020  one):..         
-00004c30: 2020 2020 2020 205f 7661 6c75 655f 7374         _value_st
-00004c40: 7220 3d20 6174 7472 5f76 616c 7565 2e5f  r = attr_value._
-00004c50: 7265 7072 5f68 746d 6c5f 2829 0d0a 2020  repr_html_()..  
-00004c60: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00004c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c80: 205f 7661 6c75 655f 7374 7220 3d20 7374   _value_str = st
-00004c90: 7228 6174 7472 5f76 616c 7565 290d 0a20  r(attr_value).. 
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004cb0: 6620 5f76 616c 7565 5f73 7472 5b30 5d20  f _value_str[0] 
-00004cc0: 3d3d 2027 3c27 2061 6e64 205f 7661 6c75  == '<' and _valu
-00004cd0: 655f 7374 725b 2d31 5d20 3d3d 2027 3e27  e_str[-1] == '>'
-00004ce0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004cf0: 2020 2020 2020 205f 7661 6c75 655f 7374         _value_st
-00004d00: 7220 3d20 5f76 616c 7565 5f73 7472 5b31  r = _value_str[1
-00004d10: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
-00004d20: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
-00004d30: 785f 6174 7472 5f6c 656e 6774 683a 0d0a  x_attr_length:..
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d50: 2020 2020 6966 206c 656e 285f 7661 6c75      if len(_valu
-00004d60: 655f 7374 7229 203e 2073 656c 662e 6d61  e_str) > self.ma
-00004d70: 785f 6174 7472 5f6c 656e 6774 683a 0d0a  x_attr_length:..
-00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d90: 2020 2020 2020 2020 5f76 616c 7565 5f73          _value_s
-00004da0: 7472 203d 2066 277b 5f76 616c 7565 5f73  tr = f'{_value_s
-00004db0: 7472 5b30 3a73 656c 662e 6d61 785f 6174  tr[0:self.max_at
-00004dc0: 7472 5f6c 656e 6774 6820 2d20 335d 7d2e  tr_length - 3]}.
-00004dd0: 2e2e 270d 0a20 2020 2020 2020 2020 2020  ..'..           
-00004de0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e00: 2020 2020 2020 2020 5f76 616c 7565 5f73          _value_s
-00004e10: 7472 203d 2061 7474 725f 7661 6c75 650d  tr = attr_value.
-00004e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e30: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00004e40: 2020 2020 2020 2020 2020 2020 5f76 616c              _val
-00004e50: 7565 5f73 7472 203d 2061 7474 725f 7661  ue_str = attr_va
-00004e60: 6c75 650d 0a0d 0a20 2020 2020 2020 2069  lue....        i
-00004e70: 6620 6972 695f 6f62 6a65 6374 2069 7320  f iri_object is 
-00004e80: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00004e90: 2020 2020 2020 205f 7661 6c75 655f 7374         _value_st
-00004ea0: 7220 2b3d 2067 6574 5f69 7269 5f69 636f  r += get_iri_ico
-00004eb0: 6e5f 6872 6566 2869 7269 5f6f 626a 6563  n_href(iri_objec
-00004ec0: 7429 2020 2320 6d61 6b65 5f68 7265 6628  t)  # make_href(
-00004ed0: 6972 695f 6f62 6a65 6374 2c20 2720 5b49  iri_object, ' [I
-00004ee0: 5249 5d27 290d 0a20 2020 2020 2020 2072  RI]')..        r
-00004ef0: 6574 7572 6e20 6627 3c6c 6920 7374 796c  eturn f'<li styl
-00004f00: 653d 226c 6973 742d 7374 796c 652d 7479  e="list-style-ty
-00004f10: 7065 3a20 6e6f 6e65 3b20 666f 6e74 2d73  pe: none; font-s
-00004f20: 7479 6c65 3a20 6974 616c 6963 223e 7b6e  tyle: italic">{n
-00004f30: 616d 657d 203a 207b 5f76 616c 7565 5f73  ame} : {_value_s
-00004f40: 7472 7d3c 2f6c 693e 270d 0a0d 0a0d 0a63  tr}</li>'......c
-00004f50: 6c61 7373 2048 3552 6570 723a 0d0a 2020  lass H5Repr:..  
-00004f60: 2020 2222 2243 6c61 7373 206d 616e 6167    """Class manag
-00004f70: 696e 6720 7468 6520 7374 696e 672f 6874  ing the sting/ht
-00004f80: 6d6c 206f 7574 7075 7420 6f66 2048 4446  ml output of HDF
-00004f90: 3520 636f 6e74 656e 7422 2222 0d0a 0d0a  5 content"""....
-00004fa0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00004fb0: 2873 656c 662c 2073 7472 5f72 6570 723a  (self, str_repr:
-00004fc0: 205f 4844 4635 5374 7275 6374 7572 6552   _HDF5StructureR
-00004fd0: 6570 7220 3d20 4e6f 6e65 2c20 6874 6d6c  epr = None, html
-00004fe0: 5f72 6570 723a 205f 4844 4635 5374 7275  _repr: _HDF5Stru
-00004ff0: 6374 7572 6552 6570 7220 3d20 4e6f 6e65  ctureRepr = None
-00005000: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-00005010: 7472 5f72 6570 7220 6973 204e 6f6e 653a  tr_repr is None:
-00005020: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00005030: 6c66 2e73 7472 5f72 6570 7220 3d20 4844  lf.str_repr = HD
-00005040: 4635 5374 7275 6374 7572 6553 7472 5265  F5StructureStrRe
-00005050: 7072 2829 0d0a 2020 2020 2020 2020 656c  pr()..        el
-00005060: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00005070: 2073 656c 662e 7374 725f 7265 7072 203d   self.str_repr =
-00005080: 2073 7472 5f72 6570 720d 0a0d 0a20 2020   str_repr....   
-00005090: 2020 2020 2069 6620 6874 6d6c 5f72 6570       if html_rep
-000050a0: 7220 6973 204e 6f6e 653a 0d0a 2020 2020  r is None:..    
-000050b0: 2020 2020 2020 2020 7365 6c66 2e68 746d          self.htm
-000050c0: 6c5f 7265 7072 203d 2048 4446 3553 7472  l_repr = HDF5Str
-000050d0: 7563 7475 7265 4854 4d4c 5265 7072 2829  uctureHTMLRepr()
-000050e0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-000050f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005100: 662e 6874 6d6c 5f72 6570 7220 3d20 6874  f.html_repr = ht
-00005110: 6d6c 5f72 6570 720d 0a0d 0a20 2020 2064  ml_repr....    d
-00005120: 6566 205f 5f68 746d 6c5f 5f28 7365 6c66  ef __html__(self
-00005130: 2c20 6772 6f75 702c 2063 6f6c 6c61 7073  , group, collaps
-00005140: 6564 3a20 626f 6f6c 203d 2054 7275 652c  ed: bool = True,
-00005150: 2070 7265 616d 626c 653a 2073 7472 203d   preamble: str =
-00005160: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00005170: 2020 2020 2020 2020 2063 6875 6e6b 733a           chunks:
-00005180: 2062 6f6f 6c20 3d20 4661 6c73 652c 206d   bool = False, m
-00005190: 6178 7368 6170 653a 2062 6f6f 6c20 3d20  axshape: bool = 
-000051a0: 4661 6c73 6529 202d 3e20 4e6f 6e65 3a0d  False) -> None:.
-000051b0: 0a20 2020 2020 2020 2064 6973 706c 6179  .        display
-000051c0: 280d 0a20 2020 2020 2020 2020 2020 2048  (..            H
-000051d0: 544d 4c28 0d0a 2020 2020 2020 2020 2020  TML(..          
-000051e0: 2020 2020 2020 7365 6c66 2e68 746d 6c5f        self.html_
-000051f0: 7265 7072 280d 0a20 2020 2020 2020 2020  repr(..         
-00005200: 2020 2020 2020 2020 2020 2067 726f 7570             group
-00005210: 3d67 726f 7570 2c0d 0a20 2020 2020 2020  =group,..       
-00005220: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00005230: 6c61 7073 6564 3d63 6f6c 6c61 7073 6564  lapsed=collapsed
-00005240: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005250: 2020 2020 2020 2070 7265 616d 626c 653d         preamble=
-00005260: 7072 6561 6d62 6c65 2c0d 0a20 2020 2020  preamble,..     
-00005270: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00005280: 6875 6e6b 733d 6368 756e 6b73 2c0d 0a20  hunks=chunks,.. 
-00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052a0: 2020 206d 6178 7368 6170 653d 6d61 7873     maxshape=maxs
-000052b0: 6861 7065 0d0a 2020 2020 2020 2020 2020  hape..          
-000052c0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-000052d0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-000052e0: 290d 0a                                  )..
+000000f0: 6f6d 206f 6e74 6f6c 7574 696c 7320 696d  om ontolutils im
+00000100: 706f 7274 204d 3449 2c20 5468 696e 670d  port M4I, Thing.
+00000110: 0a66 726f 6d20 7469 6d65 2069 6d70 6f72  .from time impor
+00000120: 7420 7065 7266 5f63 6f75 6e74 6572 5f6e  t perf_counter_n
+00000130: 730d 0a0d 0a66 726f 6d20 6835 7264 6d74  s....from h5rdmt
+00000140: 6f6f 6c62 6f78 2e77 7261 7070 6572 2e72  oolbox.wrapper.r
+00000150: 6466 2069 6d70 6f72 7420 2852 4446 5f53  df import (RDF_S
+00000160: 5542 4a45 4354 5f41 5454 525f 4e41 4d45  UBJECT_ATTR_NAME
+00000170: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000190: 2020 2020 2020 2020 2052 4446 5f50 5245           RDF_PRE
+000001a0: 4449 4341 5445 5f41 5454 525f 4e41 4d45  DICATE_ATTR_NAME
+000001b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001d0: 2020 2020 2020 2020 2052 4446 5f4f 424a           RDF_OBJ
+000001e0: 4543 545f 4154 5452 5f4e 414d 452c 0d0a  ECT_ATTR_NAME,..
+000001f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 2020 2020 2020 5244 465f 5459 5045 5f41        RDF_TYPE_A
+00000220: 5454 525f 4e41 4d45 290d 0a66 726f 6d20  TTR_NAME)..from 
+00000230: 2e20 696d 706f 7274 2067 6574 5f63 6f6e  . import get_con
+00000240: 6669 672c 2069 6465 6e74 6966 6965 7273  fig, identifiers
+00000250: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
+00000260: 6962 7574 6573 0d0a 0d0a 4835 5059 5f53  ibutes....H5PY_S
+00000270: 5045 4349 414c 5f41 5454 5249 4255 5445  PECIAL_ATTRIBUTE
+00000280: 5320 3d20 2827 4449 4d45 4e53 494f 4e5f  S = ('DIMENSION_
+00000290: 4c49 5354 272c 2027 5245 4645 5245 4e43  LIST', 'REFERENC
+000002a0: 455f 4c49 5354 272c 2027 4e41 4d45 272c  E_LIST', 'NAME',
+000002b0: 2027 434c 4153 5327 2c20 7072 6f74 6563   'CLASS', protec
+000002c0: 7465 645f 6174 7472 6962 7574 6573 2e43  ted_attributes.C
+000002d0: 4f4f 5244 494e 4154 4553 290d 0a74 7279  OORDINATES)..try
+000002e0: 3a0d 0a20 2020 2043 5353 5f53 5452 203d  :..    CSS_STR =
+000002f0: 2069 6d70 6f72 746c 6962 5f72 6573 6f75   importlib_resou
+00000300: 7263 6573 2e66 696c 6573 2827 6835 7264  rces.files('h5rd
+00000310: 6d74 6f6f 6c62 6f78 2729 2e6a 6f69 6e70  mtoolbox').joinp
+00000320: 6174 6828 2764 6174 612f 7374 796c 652e  ath('data/style.
+00000330: 6373 7327 292e 7265 6164 5f62 7974 6573  css').read_bytes
+00000340: 2829 2e64 6563 6f64 6528 2275 7466 3822  ().decode("utf8"
+00000350: 290d 0a65 7863 6570 7420 4669 6c65 4e6f  )..except FileNo
+00000360: 7446 6f75 6e64 4572 726f 723a 0d0a 2020  tFoundError:..  
+00000370: 2020 696d 706f 7274 2070 6174 686c 6962    import pathlib
+00000380: 0d0a 0d0a 2020 2020 7769 7468 206f 7065  ....    with ope
+00000390: 6e28 7061 7468 6c69 622e 5061 7468 285f  n(pathlib.Path(_
+000003a0: 5f66 696c 655f 5f29 2e70 6172 656e 7420  _file__).parent 
+000003b0: 2f20 2764 6174 612f 7374 796c 652e 6373  / 'data/style.cs
+000003c0: 7327 2920 6173 2066 3a0d 0a20 2020 2020  s') as f:..     
+000003d0: 2020 2043 5353 5f53 5452 203d 2066 2e72     CSS_STR = f.r
+000003e0: 6561 6428 292e 7273 7472 6970 2829 0d0a  ead().rstrip()..
+000003f0: 0d0a 2320 4952 495f 4943 4f4e 203d 2069  ..# IRI_ICON = i
+00000400: 6d70 6f72 746c 6962 5f72 6573 6f75 7263  mportlib_resourc
+00000410: 6573 2e66 696c 6573 2827 6835 7264 6d74  es.files('h5rdmt
+00000420: 6f6f 6c62 6f78 2729 2e6a 6f69 6e70 6174  oolbox').joinpat
+00000430: 6828 2764 6174 612f 6972 695f 6963 6f6e  h('data/iri_icon
+00000440: 2e70 6e67 2729 0d0a 2320 6966 2049 5249  .png')..# if IRI
+00000450: 5f49 434f 4e2e 6578 6973 7473 2829 3a0d  _ICON.exists():.
+00000460: 0a23 2020 2020 2049 5249 5f49 434f 4e20  .#     IRI_ICON 
+00000470: 3d20 7266 2766 696c 653a 2f2f 2f7b 4952  = rf'file:///{IR
+00000480: 495f 4943 4f4e 7d27 0d0a 2320 656c 7365  I_ICON}'..# else
+00000490: 3a0d 0a44 4546 5f49 434f 4e20 3d20 2268  :..DEF_ICON = "h
+000004a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000004b0: 6d2f 6d61 7474 6869 6173 7072 6f62 7374  m/matthiasprobst
+000004c0: 2f68 3552 444d 746f 6f6c 626f 782f 626c  /h5RDMtoolbox/bl
+000004d0: 6f62 2f64 6576 2f68 3572 646d 746f 6f6c  ob/dev/h5rdmtool
+000004e0: 626f 782f 6461 7461 2f64 6566 5f69 636f  box/data/def_ico
+000004f0: 6e2e 706e 673f 7261 773d 7472 7565 220d  n.png?raw=true".
+00000500: 0a49 5249 5f49 434f 4e20 3d20 2268 7474  .IRI_ICON = "htt
+00000510: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000520: 6d61 7474 6869 6173 7072 6f62 7374 2f68  matthiasprobst/h
+00000530: 3552 444d 746f 6f6c 626f 782f 626c 6f62  5RDMtoolbox/blob
+00000540: 2f64 6576 2f68 3572 646d 746f 6f6c 626f  /dev/h5rdmtoolbo
+00000550: 782f 6461 7461 2f69 7269 5f69 636f 6e2e  x/data/iri_icon.
+00000560: 706e 673f 7261 773d 7472 7565 220d 0a49  png?raw=true"..I
+00000570: 445f 4943 4f4e 203d 2022 6874 7470 733a  D_ICON = "https:
+00000580: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
+00000590: 7468 6961 7370 726f 6273 742f 6835 5244  thiasprobst/h5RD
+000005a0: 4d74 6f6f 6c62 6f78 2f62 6c6f 622f 6465  Mtoolbox/blob/de
+000005b0: 762f 6835 7264 6d74 6f6f 6c62 6f78 2f64  v/h5rdmtoolbox/d
+000005c0: 6174 612f 6964 5f69 636f 6e2e 706e 673f  ata/id_icon.png?
+000005d0: 7261 773d 7472 7565 220d 0a54 5950 455f  raw=true"..TYPE_
+000005e0: 4943 4f4e 203d 2022 6874 7470 733a 2f2f  ICON = "https://
+000005f0: 6769 7468 7562 2e63 6f6d 2f6d 6174 7468  github.com/matth
+00000600: 6961 7370 726f 6273 742f 6835 5244 4d74  iasprobst/h5RDMt
+00000610: 6f6f 6c62 6f78 2f62 6c6f 622f 6465 762f  oolbox/blob/dev/
+00000620: 6835 7264 6d74 6f6f 6c62 6f78 2f64 6174  h5rdmtoolbox/dat
+00000630: 612f 7479 7065 5f69 636f 6e2e 706e 673f  a/type_icon.png?
+00000640: 7261 773d 7472 7565 220d 0a0d 0a68 6173  raw=true"....has
+00000650: 556e 6974 4952 4920 3d20 7374 7228 4d34  UnitIRI = str(M4
+00000660: 492e 6861 7355 6e69 7429 0d0a 2222 220d  I.hasUnit)..""".
+00000670: 0a64 6973 636c 6169 6d65 723a 0d0a 0d0a  .disclaimer:....
+00000680: 6472 6f70 646f 776e 205f 6874 6d6c 2072  dropdown _html r
+00000690: 6570 7265 7365 6e74 6174 696f 6e20 7265  epresentation re
+000006a0: 616c 697a 6564 2077 6974 6820 2268 3566  alized with "h5f
+000006b0: 696c 655f 6874 6d6c 5f72 6570 7222 0d0a  ile_html_repr"..
+000006c0: 6973 2069 6e73 7069 7265 6420 616e 6420  is inspired and 
+000006d0: 6d6f 7374 6c79 2074 616b 656e 2066 726f  mostly taken fro
+000006e0: 6d3a 0d0a 6874 7470 733a 2f2f 6a73 6669  m:..https://jsfi
+000006f0: 6464 6c65 2e6e 6574 2f74 6179 3038 636e  ddle.net/tay08cn
+00000700: 392f 342f 2028 7861 7272 6179 2070 6163  9/4/ (xarray pac
+00000710: 6b61 6765 290d 0a0d 0a22 2222 0d0a 0d0a  kage)...."""....
+00000720: 0d0a 636c 6173 7320 4243 6f6c 6f72 733a  ..class BColors:
+00000730: 0d0a 2020 2020 2222 2243 6f6c 6f72 2063  ..    """Color c
+00000740: 6c61 7373 2074 6f20 636f 6c6f 7220 7465  lass to color te
+00000750: 7874 2222 220d 0a20 2020 2048 4541 4445  xt"""..    HEADE
+00000760: 5220 3d20 275c 3033 335b 3935 6d27 0d0a  R = '\033[95m'..
+00000770: 2020 2020 4f4b 424c 5545 203d 2027 5c30      OKBLUE = '\0
+00000780: 3333 5b39 346d 270d 0a20 2020 204f 4b43  33[94m'..    OKC
+00000790: 5941 4e20 3d20 275c 3033 335b 3936 6d27  YAN = '\033[96m'
+000007a0: 0d0a 2020 2020 4f4b 4752 4545 4e20 3d20  ..    OKGREEN = 
+000007b0: 275c 3033 335b 3932 6d27 0d0a 2020 2020  '\033[92m'..    
+000007c0: 5741 524e 494e 4720 3d20 275c 3033 335b  WARNING = '\033[
+000007d0: 3933 6d27 0d0a 2020 2020 4641 494c 203d  93m'..    FAIL =
+000007e0: 2027 5c30 3333 5b39 316d 270d 0a20 2020   '\033[91m'..   
+000007f0: 2045 4e44 4320 3d20 275c 3033 335b 306d   ENDC = '\033[0m
+00000800: 270d 0a20 2020 2042 4f4c 4420 3d20 275c  '..    BOLD = '\
+00000810: 3033 335b 316d 270d 0a20 2020 2055 4e44  033[1m'..    UND
+00000820: 4552 4c49 4e45 203d 2027 5c30 3333 5b34  ERLINE = '\033[4
+00000830: 6d27 0d0a 2020 2020 4954 414c 4943 203d  m'..    ITALIC =
+00000840: 2027 5c30 3333 5b33 6d27 0d0a 0d0a 0d0a   '\033[3m'......
+00000850: 6465 6620 6d61 6b65 5f69 7461 6c69 6328  def make_italic(
+00000860: 7374 7269 6e67 293a 0d0a 2020 2020 2222  string):..    ""
+00000870: 226d 616b 6520 7374 7269 6e67 2069 7461  "make string ita
+00000880: 6c69 6322 2222 0d0a 2020 2020 7265 7475  lic"""..    retu
+00000890: 726e 2066 227b 4243 6f6c 6f72 732e 4954  rn f"{BColors.IT
+000008a0: 414c 4943 7d7b 7374 7269 6e67 7d7b 4243  ALIC}{string}{BC
+000008b0: 6f6c 6f72 732e 454e 4443 7d22 0d0a 0d0a  olors.ENDC}"....
+000008c0: 0d0a 6465 6620 6d61 6b65 5f62 6f6c 6428  ..def make_bold(
+000008d0: 7374 7269 6e67 293a 0d0a 2020 2020 2222  string):..    ""
+000008e0: 226d 616b 6520 7374 7269 6e67 2062 6f6c  "make string bol
+000008f0: 6422 2222 0d0a 2020 2020 7265 7475 726e  d"""..    return
+00000900: 2066 227b 4243 6f6c 6f72 732e 424f 4c44   f"{BColors.BOLD
+00000910: 7d7b 7374 7269 6e67 7d7b 4243 6f6c 6f72  }{string}{BColor
+00000920: 732e 454e 4443 7d22 0d0a 0d0a 0d0a 6465  s.ENDC}"......de
+00000930: 6620 7761 726e 696e 6774 6578 7428 7374  f warningtext(st
+00000940: 7269 6e67 293a 0d0a 2020 2020 2222 226d  ring):..    """m
+00000950: 616b 6520 7374 7269 6e67 206f 7261 6e67  ake string orang
+00000960: 6522 2222 0d0a 2020 2020 7265 7475 726e  e"""..    return
+00000970: 2066 227b 4243 6f6c 6f72 732e 5741 524e   f"{BColors.WARN
+00000980: 494e 477d 7b73 7472 696e 677d 7b42 436f  ING}{string}{BCo
+00000990: 6c6f 7273 2e45 4e44 437d 220d 0a0d 0a0d  lors.ENDC}".....
+000009a0: 0a64 6566 2066 6169 6c74 6578 7428 7374  .def failtext(st
+000009b0: 7269 6e67 293a 0d0a 2020 2020 2222 226d  ring):..    """m
+000009c0: 616b 6520 7374 7269 6e67 2072 6564 2222  ake string red""
+000009d0: 220d 0a20 2020 2072 6574 7572 6e20 6622  "..    return f"
+000009e0: 7b42 436f 6c6f 7273 2e46 4149 4c7d 7b73  {BColors.FAIL}{s
+000009f0: 7472 696e 677d 7b42 436f 6c6f 7273 2e45  tring}{BColors.E
+00000a00: 4e44 437d 220d 0a0d 0a0d 0a64 6566 2066  NDC}"......def f
+00000a10: 6169 6c70 7269 6e74 2873 7472 696e 6729  ailprint(string)
+00000a20: 3a0d 0a20 2020 2022 2222 7072 696e 7420  :..    """print 
+00000a30: 7374 7269 6e67 2069 6e20 7265 6422 2222  string in red"""
+00000a40: 0d0a 2020 2020 7072 696e 7428 6661 696c  ..    print(fail
+00000a50: 7465 7874 2873 7472 696e 6729 290d 0a0d  text(string))...
+00000a60: 0a0d 0a64 6566 206f 6b74 6578 7428 7374  ...def oktext(st
+00000a70: 7269 6e67 293a 0d0a 2020 2020 2222 226d  ring):..    """m
+00000a80: 616b 6520 7374 7269 6e67 2067 7265 656e  ake string green
+00000a90: 2222 220d 0a20 2020 2072 6574 7572 6e20  """..    return 
+00000aa0: 6622 7b42 436f 6c6f 7273 2e4f 4b47 5245  f"{BColors.OKGRE
+00000ab0: 454e 7d7b 7374 7269 6e67 7d7b 4243 6f6c  EN}{string}{BCol
+00000ac0: 6f72 732e 454e 4443 7d22 0d0a 0d0a 0d0a  ors.ENDC}"......
+00000ad0: 6465 6620 6f6b 7072 696e 7428 7374 7269  def okprint(stri
+00000ae0: 6e67 293a 0d0a 2020 2020 2222 2270 7269  ng):..    """pri
+00000af0: 6e74 2073 7472 696e 6720 696e 2072 6564  nt string in red
+00000b00: 2222 220d 0a20 2020 2070 7269 6e74 286f  """..    print(o
+00000b10: 6b74 6578 7428 7374 7269 6e67 2929 0d0a  ktext(string))..
+00000b20: 0d0a 0d0a 6465 6620 6d61 6b65 5f68 7265  ....def make_hre
+00000b30: 6628 7572 6c3a 2073 7472 2c20 7465 7874  f(url: str, text
+00000b40: 3a20 7374 7229 202d 3e20 7374 723a 0d0a  : str) -> str:..
+00000b50: 2020 2020 2222 2242 7569 6c64 7320 4854      """Builds HT
+00000b60: 4d4c 2068 7970 6572 6c69 6e6b 2066 726f  ML hyperlink fro
+00000b70: 6d20 7572 6c0d 0a0d 0a20 2020 2050 6172  m url....    Par
+00000b80: 616d 6574 6572 730d 0a20 2020 202d 2d2d  ameters..    ---
+00000b90: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2075 726c  -------..    url
+00000ba0: 3a20 7374 720d 0a20 2020 2020 2020 206c  : str..        l
+00000bb0: 696e 6b20 6465 7374 696e 6174 696f 6e0d  ink destination.
+00000bc0: 0a20 2020 2074 6578 743a 2073 7472 0d0a  .    text: str..
+00000bd0: 2020 2020 2020 2020 6469 7370 6c61 7920          display 
+00000be0: 7465 7874 0d0a 0d0a 2020 2020 5265 7475  text....    Retu
+00000bf0: 726e 730d 0a20 2020 202d 2d2d 2d2d 2d2d  rns..    -------
+00000c00: 0d0a 2020 2020 5468 6520 4854 4d4c 203c  ..    The HTML <
+00000c10: 613e 2074 6167 2073 7472 696e 670d 0a20  a> tag string.. 
+00000c20: 2020 2022 2222 0d0a 2020 2020 6966 206e     """..    if n
+00000c30: 6f74 2075 726c 2e73 7461 7274 7377 6974  ot url.startswit
+00000c40: 6828 2768 7474 7027 293a 0d0a 2020 2020  h('http'):..    
+00000c50: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00000c60: 7272 6f72 2866 2749 6e76 616c 6964 2055  rror(f'Invalid U
+00000c70: 524c 3a20 227b 7572 6c7d 222e 204d 7573  RL: "{url}". Mus
+00000c80: 7420 7374 6172 7420 7769 7468 2022 6874  t start with "ht
+00000c90: 7470 2227 290d 0a20 2020 2072 6574 7572  tp"')..    retur
+00000ca0: 6e20 6627 3c61 2068 7265 663d 227b 7572  n f'<a href="{ur
+00000cb0: 6c7d 223e 7b74 6578 747d 3c2f 613e 270d  l}">{text}</a>'.
+00000cc0: 0a0d 0a0d 0a64 6566 2070 726f 6365 7373  .....def process
+00000cd0: 5f73 7472 696e 675f 666f 725f 6c69 6e6b  _string_for_link
+00000ce0: 2873 7472 696e 673a 2073 7472 2920 2d3e  (string: str) ->
+00000cf0: 2074 7970 696e 672e 5475 706c 655b 7374   typing.Tuple[st
+00000d00: 722c 2062 6f6f 6c5d 3a0d 0a20 2020 2022  r, bool]:..    "
+00000d10: 2222 7072 6f63 6573 7320 7374 7269 6e67  ""process string
+00000d20: 2074 6f20 6d61 6b65 206c 696e 6b73 2061   to make links a
+00000d30: 6374 7561 6c6c 7920 636c 6963 6b61 626c  ctually clickabl
+00000d40: 6520 696e 2068 746d 6c0d 0a0d 0a20 2020  e in html....   
+00000d50: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+00000d60: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+00000d70: 2073 7472 696e 673a 2073 7472 0d0a 2020   string: str..  
+00000d80: 2020 2020 2020 7374 7269 6e67 2074 6f20        string to 
+00000d90: 7072 6f63 6573 730d 0a0d 0a20 2020 2052  process....    R
+00000da0: 6574 7572 6e73 0d0a 2020 2020 2d2d 2d2d  eturns..    ----
+00000db0: 2d2d 2d0d 0a20 2020 2073 7472 0d0a 2020  ---..    str..  
+00000dc0: 2020 2020 2020 7072 6f63 6573 7365 6420        processed 
+00000dd0: 7374 7269 6e67 0d0a 2020 2020 626f 6f6c  string..    bool
+00000de0: 0d0a 2020 2020 2020 2020 5472 7565 2069  ..        True i
+00000df0: 6620 7374 7269 6e67 2061 6374 7561 6c6c  f string actuall
+00000e00: 7920 636f 6e74 6169 6e73 2061 206c 696e  y contains a lin
+00000e10: 6b0d 0a0d 0a20 2020 2022 2222 0d0a 2020  k....    """..  
+00000e20: 2020 6966 2027 7a65 6e6f 646f 2e27 2069    if 'zenodo.' i
+00000e30: 6e20 7374 7269 6e67 3a0d 0a20 2020 2020  n string:..     
+00000e40: 2020 2069 6620 7265 2e6d 6174 6368 2872     if re.match(r
+00000e50: 2731 305c 2e5c 647b 342c 397d 2f7a 656e  '10\.\d{4,9}/zen
+00000e60: 6f64 6f5c 2e5c 647b 342c 397d 272c 2073  odo\.\d{4,9}', s
+00000e70: 7472 696e 6729 3a0d 0a20 2020 2020 2020  tring):..       
+00000e80: 2020 2020 207a 656e 6f64 6f5f 7572 6c20       zenodo_url 
+00000e90: 3d20 6627 6874 7470 733a 2f2f 646f 692e  = f'https://doi.
+00000ea0: 6f72 672f 7b73 7472 696e 677d 270d 0a20  org/{string}'.. 
+00000eb0: 2020 2020 2020 2020 2020 2069 6d67 5f75             img_u
+00000ec0: 726c 203d 2066 2768 7474 7073 3a2f 2f7a  rl = f'https://z
+00000ed0: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
+00000ee0: 444f 492f 7b73 7472 696e 677d 2e73 7667  DOI/{string}.svg
+00000ef0: 270d 0a20 2020 2020 2020 2069 6620 7374  '..        if st
+00000f00: 7269 6e67 2e73 7461 7274 7377 6974 6828  ring.startswith(
+00000f10: 2768 7474 7073 3a2f 2f7a 656e 6f64 6f2e  'https://zenodo.
+00000f20: 6f72 672f 7265 636f 7264 2f27 293a 0d0a  org/record/'):..
+00000f30: 2020 2020 2020 2020 2020 2020 7a65 6e6f              zeno
+00000f40: 646f 5f75 726c 203d 2073 7472 696e 670d  do_url = string.
+00000f50: 0a20 2020 2020 2020 2020 2020 2069 6d67  .            img
+00000f60: 5f75 726c 203d 2066 2768 7474 7073 3a2f  _url = f'https:/
+00000f70: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
+00000f80: 652f 444f 492f 3130 2e35 3238 312f 7a65  e/DOI/10.5281/ze
+00000f90: 6e6f 646f 2e7b 7374 7269 6e67 2e73 706c  nodo.{string.spl
+00000fa0: 6974 2822 2f22 295b 2d31 5d7d 2e73 7667  it("/")[-1]}.svg
+00000fb0: 270d 0a20 2020 2020 2020 2072 6574 7572  '..        retur
+00000fc0: 6e20 6d61 6b65 5f68 7265 6628 7572 6c3d  n make_href(url=
+00000fd0: 7a65 6e6f 646f 5f75 726c 2c20 7465 7874  zenodo_url, text
+00000fe0: 3d66 273c 696d 6720 7372 633d 227b 696d  =f'<img src="{im
+00000ff0: 675f 7572 6c7d 2220 616c 743d 2244 4f49  g_url}" alt="DOI
+00001000: 223e 2729 2c20 5472 7565 0d0a 2020 2020  ">'), True..    
+00001010: 666f 7220 7020 696e 2028 7222 2868 7474  for p in (r"(htt
+00001020: 7073 3f3a 2f2f 5c53 2b29 222c 2072 2228  ps?://\S+)", r"(
+00001030: 6674 703a 2f2f 5c53 2b29 222c 2072 2228  ftp://\S+)", r"(
+00001040: 7777 775c 2e5c 532b 2922 293a 0d0a 2020  www\.\S+)"):..  
+00001050: 2020 2020 2020 7572 6c73 203d 2072 652e        urls = re.
+00001060: 6669 6e64 616c 6c28 702c 2073 7472 696e  findall(p, strin
+00001070: 6729 0d0a 2020 2020 2020 2020 6966 2075  g)..        if u
+00001080: 726c 733a 0d0a 2020 2020 2020 2020 2020  rls:..          
+00001090: 2020 666f 7220 7572 6c20 696e 2075 726c    for url in url
+000010a0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000010b0: 2020 2020 6964 656e 7469 6669 6572 203d      identifier =
+000010c0: 2069 6465 6e74 6966 6965 7273 2e66 726f   identifiers.fro
+000010d0: 6d5f 7572 6c28 7572 6c29 0d0a 2020 2020  m_url(url)..    
+000010e0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000010f0: 6465 6e74 6966 6965 723a 0d0a 2020 2020  dentifier:..    
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 6f72 6369 645f 7572 6c5f 7265 7072 203d  orcid_url_repr =
+00001120: 2069 6465 6e74 6966 6965 722e 5f72 6570   identifier._rep
+00001130: 725f 6874 6d6c 5f28 290d 0a20 2020 2020  r_html_()..     
+00001140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001150: 7472 696e 6720 3d20 7374 7269 6e67 2e72  tring = string.r
+00001160: 6570 6c61 6365 2875 726c 2c20 6f72 6369  eplace(url, orci
+00001170: 645f 7572 6c5f 7265 7072 290d 0a20 2020  d_url_repr)..   
+00001180: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00001190: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000011a0: 2020 2020 2020 2020 7374 7269 6e67 203d          string =
+000011b0: 2073 7472 696e 672e 7265 706c 6163 6528   string.replace(
+000011c0: 7572 6c2c 206d 616b 655f 6872 6566 2875  url, make_href(u
+000011d0: 726c 2c20 7572 6c29 290d 0a20 2020 2020  rl, url))..     
+000011e0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+000011f0: 7269 6e67 2c20 5472 7565 0d0a 0d0a 2020  ring, True....  
+00001200: 2020 7265 7475 726e 2073 7472 696e 672c    return string,
+00001210: 2046 616c 7365 0d0a 0d0a 0d0a 6465 6620   False......def 
+00001220: 6765 745f 6972 695f 6963 6f6e 5f68 7265  get_iri_icon_hre
+00001230: 6628 6972 693a 2073 7472 2c0d 0a20 2020  f(iri: str,..   
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 2020 2069 636f 6e5f 7572 6c3a 2073 7472     icon_url: str
+00001260: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001270: 2020 2020 2020 2020 2074 6f6f 6c74 6970           tooltip
+00001280: 7465 7874 3d4e 6f6e 6529 202d 3e20 7374  text=None) -> st
+00001290: 723a 0d0a 2020 2020 2222 2267 6574 2068  r:..    """get h
+000012a0: 746d 6c20 7265 7072 6573 656e 7461 7469  tml representati
+000012b0: 6f6e 206f 6620 616e 2049 5249 2077 6974  on of an IRI wit
+000012c0: 6820 6963 6f6e 2e20 5468 6520 5552 4c20  h icon. The URL 
+000012d0: 6973 2073 686f 776e 2061 7320 6120 746f  is shown as a to
+000012e0: 6f6c 7469 7022 2222 0d0a 2020 2020 2320  oltip"""..    # 
+000012f0: 6966 2069 7369 6e73 7461 6e63 6528 6972  if isinstance(ir
+00001300: 692c 2064 6963 7429 3a0d 0a20 2020 2023  i, dict):..    #
+00001310: 2020 2020 2074 6869 6e67 203d 2054 6869       thing = Thi
+00001320: 6e67 2e66 726f 6d5f 6a73 6f6e 6c64 2864  ng.from_jsonld(d
+00001330: 6174 613d 6972 692c 206c 696d 6974 3d31  ata=iri, limit=1
+00001340: 290d 0a20 2020 2023 2020 2020 205f 7479  )..    #     _ty
+00001350: 7065 203d 2069 7269 2e67 6574 2852 4446  pe = iri.get(RDF
+00001360: 5f54 5950 455f 4154 5452 5f4e 414d 452c  _TYPE_ATTR_NAME,
+00001370: 204e 6f6e 6529 0d0a 2020 2020 2320 2020   None)..    #   
+00001380: 2020 7468 696e 672e 706f 705f 626c 616e    thing.pop_blan
+00001390: 6b5f 6e6f 6465 5f69 6428 290d 0a20 2020  k_node_id()..   
+000013a0: 2023 2020 2020 2074 6869 6e67 5f73 7472   #     thing_str
+000013b0: 203d 2074 6869 6e67 2e5f 5f73 7472 5f5f   = thing.__str__
+000013c0: 286c 696d 6974 3d35 3029 0d0a 2020 2020  (limit=50)..    
+000013d0: 2320 2020 2020 6966 205f 7479 7065 3a0d  #     if _type:.
+000013e0: 0a20 2020 2023 2020 2020 2020 2020 205f  .    #         _
+000013f0: 7468 696e 675f 7374 7220 3d20 7468 696e  thing_str = thin
+00001400: 672e 5f5f 7374 725f 5f28 6c69 6d69 743d  g.__str__(limit=
+00001410: 3530 292e 7370 6c69 7428 2728 272c 2031  50).split('(', 1
+00001420: 295b 315d 0d0a 2020 2020 2320 2020 2020  )[1]..    #     
+00001430: 2020 2020 7468 696e 675f 7374 7220 3d20      thing_str = 
+00001440: 6627 7b5f 7479 7065 7d28 7b5f 7468 696e  f'{_type}({_thin
+00001450: 675f 7374 727d 270d 0a20 2020 2023 2020  g_str}'..    #  
+00001460: 2020 2072 6574 7572 6e20 6627 3c64 6976     return f'<div
+00001470: 2063 6c61 7373 3d22 746f 6f6c 7469 7022   class="tooltip"
+00001480: 3e27 205c 0d0a 2020 2020 2320 2020 2020  >' \..    #     
+00001490: 2020 2020 2020 2066 273c 696d 6720 636c         f'<img cl
+000014a0: 6173 733d 2273 697a 655f 6f66 5f69 6d67  ass="size_of_img
+000014b0: 2220 7372 633d 227b 6963 6f6e 5f75 726c  " src="{icon_url
+000014c0: 7d22 2061 6c74 3d22 4952 495f 4943 4f4e  }" alt="IRI_ICON
+000014d0: 2220 7769 6474 683d 2231 3622 2068 6569  " width="16" hei
+000014e0: 6768 743d 2231 3622 202f 3e27 205c 0d0a  ght="16" />' \..
+000014f0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+00001500: 2066 273c 7370 616e 2063 6c61 7373 3d22   f'<span class="
+00001510: 746f 6f6c 7469 7074 6578 7422 3e7b 7468  tooltiptext">{th
+00001520: 696e 675f 7374 727d 3c2f 7370 616e 3e3c  ing_str}</span><
+00001530: 2f64 6976 3e27 0d0a 0d0a 2020 2020 7265  /div>'....    re
+00001540: 7475 726e 2066 273c 6120 6872 6566 3d22  turn f'<a href="
+00001550: 7b69 7269 7d22 2074 6172 6765 743d 225f  {iri}" target="_
+00001560: 626c 616e 6b22 2063 6c61 7373 3d22 746f  blank" class="to
+00001570: 6f6c 7469 7022 3e20 2720 5c0d 0a20 2020  oltip"> ' \..   
+00001580: 2020 2020 2020 2020 6627 3c69 6d67 2063          f'<img c
+00001590: 6c61 7373 3d22 7369 7a65 5f6f 665f 696d  lass="size_of_im
+000015a0: 6722 2073 7263 3d22 7b69 636f 6e5f 7572  g" src="{icon_ur
+000015b0: 6c7d 2220 616c 743d 2249 5249 5f49 434f  l}" alt="IRI_ICO
+000015c0: 4e22 2077 6964 7468 3d22 3136 2220 6865  N" width="16" he
+000015d0: 6967 6874 3d22 3136 2220 2f3e 2720 5c0d  ight="16" />' \.
+000015e0: 0a20 2020 2020 2020 2020 2020 6627 203c  .           f' <
+000015f0: 7370 616e 2063 6c61 7373 3d22 746f 6f6c  span class="tool
+00001600: 7469 7074 6578 7422 3e7b 746f 6f6c 7469  tiptext">{toolti
+00001610: 7074 6578 7420 6f72 2069 7269 7d3c 2f73  ptext or iri}</s
+00001620: 7061 6e3e 3c2f 613e 270d 0a0d 0a0d 0a64  pan></a>'......d
+00001630: 6566 2067 6574 5f64 6566 5f69 636f 6e5f  ef get_def_icon_
+00001640: 6872 6566 2864 6566 5f74 6578 743a 2073  href(def_text: s
+00001650: 7472 2920 2d3e 2073 7472 3a0d 0a20 2020  tr) -> str:..   
+00001660: 2022 2222 6765 7420 6874 6d6c 2072 6570   """get html rep
+00001670: 7265 7365 6e74 6174 696f 6e20 6f66 2061  resentation of a
+00001680: 6e20 6174 7472 6962 7574 6520 6465 6669  n attribute defi
+00001690: 6e69 7469 6f6e 2077 6974 6820 6963 6f6e  nition with icon
+000016a0: 2222 220d 0a20 2020 2072 6574 7572 6e20  """..    return 
+000016b0: 6627 3c64 6976 2063 6c61 7373 3d22 746f  f'<div class="to
+000016c0: 6f6c 7469 7022 3e27 205c 0d0a 2020 2020  oltip">' \..    
+000016d0: 2020 2020 2020 2066 273c 696d 6720 636c         f'<img cl
+000016e0: 6173 733d 2273 697a 655f 6f66 5f69 6d67  ass="size_of_img
+000016f0: 2220 7372 633d 227b 4445 465f 4943 4f4e  " src="{DEF_ICON
+00001700: 7d22 2061 6c74 3d22 4422 2077 6964 7468  }" alt="D" width
+00001710: 3d22 3136 2220 6865 6967 6874 3d22 3136  ="16" height="16
+00001720: 2220 2f3e 2720 5c0d 0a20 2020 2020 2020  " />' \..       
+00001730: 2020 2020 6627 3c73 7061 6e20 636c 6173      f'<span clas
+00001740: 733d 2274 6f6f 6c74 6970 7465 7874 223e  s="tooltiptext">
+00001750: 7b64 6566 5f74 6578 747d 3c2f 7370 616e  {def_text}</span
+00001760: 3e3c 2f64 6976 3e27 0d0a 0d0a 0d0a 636c  ></div>'......cl
+00001770: 6173 7320 5f48 4446 3553 7472 7563 7475  ass _HDF5Structu
+00001780: 7265 5265 7072 3a0d 0a0d 0a20 2020 2064  reRepr:....    d
+00001790: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000017a0: 2c20 6967 6e6f 7265 5f61 7474 7273 3d4e  , ignore_attrs=N
+000017b0: 6f6e 652c 2068 6964 655f 7572 693a 2062  one, hide_uri: b
+000017c0: 6f6f 6c20 3d20 4661 6c73 6529 3a0d 0a20  ool = False):.. 
+000017d0: 2020 2020 2020 2073 656c 662e 6261 7365         self.base
+000017e0: 5f69 6e74 656e 7420 3d20 2720 2027 0d0a  _intent = '  '..
+000017f0: 2020 2020 2020 2020 7365 6c66 2e6d 6178          self.max
+00001800: 5f61 7474 725f 6c65 6e67 7468 203d 2031  _attr_length = 1
+00001810: 3030 0d0a 2020 2020 2020 2020 7365 6c66  00..        self
+00001820: 2e63 6f6c 6c61 7073 6564 203d 204e 6f6e  .collapsed = Non
+00001830: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00001840: 6869 6465 5f75 7269 203d 2068 6964 655f  hide_uri = hide_
+00001850: 7572 690d 0a0d 0a20 2020 2020 2020 2073  uri....        s
+00001860: 656c 662e 5f6f 626a 5f63 6667 203d 207b  elf._obj_cfg = {
+00001870: 7d0d 0a20 2020 2020 2020 2069 6620 6967  }..        if ig
+00001880: 6e6f 7265 5f61 7474 7273 2069 7320 4e6f  nore_attrs is No
+00001890: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000018a0: 2073 656c 662e 6967 6e6f 7265 5f61 7474   self.ignore_att
+000018b0: 7273 203d 2048 3550 595f 5350 4543 4941  rs = H5PY_SPECIA
+000018c0: 4c5f 4154 5452 4942 5554 4553 0d0a 2020  L_ATTRIBUTES..  
+000018d0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000018e0: 2020 2020 2020 2020 2073 656c 662e 6967           self.ig
+000018f0: 6e6f 7265 5f61 7474 7273 203d 2069 676e  nore_attrs = ign
+00001900: 6f72 655f 6174 7472 730d 0a0d 0a20 2020  ore_attrs....   
+00001910: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00001920: 6465 6620 6368 6563 6b62 6f78 5f73 7461  def checkbox_sta
+00001930: 7465 2873 656c 6629 202d 3e20 7374 723a  te(self) -> str:
+00001940: 0d0a 2020 2020 2020 2020 2222 2272 6574  ..        """ret
+00001950: 7572 6e20 2763 6865 636b 6564 2720 6966  urn 'checked' if
+00001960: 2074 6865 2067 726f 7570 2069 7320 636f   the group is co
+00001970: 6c6c 6170 7365 642c 2065 6c73 6520 2727  llapsed, else ''
+00001980: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00001990: 7572 6e20 2727 2069 6620 7365 6c66 2e63  urn '' if self.c
+000019a0: 6f6c 6c61 7073 6564 2065 6c73 6520 2763  ollapsed else 'c
+000019b0: 6865 636b 6564 270d 0a0d 0a20 2020 2064  hecked'....    d
+000019c0: 6566 205f 5f64 6174 6173 6574 5f5f 2873  ef __dataset__(s
+000019d0: 656c 662c 206e 616d 652c 2068 356f 626a  elf, name, h5obj
+000019e0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+000019f0: 2020 2022 2222 6f76 6572 7772 6974 6520     """overwrite 
+00001a00: 7468 6520 4835 5265 7072 2070 6172 656e  the H5Repr paren
+00001a10: 7420 6d65 7468 6f64 2222 220d 0a20 2020  t method"""..   
+00001a20: 2020 2020 2069 6620 6835 6f62 6a2e 6474       if h5obj.dt
+00001a30: 7970 652e 6368 6172 203d 3d20 2753 273a  ype.char == 'S':
+00001a40: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00001a50: 6861 6e64 656c 2073 7472 696e 6720 6461  handel string da
+00001a60: 7461 7365 7473 3a0d 0a20 2020 2020 2020  tasets:..       
+00001a70: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00001a80: 2e5f 5f73 7472 696e 6764 6174 6173 6574  .__stringdataset
+00001a90: 5f5f 286e 616d 652c 2068 356f 626a 290d  __(name, h5obj).
+00001aa0: 0a20 2020 2020 2020 2069 6620 6835 6f62  .        if h5ob
+00001ab0: 6a2e 6e64 696d 203d 3d20 303a 0d0a 2020  j.ndim == 0:..  
+00001ac0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001ad0: 2073 656c 662e 5f5f 3044 6461 7461 7365   self.__0Ddatase
+00001ae0: 745f 5f28 6e61 6d65 2c20 6835 6f62 6a29  t__(name, h5obj)
+00001af0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001b00: 2073 656c 662e 5f5f 4e44 6461 7461 7365   self.__NDdatase
+00001b10: 745f 5f28 6e61 6d65 2c20 6835 6f62 6a29  t__(name, h5obj)
+00001b20: 0d0a 0d0a 2020 2020 4061 6273 7472 6163  ....    @abstrac
+00001b30: 746d 6574 686f 640d 0a20 2020 2064 6566  tmethod..    def
+00001b40: 205f 5f73 7472 696e 6764 6174 6173 6574   __stringdataset
+00001b50: 5f5f 2873 656c 662c 206e 616d 652c 2068  __(self, name, h
+00001b60: 356f 626a 293a 0d0a 2020 2020 2020 2020  5obj):..        
+00001b70: 2222 2264 6174 6173 6574 2072 6570 7265  """dataset repre
+00001b80: 7365 6e74 6174 696f 6e22 2222 0d0a 0d0a  sentation"""....
+00001b90: 2020 2020 4061 6273 7472 6163 746d 6574      @abstractmet
+00001ba0: 686f 640d 0a20 2020 2064 6566 205f 5f30  hod..    def __0
+00001bb0: 4464 6174 6173 6574 5f5f 2873 656c 662c  Ddataset__(self,
+00001bc0: 206e 616d 652c 2068 356f 626a 293a 0d0a   name, h5obj):..
+00001bd0: 2020 2020 2020 2020 2222 2264 6174 6173          """datas
+00001be0: 6574 2072 6570 7265 7365 6e74 6174 696f  et representatio
+00001bf0: 6e22 2222 0d0a 0d0a 2020 2020 4061 6273  n"""....    @abs
+00001c00: 7472 6163 746d 6574 686f 640d 0a20 2020  tractmethod..   
+00001c10: 2064 6566 205f 5f4e 4464 6174 6173 6574   def __NDdataset
+00001c20: 5f5f 2873 656c 662c 206e 616d 652c 2068  __(self, name, h
+00001c30: 356f 626a 293a 0d0a 2020 2020 2020 2020  5obj):..        
+00001c40: 2222 2264 6174 6173 6574 2072 6570 7265  """dataset repre
+00001c50: 7365 6e74 6174 696f 6e22 2222 0d0a 0d0a  sentation"""....
+00001c60: 2020 2020 4061 6273 7472 6163 746d 6574      @abstractmet
+00001c70: 686f 640d 0a20 2020 2064 6566 205f 5f67  hod..    def __g
+00001c80: 726f 7570 5f5f 2873 656c 662c 206e 616d  roup__(self, nam
+00001c90: 652c 2068 356f 626a 293a 0d0a 2020 2020  e, h5obj):..    
+00001ca0: 2020 2020 2222 2264 6174 6173 6574 2072      """dataset r
+00001cb0: 6570 7265 7365 6e74 6174 696f 6e22 2222  epresentation"""
+00001cc0: 0d0a 0d0a 2020 2020 4061 6273 7472 6163  ....    @abstrac
+00001cd0: 746d 6574 686f 640d 0a20 2020 2064 6566  tmethod..    def
+00001ce0: 205f 5f61 7474 7273 5f5f 2873 656c 662c   __attrs__(self,
+00001cf0: 206e 616d 652c 2068 356f 626a 293a 0d0a   name, h5obj):..
+00001d00: 2020 2020 2020 2020 2222 2264 6174 6173          """datas
+00001d10: 6574 2072 6570 7265 7365 6e74 6174 696f  et representatio
+00001d20: 6e22 2222 0d0a 0d0a 0d0a 636c 6173 7320  n"""......class 
+00001d30: 4844 4635 5374 7275 6374 7572 6553 7472  HDF5StructureStr
+00001d40: 5265 7072 285f 4844 4635 5374 7275 6374  Repr(_HDF5Struct
+00001d50: 7572 6552 6570 7229 3a0d 0a0d 0a20 2020  ureRepr):....   
+00001d60: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
+00001d70: 6c66 2c20 6772 6f75 702c 2069 6e64 656e  lf, group, inden
+00001d80: 743d 302c 2070 7265 616d 626c 653d 4e6f  t=0, preamble=No
+00001d90: 6e65 2c20 6869 6465 5f75 7269 3a20 626f  ne, hide_uri: bo
+00001da0: 6f6c 203d 2046 616c 7365 293a 0d0a 2020  ol = False):..  
+00001db0: 2020 2020 2020 7365 6c66 2e68 6964 655f        self.hide_
+00001dc0: 7572 6920 3d20 6869 6465 5f75 7269 0d0a  uri = hide_uri..
+00001dd0: 2020 2020 2020 2020 6966 2070 7265 616d          if pream
+00001de0: 626c 653a 0d0a 2020 2020 2020 2020 2020  ble:..          
+00001df0: 2020 7072 696e 7428 7072 6561 6d62 6c65    print(preamble
+00001e00: 290d 0a20 2020 2020 2020 2073 7061 6365  )..        space
+00001e10: 7320 3d20 7365 6c66 2e62 6173 655f 696e  s = self.base_in
+00001e20: 7465 6e74 202a 2069 6e64 656e 740d 0a20  tent * indent.. 
+00001e30: 2020 2020 2020 2070 7265 6469 6361 7465         predicate
+00001e40: 203d 2067 726f 7570 2e72 6466 2e70 7265   = group.rdf.pre
+00001e50: 6469 6361 7465 2e67 6574 2827 5345 4c46  dicate.get('SELF
+00001e60: 272c 204e 6f6e 6529 0d0a 2020 2020 2020  ', None)..      
+00001e70: 2020 6966 2070 7265 6469 6361 7465 3a0d    if predicate:.
+00001e80: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00001e90: 6e74 2873 7061 6365 7320 2b20 6627 4070  nt(spaces + f'@p
+00001ea0: 7265 6469 6361 7465 3a20 7b70 7265 6469  redicate: {predi
+00001eb0: 6361 7465 7d27 290d 0a20 2020 2020 2020  cate}')..       
+00001ec0: 2066 6f72 2061 7474 725f 6e61 6d65 2069   for attr_name i
+00001ed0: 6e20 6772 6f75 702e 6174 7472 732e 7261  n group.attrs.ra
+00001ee0: 772e 6b65 7973 2829 3a0d 0a20 2020 2020  w.keys():..     
+00001ef0: 2020 2020 2020 2069 6620 6174 7472 5f6e         if attr_n
+00001f00: 616d 6520 3d3d 2052 4446 5f53 5542 4a45  ame == RDF_SUBJE
+00001f10: 4354 5f41 5454 525f 4e41 4d45 3a0d 0a20  CT_ATTR_NAME:.. 
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00001f30: 7269 6e74 2873 7061 6365 7320 2b20 6627  rint(spaces + f'
+00001f40: 4074 7970 653a 207b 6772 6f75 702e 6174  @type: {group.at
+00001f50: 7472 735b 6174 7472 5f6e 616d 655d 7d27  trs[attr_name]}'
+00001f60: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00001f70: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00001f80: 2020 2020 2020 6966 206e 6f74 2061 7474        if not att
+00001f90: 725f 6e61 6d65 2e69 7375 7070 6572 2829  r_name.isupper()
+00001fa0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001fb0: 2020 2020 2020 2070 7269 6e74 2873 7061         print(spa
+00001fc0: 6365 7320 2b20 7365 6c66 2e5f 5f61 7474  ces + self.__att
+00001fd0: 7273 5f5f 2861 7474 725f 6e61 6d65 2c20  rs__(attr_name, 
+00001fe0: 6772 6f75 7029 290d 0a20 2020 2020 2020  group))..       
+00001ff0: 2066 6f72 206b 6579 2c20 6974 656d 2069   for key, item i
+00002000: 6e20 6772 6f75 702e 6974 656d 7328 293a  n group.items():
+00002010: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00002020: 2069 7369 6e73 7461 6e63 6528 6974 656d   isinstance(item
+00002030: 2c20 6835 7079 2e44 6174 6173 6574 293a  , h5py.Dataset):
+00002040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002050: 2020 7072 696e 7428 7370 6163 6573 202b    print(spaces +
+00002060: 2073 656c 662e 5f5f 6461 7461 7365 745f   self.__dataset_
+00002070: 5f28 6b65 792c 2069 7465 6d29 290d 0a20  _(key, item)).. 
+00002080: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00002090: 6f72 2061 7474 725f 6e61 6d65 2069 6e20  or attr_name in 
+000020a0: 6974 656d 2e61 7474 7273 2e72 6177 2e6b  item.attrs.raw.k
+000020b0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+000020c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+000020d0: 6f74 2061 7474 725f 6e61 6d65 2e69 7375  ot attr_name.isu
+000020e0: 7070 6572 2829 2061 6e64 2061 7474 725f  pper() and attr_
+000020f0: 6e61 6d65 206e 6f74 2069 6e20 7365 6c66  name not in self
+00002100: 2e69 676e 6f72 655f 6174 7472 733a 0d0a  .ignore_attrs:..
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
+00002130: 6c66 2e62 6173 655f 696e 7465 6e74 202a  lf.base_intent *
+00002140: 2028 696e 6465 6e74 202b 2032 2920 2b20   (indent + 2) + 
+00002150: 7365 6c66 2e5f 5f61 7474 7273 5f5f 2861  self.__attrs__(a
+00002160: 7474 725f 6e61 6d65 2c20 6974 656d 2929  ttr_name, item))
+00002170: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00002180: 6966 2069 7369 6e73 7461 6e63 6528 6974  if isinstance(it
+00002190: 656d 2c20 6835 7079 2e47 726f 7570 293a  em, h5py.Group):
+000021a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000021b0: 2020 7072 696e 7428 7370 6163 6573 202b    print(spaces +
+000021c0: 2073 656c 662e 5f5f 6772 6f75 705f 5f28   self.__group__(
+000021d0: 6b65 792c 2069 7465 6d29 290d 0a20 2020  key, item))..   
+000021e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000021f0: 6628 6974 656d 2c20 696e 6465 6e74 202b  f(item, indent +
+00002200: 2031 2c20 6869 6465 5f75 7269 3d68 6964   1, hide_uri=hid
+00002210: 655f 7572 6929 0d0a 0d0a 2020 2020 6465  e_uri)....    de
+00002220: 6620 5f5f 6461 7461 7365 745f 5f28 7365  f __dataset__(se
+00002230: 6c66 2c20 6e61 6d65 3a20 7374 722c 2068  lf, name: str, h
+00002240: 356f 626a 3a20 6835 7079 2e44 6174 6173  5obj: h5py.Datas
+00002250: 6574 2920 2d3e 2073 7472 3a0d 0a20 2020  et) -> str:..   
+00002260: 2020 2020 2069 6620 6835 6f62 6a2e 6474       if h5obj.dt
+00002270: 7970 652e 6368 6172 203d 3d20 2753 273a  ype.char == 'S':
+00002280: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00002290: 6861 6e64 656c 2073 7472 696e 6720 6461  handel string da
+000022a0: 7461 7365 7473 3a0d 0a20 2020 2020 2020  tasets:..       
+000022b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000022c0: 2e5f 5f73 7472 696e 6764 6174 6173 6574  .__stringdataset
+000022d0: 5f5f 286e 616d 652c 2068 356f 626a 290d  __(name, h5obj).
+000022e0: 0a20 2020 2020 2020 2069 6620 6835 6f62  .        if h5ob
+000022f0: 6a2e 6e64 696d 203d 3d20 303a 0d0a 2020  j.ndim == 0:..  
+00002300: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002310: 2073 656c 662e 5f5f 3044 6461 7461 7365   self.__0Ddatase
+00002320: 745f 5f28 6e61 6d65 2c20 6835 6f62 6a29  t__(name, h5obj)
+00002330: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002340: 2073 656c 662e 5f5f 4e44 6461 7461 7365   self.__NDdatase
+00002350: 745f 5f28 6e61 6d65 2c20 6835 6f62 6a29  t__(name, h5obj)
+00002360: 0d0a 0d0a 2020 2020 6465 6620 5f5f 7374  ....    def __st
+00002370: 7269 6e67 6461 7461 7365 745f 5f28 7365  ringdataset__(se
+00002380: 6c66 2c20 6e61 6d65 3a20 7374 722c 2068  lf, name: str, h
+00002390: 356f 626a 3a20 6835 7079 2e44 6174 6173  5obj: h5py.Datas
+000023a0: 6574 2920 2d3e 2073 7472 3a0d 0a20 2020  et) -> str:..   
+000023b0: 2020 2020 2022 2222 7374 7269 6e67 2072       """string r
+000023c0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+000023d0: 2061 2073 7472 696e 6720 6461 7461 7365   a string datase
+000023e0: 7422 2222 0d0a 2020 2020 2020 2020 6966  t"""..        if
+000023f0: 2068 356f 626a 2e6e 6469 6d20 3d3d 2030   h5obj.ndim == 0
+00002400: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00002410: 6574 7572 6e20 6622 5c30 3333 5b31 6d7b  eturn f"\033[1m{
+00002420: 6e61 6d65 7d5c 3033 335b 306d 3a20 7b68  name}\033[0m: {h
+00002430: 356f 626a 2e76 616c 7565 735b 2829 5d7d  5obj.values[()]}
+00002440: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+00002450: 6e20 6622 5c30 3333 5b31 6d7b 6e61 6d65  n f"\033[1m{name
+00002460: 7d5c 3033 335b 306d 3a20 7b68 356f 626a  }\033[0m: {h5obj
+00002470: 2e73 6861 7065 7d2c 2064 7479 7065 3a20  .shape}, dtype: 
+00002480: 7b68 356f 626a 2e64 7479 7065 7d22 0d0a  {h5obj.dtype}"..
+00002490: 0d0a 2020 2020 6465 6620 5f5f 3044 6461  ..    def __0Dda
+000024a0: 7461 7365 745f 5f28 7365 6c66 2c20 6e61  taset__(self, na
+000024b0: 6d65 3a20 7374 722c 2068 356f 626a 3a20  me: str, h5obj: 
+000024c0: 6835 7079 2e44 6174 6173 6574 2920 2d3e  h5py.Dataset) ->
+000024d0: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
+000024e0: 2222 7374 7269 6e67 2072 6570 7265 7365  ""string represe
+000024f0: 6e74 6174 696f 6e20 6f66 2061 2030 4420  ntation of a 0D 
+00002500: 6461 7461 7365 7422 2222 0d0a 2020 2020  dataset"""..    
+00002510: 2020 2020 7661 6c75 6520 3d20 6835 6f62      value = h5ob
+00002520: 6a2e 7661 6c75 6573 5b28 295d 0d0a 2020  j.values[()]..  
+00002530: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00002540: 6e63 6528 7661 6c75 652c 2028 666c 6f61  nce(value, (floa
+00002550: 742c 206e 702e 666c 6f61 7469 6e67 2929  t, np.floating))
+00002560: 3a0d 0a20 2020 2020 2020 2020 2020 2076  :..            v
+00002570: 616c 7565 203d 2066 277b 7661 6c75 653a  alue = f'{value:
+00002580: 667d 270d 0a20 2020 2020 2020 2065 6c69  f}'..        eli
+00002590: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
+000025a0: 7565 2c20 2869 6e74 2c20 6e70 2e69 6e74  ue, (int, np.int
+000025b0: 6567 6572 2929 3a0d 0a20 2020 2020 2020  eger)):..       
+000025c0: 2020 2020 2076 616c 7565 203d 2066 277b       value = f'{
+000025d0: 696e 7428 7661 6c75 6529 3a64 7d27 0d0a  int(value):d}'..
+000025e0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+000025f0: 6e73 7461 6e63 6528 7661 6c75 652c 2028  nstance(value, (
+00002600: 626f 6f6c 2c20 6e70 2e62 6f6f 6c5f 2929  bool, np.bool_))
+00002610: 3a0d 0a20 2020 2020 2020 2020 2020 2076  :..            v
+00002620: 616c 7565 203d 2066 277b 7661 6c75 657d  alue = f'{value}
+00002630: 270d 0a20 2020 2020 2020 2065 6c73 653a  '..        else:
+00002640: 0d0a 2020 2020 2020 2020 2020 2020 7761  ..            wa
+00002650: 726e 696e 6773 2e77 6172 6e28 6627 556e  rnings.warn(f'Un
+00002660: 6578 7065 6374 6564 2074 7970 6520 7b74  expected type {t
+00002670: 7970 6528 7661 6c75 6529 7d27 2c20 5573  ype(value)}', Us
+00002680: 6572 5761 726e 696e 6729 0d0a 2020 2020  erWarning)..    
+00002690: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+000026a0: 273f 7479 7065 3f27 0d0a 2020 2020 2020  '?type?'..      
+000026b0: 2020 7265 7475 726e 2066 225c 3033 335b    return f"\033[
+000026c0: 316d 7b6e 616d 657d 5c30 3333 5b30 6d20  1m{name}\033[0m 
+000026d0: 7b76 616c 7565 7d2c 2064 7479 7065 3a20  {value}, dtype: 
+000026e0: 7b68 356f 626a 2e64 7479 7065 7d22 0d0a  {h5obj.dtype}"..
+000026f0: 0d0a 2020 2020 6465 6620 5f5f 4e44 6461  ..    def __NDda
+00002700: 7461 7365 745f 5f28 7365 6c66 2c20 6e61  taset__(self, na
+00002710: 6d65 2c20 6835 6f62 6a3a 2068 3570 792e  me, h5obj: h5py.
+00002720: 4461 7461 7365 7429 3a0d 0a20 2020 2020  Dataset):..     
+00002730: 2020 2022 2222 7374 7269 6e67 2072 6570     """string rep
+00002740: 7265 7365 6e74 6174 696f 6e20 6f66 2061  resentation of a
+00002750: 204e 4420 6461 7461 7365 7422 2222 0d0a   ND dataset"""..
+00002760: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00002770: 225c 3033 335b 316d 7b6e 616d 657d 5c30  "\033[1m{name}\0
+00002780: 3333 5b30 6d3a 207b 6835 6f62 6a2e 7368  33[0m: {h5obj.sh
+00002790: 6170 657d 2c20 6474 7970 653a 207b 6835  ape}, dtype: {h5
+000027a0: 6f62 6a2e 6474 7970 657d 220d 0a0d 0a20  obj.dtype}".... 
+000027b0: 2020 2064 6566 205f 5f67 726f 7570 5f5f     def __group__
+000027c0: 2873 656c 662c 206e 616d 652c 2069 7465  (self, name, ite
+000027d0: 6d29 202d 3e20 7374 723a 0d0a 2020 2020  m) -> str:..    
+000027e0: 2020 2020 7265 7475 726e 2066 222f 5c30      return f"/\0
+000027f0: 3333 5b31 6d7b 6e61 6d65 7d5c 3033 335b  33[1m{name}\033[
+00002800: 306d 220d 0a0d 0a20 2020 2064 6566 205f  0m"....    def _
+00002810: 5f61 7474 7273 5f5f 2873 656c 662c 206e  _attrs__(self, n
+00002820: 616d 652c 2068 356f 626a 2920 2d3e 2073  ame, h5obj) -> s
+00002830: 7472 3a0d 0a20 2020 2020 2020 2061 7474  tr:..        att
+00002840: 725f 7661 6c75 6520 3d20 6835 6f62 6a2e  r_value = h5obj.
+00002850: 6174 7472 732e 7261 775b 6e61 6d65 5d0d  attrs.raw[name].
+00002860: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
+00002870: 6c66 2e68 6964 655f 7572 693a 0d0a 2020  lf.hide_uri:..  
+00002880: 2020 2020 2020 2020 2020 7573 655f 6174            use_at
+00002890: 7472 5f6e 616d 6520 3d20 6e61 6d65 0d0a  tr_name = name..
+000028a0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000028b0: 2020 2020 2020 2020 2020 2070 7265 6420             pred 
+000028c0: 3d20 6835 6f62 6a2e 7264 665b 6e61 6d65  = h5obj.rdf[name
+000028d0: 5d2e 6765 7428 5244 465f 5052 4544 4943  ].get(RDF_PREDIC
+000028e0: 4154 455f 4154 5452 5f4e 414d 452c 204e  ATE_ATTR_NAME, N
+000028f0: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+00002900: 2020 6174 7472 7364 6566 203d 2068 356f    attrsdef = h5o
+00002910: 626a 2e72 6466 5b6e 616d 655d 2e64 6566  bj.rdf[name].def
+00002920: 696e 6974 696f 6e0d 0a20 2020 2020 2020  inition..       
+00002930: 2020 2020 2069 6620 7072 6564 2061 6e64       if pred and
+00002940: 2061 7474 7273 6465 663a 0d0a 2020 2020   attrsdef:..    
+00002950: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+00002960: 6174 7472 5f6e 616d 6520 3d20 6627 7b6e  attr_name = f'{n
+00002970: 616d 657d 2028 703d 7b70 7265 647d 2c20  ame} (p={pred}, 
+00002980: 6465 663d 7b61 7474 7273 6465 667d 2927  def={attrsdef})'
+00002990: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000029a0: 6966 2070 7265 643a 0d0a 2020 2020 2020  if pred:..      
+000029b0: 2020 2020 2020 2020 2020 7573 655f 6174            use_at
+000029c0: 7472 5f6e 616d 6520 3d20 6627 7b6e 616d  tr_name = f'{nam
+000029d0: 657d 2028 703d 7b70 7265 647d 2927 0d0a  e} (p={pred})'..
+000029e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000029f0: 2061 7474 7273 6465 663a 0d0a 2020 2020   attrsdef:..    
+00002a00: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+00002a10: 6174 7472 5f6e 616d 6520 3d20 6627 7b6e  attr_name = f'{n
+00002a20: 616d 657d 2028 6465 663d 7b61 7474 7273  ame} (def={attrs
+00002a30: 6465 667d 2927 0d0a 2020 2020 2020 2020  def})'..        
+00002a40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002a50: 2020 2020 2020 2020 2020 2075 7365 5f61             use_a
+00002a60: 7474 725f 6e61 6d65 203d 206e 616d 650d  ttr_name = name.
+00002a70: 0a0d 0a20 2020 2020 2020 2020 2020 206f  ...            o
+00002a80: 626a 5f69 7269 203d 2068 356f 626a 2e72  bj_iri = h5obj.r
+00002a90: 6466 5b6e 616d 655d 2e67 6574 2852 4446  df[name].get(RDF
+00002aa0: 5f4f 424a 4543 545f 4154 5452 5f4e 414d  _OBJECT_ATTR_NAM
+00002ab0: 452c 204e 6f6e 6529 0d0a 2020 2020 2020  E, None)..      
+00002ac0: 2020 2020 2020 6966 206f 626a 5f69 7269        if obj_iri
+00002ad0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002ae0: 2020 2061 7474 725f 7661 6c75 6520 3d20     attr_value = 
+00002af0: 6627 7b61 7474 725f 7661 6c75 657d 2028  f'{attr_value} (
+00002b00: 6f3d 7b6f 626a 5f69 7269 7d29 270d 0a0d  o={obj_iri})'...
+00002b10: 0a20 2020 2020 2020 2023 2069 6620 6973  .        # if is
+00002b20: 696e 7374 616e 6365 2861 7474 725f 7661  instance(attr_va
+00002b30: 6c75 652c 2068 3570 792e 4772 6f75 7029  lue, h5py.Group)
+00002b40: 3a0d 0a20 2020 2020 2020 2023 2020 2020  :..        #    
+00002b50: 2061 7474 725f 7661 6c75 6520 3d20 6627   attr_value = f'
+00002b60: 6772 703a 7b61 7474 725f 7661 6c75 652e  grp:{attr_value.
+00002b70: 6e61 6d65 7d27 0d0a 2020 2020 2020 2020  name}'..        
+00002b80: 2320 656c 6966 2069 7369 6e73 7461 6e63  # elif isinstanc
+00002b90: 6528 6174 7472 5f76 616c 7565 2c20 6835  e(attr_value, h5
+00002ba0: 7079 2e44 6174 6173 6574 293a 0d0a 2020  py.Dataset):..  
+00002bb0: 2020 2020 2020 2320 2020 2020 6174 7472        #     attr
+00002bc0: 5f76 616c 7565 203d 2066 2764 7365 743a  _value = f'dset:
+00002bd0: 7b61 7474 725f 7661 6c75 652e 6e61 6d65  {attr_value.name
+00002be0: 7d27 0d0a 2020 2020 2020 2020 7265 7475  }'..        retu
+00002bf0: 726e 2066 275c 3033 335b 336d 613a 207b  rn f'\033[3ma: {
+00002c00: 7573 655f 6174 7472 5f6e 616d 657d 5c30  use_attr_name}\0
+00002c10: 3333 5b30 6d3a 207b 6174 7472 5f76 616c  33[0m: {attr_val
+00002c20: 7565 7d27 0d0a 0d0a 0d0a 636c 6173 7320  ue}'......class 
+00002c30: 4844 4635 5374 7275 6374 7572 6548 544d  HDF5StructureHTM
+00002c40: 4c52 6570 7228 5f48 4446 3553 7472 7563  LRepr(_HDF5Struc
+00002c50: 7475 7265 5265 7072 293a 0d0a 0d0a 2020  tureRepr):....  
+00002c60: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+00002c70: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
+00002c80: 2020 2020 2020 2067 726f 7570 2c0d 0a20         group,.. 
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 636f 6c6c 6170 7365 643a 2062 6f6f 6c20  collapsed: bool 
+00002cb0: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+00002cc0: 2020 2020 2020 2020 2020 7072 6561 6d62            preamb
+00002cd0: 6c65 3a20 7374 7220 3d20 4e6f 6e65 2c0d  le: str = None,.
+00002ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002cf0: 2020 696e 6465 6e74 3a20 696e 7420 3d20    indent: int = 
+00002d00: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00002d10: 2020 2020 2063 6875 6e6b 733a 2062 6f6f       chunks: boo
+00002d20: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
+00002d30: 2020 2020 2020 2020 2020 2020 206d 6178               max
+00002d40: 7368 6170 653a 2062 6f6f 6c20 3d20 4661  shape: bool = Fa
+00002d50: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00002d60: 2020 2020 2020 2068 6964 655f 7572 693a         hide_uri:
+00002d70: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
+00002d80: 0a20 2020 2020 2020 2073 656c 662e 6869  .        self.hi
+00002d90: 6465 5f75 7269 203d 2068 6964 655f 7572  de_uri = hide_ur
+00002da0: 690d 0a20 2020 2020 2020 2069 6620 6973  i..        if is
+00002db0: 696e 7374 616e 6365 2867 726f 7570 2c20  instance(group, 
+00002dc0: 6835 7079 2e47 726f 7570 293a 0d0a 2020  h5py.Group):..  
+00002dd0: 2020 2020 2020 2020 2020 6835 6772 6f75            h5grou
+00002de0: 7020 3d20 6772 6f75 700d 0a20 2020 2020  p = group..     
+00002df0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00002e00: 2020 2020 2020 6835 6772 6f75 7020 3d20        h5group = 
+00002e10: 6772 6f75 705b 272f 275d 0d0a 0d0a 2020  group['/']....  
+00002e20: 2020 2020 2020 7365 6c66 2e63 6f6c 6c61        self.colla
+00002e30: 7073 6564 203d 2063 6f6c 6c61 7073 6564  psed = collapsed
+00002e40: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00002e50: 2e5f 6f62 6a5f 6366 672e 7570 6461 7465  ._obj_cfg.update
+00002e60: 287b 2763 6875 6e6b 7327 3a20 6368 756e  ({'chunks': chun
+00002e70: 6b73 2c0d 0a20 2020 2020 2020 2020 2020  ks,..           
+00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e90: 2020 2027 6d61 7873 6861 7065 273a 206d     'maxshape': m
+00002ea0: 6178 7368 6170 657d 290d 0a0d 0a20 2020  axshape})....   
+00002eb0: 2020 2020 205f 6964 203d 2068 3567 726f       _id = h5gro
+00002ec0: 7570 2e6e 616d 6520 2b20 7065 7266 5f63  up.name + perf_c
+00002ed0: 6f75 6e74 6572 5f6e 7328 292e 5f5f 7374  ounter_ns().__st
+00002ee0: 725f 5f28 290d 0a0d 0a20 2020 2020 2020  r__()....       
+00002ef0: 205f 6874 6d6c 203d 2066 273c 6865 6164   _html = f'<head
+00002f00: 3e3c 7374 796c 653e 7b43 5353 5f53 5452  ><style>{CSS_STR
+00002f10: 7d3c 2f73 7479 6c65 3e3c 2f68 6561 643e  }</style></head>
+00002f20: 270d 0a20 2020 2020 2020 2069 6620 7072  '..        if pr
+00002f30: 6561 6d62 6c65 3a0d 0a20 2020 2020 2020  eamble:..       
+00002f40: 2020 2020 205f 6874 6d6c 202b 3d20 6627       _html += f'
+00002f50: 5c6e 7b70 7265 616d 626c 657d 5c6e 270d  \n{preamble}\n'.
+00002f60: 0a20 2020 2020 2020 205f 6874 6d6c 202b  .        _html +
+00002f70: 3d20 225c 6e3c 6469 7620 636c 6173 733d  = "\n<div class=
+00002f80: 2768 3574 622d 7761 7270 273e 220d 0a20  'h5tb-warp'>".. 
+00002f90: 2020 2020 2020 205f 6874 6d6c 202b 3d20         _html += 
+00002fa0: 7365 6c66 2e5f 5f67 726f 7570 5f5f 2868  self.__group__(h
+00002fb0: 3567 726f 7570 2e6e 616d 652e 7273 706c  5group.name.rspl
+00002fc0: 6974 2827 2f27 2c20 3129 5b31 5d2c 2068  it('/', 1)[1], h
+00002fd0: 3567 726f 7570 290d 0a20 2020 2020 2020  5group)..       
+00002fe0: 205f 6874 6d6c 202b 3d20 225c 6e3c 2f64   _html += "\n</d
+00002ff0: 6976 3e22 0d0a 2020 2020 2020 2020 7265  iv>"..        re
+00003000: 7475 726e 205f 6874 6d6c 0d0a 0d0a 2020  turn _html....  
+00003010: 2020 6465 6620 5f5f 7374 7269 6e67 6461    def __stringda
+00003020: 7461 7365 745f 5f28 7365 6c66 2c20 6e61  taset__(self, na
+00003030: 6d65 2c20 6835 6f62 6a29 202d 3e20 7374  me, h5obj) -> st
+00003040: 723a 0d0a 2020 2020 2020 2020 6966 2068  r:..        if h
+00003050: 356f 626a 2e6e 6469 6d20 3d3d 2030 3a0d  5obj.ndim == 0:.
+00003060: 0a20 2020 2020 2020 2020 2020 205f 7063  .            _pc
+00003070: 6e73 203d 2070 6572 665f 636f 756e 7465  ns = perf_counte
+00003080: 725f 6e73 2829 2e5f 5f73 7472 5f5f 2829  r_ns().__str__()
+00003090: 0d0a 2020 2020 2020 2020 2020 2020 5f69  ..            _i
+000030a0: 6431 203d 2066 2764 732d 312d 7b68 356f  d1 = f'ds-1-{h5o
+000030b0: 626a 2e6e 616d 657d 2d7b 5f70 636e 737d  bj.name}-{_pcns}
+000030c0: 3127 0d0a 2020 2020 2020 2020 2020 2020  1'..            
+000030d0: 5f69 6432 203d 2066 2764 732d 322d 7b68  _id2 = f'ds-2-{h
+000030e0: 356f 626a 2e6e 616d 657d 2d7b 5f70 636e  5obj.name}-{_pcn
+000030f0: 737d 3227 0d0a 2020 2020 2020 2020 2020  s}2'..          
+00003100: 2020 7265 7475 726e 2066 2222 225c 6e0d    return f"""\n.
+00003110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003120: 2020 2020 203c 756c 2069 643d 227b 5f69       <ul id="{_i
+00003130: 6431 7d22 2063 6c61 7373 3d22 6835 7462  d1}" class="h5tb
+00003140: 2d76 6172 2d6c 6973 7422 3e0d 0a20 2020  -var-list">..   
+00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003160: 203c 696e 7075 7420 6964 3d22 7b5f 6964   <input id="{_id
+00003170: 327d 2220 636c 6173 733d 2268 3574 622d  2}" class="h5tb-
+00003180: 7661 726e 616d 652d 696e 2220 7479 7065  varname-in" type
+00003190: 3d22 6368 6563 6b62 6f78 2220 7b73 656c  ="checkbox" {sel
+000031a0: 662e 6368 6563 6b62 6f78 5f73 7461 7465  f.checkbox_state
+000031b0: 7d3e 0d0a 2020 2020 2020 2020 2020 2020  }>..            
+000031c0: 2020 2020 2020 2020 3c6c 6162 656c 2063          <label c
+000031d0: 6c61 7373 3d27 6835 7462 2d76 6172 6e61  lass='h5tb-varna
+000031e0: 6d65 2720 0d0a 2020 2020 2020 2020 2020  me' ..          
+000031f0: 2020 2020 2020 2020 2020 666f 723d 227b            for="{
+00003200: 5f69 6432 7d22 3e7b 6e61 6d65 7d3c 2f6c  _id2}">{name}</l
+00003210: 6162 656c 3e3a 205b 7b68 356f 626a 2e64  abel>: [{h5obj.d
+00003220: 7479 7065 7d5d 2064 6174 613d 7b68 356f  type}] data={h5o
+00003230: 626a 2e76 616c 7565 735b 2829 5d7d 0d0a  bj.values[()]}..
+00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003250: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00003260: 2065 6c69 6620 6835 6f62 6a2e 6e64 696d   elif h5obj.ndim
+00003270: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+00003280: 2020 2020 5f70 636e 7320 3d20 7065 7266      _pcns = perf
+00003290: 5f63 6f75 6e74 6572 5f6e 7328 292e 5f5f  _counter_ns().__
+000032a0: 7374 725f 5f28 290d 0a20 2020 2020 2020  str__()..       
+000032b0: 2020 2020 205f 6964 3120 3d20 6627 6473       _id1 = f'ds
+000032c0: 2d31 2d7b 6835 6f62 6a2e 6e61 6d65 7d2d  -1-{h5obj.name}-
+000032d0: 7b5f 7063 6e73 7d31 270d 0a20 2020 2020  {_pcns}1'..     
+000032e0: 2020 2020 2020 205f 6964 3220 3d20 6627         _id2 = f'
+000032f0: 6473 2d32 2d7b 6835 6f62 6a2e 6e61 6d65  ds-2-{h5obj.name
+00003300: 7d2d 7b5f 7063 6e73 7d32 270d 0a20 2020  }-{_pcns}2'..   
+00003310: 2020 2020 2020 2020 205f 7374 7264 6174           _strdat
+00003320: 6120 3d20 6835 6f62 6a5b 2829 5d0d 0a20  a = h5obj[()].. 
+00003330: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00003340: 696e 7374 616e 6365 285f 7374 7264 6174  instance(_strdat
+00003350: 612c 2078 722e 4461 7461 4172 7261 7929  a, xr.DataArray)
+00003360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003370: 2020 2072 6574 7572 6e20 6622 2222 5c6e     return f"""\n
+00003380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003390: 2020 2020 2020 2020 2020 3c75 6c20 6964            <ul id
+000033a0: 3d22 7b5f 6964 317d 2220 636c 6173 733d  ="{_id1}" class=
+000033b0: 2268 3574 622d 7661 722d 6c69 7374 223e  "h5tb-var-list">
+000033c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000033d0: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
+000033e0: 2069 643d 227b 5f69 6432 7d22 2063 6c61   id="{_id2}" cla
+000033f0: 7373 3d22 6835 7462 2d76 6172 6e61 6d65  ss="h5tb-varname
+00003400: 2d69 6e22 2074 7970 653d 2263 6865 636b  -in" type="check
+00003410: 626f 7822 207b 7365 6c66 2e63 6865 636b  box" {self.check
+00003420: 626f 785f 7374 6174 657d 3e0d 0a20 2020  box_state}>..   
+00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003440: 2020 2020 203c 6c61 6265 6c20 636c 6173       <label clas
+00003450: 733d 2768 3574 622d 7661 726e 616d 6527  s='h5tb-varname'
+00003460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003470: 2020 2020 2020 2020 2020 666f 723d 227b            for="{
+00003480: 5f69 6432 7d22 3e7b 6e61 6d65 7d3c 2f6c  _id2}">{name}</l
+00003490: 6162 656c 3e3a 205b 7b68 356f 626a 2e64  abel>: [{h5obj.d
+000034a0: 7479 7065 7d5d 0d0a 2020 2020 2020 2020  type}]..        
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
+000034d0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+000034e0: 2020 2020 2020 2073 7472 5f76 616c 7565         str_value
+000034f0: 7320 3d20 272c 2027 2e6a 6f69 6e28 5f73  s = ', '.join(_s
+00003500: 7472 6461 7461 290d 0a20 2020 2020 2020  trdata)..       
+00003510: 2020 2020 2065 7863 6570 7420 556e 6963       except Unic
+00003520: 6f64 6544 6563 6f64 6545 7272 6f72 3a0d  odeDecodeError:.
+00003530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003540: 2073 7472 5f76 616c 7565 7320 3d20 273c   str_values = '<
+00003550: 693e 556e 6963 6f64 6544 6563 6f64 6545  i>UnicodeDecodeE
+00003560: 7272 6f72 3c2f 693e 270d 0a20 2020 2020  rror</i>'..     
+00003570: 2020 2020 2020 2065 7863 6570 7420 5479         except Ty
+00003580: 7065 4572 726f 723a 0d0a 2020 2020 2020  peError:..      
+00003590: 2020 2020 2020 2020 2020 7374 725f 7661            str_va
+000035a0: 6c75 6573 203d 2066 273c 693e 5479 7065  lues = f'<i>Type
+000035b0: 4572 726f 723a 207b 7479 7065 285f 7374  Error: {type(_st
+000035c0: 7264 6174 6129 7d3c 2f69 3e27 0d0a 2020  rdata)}</i>'..  
+000035d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000035e0: 2066 2222 225c 6e0d 0a20 2020 2020 2020   f"""\n..       
+000035f0: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
+00003600: 2069 643d 227b 5f69 6431 7d22 2063 6c61   id="{_id1}" cla
+00003610: 7373 3d22 6835 7462 2d76 6172 2d6c 6973  ss="h5tb-var-lis
+00003620: 7422 3e0d 0a20 2020 2020 2020 2020 2020  t">..           
+00003630: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+00003640: 6964 3d22 7b5f 6964 327d 2220 636c 6173  id="{_id2}" clas
+00003650: 733d 2268 3574 622d 7661 726e 616d 652d  s="h5tb-varname-
+00003660: 696e 2220 7479 7065 3d22 6368 6563 6b62  in" type="checkb
+00003670: 6f78 2220 7b73 656c 662e 6368 6563 6b62  ox" {self.checkb
+00003680: 6f78 5f73 7461 7465 7d3e 0d0a 2020 2020  ox_state}>..    
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 3c6c 6162 656c 2063 6c61 7373 3d27 6835  <label class='h5
+000036b0: 7462 2d76 6172 6e61 6d65 270d 0a20 2020  tb-varname'..   
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2066 6f72 3d22 7b5f 6964 327d 223e 7b6e   for="{_id2}">{n
+000036e0: 616d 657d 3c2f 6c61 6265 6c3e 3a20 5b7b  ame}</label>: [{
+000036f0: 6835 6f62 6a2e 6474 7970 657d 5d20 6461  h5obj.dtype}] da
+00003700: 7461 3d22 7b73 7472 5f76 616c 7565 737d  ta="{str_values}
+00003710: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00003720: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00003730: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00003740: 5f5f 4e44 6461 7461 7365 745f 5f28 6e61  __NDdataset__(na
+00003750: 6d65 2c20 6835 6f62 6a29 0d0a 0d0a 2020  me, h5obj)....  
+00003760: 2020 6465 6620 5f5f 3044 6461 7461 7365    def __0Ddatase
+00003770: 745f 5f28 7365 6c66 2c20 6e61 6d65 3a20  t__(self, name: 
+00003780: 7374 722c 2068 356f 626a 3a20 6835 7079  str, h5obj: h5py
+00003790: 2e44 6174 6173 6574 2920 2d3e 2073 7472  .Dataset) -> str
+000037a0: 3a0d 0a20 2020 2020 2020 205f 6964 3120  :..        _id1 
+000037b0: 3d20 6627 6473 2d31 2d7b 6835 6f62 6a2e  = f'ds-1-{h5obj.
+000037c0: 6e61 6d65 7d2d 7b70 6572 665f 636f 756e  name}-{perf_coun
+000037d0: 7465 725f 6e73 2829 2e5f 5f73 7472 5f5f  ter_ns().__str__
+000037e0: 2829 7d27 0d0a 2020 2020 2020 2020 5f69  ()}'..        _i
+000037f0: 6432 203d 2066 2764 732d 322d 7b68 356f  d2 = f'ds-2-{h5o
+00003800: 626a 2e6e 616d 657d 2d7b 7065 7266 5f63  bj.name}-{perf_c
+00003810: 6f75 6e74 6572 5f6e 7328 292e 5f5f 7374  ounter_ns().__st
+00003820: 725f 5f28 297d 270d 0a20 2020 2020 2020  r__()}'..       
+00003830: 2023 2066 6967 7572 6520 6f75 7420 756e   # figure out un
+00003840: 6974 2061 7474 7269 6275 7465 2e20 4974  it attribute. It
+00003850: 206d 6179 2062 6520 756e 6974 206f 7220   may be unit or 
+00003860: 6465 6669 6e65 6420 696e 2049 5249 0d0a  defined in IRI..
+00003870: 2020 2020 2020 2020 756e 6974 7320 3d20          units = 
+00003880: 6835 6f62 6a2e 6174 7472 732e 6765 7428  h5obj.attrs.get(
+00003890: 2775 6e69 7473 272c 204e 6f6e 6529 0d0a  'units', None)..
+000038a0: 2020 2020 2020 2020 6966 2075 6e69 7473          if units
+000038b0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+000038c0: 2020 2020 2020 2075 6e69 7473 203d 2027         units = '
+000038d0: 270d 0a20 2020 2020 2020 2020 2020 2070  '..            p
+000038e0: 7265 645f 6469 6374 203d 2068 356f 626a  red_dict = h5obj
+000038f0: 2e61 7474 7273 2e67 6574 2852 4446 5f50  .attrs.get(RDF_P
+00003900: 5245 4449 4341 5445 5f41 5454 525f 4e41  REDICATE_ATTR_NA
+00003910: 4d45 2c20 4e6f 6e65 290d 0a20 2020 2020  ME, None)..     
+00003920: 2020 2020 2020 2069 6620 7072 6564 5f64         if pred_d
+00003930: 6963 743a 0d0a 2020 2020 2020 2020 2020  ict:..          
+00003940: 2020 2020 2020 666f 7220 6b2c 2076 2069        for k, v i
+00003950: 6e20 7072 6564 5f64 6963 742e 6974 656d  n pred_dict.item
+00003960: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00003970: 2020 2020 2020 2020 2020 6966 2076 203d            if v =
+00003980: 3d20 6861 7355 6e69 7449 5249 3a0d 0a20  = hasUnitIRI:.. 
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 2020 2020 2020 2075 6e69 7473 203d 2068         units = h
+000039b0: 356f 626a 2e61 7474 7273 5b6b 5d2e 7273  5obj.attrs[k].rs
+000039c0: 706c 6974 2827 2f27 2c20 3129 5b2d 315d  plit('/', 1)[-1]
+000039d0: 0d0a 2020 2020 2020 2020 5f68 746d 6c20  ..        _html 
+000039e0: 3d20 6622 2222 5c6e 0d0a 2020 2020 2020  = f"""\n..      
+000039f0: 2020 2020 2020 2020 2020 3c75 6c20 6964            <ul id
+00003a00: 3d22 7b5f 6964 317d 2220 636c 6173 733d  ="{_id1}" class=
+00003a10: 2268 3574 622d 7661 722d 6c69 7374 223e  "h5tb-var-list">
+00003a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003a30: 2020 3c69 6e70 7574 2069 643d 227b 5f69    <input id="{_i
+00003a40: 6432 7d22 2063 6c61 7373 3d22 6835 7462  d2}" class="h5tb
+00003a50: 2d76 6172 6e61 6d65 2d69 6e22 2074 7970  -varname-in" typ
+00003a60: 653d 2263 6865 636b 626f 7822 207b 7365  e="checkbox" {se
+00003a70: 6c66 2e63 6865 636b 626f 785f 7374 6174  lf.checkbox_stat
+00003a80: 657d 3e0d 0a20 2020 2020 2020 2020 2020  e}>..           
+00003a90: 2020 2020 203c 6c61 6265 6c20 636c 6173       <label clas
+00003aa0: 733d 2768 3574 622d 7661 726e 616d 6527  s='h5tb-varname'
+00003ab0: 2066 6f72 3d22 7b5f 6964 327d 223e 7b6e   for="{_id2}">{n
+00003ac0: 616d 657d 3c2f 6c61 6265 6c3e 0d0a 2020  ame}</label>..  
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00003ae0: 7061 6e20 636c 6173 733d 2268 3574 622d  pan class="h5tb-
+00003af0: 6469 6d73 223e 7b68 356f 626a 2e76 616c  dims">{h5obj.val
+00003b00: 7565 735b 2829 5d7d 205b 7b75 6e69 7473  ues[()]} [{units
+00003b10: 7d5d 2028 7b68 356f 626a 2e64 7479 7065  }] ({h5obj.dtype
+00003b20: 7d29 3c2f 7370 616e 3e22 2222 0d0a 2020  })</span>"""..  
+00003b30: 2020 2020 2020 7265 7475 726e 205f 6874        return _ht
+00003b40: 6d6c 0d0a 0d0a 2020 2020 6465 6620 5f5f  ml....    def __
+00003b50: 4e44 6461 7461 7365 745f 5f28 7365 6c66  NDdataset__(self
+00003b60: 2c20 6e61 6d65 2c20 6835 6f62 6a3a 2068  , name, h5obj: h
+00003b70: 3570 792e 4461 7461 7365 7429 3a0d 0a20  5py.Dataset):.. 
+00003b80: 2020 2020 2020 2064 735f 6469 726e 616d         ds_dirnam
+00003b90: 6520 3d20 6f73 2e70 6174 682e 6469 726e  e = os.path.dirn
+00003ba0: 616d 6528 6835 6f62 6a2e 6e61 6d65 290d  ame(h5obj.name).
+00003bb0: 0a20 2020 2020 2020 205f 7368 6170 6520  .        _shape 
+00003bc0: 3d20 6835 6f62 6a2e 7368 6170 650d 0a20  = h5obj.shape.. 
+00003bd0: 2020 2020 2020 2069 6620 6765 745f 636f         if get_co
+00003be0: 6e66 6967 2827 6164 7661 6e63 6564 5f73  nfig('advanced_s
+00003bf0: 6861 7065 5f72 6570 7227 293a 0d0a 2020  hape_repr'):..  
+00003c00: 2020 2020 2020 2020 2020 5f73 6861 7065            _shape
+00003c10: 5f72 6570 7220 3d20 2728 270d 0a20 2020  _repr = '('..   
+00003c20: 2020 2020 2020 2020 206e 6469 6d20 3d20           ndim = 
+00003c30: 6835 6f62 6a2e 6e64 696d 0d0a 2020 2020  h5obj.ndim..    
+00003c40: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00003c50: 2072 616e 6765 286e 6469 6d29 3a0d 0a20   range(ndim):.. 
+00003c60: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00003c70: 7269 675f 6469 6d5f 6e61 6d65 203d 204e  rig_dim_name = N
+00003c80: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00003c90: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00003cb0: 7269 675f 6469 6d5f 6e61 6d65 203d 2068  rig_dim_name = h
+00003cc0: 356f 626a 2e64 696d 735b 695d 5b30 5d2e  5obj.dims[i][0].
+00003cd0: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
+00003ce0: 2020 2020 2020 6578 6365 7074 2052 756e        except Run
+00003cf0: 7469 6d65 4572 726f 723a 0d0a 2020 2020  timeError:..    
+00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 7061 7373 2020 2320 6e6f 2064 696d 656e  pass  # no dimen
+00003d20: 7369 6f6e 2073 6361 6c65 2063 6f75 6c64  sion scale could
+00003d30: 2062 6520 666f 756e 640d 0a20 2020 2020   be found..     
+00003d40: 2020 2020 2020 2020 2020 2069 6620 6f72             if or
+00003d50: 6967 5f64 696d 5f6e 616d 653a 0d0a 2020  ig_dim_name:..  
+00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d70: 2020 6966 206f 732e 7061 7468 2e64 6972    if os.path.dir
+00003d80: 6e61 6d65 286f 7269 675f 6469 6d5f 6e61  name(orig_dim_na
+00003d90: 6d65 2920 3d3d 2064 735f 6469 726e 616d  me) == ds_dirnam
+00003da0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003db0: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
+00003dc0: 6e61 6d65 203d 206f 732e 7061 7468 2e62  name = os.path.b
+00003dd0: 6173 656e 616d 6528 6f72 6967 5f64 696d  asename(orig_dim
+00003de0: 5f6e 616d 6529 0d0a 2020 2020 2020 2020  _name)..        
+00003df0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00003e00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003e10: 2020 2020 2020 2020 2020 2064 696d 5f6e             dim_n
+00003e20: 616d 6520 3d20 6f72 6967 5f64 696d 5f6e  ame = orig_dim_n
+00003e30: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
+00003e40: 2020 2020 2020 2020 2069 6620 6920 3d3d           if i ==
+00003e50: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00003e60: 2020 2020 2020 2020 2020 2020 205f 7368               _sh
+00003e70: 6170 655f 7265 7072 202b 3d20 6627 7b64  ape_repr += f'{d
+00003e80: 696d 5f6e 616d 657d 3a20 7b5f 7368 6170  im_name}: {_shap
+00003e90: 655b 695d 7d27 0d0a 2020 2020 2020 2020  e[i]}'..        
+00003ea0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00003eb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003ec0: 2020 2020 2020 2020 2020 205f 7368 6170             _shap
+00003ed0: 655f 7265 7072 202b 3d20 6627 2c20 7b64  e_repr += f', {d
+00003ee0: 696d 5f6e 616d 657d 3a20 7b5f 7368 6170  im_name}: {_shap
+00003ef0: 655b 695d 7d27 0d0a 2020 2020 2020 2020  e[i]}'..        
+00003f00: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00003f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f20: 2020 2069 6620 6920 3d3d 2030 3a0d 0a20     if i == 0:.. 
+00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f40: 2020 2020 2020 205f 7368 6170 655f 7265         _shape_re
+00003f50: 7072 202b 3d20 6627 7b5f 7368 6170 655b  pr += f'{_shape[
+00003f60: 695d 7d27 0d0a 2020 2020 2020 2020 2020  i]}'..          
+00003f70: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00003f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003f90: 2020 2020 2020 2020 205f 7368 6170 655f           _shape_
+00003fa0: 7265 7072 202b 3d20 6627 2c20 7b5f 7368  repr += f', {_sh
+00003fb0: 6170 655b 695d 7d27 0d0a 2020 2020 2020  ape[i]}'..      
+00003fc0: 2020 2020 2020 5f73 6861 7065 5f72 6570        _shape_rep
+00003fd0: 7220 2b3d 2027 2927 0d0a 2020 2020 2020  r += ')'..      
+00003fe0: 2020 2020 2020 6966 205f 7368 6170 655f        if _shape_
+00003ff0: 7265 7072 203d 3d20 2728 2927 2061 6e64  repr == '()' and
+00004000: 206e 6469 6d20 3e20 303a 0d0a 2020 2020   ndim > 0:..    
+00004010: 2020 2020 2020 2020 2020 2020 5f73 6861              _sha
+00004020: 7065 5f72 6570 7220 3d20 5f73 6861 7065  pe_repr = _shape
+00004030: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00004040: 0a20 2020 2020 2020 2020 2020 205f 7368  .            _sh
+00004050: 6170 655f 7265 7072 203d 205f 7368 6170  ape_repr = _shap
+00004060: 650d 0a0d 0a20 2020 2020 2020 2069 6620  e....        if 
+00004070: 7365 6c66 2e5f 6f62 6a5f 6366 675b 2763  self._obj_cfg['c
+00004080: 6875 6e6b 7327 5d3a 0d0a 2020 2020 2020  hunks']:..      
+00004090: 2020 2020 2020 6368 756e 6b73 5f73 7472        chunks_str
+000040a0: 203d 2066 2720 6368 756e 6b73 3d7b 6835   = f' chunks={h5
+000040b0: 6f62 6a2e 6368 756e 6b73 7d27 0d0a 2020  obj.chunks}'..  
+000040c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000040d0: 2020 2020 2020 2020 2063 6875 6e6b 735f           chunks_
+000040e0: 7374 7220 3d20 2727 0d0a 0d0a 2020 2020  str = ''....    
+000040f0: 2020 2020 6966 2073 656c 662e 5f6f 626a      if self._obj
+00004100: 5f63 6667 5b27 6d61 7873 6861 7065 275d  _cfg['maxshape']
+00004110: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
+00004120: 6178 7368 6170 655f 7374 7220 3d20 6627  axshape_str = f'
+00004130: 206d 6178 7368 6170 653d 7b68 356f 626a   maxshape={h5obj
+00004140: 2e6d 6178 7368 6170 657d 270d 0a20 2020  .maxshape}'..   
+00004150: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00004160: 2020 2020 2020 2020 6d61 7873 6861 7065          maxshape
+00004170: 5f73 7472 203d 2027 270d 0a0d 0a20 2020  _str = ''....   
+00004180: 2020 2020 205f 6964 3120 3d20 6627 6473       _id1 = f'ds
+00004190: 2d31 2d7b 6835 6f62 6a2e 6e61 6d65 7d2d  -1-{h5obj.name}-
+000041a0: 7b70 6572 665f 636f 756e 7465 725f 6e73  {perf_counter_ns
+000041b0: 2829 2e5f 5f73 7472 5f5f 2829 7d27 0d0a  ().__str__()}'..
+000041c0: 2020 2020 2020 2020 5f69 6432 203d 2066          _id2 = f
+000041d0: 2764 732d 322d 7b68 356f 626a 2e6e 616d  'ds-2-{h5obj.nam
+000041e0: 657d 2d7b 7065 7266 5f63 6f75 6e74 6572  e}-{perf_counter
+000041f0: 5f6e 7328 292e 5f5f 7374 725f 5f28 297d  _ns().__str__()}
+00004200: 270d 0a0d 0a20 2020 2020 2020 205f 6874  '....        _ht
+00004210: 6d6c 203d 2066 2222 225c 6e0d 0a20 2020  ml = f"""\n..   
+00004220: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
+00004230: 2069 643d 227b 5f69 6431 7d22 2063 6c61   id="{_id1}" cla
+00004240: 7373 3d22 6835 7462 2d76 6172 2d6c 6973  ss="h5tb-var-lis
+00004250: 7422 3e0d 0a20 2020 2020 2020 2020 2020  t">..           
+00004260: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+00004270: 6964 3d22 7b5f 6964 327d 2220 636c 6173  id="{_id2}" clas
+00004280: 733d 2268 3574 622d 7661 726e 616d 652d  s="h5tb-varname-
+00004290: 696e 2220 7479 7065 3d22 6368 6563 6b62  in" type="checkb
+000042a0: 6f78 2220 7b73 656c 662e 6368 6563 6b62  ox" {self.checkb
+000042b0: 6f78 5f73 7461 7465 7d3e 0d0a 2020 2020  ox_state}>..    
+000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042d0: 3c6c 6162 656c 2063 6c61 7373 3d27 6835  <label class='h5
+000042e0: 7462 2d76 6172 6e61 6d65 2720 666f 723d  tb-varname' for=
+000042f0: 227b 5f69 6432 7d22 3e7b 6e61 6d65 7d3c  "{_id2}">{name}<
+00004300: 2f6c 6162 656c 3e0d 0a20 2020 2020 2020  /label>..       
+00004310: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
+00004320: 616e 2063 6c61 7373 3d22 6835 7462 2d64  an class="h5tb-d
+00004330: 696d 7322 3e7b 5f73 6861 7065 5f72 6570  ims">{_shape_rep
+00004340: 727d 205b 7b68 356f 626a 2e64 7479 7065  r} [{h5obj.dtype
+00004350: 7d5d 7b63 6875 6e6b 735f 7374 727d 7b6d  }]{chunks_str}{m
+00004360: 6178 7368 6170 655f 7374 727d 3c2f 7370  axshape_str}</sp
+00004370: 616e 3e22 2222 0d0a 2020 2020 2020 2020  an>"""..        
+00004380: 7265 7475 726e 205f 6874 6d6c 0d0a 0d0a  return _html....
+00004390: 2020 2020 6465 6620 5f5f 6461 7461 7365      def __datase
+000043a0: 745f 5f28 7365 6c66 2c20 6e61 6d65 2c20  t__(self, name, 
+000043b0: 6835 6f62 6a29 202d 3e20 7374 723a 0d0a  h5obj) -> str:..
+000043c0: 2020 2020 2020 2020 2222 2267 656e 6572          """gener
+000043d0: 6174 6520 6874 6d6c 2072 6570 7265 7365  ate html represe
+000043e0: 6e74 6174 696f 6e20 6f66 2061 2064 6174  ntation of a dat
+000043f0: 6173 6574 2222 220d 0a0d 0a20 2020 2020  aset"""....     
+00004400: 2020 2023 2069 7269 203d 2068 356f 626a     # iri = h5obj
+00004410: 2e72 6466 2e70 7265 6469 6361 7465 2e67  .rdf.predicate.g
+00004420: 6574 2827 5345 4c46 272c 204e 6f6e 6529  et('SELF', None)
+00004430: 0d0a 2020 2020 2020 2020 7365 6c66 5f70  ..        self_p
+00004440: 7265 6469 6361 7465 203d 2068 356f 626a  redicate = h5obj
+00004450: 2e72 6466 2e70 7265 6469 6361 7465 2e67  .rdf.predicate.g
+00004460: 6574 2827 5345 4c46 272c 204e 6f6e 6529  et('SELF', None)
+00004470: 0d0a 2020 2020 2020 2020 7365 6c66 5f74  ..        self_t
+00004480: 7970 6520 3d20 6835 6f62 6a2e 7264 662e  ype = h5obj.rdf.
+00004490: 7479 7065 0d0a 2020 2020 2020 2020 7365  type..        se
+000044a0: 6c66 5f49 4420 3d20 6835 6f62 6a2e 7264  lf_ID = h5obj.rd
+000044b0: 662e 7375 626a 6563 740d 0a20 2020 2020  f.subject..     
+000044c0: 2020 205f 6473 6e61 6d65 203d 206e 616d     _dsname = nam
+000044d0: 650d 0a0d 0a20 2020 2020 2020 2069 6620  e....        if 
+000044e0: 7365 6c66 5f74 7970 6520 6973 206e 6f74  self_type is not
+000044f0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00004500: 2020 2020 5f64 736e 616d 6520 2b3d 2067      _dsname += g
+00004510: 6574 5f69 7269 5f69 636f 6e5f 6872 6566  et_iri_icon_href
+00004520: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00004530: 2020 2073 656c 665f 7479 7065 2c20 6963     self_type, ic
+00004540: 6f6e 5f75 726c 3d54 5950 455f 4943 4f4e  on_url=TYPE_ICON
+00004550: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004560: 2020 2074 6f6f 6c74 6970 7465 7874 3d66     tooltiptext=f
+00004570: 2740 7479 7065 3d7b 7365 6c66 5f74 7970  '@type={self_typ
+00004580: 657d 2729 0d0a 0d0a 2020 2020 2020 2020  e}')....        
+00004590: 6966 2073 656c 665f 4944 2069 7320 6e6f  if self_ID is no
+000045a0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+000045b0: 2020 2020 205f 6473 6e61 6d65 202b 3d20       _dsname += 
+000045c0: 6765 745f 6972 695f 6963 6f6e 5f68 7265  get_iri_icon_hre
+000045d0: 6628 0d0a 2020 2020 2020 2020 2020 2020  f(..            
+000045e0: 2020 2020 7365 6c66 5f49 442c 2069 636f      self_ID, ico
+000045f0: 6e5f 7572 6c3d 4944 5f49 434f 4e2c 0d0a  n_url=ID_ICON,..
+00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004610: 746f 6f6c 7469 7074 6578 743d 6627 4069  tooltiptext=f'@i
+00004620: 643d 7b73 656c 665f 4944 7d27 290d 0a0d  d={self_ID}')...
+00004630: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00004640: 5f70 7265 6469 6361 7465 2069 7320 6e6f  _predicate is no
+00004650: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00004660: 2020 2020 205f 6473 6e61 6d65 202b 3d20       _dsname += 
+00004670: 6765 745f 6972 695f 6963 6f6e 5f68 7265  get_iri_icon_hre
+00004680: 6628 7365 6c66 5f70 7265 6469 6361 7465  f(self_predicate
+00004690: 2c20 6963 6f6e 5f75 726c 3d49 5249 5f49  , icon_url=IRI_I
+000046a0: 434f 4e29 0d0a 0d0a 2020 2020 2020 2020  CON)....        
+000046b0: 6973 5f73 7472 696e 675f 6461 7461 7365  is_string_datase
+000046c0: 7420 3d20 6835 6f62 6a2e 6474 7970 652e  t = h5obj.dtype.
+000046d0: 6368 6172 203d 3d20 2753 270d 0a20 2020  char == 'S'..   
+000046e0: 2020 2020 2069 6620 6973 5f73 7472 696e       if is_strin
+000046f0: 675f 6461 7461 7365 743a 0d0a 2020 2020  g_dataset:..    
+00004700: 2020 2020 2020 2020 5f68 746d 6c5f 7072          _html_pr
+00004710: 6520 3d20 7365 6c66 2e5f 5f73 7472 696e  e = self.__strin
+00004720: 6764 6174 6173 6574 5f5f 285f 6473 6e61  gdataset__(_dsna
+00004730: 6d65 2c20 6835 6f62 6a29 0d0a 2020 2020  me, h5obj)..    
+00004740: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00004750: 2020 2020 2020 2069 6620 6835 6f62 6a2e         if h5obj.
+00004760: 6e64 696d 203d 3d20 303a 0d0a 2020 2020  ndim == 0:..    
+00004770: 2020 2020 2020 2020 2020 2020 5f68 746d              _htm
+00004780: 6c5f 7072 6520 3d20 7365 6c66 2e5f 5f30  l_pre = self.__0
+00004790: 4464 6174 6173 6574 5f5f 285f 6473 6e61  Ddataset__(_dsna
+000047a0: 6d65 2c20 6835 6f62 6a29 0d0a 2020 2020  me, h5obj)..    
+000047b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000047c0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+000047d0: 6874 6d6c 5f70 7265 203d 2073 656c 662e  html_pre = self.
+000047e0: 5f5f 4e44 6461 7461 7365 745f 5f28 5f64  __NDdataset__(_d
+000047f0: 736e 616d 652c 2068 356f 626a 290d 0a0d  sname, h5obj)...
+00004800: 0a20 2020 2020 2020 2023 206e 6f77 2061  .        # now a
+00004810: 6c6c 2061 7474 7269 6275 7465 7320 6f66  ll attributes of
+00004820: 2074 6865 2064 6174 6173 6574 3a0d 0a20   the dataset:.. 
+00004830: 2020 2020 2020 2023 206f 7065 6e20 6174         # open at
+00004840: 7472 6962 7574 6520 7365 6374 696f 6e3a  tribute section:
+00004850: 0d0a 2020 2020 2020 2020 5f68 746d 6c5f  ..        _html_
+00004860: 6473 5f61 7474 7273 203d 2022 2222 5c6e  ds_attrs = """\n
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 3c75 6c20 636c 6173 733d 2268 3574 622d  <ul class="h5tb-
+00004890: 6174 7472 2d6c 6973 7422 3e22 2222 0d0a  attr-list">"""..
+000048a0: 0d0a 2020 2020 2020 2020 666f 7220 6b20  ..        for k 
+000048b0: 696e 2068 356f 626a 2e61 7474 7273 2e6b  in h5obj.attrs.k
+000048c0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+000048d0: 2020 2020 6966 206b 206e 6f74 2069 6e20      if k not in 
+000048e0: 7365 6c66 2e69 676e 6f72 655f 6174 7472  self.ignore_attr
+000048f0: 7320 616e 6420 6e6f 7420 6b2e 6973 7570  s and not k.isup
+00004900: 7065 7228 293a 0d0a 2020 2020 2020 2020  per():..        
+00004910: 2020 2020 2020 2020 5f68 746d 6c5f 6473          _html_ds
+00004920: 5f61 7474 7273 202b 3d20 7365 6c66 2e5f  _attrs += self._
+00004930: 5f61 7474 7273 5f5f 286b 2c20 6835 6f62  _attrs__(k, h5ob
+00004940: 6a29 0d0a 0d0a 2020 2020 2020 2020 2320  j)....        # 
+00004950: 636c 6f73 6520 6174 7472 6962 7574 6520  close attribute 
+00004960: 7365 6374 696f 6e0d 0a20 2020 2020 2020  section..       
+00004970: 205f 6874 6d6c 5f64 735f 6174 7472 7320   _html_ds_attrs 
+00004980: 2b3d 2022 2222 5c6e 2020 2020 2020 2020  += """\n        
+00004990: 2020 2020 2020 2020 3c2f 756c 3e22 2222          </ul>"""
+000049a0: 0d0a 0d0a 2020 2020 2020 2020 2320 636c  ....        # cl
+000049b0: 6f73 6520 6461 7461 7365 7420 7365 6374  ose dataset sect
+000049c0: 696f 6e0d 0a20 2020 2020 2020 205f 6874  ion..        _ht
+000049d0: 6d6c 5f70 6f73 7420 3d20 2222 225c 6e20  ml_post = """\n 
+000049e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000049f0: 2f75 6c3e 2222 220d 0a20 2020 2020 2020  /ul>"""..       
+00004a00: 205f 6874 6d6c 5f64 7320 3d20 5f68 746d   _html_ds = _htm
+00004a10: 6c5f 7072 6520 2b20 5f68 746d 6c5f 6473  l_pre + _html_ds
+00004a20: 5f61 7474 7273 202b 205f 6874 6d6c 5f70  _attrs + _html_p
+00004a30: 6f73 740d 0a20 2020 2020 2020 2072 6574  ost..        ret
+00004a40: 7572 6e20 5f68 746d 6c5f 6473 0d0a 0d0a  urn _html_ds....
+00004a50: 2020 2020 6465 6620 5f5f 6772 6f75 705f      def __group_
+00004a60: 5f28 7365 6c66 2c20 6e61 6d65 2c20 6835  _(self, name, h5
+00004a70: 6f62 6a3a 2022 6835 7462 782e 4772 6f75  obj: "h5tbx.Grou
+00004a80: 7022 2920 2d3e 2073 7472 3a0d 0a20 2020  p") -> str:..   
+00004a90: 2020 2020 206e 6b65 7973 203d 206c 656e       nkeys = len
+00004aa0: 2868 356f 626a 2e6b 6579 7328 2929 0d0a  (h5obj.keys())..
+00004ab0: 2020 2020 2020 2020 5f69 6420 3d20 6627          _id = f'
+00004ac0: 6473 2d7b 6e61 6d65 7d2d 7b70 6572 665f  ds-{name}-{perf_
+00004ad0: 636f 756e 7465 725f 6e73 2829 2e5f 5f73  counter_ns().__s
+00004ae0: 7472 5f5f 2829 7d27 0d0a 2020 2020 2020  tr__()}'..      
+00004af0: 2020 5f67 726f 7570 6e61 6d65 203d 206f    _groupname = o
+00004b00: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+00004b10: 6835 6f62 6a2e 6e61 6d65 290d 0a0d 0a20  h5obj.name).... 
+00004b20: 2020 2020 2020 2069 6620 5f67 726f 7570         if _group
+00004b30: 6e61 6d65 203d 3d20 2727 3a0d 0a20 2020  name == '':..   
+00004b40: 2020 2020 2020 2020 205f 6772 6f75 706e           _groupn
+00004b50: 616d 6520 3d20 272f 2720 2023 2072 6563  ame = '/'  # rec
+00004b60: 6f76 6572 2072 6f6f 7420 6e61 6d65 0d0a  over root name..
+00004b70: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+00004b80: 6b62 6f78 5f73 7461 7465 203d 2027 6368  kbox_state = 'ch
+00004b90: 6563 6b65 6427 0d0a 2020 2020 2020 2020  ecked'..        
+00004ba0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00004bb0: 2020 2063 6865 636b 626f 785f 7374 6174     checkbox_stat
+00004bc0: 6520 3d20 7365 6c66 2e63 6865 636b 626f  e = self.checkbo
+00004bd0: 785f 7374 6174 650d 0a0d 0a20 2020 2020  x_state....     
+00004be0: 2020 2073 656c 665f 7072 6564 6963 6174     self_predicat
+00004bf0: 6520 3d20 6835 6f62 6a2e 7264 662e 7072  e = h5obj.rdf.pr
+00004c00: 6564 6963 6174 652e 6765 7428 2753 454c  edicate.get('SEL
+00004c10: 4627 2c20 4e6f 6e65 290d 0a20 2020 2020  F', None)..     
+00004c20: 2020 2073 656c 665f 7479 7065 203d 2068     self_type = h
+00004c30: 356f 626a 2e72 6466 2e74 7970 650d 0a20  5obj.rdf.type.. 
+00004c40: 2020 2020 2020 2073 656c 665f 4944 203d         self_ID =
+00004c50: 2068 356f 626a 2e72 6466 2e73 7562 6a65   h5obj.rdf.subje
+00004c60: 6374 0d0a 0d0a 2020 2020 2020 2020 6966  ct....        if
+00004c70: 2073 656c 665f 7479 7065 2069 7320 6e6f   self_type is no
+00004c80: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00004c90: 2020 2020 205f 6772 6f75 706e 616d 6520       _groupname 
+00004ca0: 2b3d 2067 6574 5f69 7269 5f69 636f 6e5f  += get_iri_icon_
+00004cb0: 6872 6566 2873 656c 665f 7479 7065 2c20  href(self_type, 
+00004cc0: 6963 6f6e 5f75 726c 3d54 5950 455f 4943  icon_url=TYPE_IC
+00004cd0: 4f4e 2c0d 0a20 2020 2020 2020 2020 2020  ON,..           
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2074 6f6f 6c74 6970 7465 7874 3d66 2740   tooltiptext=f'@
+00004d10: 7479 7065 3a20 7b73 656c 665f 7479 7065  type: {self_type
+00004d20: 7d27 290d 0a0d 0a20 2020 2020 2020 2069  }')....        i
+00004d30: 6620 7365 6c66 5f49 4420 6973 206e 6f74  f self_ID is not
+00004d40: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00004d50: 2020 2020 5f67 726f 7570 6e61 6d65 202b      _groupname +
+00004d60: 3d20 6765 745f 6972 695f 6963 6f6e 5f68  = get_iri_icon_h
+00004d70: 7265 6628 7365 6c66 5f49 442c 2069 636f  ref(self_ID, ico
+00004d80: 6e5f 7572 6c3d 4944 5f49 434f 4e2c 0d0a  n_url=ID_ICON,..
+00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004db0: 2020 2020 2020 2020 2020 2020 746f 6f6c              tool
+00004dc0: 7469 7074 6578 743d 6627 4069 643a 207b  tiptext=f'@id: {
+00004dd0: 7365 6c66 5f49 447d 2729 0d0a 0d0a 2020  self_ID}')....  
+00004de0: 2020 2020 2020 6966 2073 656c 665f 7072        if self_pr
+00004df0: 6564 6963 6174 6520 6973 206e 6f74 204e  edicate is not N
+00004e00: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00004e10: 2020 5f67 726f 7570 6e61 6d65 202b 3d20    _groupname += 
+00004e20: 6765 745f 6972 695f 6963 6f6e 5f68 7265  get_iri_icon_hre
+00004e30: 6628 7365 6c66 5f70 7265 6469 6361 7465  f(self_predicate
+00004e40: 2c20 6963 6f6e 5f75 726c 3d49 5249 5f49  , icon_url=IRI_I
+00004e50: 434f 4e29 0d0a 0d0a 2020 2020 2020 2020  CON)....        
+00004e60: 5f68 746d 6c20 3d20 6622 2222 5c6e 0d0a  _html = f"""\n..
+00004e70: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
+00004e80: 6c20 7374 796c 653d 226c 6973 742d 7374  l style="list-st
+00004e90: 796c 652d 7479 7065 3a20 6e6f 6e65 3b22  yle-type: none;"
+00004ea0: 2063 6c61 7373 3d22 6835 6772 702d 7365   class="h5grp-se
+00004eb0: 6374 696f 6e73 223e 0d0a 2020 2020 2020  ctions">..      
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+00004ed0: 693e 0d0a 2020 2020 2020 2020 2020 2020  i>..            
+00004ee0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+00004ef0: 7574 2069 643d 2267 726f 7570 2d7b 5f69  ut id="group-{_i
+00004f00: 647d 2220 7479 7065 3d22 6368 6563 6b62  d}" type="checkb
+00004f10: 6f78 2220 7b63 6865 636b 626f 785f 7374  ox" {checkbox_st
+00004f20: 6174 657d 3e0d 0a20 2020 2020 2020 2020  ate}>..         
+00004f30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004f40: 6c61 6265 6c20 7374 796c 653d 2266 6f6e  label style="fon
+00004f50: 742d 7765 6967 6874 3a20 626f 6c64 2220  t-weight: bold" 
+00004f60: 666f 723d 2267 726f 7570 2d7b 5f69 647d  for="group-{_id}
+00004f70: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+00004f80: 2020 2020 2020 2020 2020 2020 7b5f 6772              {_gr
+00004f90: 6f75 706e 616d 657d 3c73 7061 6e3e 287b  oupname}<span>({
+00004fa0: 6e6b 6579 737d 293c 2f73 7061 6e3e 3c2f  nkeys})</span></
+00004fb0: 6c61 6265 6c3e 0d0a 2020 2020 2020 2020  label>..        
+00004fc0: 2020 2020 2020 2020 2020 2222 220d 0a0d            """...
+00004fd0: 0a20 2020 2020 2020 205f 6874 6d6c 202b  .        _html +
+00004fe0: 3d20 2222 225c 6e3c 756c 2063 6c61 7373  = """\n<ul class
+00004ff0: 3d22 6835 7462 2d61 7474 722d 6c69 7374  ="h5tb-attr-list
+00005000: 223e 2222 220d 0a20 2020 2020 2020 2023  ">"""..        #
+00005010: 2077 7269 7465 2061 7474 7269 6275 7465   write attribute
+00005020: 733a 0d0a 2020 2020 2020 2020 666f 7220  s:..        for 
+00005030: 6b20 696e 2068 356f 626a 2e61 7474 7273  k in h5obj.attrs
+00005040: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00005050: 2020 2020 2020 6966 206e 6f74 206b 2e69        if not k.i
+00005060: 7375 7070 6572 2829 3a0d 0a20 2020 2020  supper():..     
+00005070: 2020 2020 2020 2020 2020 205f 6874 6d6c             _html
+00005080: 202b 3d20 7365 6c66 2e5f 5f61 7474 7273   += self.__attrs
+00005090: 5f5f 286b 2c20 6835 6f62 6a29 0d0a 2020  __(k, h5obj)..  
+000050a0: 2020 2020 2020 2320 636c 6f73 6520 6174        # close at
+000050b0: 7472 6962 7574 6520 7365 6374 696f 6e0d  tribute section.
+000050c0: 0a20 2020 2020 2020 205f 6874 6d6c 202b  .        _html +
+000050d0: 3d20 2222 220d 0a20 2020 2020 2020 2020  = """..         
+000050e0: 2020 2020 2020 2020 2020 203c 2f75 6c3e             </ul>
+000050f0: 2222 220d 0a0d 0a20 2020 2020 2020 2064  """....        d
+00005100: 6174 6173 6574 7320 3d20 5b28 6b2c 2076  atasets = [(k, v
+00005110: 2920 666f 7220 6b2c 2076 2069 6e20 6835  ) for k, v in h5
+00005120: 6f62 6a2e 6974 656d 7328 2920 6966 2069  obj.items() if i
+00005130: 7369 6e73 7461 6e63 6528 762c 2068 3570  sinstance(v, h5p
+00005140: 792e 4461 7461 7365 7429 5d0d 0a20 2020  y.Dataset)]..   
+00005150: 2020 2020 2067 726f 7570 7320 3d20 5b28       groups = [(
+00005160: 6b2c 2076 2920 666f 7220 6b2c 2076 2069  k, v) for k, v i
+00005170: 6e20 6835 6f62 6a2e 6974 656d 7328 2920  n h5obj.items() 
+00005180: 6966 2069 7369 6e73 7461 6e63 6528 762c  if isinstance(v,
+00005190: 2068 3570 792e 4772 6f75 7029 5d0d 0a0d   h5py.Group)]...
+000051a0: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
+000051b0: 7620 696e 2064 6174 6173 6574 733a 0d0a  v in datasets:..
+000051c0: 2020 2020 2020 2020 2020 2020 5f68 746d              _htm
+000051d0: 6c20 2b3d 2073 656c 662e 5f5f 6461 7461  l += self.__data
+000051e0: 7365 745f 5f28 6b2c 2076 290d 0a0d 0a20  set__(k, v).... 
+000051f0: 2020 2020 2020 2066 6f72 206b 2c20 7620         for k, v 
+00005200: 696e 2067 726f 7570 733a 0d0a 2020 2020  in groups:..    
+00005210: 2020 2020 2020 2020 5f68 746d 6c20 2b3d          _html +=
+00005220: 2073 656c 662e 5f5f 6772 6f75 705f 5f28   self.__group__(
+00005230: 6b2c 2076 290d 0a20 2020 2020 2020 205f  k, v)..        _
+00005240: 6874 6d6c 202b 3d20 275c 6e3c 2f6c 693e  html += '\n</li>
+00005250: 270d 0a20 2020 2020 2020 205f 6874 6d6c  '..        _html
+00005260: 202b 3d20 275c 6e3c 2f75 6c3e 270d 0a20   += '\n</ul>'.. 
+00005270: 2020 2020 2020 2072 6574 7572 6e20 5f68         return _h
+00005280: 746d 6c0d 0a0d 0a20 2020 2064 6566 205f  tml....    def _
+00005290: 5f61 7474 7273 5f5f 2873 656c 662c 206e  _attrs__(self, n
+000052a0: 616d 652c 2068 356f 626a 293a 0d0a 2020  ame, h5obj):..  
+000052b0: 2020 2020 2020 6174 7472 5f76 616c 7565        attr_value
+000052c0: 203d 2068 356f 626a 2e61 7474 7273 2e72   = h5obj.attrs.r
+000052d0: 6177 5b6e 616d 655d 0d0a 0d0a 2020 2020  aw[name]....    
+000052e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000052f0: 6528 6174 7472 5f76 616c 7565 2c20 6e70  e(attr_value, np
+00005300: 2e62 7974 6573 5f29 3a0d 0a20 2020 2020  .bytes_):..     
+00005310: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00005320: 2020 2020 2020 2020 2020 2020 2061 7474               att
+00005330: 725f 7661 6c75 6520 3d20 6174 7472 5f76  r_value = attr_v
+00005340: 616c 7565 2e64 6563 6f64 6528 2775 7466  alue.decode('utf
+00005350: 2d38 2729 0d0a 2020 2020 2020 2020 2020  -8')..          
+00005360: 2020 6578 6365 7074 2055 6e69 636f 6465    except Unicode
+00005370: 4465 636f 6465 4572 726f 723a 0d0a 2020  DecodeError:..  
+00005380: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+00005390: 726e 696e 6773 2e77 6172 6e28 6627 4361  rnings.warn(f'Ca
+000053a0: 6e6e 6f74 2064 6563 6f64 6520 6174 7472  nnot decode attr
+000053b0: 6962 7574 6520 7661 6c75 6520 666f 7220  ibute value for 
+000053c0: 7b6e 616d 657d 272c 2052 756e 7469 6d65  {name}', Runtime
+000053d0: 5761 726e 696e 6729 0d0a 2020 2020 2020  Warning)..      
+000053e0: 2020 7264 6620 3d20 6835 6f62 6a2e 7264    rdf = h5obj.rd
+000053f0: 662e 6765 7428 6e61 6d65 290d 0a0d 0a20  f.get(name).... 
+00005400: 2020 2020 2020 2064 6973 705f 6e61 6d65         disp_name
+00005410: 203d 206e 616d 650d 0a0d 0a20 2020 2020   = name....     
+00005420: 2020 2072 6466 5f70 7265 6469 6361 7465     rdf_predicate
+00005430: 203d 2072 6466 2e70 7265 6469 6361 7465   = rdf.predicate
+00005440: 0d0a 2020 2020 2020 2020 6966 2072 6466  ..        if rdf
+00005450: 5f70 7265 6469 6361 7465 2069 7320 6e6f  _predicate is no
+00005460: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00005470: 2020 2020 2064 6973 705f 6e61 6d65 202b       disp_name +
+00005480: 3d20 6765 745f 6972 695f 6963 6f6e 5f68  = get_iri_icon_h
+00005490: 7265 6628 7264 665f 7072 6564 6963 6174  ref(rdf_predicat
+000054a0: 652c 2069 636f 6e5f 7572 6c3d 4952 495f  e, icon_url=IRI_
+000054b0: 4943 4f4e 290d 0a0d 0a20 2020 2020 2020  ICON)....       
+000054c0: 2061 7474 7273 5f64 6566 203d 2068 356f   attrs_def = h5o
+000054d0: 626a 2e72 6466 5b6e 616d 655d 2e64 6566  bj.rdf[name].def
+000054e0: 696e 6974 696f 6e0d 0a20 2020 2020 2020  inition..       
+000054f0: 2069 6620 6174 7472 735f 6465 6620 6973   if attrs_def is
+00005500: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00005510: 2020 2020 2020 2020 6469 7370 5f6e 616d          disp_nam
+00005520: 6520 2b3d 2067 6574 5f64 6566 5f69 636f  e += get_def_ico
+00005530: 6e5f 6872 6566 2861 7474 7273 5f64 6566  n_href(attrs_def
+00005540: 290d 0a0d 0a20 2020 2020 2020 2072 6466  )....        rdf
+00005550: 5f6f 626a 6563 7420 3d20 7264 662e 6f62  _object = rdf.ob
+00005560: 6a65 6374 0d0a 0d0a 2020 2020 2020 2020  ject....        
+00005570: 6966 2069 7369 6e73 7461 6e63 6528 6174  if isinstance(at
+00005580: 7472 5f76 616c 7565 2c20 6e64 6172 7261  tr_value, ndarra
+00005590: 7929 3a0d 0a0d 0a20 2020 2020 2020 2020  y):....         
+000055a0: 2020 2069 6620 616c 6c28 6973 696e 7374     if all(isinst
+000055b0: 616e 6365 2869 7465 6d2c 2073 7472 2920  ance(item, str) 
+000055c0: 666f 7220 6974 656d 2069 6e20 6174 7472  for item in attr
+000055d0: 5f76 616c 7565 293a 0d0a 2020 2020 2020  _value):..      
+000055e0: 2020 2020 2020 2020 2020 5f73 7472 696e            _strin
+000055f0: 675f 7661 6c75 655f 6c69 7374 203d 205b  g_value_list = [
+00005600: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00005610: 2020 2066 6f72 2069 7465 6d20 696e 2061     for item in a
+00005620: 7474 725f 7661 6c75 653a 0d0a 2020 2020  ttr_value:..    
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 5f76 616c 7565 2c20 6973 5f75 726c 203d  _value, is_url =
+00005650: 2070 726f 6365 7373 5f73 7472 696e 675f   process_string_
+00005660: 666f 725f 6c69 6e6b 2869 7465 6d29 0d0a  for_link(item)..
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 2020 2020 6966 2069 735f 7572 6c3a 0d0a      if is_url:..
+00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056a0: 2020 2020 2020 2020 5f73 7472 696e 675f          _string_
+000056b0: 7661 6c75 655f 6c69 7374 2e61 7070 656e  value_list.appen
+000056c0: 6428 5f76 616c 7565 290d 0a20 2020 2020  d(_value)..     
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000056e0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000056f0: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
+00005700: 7472 696e 675f 7661 6c75 655f 6c69 7374  tring_value_list
+00005710: 2e61 7070 656e 6428 6974 656d 290d 0a20  .append(item).. 
+00005720: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00005730: 7661 6c75 655f 7374 7220 3d20 222c 2022  value_str = ", "
+00005740: 2e6a 6f69 6e28 5f73 7472 696e 675f 7661  .join(_string_va
+00005750: 6c75 655f 6c69 7374 290d 0a0d 0a20 2020  lue_list)....   
+00005760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005770: 7264 665f 6f62 6a65 6374 2069 7320 6e6f  rdf_object is no
+00005780: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00005790: 2020 2020 2020 2020 2020 2020 205f 7661               _va
+000057a0: 6c75 655f 7374 7220 2b3d 2067 6574 5f69  lue_str += get_i
+000057b0: 7269 5f69 636f 6e5f 6872 6566 2872 6466  ri_icon_href(rdf
+000057c0: 5f6f 626a 6563 742c 2069 636f 6e5f 7572  _object, icon_ur
+000057d0: 6c3d 4952 495f 4943 4f4e 290d 0a20 2020  l=IRI_ICON)..   
+000057e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000057f0: 7572 6e20 273c 6c69 2073 7479 6c65 3d22  urn '<li style="
+00005800: 6c69 7374 2d73 7479 6c65 2d74 7970 653a  list-style-type:
+00005810: 206e 6f6e 653b 2027 205c 0d0a 2020 2020   none; ' \..    
+00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005830: 2020 2066 2766 6f6e 742d 7374 796c 653a     f'font-style:
+00005840: 2069 7461 6c69 6322 3e7b 6469 7370 5f6e   italic">{disp_n
+00005850: 616d 657d 3a20 7b5f 7661 6c75 655f 7374  ame}: {_value_st
+00005860: 727d 3c2f 6c69 3e27 0d0a 2020 2020 2020  r}</li>'..      
+00005870: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00005880: 2020 2020 2020 2020 2020 2020 205f 7661               _va
+00005890: 6c75 6520 3d20 6174 7472 5f76 616c 7565  lue = attr_value
+000058a0: 2e5f 5f72 6570 725f 5f28 290d 0a0d 0a20  .__repr__().... 
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000058c0: 6620 6c65 6e28 5f76 616c 7565 2920 3e20  f len(_value) > 
+000058d0: 7365 6c66 2e6d 6178 5f61 7474 725f 6c65  self.max_attr_le
+000058e0: 6e67 7468 3a0d 0a20 2020 2020 2020 2020  ngth:..         
+000058f0: 2020 2020 2020 2020 2020 205f 7661 6c75             _valu
+00005900: 6520 3d20 6627 7b5f 7661 6c75 655b 303a  e = f'{_value[0:
+00005910: 7365 6c66 2e6d 6178 5f61 7474 725f 6c65  self.max_attr_le
+00005920: 6e67 7468 5d7d 2e2e 2e27 0d0a 0d0a 2020  ngth]}...'....  
+00005930: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005940: 2072 6466 5f6f 626a 6563 7420 6973 206e   rdf_object is n
+00005950: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00005960: 2020 2020 2020 2020 2020 2020 2020 5f76                _v
+00005970: 616c 7565 202b 3d20 6765 745f 6972 695f  alue += get_iri_
+00005980: 6963 6f6e 5f68 7265 6628 7264 665f 7072  icon_href(rdf_pr
+00005990: 6564 6963 6174 652c 2069 636f 6e5f 7572  edicate, icon_ur
+000059a0: 6c3d 4952 495f 4943 4f4e 290d 0a0d 0a20  l=IRI_ICON).... 
+000059b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000059c0: 6574 7572 6e20 6627 3c6c 6920 7374 796c  eturn f'<li styl
+000059d0: 653d 226c 6973 742d 7374 796c 652d 7479  e="list-style-ty
+000059e0: 7065 3a20 6e6f 6e65 3b20 666f 6e74 2d73  pe: none; font-s
+000059f0: 7479 6c65 3a20 6974 616c 6963 223e 7b64  tyle: italic">{d
+00005a00: 6973 705f 6e61 6d65 7d3a 207b 5f76 616c  isp_name}: {_val
+00005a10: 7565 7d3c 2f6c 693e 270d 0a0d 0a20 2020  ue}</li>'....   
+00005a20: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00005a30: 6365 2861 7474 725f 7661 6c75 652c 2073  ce(attr_value, s
+00005a40: 7472 293a 0d0a 2020 2020 2020 2020 2020  tr):..          
+00005a50: 2020 5f76 616c 7565 5f73 7472 203d 2066    _value_str = f
+00005a60: 277b 6174 7472 5f76 616c 7565 7d27 0d0a  '{attr_value}'..
+00005a70: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00005a80: 656e 285f 7661 6c75 655f 7374 7229 203e  en(_value_str) >
+00005a90: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00005aa0: 2020 2020 2069 6620 5f76 616c 7565 5f73       if _value_s
+00005ab0: 7472 5b30 5d20 3d3d 2027 3c27 2061 6e64  tr[0] == '<' and
+00005ac0: 205f 7661 6c75 655f 7374 725b 2d31 5d20   _value_str[-1] 
+00005ad0: 3d3d 2027 3e27 3a0d 0a20 2020 2020 2020  == '>':..       
+00005ae0: 2020 2020 2020 2020 2020 2020 205f 7661               _va
+00005af0: 6c75 655f 7374 7220 3d20 5f76 616c 7565  lue_str = _value
+00005b00: 5f73 7472 5b31 3a2d 315d 0d0a 0d0a 2020  _str[1:-1]....  
+00005b10: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
+00005b20: 6b20 6966 2069 7420 6973 2061 2069 6465  k if it is a ide
+00005b30: 6e74 6966 6965 723a 0d0a 2020 2020 2020  ntifier:..      
+00005b40: 2020 2020 2020 6964 656e 7469 6669 6572        identifier
+00005b50: 203d 2069 6465 6e74 6966 6965 7273 2e66   = identifiers.f
+00005b60: 726f 6d5f 7572 6c28 5f76 616c 7565 5f73  rom_url(_value_s
+00005b70: 7472 290d 0a20 2020 2020 2020 2020 2020  tr)..           
+00005b80: 2069 6620 6964 656e 7469 6669 6572 2069   if identifier i
+00005b90: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00005ba0: 2020 2020 2020 2020 2020 2020 205f 7661               _va
+00005bb0: 6c75 655f 6874 6d6c 203d 2069 6465 6e74  lue_html = ident
+00005bc0: 6966 6965 722e 5f72 6570 725f 6874 6d6c  ifier._repr_html
+00005bd0: 5f28 290d 0a20 2020 2020 2020 2020 2020  _()..           
+00005be0: 2020 2020 2069 735f 7572 6c20 3d20 5472       is_url = Tr
+00005bf0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00005c00: 656c 7365 3a20 2023 206d 6179 6265 2073  else:  # maybe s
+00005c10: 6f6d 6520 6f74 6865 7220 7572 6c3a 0d0a  ome other url:..
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 5f76 616c 7565 5f68 746d 6c2c 2069 735f  _value_html, is_
+00005c40: 7572 6c20 3d20 7072 6f63 6573 735f 7374  url = process_st
+00005c50: 7269 6e67 5f66 6f72 5f6c 696e 6b28 5f76  ring_for_link(_v
+00005c60: 616c 7565 5f73 7472 290d 0a20 2020 2020  alue_str)..     
+00005c70: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+00005c80: 6973 5f75 726c 2061 6e64 206e 6f74 205f  is_url and not _
+00005c90: 7661 6c75 655f 6874 6d6c 2e73 7461 7274  value_html.start
+00005ca0: 7377 6974 6828 277b 2729 3a0d 0a0d 0a20  swith('{'):.... 
+00005cb0: 2020 2020 2020 2020 2020 2023 2061 6464             # add
+00005cc0: 2072 6466 2069 636f 6e20 6966 2061 7661   rdf icon if ava
+00005cd0: 696c 6162 6c65 3a0d 0a20 2020 2020 2020  ilable:..       
+00005ce0: 2020 2020 2069 6620 7264 665f 6f62 6a65       if rdf_obje
+00005cf0: 6374 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ct is not None:.
+00005d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d10: 205f 7661 6c75 655f 6874 6d6c 202b 3d20   _value_html += 
+00005d20: 6765 745f 6972 695f 6963 6f6e 5f68 7265  get_iri_icon_hre
+00005d30: 6628 7264 665f 6f62 6a65 6374 2c20 6963  f(rdf_object, ic
+00005d40: 6f6e 5f75 726c 3d49 5249 5f49 434f 4e29  on_url=IRI_ICON)
+00005d50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00005d60: 6966 2069 735f 7572 6c20 616e 6420 6e6f  if is_url and no
+00005d70: 7420 5f76 616c 7565 5f68 746d 6c2e 7374  t _value_html.st
+00005d80: 6172 7473 7769 7468 2827 7b27 293a 2020  artswith('{'):  
+00005d90: 2320 544f 444f 3a20 7768 7920 7468 6520  # TODO: why the 
+00005da0: 7365 636f 6e64 2063 6f6e 6469 7469 6f6e  second condition
+00005db0: 3f0d 0a20 2020 2020 2020 2020 2020 2020  ?..             
+00005dc0: 2020 2072 6574 7572 6e20 6627 3c6c 6920     return f'<li 
+00005dd0: 7374 796c 653d 226c 6973 742d 7374 796c  style="list-styl
+00005de0: 652d 7479 7065 3a20 6e6f 6e65 3b20 666f  e-type: none; fo
+00005df0: 6e74 2d73 7479 6c65 3a20 6974 616c 6963  nt-style: italic
+00005e00: 223e 7b64 6973 705f 6e61 6d65 7d3a 207b  ">{disp_name}: {
+00005e10: 5f76 616c 7565 5f68 746d 6c7d 3c2f 6c69  _value_html}</li
+00005e20: 3e27 0d0a 2020 2020 2020 2020 2020 2020  >'..            
+00005e30: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005e40: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00005e50: 6178 5f61 7474 725f 6c65 6e67 7468 3a0d  ax_attr_length:.
+00005e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005e70: 2020 2020 2069 6620 6c65 6e28 5f76 616c       if len(_val
+00005e80: 7565 5f73 7472 2920 3e20 7365 6c66 2e6d  ue_str) > self.m
+00005e90: 6178 5f61 7474 725f 6c65 6e67 7468 3a0d  ax_attr_length:.
+00005ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005eb0: 2020 2020 2020 2020 205f 7661 6c75 655f           _value_
+00005ec0: 7374 7220 3d20 6627 7b5f 7661 6c75 655f  str = f'{_value_
+00005ed0: 7374 725b 303a 7365 6c66 2e6d 6178 5f61  str[0:self.max_a
+00005ee0: 7474 725f 6c65 6e67 7468 202d 2033 5d7d  ttr_length - 3]}
+00005ef0: 2e2e 2e27 0d0a 2020 2020 2020 2020 2020  ...'..          
+00005f00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00005f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f20: 2020 2020 2020 2020 205f 7661 6c75 655f           _value_
+00005f30: 7374 7220 3d20 6174 7472 5f76 616c 7565  str = attr_value
+00005f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005f50: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00005f60: 2020 2020 2020 2020 2020 2020 205f 7661               _va
+00005f70: 6c75 655f 7374 7220 3d20 6174 7472 5f76  lue_str = attr_v
+00005f80: 616c 7565 0d0a 2020 2020 2020 2020 2020  alue..          
+00005f90: 2020 6966 2072 6466 5f6f 626a 6563 7420    if rdf_object 
+00005fa0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00005fb0: 2020 2020 2020 2020 2020 2020 2020 5f76                _v
+00005fc0: 616c 7565 5f73 7472 202b 3d20 6765 745f  alue_str += get_
+00005fd0: 6972 695f 6963 6f6e 5f68 7265 6628 7264  iri_icon_href(rd
+00005fe0: 665f 6f62 6a65 6374 2c20 6963 6f6e 5f75  f_object, icon_u
+00005ff0: 726c 3d49 5249 5f49 434f 4e29 0d0a 2020  rl=IRI_ICON)..  
+00006000: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006010: 2066 273c 6c69 2073 7479 6c65 3d22 6c69   f'<li style="li
+00006020: 7374 2d73 7479 6c65 2d74 7970 653a 206e  st-style-type: n
+00006030: 6f6e 653b 2066 6f6e 742d 7374 796c 653a  one; font-style:
+00006040: 2069 7461 6c69 6322 3e7b 6469 7370 5f6e   italic">{disp_n
+00006050: 616d 657d 3a20 7b5f 7661 6c75 655f 7374  ame}: {_value_st
+00006060: 727d 3c2f 6c69 3e27 0d0a 0d0a 2020 2020  r}</li>'....    
+00006070: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00006080: 7461 6e63 6528 6174 7472 5f76 616c 7565  tance(attr_value
+00006090: 2c20 6e64 6172 7261 7929 3a0d 0a20 2020  , ndarray):..   
+000060a0: 2020 2020 2020 2020 2069 6620 6765 7461           if geta
+000060b0: 7474 7228 6174 7472 5f76 616c 7565 2c20  ttr(attr_value, 
+000060c0: 275f 7265 7072 5f68 746d 6c5f 272c 204e  '_repr_html_', N
+000060d0: 6f6e 6529 3a0d 0a20 2020 2020 2020 2020  one):..         
+000060e0: 2020 2020 2020 205f 7661 6c75 655f 7374         _value_st
+000060f0: 7220 3d20 6174 7472 5f76 616c 7565 2e5f  r = attr_value._
+00006100: 7265 7072 5f68 746d 6c5f 2829 0d0a 2020  repr_html_()..  
+00006110: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00006120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006130: 205f 7661 6c75 655f 7374 7220 3d20 7374   _value_str = st
+00006140: 7228 6174 7472 5f76 616c 7565 290d 0a20  r(attr_value).. 
+00006150: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006160: 6620 5f76 616c 7565 5f73 7472 5b30 5d20  f _value_str[0] 
+00006170: 3d3d 2027 3c27 2061 6e64 205f 7661 6c75  == '<' and _valu
+00006180: 655f 7374 725b 2d31 5d20 3d3d 2027 3e27  e_str[-1] == '>'
+00006190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000061a0: 2020 2020 2020 205f 7661 6c75 655f 7374         _value_st
+000061b0: 7220 3d20 5f76 616c 7565 5f73 7472 5b31  r = _value_str[1
+000061c0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
+000061d0: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
+000061e0: 785f 6174 7472 5f6c 656e 6774 683a 0d0a  x_attr_length:..
+000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006200: 2020 2020 6966 206c 656e 285f 7661 6c75      if len(_valu
+00006210: 655f 7374 7229 203e 2073 656c 662e 6d61  e_str) > self.ma
+00006220: 785f 6174 7472 5f6c 656e 6774 683a 0d0a  x_attr_length:..
+00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006240: 2020 2020 2020 2020 5f76 616c 7565 5f73          _value_s
+00006250: 7472 203d 2066 277b 5f76 616c 7565 5f73  tr = f'{_value_s
+00006260: 7472 5b30 3a73 656c 662e 6d61 785f 6174  tr[0:self.max_at
+00006270: 7472 5f6c 656e 6774 6820 2d20 335d 7d2e  tr_length - 3]}.
+00006280: 2e2e 270d 0a20 2020 2020 2020 2020 2020  ..'..           
+00006290: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062b0: 2020 2020 2020 2020 5f76 616c 7565 5f73          _value_s
+000062c0: 7472 203d 2061 7474 725f 7661 6c75 650d  tr = attr_value.
+000062d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000062e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000062f0: 2020 2020 2020 2020 2020 2020 5f76 616c              _val
+00006300: 7565 5f73 7472 203d 2061 7474 725f 7661  ue_str = attr_va
+00006310: 6c75 650d 0a0d 0a20 2020 2020 2020 2069  lue....        i
+00006320: 6620 7264 665f 6f62 6a65 6374 2069 7320  f rdf_object is 
+00006330: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00006340: 2020 2020 2020 205f 7661 6c75 655f 7374         _value_st
+00006350: 7220 2b3d 2067 6574 5f69 7269 5f69 636f  r += get_iri_ico
+00006360: 6e5f 6872 6566 2872 6466 5f6f 626a 6563  n_href(rdf_objec
+00006370: 742c 2069 636f 6e5f 7572 6c3d 4952 495f  t, icon_url=IRI_
+00006380: 4943 4f4e 290d 0a20 2020 2020 2020 2072  ICON)..        r
+00006390: 6574 7572 6e20 6627 3c6c 6920 7374 796c  eturn f'<li styl
+000063a0: 653d 226c 6973 742d 7374 796c 652d 7479  e="list-style-ty
+000063b0: 7065 3a20 6e6f 6e65 3b20 666f 6e74 2d73  pe: none; font-s
+000063c0: 7479 6c65 3a20 6974 616c 6963 223e 7b6e  tyle: italic">{n
+000063d0: 616d 657d 3a20 7b5f 7661 6c75 655f 7374  ame}: {_value_st
+000063e0: 727d 3c2f 6c69 3e27 0d0a 0d0a 0d0a 636c  r}</li>'......cl
+000063f0: 6173 7320 4835 5265 7072 3a0d 0a20 2020  ass H5Repr:..   
+00006400: 2022 2222 436c 6173 7320 6d61 6e61 6769   """Class managi
+00006410: 6e67 2074 6865 2073 7469 6e67 2f68 746d  ng the sting/htm
+00006420: 6c20 6f75 7470 7574 206f 6620 4844 4635  l output of HDF5
+00006430: 2063 6f6e 7465 6e74 2222 220d 0a0d 0a20   content""".... 
+00006440: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00006450: 7365 6c66 2c20 7374 725f 7265 7072 3a20  self, str_repr: 
+00006460: 5f48 4446 3553 7472 7563 7475 7265 5265  _HDF5StructureRe
+00006470: 7072 203d 204e 6f6e 652c 2068 746d 6c5f  pr = None, html_
+00006480: 7265 7072 3a20 5f48 4446 3553 7472 7563  repr: _HDF5Struc
+00006490: 7475 7265 5265 7072 203d 204e 6f6e 652c  tureRepr = None,
+000064a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000064b0: 2020 202a 2a6b 7761 7267 7329 3a0d 0a20     **kwargs):.. 
+000064c0: 2020 2020 2020 2069 6620 7374 725f 7265         if str_re
+000064d0: 7072 2069 7320 4e6f 6e65 3a0d 0a20 2020  pr is None:..   
+000064e0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000064f0: 725f 7265 7072 203d 2048 4446 3553 7472  r_repr = HDF5Str
+00006500: 7563 7475 7265 5374 7252 6570 7228 2a2a  uctureStrRepr(**
+00006510: 6b77 6172 6773 290d 0a20 2020 2020 2020  kwargs)..       
+00006520: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00006530: 2020 2020 7365 6c66 2e73 7472 5f72 6570      self.str_rep
+00006540: 7220 3d20 7374 725f 7265 7072 0d0a 0d0a  r = str_repr....
+00006550: 2020 2020 2020 2020 6966 2068 746d 6c5f          if html_
+00006560: 7265 7072 2069 7320 4e6f 6e65 3a0d 0a20  repr is None:.. 
+00006570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006580: 6874 6d6c 5f72 6570 7220 3d20 4844 4635  html_repr = HDF5
+00006590: 5374 7275 6374 7572 6548 544d 4c52 6570  StructureHTMLRep
+000065a0: 7228 2a2a 6b77 6172 6773 290d 0a20 2020  r(**kwargs)..   
+000065b0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000065c0: 2020 2020 2020 2020 7365 6c66 2e68 746d          self.htm
+000065d0: 6c5f 7265 7072 203d 2068 746d 6c5f 7265  l_repr = html_re
+000065e0: 7072 0d0a 0d0a 2020 2020 6465 6620 5f5f  pr....    def __
+000065f0: 6874 6d6c 5f5f 2873 656c 662c 2067 726f  html__(self, gro
+00006600: 7570 2c20 636f 6c6c 6170 7365 643a 2062  up, collapsed: b
+00006610: 6f6f 6c20 3d20 5472 7565 2c20 7072 6561  ool = True, prea
+00006620: 6d62 6c65 3a20 7374 7220 3d20 4e6f 6e65  mble: str = None
+00006630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006640: 2020 2020 6368 756e 6b73 3a20 626f 6f6c      chunks: bool
+00006650: 203d 2046 616c 7365 2c20 6d61 7873 6861   = False, maxsha
+00006660: 7065 3a20 626f 6f6c 203d 2046 616c 7365  pe: bool = False
+00006670: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00006680: 2020 2020 6469 7370 6c61 7928 0d0a 2020      display(..  
+00006690: 2020 2020 2020 2020 2020 4854 4d4c 280d            HTML(.
+000066a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000066b0: 2073 656c 662e 6874 6d6c 5f72 6570 7228   self.html_repr(
+000066c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000066d0: 2020 2020 2020 6772 6f75 703d 6772 6f75        group=grou
+000066e0: 702c 0d0a 2020 2020 2020 2020 2020 2020  p,..            
+000066f0: 2020 2020 2020 2020 636f 6c6c 6170 7365          collapse
+00006700: 643d 636f 6c6c 6170 7365 642c 0d0a 2020  d=collapsed,..  
+00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006720: 2020 7072 6561 6d62 6c65 3d70 7265 616d    preamble=pream
+00006730: 626c 652c 0d0a 2020 2020 2020 2020 2020  ble,..          
+00006740: 2020 2020 2020 2020 2020 6368 756e 6b73            chunks
+00006750: 3d63 6875 6e6b 732c 0d0a 2020 2020 2020  =chunks,..      
+00006760: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00006770: 7873 6861 7065 3d6d 6178 7368 6170 650d  xshape=maxshape.
+00006780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006790: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000067a0: 290d 0a20 2020 2020 2020 2029 0d0a       )..        )..
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/_user.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import appdirs
 import importlib_resources
 import pathlib
 import shutil
+import time
 from itertools import count
 from typing import Tuple
 
 _filecounter = count()
 _dircounter = count()
 
 _user_root_dir = pathlib.Path(appdirs.user_data_dir('h5rdmtoolbox'))
+_now = time.time()
 
 
 class DirManger:
     """Directory Manager class"""
 
     def __init__(self):
         toolbox_tmp_folder = _user_root_dir / 'tmp'
@@ -29,16 +31,25 @@
             i += 1
             tmp_dir = toolbox_tmp_folder / f'tmp_{i}'
 
         self.user_dirs = {'root': _user_root_dir,
                           'tmp': tmp_dir,
                           'convention': _user_root_dir / 'convention',
                           'layouts': _user_root_dir / 'layouts',
+                          'repository': _user_root_dir / 'repository',
                           'standard_name_tables': _user_root_dir / 'standard_name_tables',
                           'cache': _user_root_dir / 'cache'}
+        self.clear_cache(6)
+
+    def __str__(self):
+        dirs = ', '.join(f'{k}' for k in self.user_dirs.keys())
+        return f'{self.__class__.__name__}({dirs})'
+
+    def __repr__(self):
+        return self.__str__()
 
     def __getitem__(self, item):
         return self._get_dir(item)
 
     @property
     def names(self) -> Tuple[str]:
         """Get the names of the user directories."""
@@ -81,18 +92,39 @@
 
             shutil.copy2(fluid_v1, self.user_dirs['standard_name_tables'])
             shutil.copy2(piv_v1, self.user_dirs['standard_name_tables'])
             shutil.copy2(tutorial_standard_name_table, self.user_dirs['standard_name_tables'])
 
         return self.user_dirs[name]
 
-    def clear_cache(self):
-        """Clear the cache directory."""
-        if self.user_dirs['cache'].exists():
+    def clear_cache(self, delta_days: int, utime: bool = False):
+        """Clear the cache directory. The delta_days arguments will be used
+        to delete files older than delta_days days. This is only applied to files
+
+        Parameters
+        ----------
+        delta_days : int
+            The number of days to keep the files in the cache.
+        utime : bool
+            If True, the file access time will be used to determine the age of the file.
+            Otherwise, the file creation time will be used.
+        """
+        if delta_days == 0:
             shutil.rmtree(self.user_dirs['cache'])
+            return
+        if self.user_dirs['cache'].exists():
+            for f in self.user_dirs['cache'].iterdir():
+                # get the file creation time
+                if utime:
+                    fct = f.stat().st_atime
+                else:
+                    fct = f.stat().st_ctime
+                dt = _now - fct
+                if dt > delta_days * 86400:
+                    f.unlink()
 
     def reset(self):
         """Deletes all user data"""
         shutil.rmtree(self.user_dirs['cache'])
         shutil.rmtree(self.user_dirs['convention'])
         shutil.rmtree(self.user_dirs['standard_name_tables'])
         shutil.rmtree(self.user_dirs['layouts'])
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/__init__.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,21 +7,35 @@
 A convention (class `Convention` includes a set of standard attributes, which are defined in a YAML file.
 
 Helpful functions:
  - `get_registered_conventions`
  - `get_current_convention`
 """
 
-from h5rdmtoolbox.utils import create_tbx_logger
-
-logger = create_tbx_logger('convention')
+import pathlib
 
+from . import standard_names
 from .core import Convention, from_yaml, from_repo, get_current_convention, from_zenodo, get_registered_conventions
 from .standard_attributes import StandardAttribute
-from . import standard_names
-from . import _h5tbx as __h5tbx_convention
 from .toolbox_validators import get_list_of_validators
+from .._user import UserDir
+
+__this_dir__ = pathlib.Path(__file__).parent
+
+convention_user_dir = UserDir['convention'] / 'h5tbx'
+
+
+def build_convention():
+    """Build the toolbox convention from the yaml file"""
+    from . import generate
+    h5tbx_convention_yaml = __this_dir__.parent / f'data/h5tbx.yaml'
+    convention_user_dir.mkdir(parents=True, exist_ok=True)
+    generate.write_convention_module_from_yaml(h5tbx_convention_yaml)
+
+
+if not (convention_user_dir / f'h5tbx.py').exists():
+    build_convention()
 
 __all__ = ['Convention', 'from_yaml', 'from_zenodo', 'from_repo',
            'get_current_convention', 'get_registered_conventions',
            'from_zenodo', 'StandardAttribute',
            'get_list_of_validators']
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/consts.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/consts.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/core.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 import copy
 import forge
 import h5py
 import inspect
+import logging
 import pathlib
 import re
 import shutil
 import sys
 import warnings
 import yaml
 from pydoc import locate
@@ -14,23 +15,23 @@
 
 from h5rdmtoolbox import errors
 from h5rdmtoolbox.repository import RepositoryInterface
 from h5rdmtoolbox.wrapper import ds_decoder
 from . import cfg
 from . import consts
 from . import errors
-from . import logger
 from .errors import ConventionNotFound
 from .standard_attributes import StandardAttribute, __doc_string_parser__
 from .utils import json2yaml
 from .._repr import make_italic, make_bold
 from .._user import UserDir
 from ..repository import zenodo
 from ..repository.zenodo.utils import recid_from_doi_or_redid
 
+logger = logging.getLogger('h5rdmtoolbox')
 CV_DIR = UserDir['convention']
 
 datetime_str = '%Y-%m-%dT%H:%M:%SZ%z'
 
 
 class MissingAttribute:
 
@@ -723,16 +724,16 @@
     """Download a YAML file from a zenodo repository
 
     Depreciated. Use `from_repo` in future.
 
     Parameters
     ----------
     doi_or_recid: str
-        DOI of the zenodo repository. Can be a short DOI or a full DOI or the URL (e.g. 10156750 or
-        10.5281/zenodo.10156750 or https://doi.org/10.5281/zenodo.10156750 or only the record id, e.g. 10156750)
+        DOI of the zenodo repository. Can be a short DOI or a full DOI or the URL (e.g. 10428822 or
+        10.5281/zenodo.10428822 or https://doi.org/10.5281/zenodo.10428822 or only the record id, e.g. 10428822)
     name: str=None
         Name to be sed for the filename. If None, the name is taken from the zenodo record.
     overwrite: bool = False
         Whether to overwrite existing convention with the same name. Default is False
     force_download: bool
         Whether to force download the file even if it is already cached. Default is False
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/errors.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/errors.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/generate.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Module to generate a convention Python file from a YAML file"""
 import ast
+import logging
 import pathlib
 import re
 import shutil
 import warnings
 import yaml
 from itertools import count
 from typing import Dict
 from typing import List, Union
 
 from h5rdmtoolbox._user import UserDir
 from h5rdmtoolbox.convention import toolbox_validators
-from . import logger
+
+logger = logging.getLogger('h5rdmtoolbox')
 
 regex_counter = count()
 
 INDENT = '    '
 
 
 def write_convention_module_from_yaml(yaml_filename: pathlib.Path, name=None):
@@ -204,22 +206,20 @@
             f.write('\n\n')
             auto_created_classes[_validator] = k
 
         # with open(py_filename, 'a') as f:
         f.write('\nvalidator_dict = {\n' + INDENT)
         f.write(f'\n{INDENT}'.join(f"\n'{k}': {k[1:]}," for k, v in class_definitions.items()))
         f.write(f'\n{INDENT}'.join(f"'{k}': {v}," for k, v in used_toolbox_validators.items()))
-        # f.write(f"\n{INDENT}'$int': IntValidator,  # see h5rdmtoolbox.convention.toolbox_validators")
-        # f.write(f"\n{INDENT}'$str': StringValidator,  # see h5rdmtoolbox.convention.toolbox_validators")
-        # f.write(f"\n{INDENT}'$float': FloatValidator,  # see h5rdmtoolbox.convention.toolbox_validators")
         f.write("\n}\n")
-        # f.writelines(f'standard_attributes_dict = {standard_attributes}\n')
 
         f.write('\n')
-        f.write(f'from h5rdmtoolbox.convention import Convention, standard_attributes, logger\n\n')
+        f.write('from h5rdmtoolbox.convention import Convention, standard_attributes\n')
+        f.write('import logging\n')
+        f.write('logger = logging.getLogger("h5rdmtoolbox")\n\n')
         f.write('generated_standard_attributes = {\n')
 
     with open(py_filename, 'a') as f:
         for kk, vv in standard_attributes.items():
             _default_value = _process_paths(vv.get('default_value', None), relative_to=yaml_filename.parent)
             if _default_value is None:
                 _default_value_str = 'None'
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_attributes.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """standard attribute module"""
-import enum
+import h5py
 import json
+import logging
 import pydantic
 import typing_extensions
 import warnings
 from typing import Dict, List, Union
 
-from . import errors, logger
+from . import errors
 from . import warnings as convention_warnings
 from .consts import DefaultValue
 from .. import get_config
 from ..utils import DocStringParser, parse_object_for_attribute_setting
 from ..wrapper.core import File, Group, Dataset
 
+logger = logging.getLogger('h5rdmtoolbox')
+
 __doc_string_parser__ = {File: {'__init__': DocStringParser(File)},
                          Group: {'create_group': DocStringParser(Group.create_group),
                                  'create_dataset': DocStringParser(Group.create_dataset)}}
 
 __all__ = ['StandardAttribute', ]
 
 
@@ -71,21 +74,19 @@
                  alternative_standard_attribute: str = None,
                  position: Union[None, Dict[str, str]] = None,
                  requirements: List[str] = None,
                  type_hint: str = None,
                  **kwargs):
         # name of attribute:
         self.name = name.split('-', 1)[0]  # the attrs key
-        if validator is None:
-            raise TypeError(f'validator must not be None.')
 
-        if not isinstance(validator, typing_extensions._AnnotatedAlias):
-            if not issubclass(validator, pydantic.BaseModel):
-                raise TypeError(f'validator must be a pydantic.BaseModel or a typing_extensions._AnnotatedAlias. '
-                                f'Got {type(validator)} instead.')
+        # if not isinstance(validator, typing_extensions._AnnotatedAlias):
+        #     if not issubclass(validator, pydantic.BaseModel):
+        #         raise TypeError(f'validator must be a pydantic.BaseModel or a typing_extensions._AnnotatedAlias. '
+        #                         f'Got {type(validator)} instead.')
         self.validator = validator
         # assert isinstance(self.validator, StandardAttributeValidator)
 
         # the human readable description of the attribute:
         if description[-1] != '.':
             description += '.'
         self.description = description
@@ -220,20 +221,20 @@
                             f'Expected fields: {self.validator.model_fields}\nPydantic error: {err}')
                     validated_value = getattr(_validated_value, key0)
                 return super(type(parent.attrs), parent.attrs).__setitem__(
                     self.name,
                     parse_object_for_attribute_setting(validated_value)
                 )
 
-    def get(self, parent):
+    def get(self, parent: Union[h5py.File, h5py.Group, h5py.Dataset]):
         """Read the attribute from `parent`
 
         Parameters
         ----------
-        parent: h5py.File, h5py.Group, h5py.Dataset
+        parent: Union[h5py.File, h5py.Group, h5py.Dataset]
             The parent object from which the attribute is read
 
         Returns
         -------
         any
             The value of the attribute. The validator has a get method that is called on the return
             The type of the return value is thus dependent the validator. If the get method is not
@@ -298,33 +299,33 @@
         return ret_val
 
         # return self.validate(ret_val, parent=parent)
         # try:
         #     ret_val = self.validate(ret_val, parent=parent)
         # except pydantic.ValidationError as e:
         #     errors.StandardAttributeError(f'The convention "{parent.convention.name}" detected an invalid attribute: '
-        #                                   f'Value "{ret_val}" for "{self.name}" is invalid.')
+        #                                   f'Parameter "{ret_val}" for "{self.name}" is invalid.')
         # finally:
         #     return ret_val
 
-    def to_dict(self):
-        """return a dict representation of the standard attribute"""
-
-        if self.default_value is DefaultValue.NONE:
-            default_value_str = '$optional'
-        elif self.default_value is DefaultValue.EMPTY:
-            default_value_str = '$obligatory'
-        else:
-            default_value_str = self.default_value
-
-        return dict(description=self.description,
-                    target_method=self.target_method,
-                    validator=f'${self.validator.__name__}',
-                    default_value=default_value_str)
-
+    # def to_dict(self):
+    #     """return a dict representation of the standard attribute"""
+    #
+    #     if self.default_value is DefaultValue.NONE:
+    #         default_value_str = '$optional'
+    #     elif self.default_value is DefaultValue.EMPTY:
+    #         default_value_str = '$obligatory'
+    #     else:
+    #         default_value_str = self.default_value
+    #
+    #     return dict(description=self.description,
+    #                 target_method=self.target_method,
+    #                 validator=f'${self.validator.__name__}',
+    #                 default_value=default_value_str)
+    #
     def validate(self, value, parent=None, attrs=None) -> bool:
         """validate"""
         if value is None:
             return True
 
         if isinstance(value, dict):
             try:
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/__init__.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import json
+import logging
 import pathlib
 from typing import Union
 
 from h5rdmtoolbox._user import UserDir
 from . import cache
 from .h5interface import HDF5StandardNameInterface
 from .name import StandardName
 from .table import StandardNameTable
-from .. import logger
 from ..consts import DefaultValue
 
+logger = logging.getLogger('h5rdmtoolbox')
+
 
 def parse_snt(snt: Union[str, dict, StandardNameTable]) -> StandardNameTable:
     """Returns a StandardNameTable object from a string, dict or StandardNameTable object"""
     if isinstance(snt, str):
         # could be web address or local file
         if snt[0] == '{':
             return StandardNameTable.from_dict(json.loads(snt))
@@ -27,16 +29,17 @@
         fname = pathlib.Path(snt)
         logger.debug(f'Reading standard name table from file {snt}')
         if fname.exists() and fname.suffix in ('.yaml', '.yml'):
             return StandardNameTable.from_yaml(fname)
         if snt in cache.snt:
             return cache.snt[snt]
         # maybe that's the name in the local dir:
-        if UserDir['standard_name_tables'] / f'{fname}.yaml':
-            return StandardNameTable.from_yaml(UserDir['standard_name_tables'] / f'{fname}.yaml')
+        _fname = UserDir['standard_name_tables'] / fname.with_suffix('.yaml')
+        if _fname.exists():
+            return StandardNameTable.from_yaml(_fname)
         raise FileNotFoundError(f'File {fname} not found or not a yaml file')
     if isinstance(snt, StandardNameTable):
         return snt
     if isinstance(snt, dict):
         return StandardNameTable.from_dict(snt)
     if isinstance(snt, pathlib.Path):
         return parse_snt(str(snt))
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/accessor.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/accessor.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/affixes.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/affixes.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/h5interface.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/h5interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import numpy as np
 import pathlib
-import xarray as xr
 from typing import Dict
 
+import numpy as np
+import xarray as xr
+
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox.database import ObjDB
 
 
 class StandardCoordinate:
     """Collection of 1D coordinates"""
 
@@ -129,21 +130,21 @@
                     setattr(self, k, coord)
         self.standard_names = standard_names
         self.standard_dict = standard_dict
 
     @classmethod
     def from_hdf(cls, hdf_filename, group='/', recursive: bool = False):
         """search withing a group. Note, that duplicate standard names are not considered"""
-        from ...database.lazy import lazy
+        from ...wrapper.lazy import lazy
         hdf_filename = pathlib.Path(hdf_filename)
         standard_datasets = {}
         with h5tbx.File(hdf_filename) as h5:
             std_ds = ObjDB(h5).find({'standard_name': {'$regex': '.*'}},
-                                      recursive=recursive,
-                                      objfilter='$dataset')
+                                    recursive=recursive,
+                                    objfilter='$dataset')
             # std_ds = h5[group].find({'standard_name': {'$regex': '.*'}}, rec=rec, objfilter='$dataset')
             for ds in std_ds:
                 if ds.attrs['standard_name'] not in standard_datasets:
                     standard_datasets[ds.attrs['standard_name']] = lazy(ds)
         return cls(standard_datasets)
 
     def __repr__(self):
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/name.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/name.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/table.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Standard name table module"""
 import h5py
 import json
+import logging
 import pathlib
 import pint
 import warnings
 import yaml
 from IPython.display import display, HTML
 from datetime import datetime, timezone
 from typing import List, Union, Dict, Tuple
@@ -13,18 +14,18 @@
 from h5rdmtoolbox.database import ObjDB
 from h5rdmtoolbox.repository import zenodo
 from h5rdmtoolbox.utils import generate_temporary_filename, download_file, is_xml_file
 from . import cache
 from . import consts
 from .affixes import Affix
 from .transformation import *
-from .. import logger
-from ..utils import dict2xml, get_similar_names_ratio
+from ..utils import get_similar_names_ratio
 from ... import errors
 
+logger = logging.getLogger('h5rdmtoolbox')
 __this_dir__ = pathlib.Path(__file__).parent
 
 
 class Transformations:
     """Container for transformations"""
 
     def __init__(self):
@@ -234,19 +235,19 @@
                          get_similar_names_ratio(standard_name, k) > 0.75]
         if similar_names:
             raise errors.StandardNameError(f'{standard_name} not found in Standard Name Table "{self.name}".'
                                            ' Did you mean one of these: '
                                            f'{similar_names}?')
         raise errors.StandardNameError(f'"{standard_name}" not found in Standard Name Table "{self.name}".')
 
-    def __to_h5attrs__(self) -> str:
-        """Write standard name table to HDF5 attributes"""
-        if 'zenodo_doi' in self.meta:
-            return self.meta['zenodo_doi']
-        return self.to_sdict()
+    # def __to_h5attrs__(self) -> str:
+    #     """Write standard name table to HDF5 attributes"""
+    #     if 'zenodo_doi' in self.meta:
+    #         return self.meta['zenodo_doi']
+    #     return self.to_sdict()
 
     def _repr_html_(self):
         return f"""<li style="list-style-type: none; font-style: italic">{self.__repr__()[1:-1]}</li>"""
 
     @property
     def transformations(self) -> Transformations:
         """List of available transformations"""
@@ -436,15 +437,15 @@
         if 'name' not in snt_dict:
             snt_dict['name'] = pathlib.Path(yaml_filename).stem
 
         return StandardNameTable.from_dict(snt_dict)
 
     @staticmethod
     def from_dict(snt_dict: Dict):
-        """Initialize a StandardNameTable from a YAML file"""
+        """Initialize a StandardNameTable from a dictionary"""
 
         DEFAULT_KEYS = ['standard_names',
                         'name',
                         'version',
                         'contact',
                         ('valid_characters', None),
                         ('pattern', None), ]
@@ -704,14 +705,15 @@
 
         z = zenodo.ZenodoRecord(rec_id)
         assert z.exists()
 
         filenames = z.download_files(target_folder=UserDir['standard_name_tables'])
         assert len(filenames) == 1
         filename = filenames[0]
+        assert filename.exists()
         assert filename.suffix == '.yaml'
         new_filename = UserDir['standard_name_tables'] / f'{rec_id}.yaml'
         if new_filename.exists():
             new_filename.unlink()
         yaml_filename = filename.rename(UserDir['standard_name_tables'] / f'{rec_id}.yaml')
         snt = StandardNameTable.from_yaml(yaml_filename)
         snt._meta.update(dict(zenodo_doi=doi_or_recid))
@@ -743,53 +745,14 @@
         snt_dict = self.to_dict()
 
         with open(yaml_filename, 'w') as f:
             yaml.safe_dump(snt_dict, f, sort_keys=False)
 
         return yaml_filename
 
-    def to_xml(self,
-               xml_filename: pathlib.Path,
-               datetime_str: Union[str, None] = None) -> pathlib.Path:
-        """Export the SNT in a XML file
-
-        Parameters
-        ----------
-        xml_filename: pathlib.Path
-            Path to use for the XML file
-        datetime_str: str, optional
-            Datetime format to use for the last_modified field. If None, then
-            ISO 6801 format is used.
-
-        Returns
-        -------
-        pathlib.Path
-            Path to the XML file
-        """
-        if datetime_str is None:
-            last_modified = datetime.now(datetime.timezone.utc).isoformat()
-        else:
-            last_modified = datetime.now().strftime(datetime_str)
-
-        xml_parent = xml_filename.parent
-        xml_name = xml_filename.name
-        xml_translation_filename = xml_parent / 'translation' / xml_name
-        if not xml_translation_filename.parent.exists():
-            xml_translation_filename.parent.mkdir(parents=True)
-
-        meta = self.meta
-        meta.update(last_modified=last_modified)
-
-        meta.update(dict(version=self.version))
-
-        return dict2xml(filename=xml_filename,
-                        name=self.name,
-                        dictionary=self.standard_names,
-                        **meta)
-
     def to_markdown(self, markdown_filename) -> pathlib.Path:
         """Export the SNT to a markdown file"""
         markdown_filename = pathlib.Path(markdown_filename)
         with open(markdown_filename, 'w') as f:
             f.write(consts.README_HEADER)
             for k, v in self.sort().standard_names.items():
                 f.write(f'| {k} | {v["units"]} | {v["description"]} |\n')
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/transformation.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/transformation.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/standard_names/utils.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """utils module for standard_name subpackage"""
 import h5py
+import logging
 import pathlib
 import re
 from typing import Union, Dict
 
-from .. import logger
+logger = logging.getLogger('h5rdmtoolbox')
 
 
 def _units_power_fix(_str: str):
     """Fixes strings like 'm s-1' to 'm s^-1'"""
     s = re.search('[a-zA-Z][+|-]', _str)
     if s:
         return _str[0:s.span()[0] + 1] + '^' + _str[s.span()[1] - 1:]
@@ -60,8 +61,8 @@
                 return
             _assign(node, sn)
 
     h5grp = group_or_filename
     if rec:
         return h5grp.visititems(sn_update)
     for key, obj in h5grp.items():
-        sn_update(key, obj)
+        sn_update(key, obj)
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/toolbox_validators.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/toolbox_validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 def __validate_standard_name_table(value, handler, info) -> "StandardNameTable":
     from h5rdmtoolbox.convention import standard_names
     return standard_names.parse_snt(value)
 
 
-def __validate_standard_name(value, handler, info) -> "StandardNameTable":
+def __validate_standard_name(value, handler, info) -> "StandardName":
     from h5rdmtoolbox.convention import standard_names
     if not isinstance(value, (str, standard_names.StandardName)):
         raise TypeError(f'Expected a string or StandardName object, got {type(value)}')
     if info.context:
         parent = info.context.get('parent', None)
         if parent is None:
             raise KeyError('No parent dataset found, which is needed to get the standard name table information!')
@@ -120,92 +120,83 @@
         raise TypeError(f'Expected a string but got {type(value)}')
     try:
         return get_ureg().Unit(value)
     except (pint.UndefinedUnitError, TypeError) as e:
         raise ValueError(f'Units cannot be understood using ureg package: {value}. Original error: {e}')
 
 
-def __validate_scale(value, handler, info):
-    if not info.context:
-        raise RuntimeError('Require context to validate offset!')
-    parent = info.context.get('parent', None)
-    if parent is None:
-        raise RuntimeError('Require parent dataset to validate offset!')
-    # attrs = info.context.get('attrs', None)
-
-    parent_group = info.context['parent'].parent
-
-    if isinstance(value, str) and value in parent_group:
-        return parent_group[value][()]
-
-    raise KeyError(f'No dataset found with name {value}!')
-
-
-def __validate_offset_or_scale(value, handler, info):
-    if not info.context:
-        raise RuntimeError('Require context to validate offset!')
-    parent = info.context.get('parent', None)
-    if parent is None:
-        raise RuntimeError('Require parent dataset to validate offset!')
-
-    parent_group = info.context['parent'].parent
-
-    if isinstance(value, str):
-        if value.startswith('/'):
-            try:
-                offset_or_scale_ds = parent.rootparent[value]
-            except KeyError:
-                raise KeyError(f'No dataset found with name {value}!')
-        else:
-            try:
-                offset_or_scale_ds = parent_group[value]
-            except KeyError:
-                raise KeyError(f'No dataset found with name {value}!')
-    else:
-        raise TypeError(f'Offset dataset must be dataset name of dataset object, not {type(value)}')
-
-    assert offset_or_scale_ds.ndim == 0
-
-    offset_or_scale_ds_name = offset_or_scale_ds.name
-    return offset_or_scale_ds_name
+# def __validate_scale(value, handler, info):
+#     if not info.context:
+#         raise RuntimeError('Require context to validate offset!')
+#     parent = info.context.get('parent', None)
+#     if parent is None:
+#         raise RuntimeError('Require parent dataset to validate offset!')
+#     # attrs = info.context.get('attrs', None)
+#
+#     parent_group = info.context['parent'].parent
+#
+#     if isinstance(value, str) and value in parent_group:
+#         return parent_group[value][()]
+#
+#     raise KeyError(f'No dataset found with name {value}!')
+
+
+# def __validate_offset_or_scale(value, handler, info):
+#     if not info.context:
+#         raise RuntimeError('Require context to validate offset!')
+#     parent = info.context.get('parent', None)
+#     if parent is None:
+#         raise RuntimeError('Require parent dataset to validate offset!')
+#
+#     parent_group = info.context['parent'].parent
+#
+#     if isinstance(value, str):
+#         if value.startswith('/'):
+#             try:
+#                 offset_or_scale_ds = parent.rootparent[value]
+#             except KeyError:
+#                 raise KeyError(f'No dataset found with name {value}!')
+#         else:
+#             try:
+#                 offset_or_scale_ds = parent_group[value]
+#             except KeyError:
+#                 raise KeyError(f'No dataset found with name {value}!')
+#     else:
+#         raise TypeError(f'Offset dataset must be dataset name of dataset object, not {type(value)}')
+#
+#     assert offset_or_scale_ds.ndim == 0
+#
+#     offset_or_scale_ds_name = offset_or_scale_ds.name
+#     return offset_or_scale_ds_name
 
 
 def __validate_date_format(value, handler, info):
     """value: str, e.g. '1991-01-19T13:45:05TZD'"""
     import dateutil.parser
     import warnings
     # will raise an error if not a valid datetime
     try:
         warnings.filterwarnings("error")
         dt = dateutil.parser.parse(value)
-    except RuntimeWarning as e:
-        raise ValueError(f'Invalid datetime: {value}. Original error: {e}')
+    except TypeError as e:
+        raise TypeError(f'Invalid datetime: {value}. Original error: {e}')
     finally:
         warnings.filterwarnings("ignore")
     return dt
 
 
-def _get_validate_type(_type):
-    def __validate_type(value, handler, info):
-        if not isinstance(value, _type):
-            raise TypeError(f'Value must be a string but got {type(value)}')
-        return value
-
-    return __validate_type
-
-
 unitsType = Annotated[str, WrapValidator(__validate_units)]
 
 dateFormatType = Annotated[str, WrapValidator(__validate_date_format)]
 
 quantityType = Annotated[str, WrapValidator(__validate_quantity)]
 
-dataOffsetType = Annotated[str, WrapValidator(__validate_offset_or_scale)]
-
-dataScaleType = Annotated[str, WrapValidator(__validate_offset_or_scale)]
+# dataOffsetType = Annotated[str, WrapValidator(__validate_offset_or_scale)]
+#
+# dataScaleType = Annotated[str, WrapValidator(__validate_offset_or_scale)]
 
 orcidType = Annotated[str, WrapValidator(__validate_orcid)]
 
 identifierType = Annotated[str, WrapValidator(__validate_identifier)]
 
 standardNameTableType = Annotated[Union[str, Dict], WrapValidator(__validate_standard_name_table)]
 
@@ -215,16 +206,16 @@
 
 versionType = Annotated[str, WrapValidator(__verify_version)]
 
 validators = {
     'units': unitsType,
     'dateFormat': dateFormatType,
     'quantity': quantityType,
-    'data_offset': dataOffsetType,
-    'data_scale': dataScaleType,
+    # 'data_offset': dataOffsetType,
+    # 'data_scale': dataScaleType,
     'orcid': orcidType,
     'identifier': identifierType,
     'standard_name_table': standardNameTableType,
     'standard_name': standardNameType,
     'url': urlType,
     'version': versionType
 }
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/convention/utils.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/fluid-v1.yml` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/fluid-v1.yml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/h5tbx.yaml` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/h5tbx.yaml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/piv-v1.yml` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/piv-v1.yml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/style.css` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/style.css`

 * *Files 16% similar despite different names*

```diff
@@ -177,8 +177,40 @@
     padding-bottom: 6px;
     color: #6a6c73;
 }
 
 .h5tb-attr-list li,
 .h5tb-attr-list li:hover {
     background-color: rgba(0,0,0,.0);
+}
+
+
+/* Tooltip container */
+.tooltip {
+position: relative;
+display: inline-block;
+cursor: pointer;
+}
+
+/* Tooltip text */
+.tooltip .tooltiptext {
+visibility: hidden;
+width: 300px;
+background-color: #555;
+color: #fff;
+text-align: center;
+border-radius: 6px;
+padding: 5px;
+position: absolute;
+z-index: 1;
+bottom: 125%;
+left: 50%;
+margin-left: -60px;
+opacity: 0;
+transition: opacity 0.3s;
+}
+
+/* Show the tooltip on hover */
+.tooltip:hover .tooltiptext {
+visibility: visible;
+opacity:  1;
 }
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/tutorial_convention.yaml` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_convention.yaml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/data/tutorial_standard_name_table.yaml` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_standard_name_table.yaml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/filedb.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/filedb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,66 @@
-import h5py
 import pathlib
-from typing import Union, Generator, List
+from typing import Union, Generator, List, Optional
+
+import h5py
 
 from .objdb import ObjDB
-from .nonsearchable import NonInsertableDatabaseInterface
-from .. import lazy
-from ..template import HDF5DBInterface
+from ..interface import HDF5DBInterface, NonInsertableDatabaseInterface
+from ...wrapper import lazy
 
 
 class FileDB(NonInsertableDatabaseInterface, HDF5DBInterface):
     """A database interface for an HDF5 file, where the filename is given."""
 
     def __init__(self, filename: Union[str, pathlib.Path]):
-        self.filename = pathlib.Path(filename)
+        self.filename: str = str(filename)
         self.find = self._instance_find  # allow `find` to be a static method and instance method
         self.find_one = self._instance_find_one  # allow `find_one` to be a static method and instance method
+        self.rdf_find = self._instance_rdf_find
 
     @staticmethod
-    def find_one(file_or_filename, *args, **kwargs) -> lazy.LHDFObject:
+    def find_one(filename: Union[str, pathlib.Path], *args, **kwargs) -> lazy.LHDFObject:
         """Please refer to the docstring of the find_one method of the ObjDB class"""
-        if isinstance(file_or_filename, (h5py.Group, h5py.Dataset)):
-            return ObjDB(file_or_filename).find_one(*args, **kwargs)
-        with h5py.File(file_or_filename, 'r') as h5:
+        with h5py.File(str(filename), 'r') as h5:
             return ObjDB(h5).find_one(*args, **kwargs)
 
     def _instance_find(self, *args, **kwargs):
         with h5py.File(self.filename, 'r') as h5:
             return list(ObjDB(h5).find(*args, **kwargs))
 
+    def _instance_rdf_find(self, *,
+                           rdf_subject: Optional[str] = None,
+                           rdf_type: Optional[str] = None,
+                           rdf_predicate: Optional[str] = None,
+                           rdf_object: Optional[str] = None,
+                           recursive: bool = True):
+        with h5py.File(self.filename, 'r') as h5:
+            return list(ObjDB(h5).rdf_find(rdf_subject=rdf_subject,
+                                           rdf_type=rdf_type,
+                                           rdf_predicate=rdf_predicate,
+                                           rdf_object=rdf_object,
+                                           recursive=recursive))
+
     def _instance_find_one(self, *args, **kwargs):
         with h5py.File(self.filename, 'r') as h5:
             return ObjDB(h5).find_one(*args, **kwargs)
 
     @staticmethod
     def find(file_or_filename, *args, **kwargs) -> Generator[lazy.LHDFObject, None, None]:
         """Please refer to the docstring of the find method of the ObjDB class"""
         if isinstance(file_or_filename, (h5py.Group, h5py.Dataset)):
-            results = list(ObjDB(file_or_filename).find(*args, **kwargs))
-            for r in results:
-                yield r
+            return list(ObjDB(file_or_filename).find(*args, **kwargs))
+            # for r in results:
+            #     yield r
         else:
             with h5py.File(file_or_filename, 'r') as h5:
                 results = list(ObjDB(h5).find(*args, **kwargs))
-            for r in results:
-                yield r
+            return results
+            # for r in results:
+            #     yield r
 
 
 class FilesDB(NonInsertableDatabaseInterface, HDF5DBInterface):
     """A database interface for an HDF5 file, where the filename is given."""
 
     def __init__(self, filenames: List[Union[str, pathlib.Path]]):
         self.filenames = list(set(pathlib.Path(filename) for filename in filenames))
@@ -77,20 +90,19 @@
         self.filenames = list(set(self.filenames))
 
     def find_one(self, *args, **kwargs) -> lazy.LHDFObject:
         """Call find_one on all the files registerd. If more than one file
         contains the object, the first one is returned. If you want to find one per file,
         call find_one_per_file instead."""
         for filename in self.filenames:
-            with h5py.File(filename, 'r') as h5:
+            with h5py.File(filename, mode='r') as h5:
                 ret = ObjDB(h5).find_one(*args, **kwargs)
                 if ret:
                     return ret
-        return
 
     def find(self, *args, **kwargs) -> Generator[lazy.LHDFObject, None, None]:
-        all_results = []
+        """Call find on all the files"""
         for filename in self.filenames:
             with h5py.File(filename, 'r') as h5:
                 ret = ObjDB(h5).find(*args, **kwargs)
-                all_results.extend(ret)
-        return all_results
+                for r in ret:
+                    yield r
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/objdb.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/objdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import h5py
+import json
 import numpy as np
-from typing import Union, Dict, List, Callable, Generator
+from typing import Type
+from typing import Union, Dict, List, Callable, Optional
 
 from . import query, utils
-from .nonsearchable import NonInsertableDatabaseInterface
-from .. import lazy
-from ..template import HDF5DBInterface
+from ..interface import HDF5DBInterface, NonInsertableDatabaseInterface
+from ...protocols import LazyDataset, LazyGroup, LazyObject
+from ...wrapper import lazy
 
 
 def basename(name: str) -> str:
     """Return basename of a name, which is the last occurrence in
     a string with forward slashes"""
     return name.rsplit('/', 1)[-1]
 
 
 class RecFind:
     """Visititems class to find all objects with a certain attribute value"""
 
     def __init__(self, func: Callable, attribute, value, objfilter, ignore_attribute_error):
         self._func = func
         self._attribute = attribute
+        if isinstance(value, set):
+            raise TypeError(
+                'It seems that your query has a typo. Expecting a dictionary or base string or number but got '
+                f'a set: {value}'
+            )
+        # if isinstance(value, dict):
+        #     _operators = query.operator.get(k) for k in value.keys()
         self._value = value
         self.found_objects = []
         self.objfilter = objfilter
         self.ignore_attribute_error = ignore_attribute_error
 
     def __call__(self, name, h5obj):
         if self.objfilter:
             if not isinstance(h5obj, self.objfilter):
                 return
         try:
             objattr = h5obj.__getattribute__(self._attribute)
             if self._func(objattr, self._value):
                 self.found_objects.append(h5obj)
-        except AttributeError as e:
+        except AttributeError:
             return
-            if not self.ignore_attribute_error:
-                raise AttributeError(f'HDF object {h5obj} has no attribute "{self._attribute}". You may add '
-                                     'an objfilter, because dataset and groups dont share all attributes. '
-                                     'One example is "dtype", which is only available with datasets') from e
+            # if not self.ignore_attribute_error:
+            #     raise AttributeError(f'HDF object {h5obj} has no attribute "{self._attribute}". You may add '
+            #                          'an objfilter, because dataset and groups dont share all attributes. '
+            #                          'One example is "dtype", which is only available with datasets') from e
 
 
 class RecValueFind:
     def __init__(self, transformer_func: Callable, comparison_func: Callable, comparison_value):
         self._tfunc = transformer_func
         self._cfunc = comparison_func
         self._value = comparison_value
@@ -73,62 +82,67 @@
     def __call__(self, name, obj):
         if self.objfilter:
             if not isinstance(obj, self.objfilter):
                 return
         if '.' in self._attribute:
             # dict comparison:
             attr_name, dict_path = self._attribute.split('.', 1)
-            if attr_name in obj.attrs:
-                _attr_dict = dict(obj.attrs[attr_name])
-                for _item in dict_path.split('.'):
-                    try:
-                        _attr_value = _attr_dict[_item]
-                    except KeyError:
-                        _attr_value = None
-                        break
-                if _attr_value:
-                    if self._func(_attr_value, self._value):
-                        self.found_objects.append(obj)
+            attr_value = obj.attrs.get(attr_name, None)
+            if attr_value is not None:
+                if isinstance(attr_value, str) and attr_value.startswith('{') and attr_value.endswith('}'):
+                    _attr_dict = json.loads(attr_value)
+
+                    _attr_value = None
+                    for _item in dict_path.split('.'):
+                        try:
+                            _attr_value = _attr_dict[_item]
+                        except KeyError:
+                            break
+
+                    if _attr_value:
+                        if self._func(_attr_value, self._value):
+                            self.found_objects.append(obj)
+
         if self._func(obj.attrs.get(self._attribute, None), self._value):
             self.found_objects.append(obj)
 
 
 class RecPropCollect:
     """Visititems class to collect all class attributes matching a certain string"""
 
-    def __init__(self, attribute_name: str, objfilter: Union[h5py.Group, h5py.Dataset, None]):
+    def __init__(self, attribute_name: str, objfilter: Optional[Union[Type[h5py.Dataset], Type[h5py.Group]]]):
         self._attribute_name = attribute_name
         self._objfilter = objfilter
         self.found_objects = []
 
-    def __call__(self, name, obj):
+    def __call__(self, name: str, obj: Union[h5py.Group, h5py.Dataset]):
         if self._objfilter is None:
             try:
-                propval = obj.__getattribute__(self._attribute_name)
-                self.found_objects.append(propval)
+                property_value = obj.__getattribute__(self._attribute_name)
+                self.found_objects.append(property_value)
             except AttributeError:
                 pass
         else:
             if isinstance(obj, self._objfilter):
                 try:
-                    propval = obj.__getattribute__(self._attribute_name)
-                    self.found_objects.append(propval)
+                    property_value = obj.__getattribute__(self._attribute_name)
+                    self.found_objects.append(property_value)
                 except AttributeError:
                     pass
 
 
 class RecAttrCollect:
     """Visititems class to collect all attributes matching a certain string"""
 
-    def __init__(self, attribute_name: str, objfilter: Union[h5py.Group, h5py.Dataset, None]):
+    def __init__(self, attribute_name: str, objfilter: Optional[Union[Type[h5py.Dataset], Type[h5py.Group]]]):
         self._attribute_name = attribute_name
         self._objfilter = objfilter
         self.found_objects = []
 
-    def __call__(self, name, obj):
+    def __call__(self, name: str, obj: Union[h5py.Group, h5py.Dataset]):
         if self._objfilter is None:
             if self._attribute_name in obj.attrs:
                 self.found_objects.append(obj.attrs[self._attribute_name])
         else:
             if isinstance(obj, self._objfilter):
                 if self._attribute_name in obj.attrs:
                     self.found_objects.append(obj.attrs[self._attribute_name])
@@ -142,16 +156,21 @@
     h5obj: h5py.Group, h5py.Dataset
         h5py object (group or dataset) to start search from
 
     Returns
     -------
 
     """
-    found_objs = []
 
+    if qk == '$basename':
+        qk = '$name'
+        assert isinstance(qv, str), 'Expected {$basename: "search value"} but value is not a string'
+        qv = {'$basename': qv}
+
+    found_objs = []
     if qk in query.value_operator:
         # user wants to compare qv to the value of the object
 
         if not isinstance(qv, Dict):
             qv = {'$eq': qv}
 
         if len(qv) != 1:
@@ -180,21 +199,21 @@
                     if isinstance(target_obj, h5py.Dataset):
                         transformed_value = query.math_operator[math_operator_name](target_obj, comparison_value)
                         if transformed_value is not None:
                             if query.value_operator[qk](transformed_value, comparison_value):
                                 found_objs.append(target_obj)
             return found_objs
 
+        if isinstance(qv, Dict) and len(qv) != 1:
+            raise ValueError(f'Cannot use query.operator "{qk}" for dict with more than one key')
+
         if isinstance(qv, (float, int)):
             qv_ndim = 0
-        elif isinstance(qv, Dict):
-            if len(qv) != 1:
-                raise ValueError(f'Cannot use query.operator "{qk}" for dict with more than one key')
-
         else:
+            assert isinstance(qv, (str, np.ndarray)), f'Unexpected type: {type(qv)}'
             qv_ndim = np.ndim(qv)
 
         if qv_ndim > 0 and qk != '$eq':
             raise ValueError(f'Cannot use query.operator "{qk}" for non-scalar value "{qv}"')
         if qk == '$eq':
             qk = '$arreq'
 
@@ -229,19 +248,19 @@
                         _skip = True
                 if not _skip:
                     if '.' in qk:
                         # dict comparison:
                         attr_name, dict_path = qk.split('.', 1)
                         if attr_name in h5obj.attrs:
                             _attr_dict = dict(h5obj.attrs[attr_name])
+                            _attr_value = None
                             for _item in dict_path.split('.'):
                                 try:
                                     _attr_value = _attr_dict[_item]
                                 except KeyError:
-                                    _attr_value = None
                                     break
                             if _attr_value:
                                 if query.operator[ok](_attr_value, ov):
                                     found_objs.append(h5obj)
                     elif qk in h5obj.attrs:
                         if query.operator[ok](h5obj.attrs[qk], ov):
                             found_objs.append(h5obj)
@@ -260,14 +279,15 @@
                                 found_objs.append(hv)
     else:
         for ok, ov in qv.items():
             if recursive:
                 rf = RecFind(query.operator[ok], qk[1:], ov, objfilter=objfilter,
                              ignore_attribute_error=ignore_attribute_error)
                 rf(name='/', h5obj=h5obj)  # visit the root group
+                # rf(name=h5obj.name, h5obj=h5obj)  # visit the root group
                 h5obj.visititems(rf)  # will not visit the root group
                 for found_obj in rf.found_objects:
                     found_objs.append(found_obj)
             else:
                 if isinstance(h5obj, h5py.Dataset):
                     iterator = [(basename(h5obj.name), h5obj), ]
                 else:
@@ -281,28 +301,57 @@
                         try:
                             objattr = hv.__getattribute__(qk[1:])
                         except AttributeError:
                             if ignore_attribute_error:
                                 continue
                             raise ValueError(f'No such attribute: {qk[1:]}.')
 
-                    try:
-                        if query.operator[ok](objattr, ov):
-                            found_objs.append(hv)
-                    except Exception as e:
-                        raise Exception(f'Error while filtering for "{qk}" with "{ok}" and "{ov}"') from e
+                        try:
+                            if query.operator[ok](objattr, ov):
+                                found_objs.append(hv)
+                        except Exception as e:
+                            raise Exception(f'Error while filtering for "{qk}" with "{ok}" and "{ov}": {e}')
     return found_objs
 
 
+ListOfLazyObjs = List[Union[LazyDataset, LazyGroup]]
+
+
 def find(h5obj: Union[h5py.Group, h5py.Dataset],
-         flt: [Dict, str, List[str]],
+         flt: Union[Dict, str, List[str]],
          objfilter: Union[h5py.Group, h5py.Dataset, None],
          recursive: bool,
          find_one: bool,
-         ignore_attribute_error):
+         ignore_attribute_error) -> Optional[Union[List[LazyObject], LazyObject]]:
+    """Find datasets or groups in an object.
+
+    Parameters
+    ----------
+    h5obj: Group or Dataset
+        obj from where to start searching
+    flt: Union[Dict, str, List[str]]
+        The filter query similar to the pymongo syntax.
+    objfilter: Optional
+        Filter only for dataset or group. if None, consider both types.
+    recursive: bool
+        Whether to recursively search in subgroups, too
+    find_one: bool
+        If True, the first search result is returned
+    ignore_attribute_error: bool
+        If True, attribute errors are ignored.
+
+    Examples
+    --------
+    >>> from h5rdmtoolbox.database import hdfdb
+    >>> with h5tbx.File(filename) as h5:
+    ...     # find the obj with standard_name=='x_velocity':
+    ...     hdfdb.ObjDB(h5).find({'standard_name': 'x_velocity'})
+    ...     # all datasets must be gzip-compressed:
+    ...     hdfdb.ObjDB(h5).find({'$compression': 'gzip'}, objfilter='dataset')
+    """
     if flt == {}:  # just find any!
         flt = {'$name': {'$regex': '.*'}}
     if isinstance(flt, str):  # just find the attribute and don't filter for the value:
         flt = {flt: {'$regex': '.*'}}
     if isinstance(flt, List):
         if all(isinstance(f, str) for f in flt):
             flt = {f: {'$regex': '.*'} for f in flt}
@@ -325,74 +374,88 @@
     if find_one:
         if len(common_results):
             return common_results[0]
         return  # Nothing found
     return common_results
 
 
-def distinct(h5obj: Union[h5py.Group, h5py.Dataset], key: str,
-             objfilter: Union[h5py.Group, h5py.Dataset, None]) -> List[str]:
+def distinct(h5obj: Union[h5py.Group, h5py.Dataset],
+             key: str,
+             objfilter: Optional[Union[Type[h5py.Group], Type[h5py.Dataset]]]) -> List[str]:
     """Return a distinct list of all found targets. A target generally is
     understood to be an attribute name. However, by adding a $ in front, class
     properties can be found, too, e.g. $shape will return all distinct shapes of the
     passed group."""
     objfilter = utils.parse_obj_filter_input(objfilter)
     if key[0] == '$':
         rpc = RecPropCollect(key[1:], objfilter)
 
         h5obj.visititems(rpc)
         if objfilter:
             if isinstance(h5obj, objfilter):
                 try:
-                    propval = h5obj.__getattribute__(key[1:])
-                    rpc.found_objects.append(propval)
+                    property_value = h5obj.__getattribute__(key[1:])
+                    rpc.found_objects.append(property_value)
                 except AttributeError:
                     pass
         else:
             try:
-                propval = h5obj.__getattribute__(key[1:])
-                rpc.found_objects.append(propval)
+                property_value = h5obj.__getattribute__(key[1:])
+                rpc.found_objects.append(property_value)
             except AttributeError:
                 pass
 
         return list(set(rpc.found_objects))
 
     rac = RecAttrCollect(key, objfilter)
-    for k, v in h5obj.attrs.raw.items():
+    for k, v in h5obj.attrs.items():
         if k == key:
             rac.found_objects.append(v)
     if isinstance(h5obj, h5py.Group):
         h5obj.visititems(rac)
         if objfilter:
             if isinstance(h5obj, objfilter):
-                if key in h5obj.attrs.raw:
-                    rac.found_objects.append(h5obj.attrs.raw[key])
+                if key in h5obj.attrs:
+                    rac.found_objects.append(h5obj.attrs[key])
         else:
-            if key in h5obj.attrs.raw:
-                rac.found_objects.append(h5obj.attrs.raw[key])
+            if key in h5obj.attrs:
+                rac.found_objects.append(h5obj.attrs[key])
 
     return list(set(rac.found_objects))
 
 
 class ObjDB(NonInsertableDatabaseInterface, HDF5DBInterface):
     """HDF5 Group or Dataset as a database"""
 
     def __init__(self, obj: Union[h5py.Dataset, h5py.Group]):
         if isinstance(obj, h5py.Group):
             self.src_obj = h5py.Group(obj.id)
         elif isinstance(obj, h5py.Dataset):
             self.src_obj = h5py.Dataset(obj.id)
         else:
             raise TypeError(f'Unexpected type: {type(obj)}')
-
-    def find_one(self,
-                 flt: Union[Dict, str],
-                 objfilter=None,
-                 recursive: bool = True,
-                 ignore_attribute_error: bool = False) -> lazy.LHDFObject:
+        self.find = self._instance_find  # allow `find` to be a static method and instance method
+        self.rdf_find = self._instance_rdf_find  # allow `find` to be a static method and instance method
+        self.find_one = self._instance_find_one  # allow `find_one` to be a static method and instance method
+
+    @staticmethod
+    def find_one(obj: Union[h5py.Dataset, h5py.Group], *args, **kwargs) -> Union[LazyObject]:
+        """Please refer to the docstring of the find_one method of the ObjDB class"""
+        return ObjDB(obj).find_one(*args, **kwargs)
+
+    @staticmethod
+    def find(obj: Union[h5py.Dataset, h5py.Group], *args, **kwargs) -> List[LazyObject]:
+        """Please refer to the docstring of the find_one method of the ObjDB class"""
+        return ObjDB(obj).find(*args, **kwargs)
+
+    def _instance_find_one(self,
+                           flt: Union[Dict, str],
+                           objfilter=None,
+                           recursive: bool = True,
+                           ignore_attribute_error: bool = False) -> LazyObject:
         """Find one object in the obj
 
         Parameters
         ----------
         flt : Union[Dict, str]
             The filter query similar to the pymongo syntax.
         objfilter : Union[h5py.Group, h5py.Dataset, None]
@@ -401,41 +464,57 @@
             If True, the search will be recursive. If False, only the current obj
             will be searched.
         ignore_attribute_error : bool
             If True, an AttributeError will be ignored if the attribute is not found.
         """
         if isinstance(self.src_obj, h5py.Dataset) and recursive:
             recursive = False
-        return lazy.lazy(
-            find(
-                self.src_obj,
-                flt=flt,
-                objfilter=objfilter,
-                recursive=recursive,
-                find_one=True,
-                ignore_attribute_error=ignore_attribute_error)
+
+        return find(
+            self.src_obj,
+            flt=flt,
+            objfilter=objfilter,
+            recursive=recursive,
+            find_one=True,
+            ignore_attribute_error=ignore_attribute_error
         )
 
-    def find(self,
-             flt: Union[Dict, str],
-             objfilter=None,
-             recursive: bool = True,
-             ignore_attribute_error: bool = False) -> Generator[lazy.LHDFObject, None, None]:
+    def _instance_find(self,
+                       flt: Union[Dict, str],
+                       objfilter=None,
+                       recursive: bool = True,
+                       ignore_attribute_error: bool = False) -> List[LazyObject]:
         if isinstance(self.src_obj, h5py.Dataset) and recursive:
             recursive = False
         results = find(self.src_obj,
                        flt=flt,
                        objfilter=objfilter,
                        recursive=recursive,
                        find_one=False,
                        ignore_attribute_error=ignore_attribute_error)
+        return results
 
-        for r in results:
-            yield r
+    def _instance_rdf_find(self, *,
+                           rdf_subject: Optional[str] = None,
+                           rdf_type: Optional[str] = None,
+                           rdf_predicate: Optional[str] = None,
+                           rdf_object: Optional[str] = None,
+                           recursive: bool = True) -> Optional[List[Union[LazyDataset, LazyGroup]]]:
+        """Find objects based on rdf triples"""
+        import h5rdmtoolbox as h5tbx
+        if isinstance(self.src_obj, h5py.Group):
+            src_obj = h5tbx.Group(self.src_obj)
+        else:
+            src_obj = h5tbx.Dataset(self.src_obj)
+        return lazy.lazy(src_obj.rdf.find(rdf_subject=rdf_subject,
+                                          rdf_type=rdf_type,
+                                          rdf_predicate=rdf_predicate,
+                                          rdf_object=rdf_object,
+                                          recursive=recursive))
 
     def distinct(self, key: str,
-                 objfilter: Union[h5py.Group, h5py.Dataset, None]):
+                 objfilter: Optional[Union[h5py.Group, h5py.Dataset]] = None):
         """Return a distinct list of all found targets. A target generally is
         understood to be an attribute name. However, by adding a $ in front, class
         properties can be found, too, e.g. $shape will return all distinct shapes of the
         passed obj."""
         return distinct(h5obj=self.src_obj, key=key, objfilter=objfilter)
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/query.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-import numpy as np
+"""query module"""
+import logging
 import re
 import warnings
 
+import numpy as np
+
+logger = logging.getLogger('h5rdmtoolbox')
+
 
 def _eq(a, b):
     """Check if a == b"""
     if a is None or b is None:
         return False
     return a == b
 
@@ -29,14 +34,15 @@
     if a is None or b is None:
         return False
     return a >= b
 
 
 def _lt(a, b):
     """Check if a < b"""
+    logger.debug(f'checking if a < b ({a} < {b})')
     if a is None or b is None:
         return False
     return a < b
 
 
 def _lte(a, b):
     """Check if a <= b"""
@@ -51,27 +57,32 @@
 
     if isinstance(value, np.bytes_):
         try:
             value = value.decode()
         except UnicodeDecodeError:
             warnings.warn(f'could not decode {value}', UserWarning)
             return False
+
     if isinstance(value, bytes):
         value = value.decode()
 
+    value = str(value)
+
     match = re.search(pattern, value)
     if match is None:
         return False
     return True
 
+
 def _userdefined(value, func) -> bool:
     if value is None:
         return False
     return func(value)
 
+
 def _basename(value, basename) -> bool:
     if value is None:
         return False
     return _regex(value, pattern=f'^.*/{basename}$')
 
 
 def _exists(value, tf: bool) -> bool:
@@ -87,16 +98,14 @@
             '$gte': _gte,
             '$lt': _lt,
             '$lte': _lte,
             '$exists': _exists,
             '$userdefined': _userdefined}
 value_operator = {'$eq': _arreq, '$gt': _gt, '$gte': _gte, '$lt': _lt, '$lte': _lte}
 
-AV_SPECIAL_FILTERS = ('$basename', '$name')
-
 
 def _pass(obj, comparison_value):
     if get_ndim(comparison_value) == obj.ndim:
         return obj[()]
     return None
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/hdfdb/utils.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,44 @@
+from typing import Type, Optional, Union
+
 import h5py
-from typing import Union
 
 OBJ_FLT_DICT = {'group': h5py.Group,
                 'groups': h5py.Group,
                 'dataset': h5py.Dataset,
                 'datasets': h5py.Dataset,
                 '$group': h5py.Group,
                 '$groups': h5py.Group,
                 '$dataset': h5py.Dataset,
                 '$datasets': h5py.Dataset}
 
+AnyH5Like = Optional[Union[str, Type[h5py.Group], Type[h5py.Dataset], h5py.Dataset, h5py.Group]]
+
 
-def parse_obj_filter_input(objfilter: Union[str, h5py.Dataset, h5py.Group]) -> Union[h5py.Dataset, h5py.Group, None]:
+def parse_obj_filter_input(objfilter: AnyH5Like) -> Optional[Union[Type[h5py.Group], Type[h5py.Dataset]]]:
     """Return the object based on the input string
 
     Parameters
     ----------
-    objfilter : str or h5py.Dataset or h5py.Group
-        The object to filter for. If it is a string, it must be one of the following:
+    objfilter : AnyH5Like
+        Any HDF5-like object or class or string indicating the object type/class.
+         If it is a string, it must be one of the following:
         'group', 'groups', 'dataset', 'datasets', '$group', '$groups', '$dataset', '$datasets'
+        None returns None.
 
     Raises
     ------
     ValueError
         If the input string is not in the list of valid strings (see OBJ_FLT_DICT)
     TypeError
         If the input is not a string or a h5py object (h5py.Dataset or h5py.Group)
 
     Returns
     -------
-    h5py.Dataset or h5py.Group or None
+    Optional[Union[Type[h5py.Group], Type[h5py.Dataset]]]
         The object to filter for
     """
     if objfilter is None:
         return
     if isinstance(objfilter, str):
         _obj_cls = OBJ_FLT_DICT.get(objfilter.lower(), None)
         if _obj_cls is None:
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/lazy.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/lazy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """lazy objects. user can work with datasets and groups without having to open the file him/her-self"""
-import h5py
 import pathlib
-from typing import Union, List, Dict
+from typing import Union, List, Dict, Optional
+
+import h5py
+
+from h5rdmtoolbox.protocols import LazyObject
 
 
 class LHDFObject:
-    """Lazy HDF object. This object is a proxy for a HDF object (dataset or group) that returns data
+    """Lazy HDF object. This object is a proxy for an HDF object (dataset or group) that returns data
     on-demand. This means, that the file is opened when the object is accessed and closed when the object
     is no longer needed. This is useful for working with large files, where the user does not want to
     open the file manually, but still wants to work with the dataset.
     """
 
-    def __init__(self, obj: h5py.Group):
+    def __init__(self, obj: Union[h5py.Group, h5py.Dataset]):
         self.filename = pathlib.Path(obj.file.filename)
-        if isinstance(obj.attrs, h5py.AttributeManager):
-            self._attrs = dict(obj.attrs)
-        else:
-            self._attrs = dict(obj.attrs.raw)
-
-        for k, v in _get_dataset_properties(obj, ('file', 'name',)).items():
-            setattr(self, k, v)
+        self._attrs = dict(obj.attrs)
+        self.name = obj.name
+        self._file = None
 
     def __repr__(self):
         return f'<{self.__class__.__name__} "{self.name}" in "{self.filename}">'
 
     def __lt__(self, other):
         return self.name < other.name
 
@@ -62,37 +61,14 @@
         """Return the attributes of the group as a LAttributeManager object"""
         return self._attrs
 
     @property
     def hdf_filename(self):
         """Return the hdf filename"""
         return self.filename
-    # def find(self, flt: Union[Dict, str],
-    #          objfilter: Union[str, h5py.Dataset, h5py.Group, None] = None,
-    #          rec: bool = True,
-    #          ignore_attribute_error: bool = False):
-    #     """Find"""
-    #     from .file import find as _find
-    #     with self as obj:
-    #         if isinstance(obj, h5py.Dataset):
-    #             return [lazy(i) for i in _find(obj, flt, objfilter, find_one=False, recursive=False,
-    #                                            ignore_attribute_error=ignore_attribute_error)]
-    #         return [lazy(i) for i in _find(obj, flt, objfilter, find_one=False, recursive=rec,
-    #                                        ignore_attribute_error=ignore_attribute_error)]
-    #
-    # def find_one(self,
-    #              flt: Union[Dict, str],
-    #              objfilter=None,
-    #              rec: bool = True,
-    #              ignore_attribute_error: bool = False):
-    #     """Find one occurrence"""
-    #     from .file import find as _find
-    #     with self as obj:
-    #         return lazy(_find(obj, flt, objfilter, find_one=True, recursive=rec,
-    #                           ignore_attribute_error=ignore_attribute_error))
 
 
 class LGroup(LHDFObject):
     """Lazy Group"""
 
     def __init__(self, obj: h5py.Group):
         super().__init__(obj)
@@ -108,33 +84,40 @@
                 if ' ' not in k and not hasattr(self, k):
                     setattr(self, k, self._children[k])
 
     def keys(self):
         """Return the keys of the group which are the names of datasets and groups"""
         return self._children.keys()
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: str):
         if item in self._children:
             return self._children[item]
-        return super(LGroup, self).__getitem__(item)
+        raise KeyError(f'No such item: {item}. Known items: {self.keys()}')
 
 
 class LDataset(LHDFObject):
     """Lazy Dataset"""
 
     def __init__(self, obj: h5py.Dataset):
         super().__init__(obj)
+        # self.name = obj.name  # parent class already has this
+        self.ndim = obj.ndim
+        self.shape = obj.shape
+        self.dtype = obj.dtype
+        self.size = obj.size
+        self.chunks = obj.chunks
+        self.compression = obj.compression
+        self.compression_opts = obj.compression_opts
+        self.shuffle = obj.shuffle
+        self.fletcher32 = obj.fletcher32
+        self.maxshape = obj.maxshape
+        self.fillvalue = obj.fillvalue
+        self.scaleoffset = obj.scaleoffset
+        self.external = obj.external
 
-        keys = ("name", "ndim", "shape", "dtype", "size", "chunks",
-                "compression", "compression_opts",
-                "shuffle", "fletcher32", "maxshape",
-                "fillvalue", "scaleoffset", "external",
-                "file")
-        for k, v in _get_dataset_properties(obj, keys).items():
-            setattr(self, k, v)
         self._file = None
 
     def __repr__(self):
         attrs_str = ', '.join({f'{k}={v}' for k, v in self.attrs.items() if not k.isupper()})
         return f'<LDataset "{self.name}" in "{self.filename}" attrs=({attrs_str})>'
 
     def __getitem__(self, item):
@@ -153,43 +136,41 @@
             return h5[self.name].isel(**indexers)
 
     def sel(self, **coords):
         from .. import File
         with File(self.filename) as h5:
             return h5[self.name].sel(**coords)
 
-    def find(self, flt: Union[Dict, str],
-             objfilter: Union[str, h5py.Dataset, h5py.Group, None] = None,
-             ignore_attribute_error: bool = False):
-        """Find"""
-        return super().find(flt, objfilter, rec=False, ignore_attribute_error=ignore_attribute_error)
-
-    def find_one(self,
-                 flt: Union[Dict, str],
-                 objfilter=None,
-                 ignore_attribute_error: bool = False):
-        """Find one occurrence"""
-        return super().find_one(flt, objfilter, rec=False, ignore_attribute_error=ignore_attribute_error)
+    # def find(self, flt: Union[Dict, str],
+    #          objfilter: Union[str, h5py.Dataset, h5py.Group, None] = None,
+    #          ignore_attribute_error: bool = False):
+    #     """Find"""
+    #     return super().find(flt, objfilter, rec=False, ignore_attribute_error=ignore_attribute_error)
+    #
+    # def find_one(self,
+    #              flt: Union[Dict, str],
+    #              objfilter=None,
+    #              ignore_attribute_error: bool = False):
+    #     """Find one occurrence"""
+    #     return super().find_one(flt, objfilter, rec=False, ignore_attribute_error=ignore_attribute_error)
 
 
-def _get_dataset_properties(h5obj, keys):
-    return {k: getattr(h5obj, k) for k in keys}
+LazyInput = Union[h5py.Group, h5py.Dataset, LHDFObject, List[Union[h5py.Group, h5py.Dataset, LHDFObject]]]
 
 
-def lazy(h5obj: Union[List[Union[h5py.Group, h5py.Dataset, LHDFObject]],
-                      h5py.Dataset, h5py.Group, LHDFObject]) -> Union[None, LDataset, LGroup]:
+def lazy(h5obj: LazyInput) -> Optional[Union[List[LazyObject], LazyObject]]:
     """Make a lazy object from a h5py object"""
-    if isinstance(h5obj, LHDFObject):
+    if isinstance(h5obj, (LDataset, LGroup)):
         return h5obj
     if isinstance(h5obj, list):
         return [lazy(i) for i in h5obj]
     if h5obj is None:
         return None
     if isinstance(h5obj, h5py.Group):
         return LGroup(h5obj)
     elif isinstance(h5obj, h5py.Dataset):
         return LDataset(h5obj)
-    elif isinstance(h5obj, (tuple, list)):
-        # expecting h5obj=(filename, obj_name)
-        with h5py.File(h5obj[0]) as h5:
-            return lazy(h5[h5obj[1]])
+    # elif isinstance(h5obj, (tuple, list)):
+    #     # expecting h5obj=(filename, obj_name)
+    #     with h5py.File(h5obj[0]) as h5:
+    #         return lazy(h5[h5obj[1]])
     raise TypeError(f'Cannot make {type(h5obj)} lazy')
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/mongo.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import h5py
-import numpy as np
 import os
 import pathlib
-import pymongo
 import warnings
 from datetime import datetime
 from typing import List, Dict, Any, Union, Generator
 
-from . import lazy
-from .template import HDF5DBInterface
+import h5py
+import numpy as np
+import pymongo
+
+from .interface import HDF5DBInterface
 from .. import protected_attributes
+from ..wrapper import lazy
 
 
 def get_file_creation_time(filename: Union[str, pathlib.Path], tz=None) -> datetime:
     """Return the creation time of the passed filename
 
     Parameters
     ----------
@@ -61,15 +62,17 @@
     if value is None:
         return None
     if isinstance(value, np.ndarray):
         return value.tolist()
     try:
         if isinstance(value, np.integer):
             return int(value)
-        return float(value)
+        if isinstance(value, np.floating):
+            return float(value)
+        return str(value)
     except Exception as e:
         warnings.warn(f'Could not determine/convert {value}. Try to continue with type {type(value)} of {value}. '
                       f'Original error: {e}')
     return str(value)
 
 
 def _generate_dataset_document(
@@ -266,24 +269,25 @@
     if recursive:
         include_dataset = True
 
     if include_dataset or recursive:
         for h5obj in grp.values():
             if isinstance(h5obj, h5py.Dataset):
                 if include_dataset:
-                    h5obj.mongo.insert(axis=None,
-                                       collection=collection,
-                                       update=update,
-                                       ignore_attrs=ignore_attrs)
+                    _insert_dataset(h5obj, collection=collection,
+                                    axis=None,
+                                    update=update,
+                                    ignore_attrs=ignore_attrs)
             else:
                 if recursive:
-                    h5obj.mongo.insert(collection, recursive=recursive,
-                                       update=update,
-                                       include_dataset=include_dataset,
-                                       ignore_attrs=ignore_attrs)
+                    _insert_group(h5obj, collection=collection, recursive=recursive,
+                                  update=update,
+                                  include_dataset=include_dataset,
+                                  ignore_attrs=ignore_attrs)
+
     return collection
 
 
 class MongoDBLazyDataset(lazy.LDataset):
 
     def __init__(self, obj: h5py.Dataset, mongo_doc):
         super().__init__(obj)
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/database/template.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 import abc
-import h5py
 from typing import Generator
 
-from .lazy import LHDFObject
+import h5py
+
+from ..wrapper.lazy import LHDFObject
+
+
+class NonInsertableDatabaseInterface:
+    """A database interface that does not allow inserting datasets"""
+
+    def insert_dataset(self, *args, **kwargs):
+        """Insert a dataset. This is not possible for an HDF5 file."""
+        raise NotImplementedError('By using an HDF5 file as a database, you cannot insert datasets')
+
+    def insert_group(self, *args, **kwargs):
+        """Insert a group. This is not possible for an HDF5 file."""
+        raise NotImplementedError('By using an HDF5 file as a database, you cannot insert groups')
 
 
 class HDF5DBInterface(abc.ABC):
     """Abstract HDF5 Database interface.
 
     The init method is not abstract. Each database implementation
     needs to implement it on its own.
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/identifiers.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/identifiers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
 import appdirs
 import pathlib
 import re
 import requests
-import warnings
 from typing import Union, List
 
 
 class ObjectIdentifier(abc.ABC):
     """Abstract base class for identifiers"""
 
     wikidata: str = None  # url to wikidata page if exists
@@ -33,31 +32,34 @@
     def check_pattern(cls, identifier: str) -> bool:
         """Check if it fulfills the pattern"""
         if cls.pattern is None:
             raise NotImplementedError('Pattern not implemented')
         return re.match(cls.pattern, identifier) is not None
 
 
+KNOWN_ORCID_FILENAME = pathlib.Path(appdirs.user_data_dir('h5rdmtoolbox')) / 'known_and_validated_orcids.txt'
+
+
 class ORCID(ObjectIdentifier):
     """https://www.wikidata.org/wiki/Property:P496"""
-    known_orcid_filename = pathlib.Path(appdirs.user_data_dir('h5rdmtoolbox')) / 'known_and_validated_orcids.txt'
     pattern = r'^(https:\/\/orcid\.org\/)?(\d{4}-){3}\d{3}(\d|X)$'
 
     def __init__(self, orcid: str):
         if not orcid.startswith('https://orcid.org/'):
             orcid = f'https://orcid.org/{orcid}'
         self.id = str(orcid)
 
-    def get_validated_orcids(self) -> List[str]:
+    @classmethod
+    def get_existing_orcids(cls) -> List[str]:
         """Return list of validated ORCIDs. They have been saved
         in a file when they were validated the first time."""
 
-        if not self.known_orcid_filename.exists():
+        if not KNOWN_ORCID_FILENAME.exists():
             return []
-        with open(self.known_orcid_filename) as f:
+        with open(KNOWN_ORCID_FILENAME) as f:
             return [l.strip() for l in f.readlines()]
 
     def check_checksum(self) -> bool:
         """Calculate the check digit for the base digits provided based on
         https://support.orcid.org/hc/en-us/articles/360006897674-Structure-of-the-ORCID-Identifier"""
 
         # get base digits:
@@ -84,27 +86,27 @@
 
     def exists(self,
                timeout: Union[int, None] = None,
                raise_error: bool = True) -> bool:
         """Check if it can be found online or in known ORCIDs file"""
         # small hack: we saved already validated orcids in a file,
         # so we don't have to check them again
-        if str(self) in self.get_validated_orcids():
+        if str(self) in self.get_existing_orcids():
             return True
         headers = {'Accept': 'application/vnd.orcid+json'}
         try:
             response = requests.get(self, headers=headers, timeout=timeout)  # wait 1 sec
         except requests.exceptions.ConnectionError as e:
             if raise_error:
                 raise Exception(e) from e
             return False
         if response.status_code == 200:  # 200=OK
-            orcids = self.get_validated_orcids()
+            orcids = self.get_existing_orcids()
             orcids.append(str(self))
-            with open(self.known_orcid_filename, 'w') as f:
+            with open(KNOWN_ORCID_FILENAME, 'w') as f:
                 f.write('\n'.join(orcids))
             return True
         return False
 
     def __str__(self):
         return self.id
 
@@ -211,23 +213,24 @@
 
     def __str__(self):
         if not self.id.startswith('https://ror.org/'):
             return f'https://ror.org/{self.id}'
         return str(self.id)
 
     def check_checksum(self) -> bool:
-        warnings.warn('Checksum not implemented yet')
-        return True
+        """Checking the checksum not implemented yet"""
+        raise NotImplementedError('Checksum not implemented yet')
 
     def _repr_html_(self):
         return f'<a href="{self.id}"><img alt="ROR logo" ' \
                f'src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg" ' \
                f'width="16" height="16" />{self.id}</a>'
 
     def validate(self):
+        """Check if it fulfills the pattern"""
         return self.check_pattern(self.id)
 
 
 class URN(ObjectIdentifier):
     pattern = r'^urn:[a-z0-9][a-z0-9-]{0,31}:[a-z0-9()+,\-.:=@;$_!*\'%/?#]+$'
 
     def __init__(self, urn: str):
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/plotting.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/plotting.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/interface.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 import abc
-from typing import List, Callable
+import pathlib
+from typing import Callable, Iterable, Union
 
 
 class RepositoryInterface(abc.ABC):
     """Abstract base class for repository interfaces."""
 
     # __init__  must be implemented in the child class
     def __init__(self):
         raise RuntimeError('Not implemented.')
 
     @abc.abstractmethod
     def exists(self):
         """Check if the repository exists."""
 
-    @property
     @abc.abstractmethod
-    def metadata(self):
+    def get_metadata(self):
         """Get the metadata of the repository."""
 
-    @metadata.setter
     @abc.abstractmethod
-    def metadata(self, value):
+    def set_metadata(self, value):
         """Set the metadata of the repository."""
 
     @abc.abstractmethod
     def download_file(self, filename):
         """Download a specific file from the repository."""
 
     @abc.abstractmethod
     def download_files(self):
         """Download all files from the repository."""
 
     @abc.abstractmethod
-    def get_filenames(self) -> List[str]:
+    def get_filenames(self) -> Iterable:
         """Get a list of all filenames."""
 
     @abc.abstractmethod
     def upload_file(self, filename, overwrite: bool = False):
         """Upload a file to the repository."""
 
-    def upload_hdf_file(self, filename, metamapper: Callable, overwrite: bool = False):
+    def upload_hdf_file(self,
+                        filename,
+                        metamapper: Callable[[Union[str, pathlib.Path]], pathlib.Path],
+                        overwrite: bool = False):
         """Upload an HDF5 file. Additionally a metadata file will be extracted from the
-        HDF5 file using the metamapper function and is uploaded as well."""
-        meta_data_file = metamapper(filename)
+        HDF5 file using the metamapper function and is uploaded as well.
+        The metamapper function takes a filename, extracts the metadata and stores it in
+        a file. The filename of it is returned by the function. It is automatically uploaded
+        with the HDF5 file."""
+        if metamapper:
+            meta_data_file = metamapper(filename)
         self.upload_file(filename=filename, overwrite=overwrite)
-        self.upload_file(filename=meta_data_file, overwrite=overwrite)
+        if metamapper:
+            self.upload_file(filename=meta_data_file, overwrite=overwrite)
 
     @abc.abstractmethod
     def get_doi(self):
         """Get the DOI of the repository."""
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/metadata.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 This code implements the zenodo API as described in https://developers.zenodo.org/#rest-api
 
 As this is done also by the above mentioned library some code might look identical, however, it is just
 the implementation of the API.
 
 Also note, that the above mentioned library cannot be used as not all required fields are implemented.
 """
-
+import pydantic
 import re
 from datetime import datetime
-from pydantic import BaseModel, field_validator, Field
-from typing import Optional, Union, List
+from pydantic import BaseModel, field_validator, Field, ConfigDict
+from typing import Optional, Union, List, Dict
 from typing_extensions import Literal
 
 
 def verify_version(version: str) -> str:
     """Verify that version is a valid as defined in https://semver.org/"""
     re_pattern = r'^(?P<major>0|[1-9]\d*)\.(?P<minor>0|[1-9]\d*)\.(?P<patch>0|[1-9]\d*)(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+(?P<buildmetadata>[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$'
     return re.match(pattern=re_pattern, string=version) is not None
@@ -30,15 +30,16 @@
 
     name: str
     affiliation: Optional[str] = Field(default=None)
     orcid: Optional[str] = Field(default=None)
     gnd: Optional[str] = Field(default=None)
 
     @field_validator('name')
-    def validate_name(cls, value):
+    @classmethod
+    def _validate_name(cls, value):
         if "," not in value:
             raise ValueError(f'The creator name should be formatted "family name, given names" but is {value}')
         return value
 
 
 ContributorType = Literal[
     "ContactPerson",
@@ -110,32 +111,93 @@
     "plot",
     "drawing",
     "diagram",
     "photo",
     "other"
 ]
 
+Datetypes = Literal[
+    "created",
+    "accepted",
+    "available",
+    "collected",
+    "copyrighted",
+    "created",
+    "issued",
+    "other",
+    "submitted",
+    "updated",
+    "valid",
+    "withdrawn",
+    'Created',
+    'Accepted',
+    'Available',
+    'Collected',
+    'Copyrighted',
+    'Created',
+    'Issued',
+    'Other',
+    'Submitted',
+    'Updated',
+    'Valid',
+    'Withdrawn'
+]
+
+
+class DateType(BaseModel):
+    """Datetype as used in Zenodo"""
+    # date: Union[str, datetime]
+    type: Datetypes
+    description: Optional[str] = None
+
+    # @field_validator('date')
+    # @classmethod
+    # def validate_date(cls, value):
+    #     """Format Date or Date/Date where Date is YYYY or YYYY-MM or YYYY-MM-DD"""
+    #     if isinstance(value, datetime):
+    #         return value.strftime('%Y-%m-%d')
+    #
+    #     if value is None or value.lower() in ('today', 'now', 'none'):
+    #         return datetime.today().strftime('%Y-%m-%d')
+    #
+    #     formats = ['%Y-%m-%d', '%Y-%m', '%Y']
+    #
+    #     def _check_date(value, format):
+    #         try:
+    #             datetime.strptime(value, format)
+    #             return True
+    #         except ValueError:
+    #             return False
+    #
+    #     if not any([_check_date(value, format) for format in formats]):
+    #         raise ValueError(f'invalid date format: {value}')
+    #     return value
+
 
 class Metadata(BaseModel):
     """Zeno Metadata class according to Zenodo spec: https://developers.zenodo.org/."""
-    version: str
-    title: str
+    version: Optional[str]
+    title: Optional[str]
     description: str
     creators: List[Creator]
     upload_type: UploadType
+    additional_description: Optional[Dict] = None
+    dates: List[DateType] = pydantic.Field(default_factory=list)
+    publication_date: Optional[Union[str, datetime]] = Field(default_factory=datetime.today)
     publication_type: Optional[PublicationType] = None  # if upload_type == publication
     image_type: Optional[ImageType] = None  # if upload_type == image
-    keywords: List[str]
+    keywords: List[str] = None
     notes: Optional[str] = None
-    contributors: Optional[List[Contributor]] = []
+    contributors: Optional[List[Contributor]] = pydantic.Field(default_factory=list)
     access_right: Optional[Literal["open", "closed", "restricted", "embargoed"]] = "open"
-    publication_date: Optional[Union[str, datetime]] = Field(default_factory=datetime.today)
     license: Optional[str] = "cc-by-4.0"
     embargo_date: Optional[Union[str, datetime]] = None
 
+    model_config = ConfigDict(extra='forbid')
+
     @field_validator('publication_date')
     @classmethod
     def validate_publication_date(cls, value):
         """See https://developers.zenodo.org/#representation"""
         if isinstance(value, datetime):
             return value.strftime('%Y-%m-%d')
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/repository/zenodo/utils.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/tutorial.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/tutorial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Tutorial module providing easy access to particular data.
 """
-import numpy as np
 import os
 import pathlib
-import xarray as xr
 from typing import List
 
+import numpy as np
+import xarray as xr
+from rdflib import FOAF
+
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox.convention.standard_names.table import StandardNameTable
 from .utils import generate_temporary_directory
 from .wrapper.core import File
 
 __this_dir__ = pathlib.Path(__file__).parent
 testdir = __this_dir__ / '../tests/data'
@@ -199,15 +201,15 @@
             ifolder = np.random.randint(0, len(_folders))
             # create folder if not exist:
             os.makedirs(folders[ifolder], exist_ok=True)
 
             filename = pathlib.Path(folders[ifolder]) / f'repofile_{fid:05d}.hdf'
             with File(filename, 'w') as h5:
                 h5.attrs['contact_person'] = contact_persons[np.random.randint(4)]
-                h5.iri['contact_person'].name = 'http://www.w3.org/ns/prov#Person'
+                h5.rdf['contact_person'].name = 'http://www.w3.org/ns/prov#Person'
 
                 if fid % 2:
                     __ftype__ = db_file_type[0]
                 else:
                     __ftype__ = db_file_type[1]
                 h5.attrs['__db_file_type__'] = __ftype__
 
@@ -239,15 +241,15 @@
                                       attach_scales=(None, None, None, 'x', None))
                     g = h5.create_group('timeAverages',
                                         attrs=dict(long_name='time averaged data'))
                     g.create_dataset('u', attrs={'units': 'm/s', 'long_name': 'mean u-component'},
                                      shape=(zplanes, 64, 86, 2))
                     g.create_dataset('v', attrs={'units': 'm/s', 'long_name': 'mean v-component'},
                                      shape=(zplanes, 64, 86, 2))
-                    g.iri['units'].name = 'http://qudt.org/schema/qudt/Unit'
+                    g.rdf['units'].name = 'http://qudt.org/schema/qudt/Unit'
 
     @staticmethod
     def generate_test_files(n_files: int = 5) -> List[pathlib.Path]:
         """Generate a nested filestructure of hdf files and return list of the filenames"""
         tocdir = generate_temporary_directory('test_repo')
         Database.build_test_repo(tocdir, n_files=n_files)
         return sorted(tocdir.rglob('*.hdf'))
@@ -317,20 +319,23 @@
                             attach_scales=scales)
         if z is not None:
             self.create_dataset('w', data=w,
                                 attrs=dict(units='m/s', standard_name='z_velocity'),
                                 attach_scales=scales)
 
 
-def generate_fluid_hdf_file() -> pathlib.Path:
-    """Generate a hdf file with a velocity and pressure dataset"""
+def generate_sample_file() -> pathlib.Path:
+    """Generate a sample hdf file with a velocity and pressure dataset"""
     with h5tbx.File() as h5:
-        h5.write_iso_timestamp(name='timestamp', dt=None)  # writes the current date time in iso format to the attribute
+        h5.attrs.write_iso_timestamp(name='timestamp', dt=None)  # writes the current date time in iso format to the attribute
         h5.attrs['project'] = 'tutorial'
-        h5.attrs['contact'] = {'name': 'John Doe', 'surname': 'Doe'}
+        contact_grp = h5.create_group('contact')
+        contact_grp.attrs['name', FOAF.firstName] = 'John'
+        contact_grp.attrs['surname', FOAF.lastName] = 'Doe'
+
         h5.attrs['check_value'] = 0
         h5.create_dataset('pressure1', data=np.random.random(size=10) * 800,
                           attrs=dict(units='Pa', standard_name='pressure',
                                      check_value=-140.3))
         h5.create_dataset('velocity', data=[1, 2, -1],
                           attrs=dict(units='m/s', standard_name='velocity',
                                      check_value=14.2))
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/utils.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,44 @@
 """utilities of the h5rdmtoolbox"""
-import appdirs
 import datetime
 import h5py
 import hashlib
 import json
 import logging
 import numpy as np
 import os
 import pathlib
 import pint
 import re
 import requests
 import warnings
 from h5py import File
-from logging.handlers import RotatingFileHandler
+from pydantic import HttpUrl, validate_call
+from rdflib.plugins.shared.jsonld.context import Context
 from re import sub as re_sub
-from typing import Dict, Union, Callable, List, Tuple
+from typing import Dict
+from typing import Union, Callable, List, Tuple
 
-from . import _user, get_config, get_ureg, consts
+from . import _user, get_config, get_ureg
 from ._version import __version__
+from .wrapper import rdf
 
+logger = logging.getLogger('h5rdmtoolbox')
 DEFAULT_LOGGING_LEVEL = logging.INFO
 
 
-class ToolboxLogger(logging.Logger):
-    """Wrapper class for logging.Logger to add a setLevel method"""
-
-    def __init__(self, name, level=logging.NOTSET, directory=None):
-        super().__init__(name, level)
-        self._directory = directory
-
-    def setLevel(self, level):
-        """change the log level which displays on the console"""
-        old_level = self.handlers[1].level
-        self.handlers[1].setLevel(level)
-
-
-def create_tbx_logger(name, logdir=None) -> ToolboxLogger:
-    """Create logger based on name"""
-    if logdir is None:
-        _logdir = pathlib.Path(appdirs.user_log_dir('h5rdmtoolbox'))
-    else:
-        _logdir = pathlib.Path(logdir)
-
-    _logdir.mkdir(parents=True, exist_ok=True)
-
-    _logger = ToolboxLogger(logging.getLogger(name), directory=_logdir)
-
-    _formatter = logging.Formatter(
-        '%(asctime)s,%(msecs)d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
-        datefmt='%Y-%m-%d_%H:%M:%S')
-
-    _file_handler = RotatingFileHandler(_logdir / f'{name}.log')
-    _file_handler.setLevel(logging.DEBUG)  # log everything to file!
-    _file_handler.setFormatter(_formatter)
-
-    _stream_handler = logging.StreamHandler()
-    _stream_handler.setLevel(DEFAULT_LOGGING_LEVEL)
-    _stream_handler.setFormatter(_formatter)
-
-    _logger.addHandler(_file_handler)
-    _logger.addHandler(_stream_handler)
-
-    return _logger
+def get_filesize(filename: Union[str, pathlib.Path]) -> int:
+    """Get the size of a file in bytes"""
+    return os.path.getsize(filename) * get_ureg().byte
 
 
-def get_filesize(path: Union[str, pathlib.Path]) -> int:
-    """Get the size of a file in bytes"""
-    return os.path.getsize(path) * get_ureg().byte
+def get_checksum(filename: Union[str, pathlib.Path], hash_func: Callable = hashlib.md5) -> str:
+    """Get the checksum of a file. Default hash function is hashlib.md5"""
+    with open(str(filename), 'rb') as file:
+        return hash_func(file.read()).hexdigest()
 
 
 def has_internet_connection(timeout: int = 5) -> bool:
     """Figure out whether there's an internet connection"""
     try:
         requests.get('https://git.scc.kit.edu', timeout=timeout)
         return True
@@ -88,15 +55,15 @@
 
         # Calculate the hash of the downloaded content
         calculated_hash = hashlib.sha256(content).hexdigest()
         if known_hash:
             if not calculated_hash == known_hash:
                 raise ValueError('File does not match the expected has')
         else:
-            warnings.warn('No has given!')
+            warnings.warn('No hash given! This is recommended when downloading files from the web.', UserWarning)
 
         # Save the content to a file
         fname = generate_temporary_filename()
         with open(fname, "wb") as f:
             f.write(content)
 
         return fname
@@ -186,16 +153,20 @@
     tmp_filename: pathlib.Path
         The generated temporary filename
     """
     _filename = _user.UserDir['tmp'] / f"{prefix}{next(_user._filecounter)}{suffix}"
     while _filename.exists():
         _filename = _user.UserDir['tmp'] / f"{prefix}{next(_user._filecounter)}{suffix}"
     if touch:
-        with h5py.File(_filename, 'w'):
-            pass
+        if _filename.suffix in ('.h5', '.hdf', '.hdf5'):
+            with h5py.File(_filename, 'w'):
+                pass
+        else:
+            with open(_filename, 'w'):
+                pass
     return _filename
 
 
 def generate_temporary_directory(prefix='tmp') -> pathlib.Path:
     """generates a temporary directory in user tmp file directory
 
     Parameters
@@ -211,14 +182,30 @@
     _dir = _user.UserDir['tmp'] / f"{prefix}{next(_user._dircounter)}"
     while _dir.exists():
         _dir = _user.UserDir['tmp'] / f"{prefix}{next(_user._dircounter)}"
     _dir.mkdir(parents=True)
     return _dir
 
 
+def create_h5tbx_version_grp(root: h5py.Group) -> h5py.Group:
+    """Creates a group in an HDF5 file with the h5rdmtoolbox version as an attribute"""
+    logger.debug('Creating group "h5rdmtoolbox" with attribute "__h5rdmtoolbox_version__" in file')
+    version_group = root.create_group('h5rdmtoolbox')
+    # g.rdf.object = 'https://schema.org/SoftwareSourceCode'
+    version_group.attrs['__h5rdmtoolbox_version__'] = __version__
+    # version_group.attrs['name'] = "h5rdmtoolbox"
+    version_group.attrs['code_repository'] = "https://github.com/matthiasprobst/h5RDMtoolbox"
+    version_group.attrs[rdf.RDF_PREDICATE_ATTR_NAME] = json.dumps(
+        {'code_repository': 'https://schema.org/codeRepository',
+         '__h5rdmtoolbox_version__': 'https://schema.org/softwareVersion'}
+    )
+    version_group.attrs[rdf.RDF_TYPE_ATTR_NAME] = 'https://schema.org/SoftwareSourceCode'
+    return version_group
+
+
 def touch_tmp_hdf5_file(touch=True, attrs=None) -> pathlib.Path:
     """
     Generates a file path in directory h5rdmtoolbox/.tmp
     with filename dsXXXX.hdf where XXXX is more or less a
     random number leading to a unique filename in the tmp
     location. The file is created and the file path is returned
 
@@ -229,17 +216,16 @@
     touch : bool, optional=True
         touches the file
 
     """
     hdf_filepath = generate_temporary_filename(suffix='.hdf')
     if touch:
         with File(hdf_filepath, "w") as h5touch:
-            h5touch.attrs['__h5rdmtoolbox_version__'] = __version__
-            h5touch.attrs[
-                consts.IRI_PREDICATE_ATTR_NAME] = json.dumps({'__h5rdmtoolbox_version__': consts.VERSION_IRI})
+            if get_config('auto_create_h5tbx_version'):
+                create_h5tbx_version_grp(h5touch)
             if attrs is not None:
                 for ak, av in attrs.items():
                     create_special_attribute(h5touch.attrs, ak, av)
     return hdf_filepath
 
 
 def try_making_serializable(d: Dict) -> Dict:
@@ -291,15 +277,15 @@
         _value = value
 
     # parse name as well, it could be an identifier (URI or IRI):
     if hasattr(name, 'fragment'):
         fragment = name.fragment
         if not fragment:
             raise ValueError(f'Name {name} has no fragment')
-        from h5rdmtoolbox.wrapper.iri import set_predicate
+        from h5rdmtoolbox.wrapper.rdf import set_predicate
         set_predicate(h5obj, fragment, name)
         name = fragment
 
     try:
         h5obj.create(name, data=_value)
     except TypeError:
         try:
@@ -331,15 +317,14 @@
     if isinstance(value, (int, float, bool)):
         return value
     if isinstance(value, (h5py.Dataset, h5py.Group)):
         return value.name
     try:
         return str(value)  # try parsing to string
     except TypeError:
-        print(type(value))
         raise TypeError(f"Cannot parse type {type(value)} to string")
 
 
 OBJ_FLT_DICT = {'group': h5py.Group,
                 'groups': h5py.Group,
                 'dataset': h5py.Dataset,
                 'datasets': h5py.Dataset,
@@ -533,7 +518,36 @@
                         'type': param_type,
                         'default': param_default,
                         'description': desc.strip(),
                     }
                     rkw.append(current_ret_param)
 
         return abstract, kw, rkw, notes_lines
+
+
+@validate_call
+def download_context(url_source: Union[HttpUrl, List[HttpUrl]], force_download: bool = False) -> Context:
+    """Download a context file from one URL or list of URLs
+    Will check if a context file is already downloaded and use that one.
+
+    Examples
+    --------
+    >>> from h5rdmtoolbox.utils import download_context
+    >>> context = download_context('https://raw.githubusercontent.com/codemeta/codemeta/2.0/codemeta.jsonld')
+    """
+    if not isinstance(url_source, list):
+        url_source = [url_source]
+
+    filenames = []
+    for url in url_source:
+        _url = str(url)
+        _fname = _url.rsplit('/', 1)[-1]
+        context_file = _user.UserDir['cache'] / _fname
+        if not context_file.exists() or force_download:
+            logger.debug(f'Downloading context file from {_url} to {context_file}')
+            try:
+                with open(context_file, 'wb') as f:
+                    f.write(requests.get(_url).content)
+            except requests.RequestException:
+                raise RuntimeError(f'Failed to download context file from {_url}')
+        filenames.append(str(context_file))
+    return Context(filenames)
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/core.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,78 @@
 """Core wrapper module containing basic wrapper implementation of File, Dataset and Group
 """
-import datetime
+
 import h5py
+import json
+import logging
 import numpy as np
 import os
 import pathlib
 # noinspection PyUnresolvedReferences
 import pint
 import shutil
 import warnings
 import xarray as xr
 from collections.abc import Iterable
 from datetime import datetime, timezone
 from h5py._hl.base import phil, with_phil
 from h5py._objects import ObjectID
 from pathlib import Path
-from typing import List, Dict, Union, Tuple, Callable
+from typing import List, Dict, Union, Tuple, Optional
 
-from h5rdmtoolbox.database import ObjDB
-from . import logger, iri
 # noinspection PyUnresolvedReferences
-from . import xr2hdf
+from . import xr2hdf, rdf
 from .ds_decoder import dataset_value_decoder
 from .h5attr import H5_DIM_ATTRS, pop_hdf_attributes, WrapperAttributeManager
 from .h5utils import _is_not_valid_natural_name, get_rootparent
 from .. import _repr, get_config, convention, utils, consts, protected_attributes
 from .. import get_ureg
+from .. import protocols
 from .._repr import H5Repr, H5PY_SPECIAL_ATTRIBUTES
-from .._version import __version__
 from ..convention.consts import DefaultValue
 
+logger = logging.getLogger('h5rdmtoolbox')
+
 MODIFIABLE_PROPERTIES_OF_A_DATASET = ('name', 'chunks', 'compression', 'compression_opts',
                                       'dtype', 'maxshape')
 H5KWARGS = ('driver', 'libver', 'userblock_size', 'swmr',
             'rdcc_nslots', 'rdcc_nbytes', 'rdcc_w0', 'track_order',
             'fs_strategy', 'fs_persist', 'fs_threshold', 'fs_page_size',
             'page_buf_size', 'min_meta_keep', 'min_raw_keep', 'locking',
             'alignment_threshold', 'alignment_interval', 'meta_block_size')
 
 
+def assert_filename_existence(filename: pathlib.Path) -> pathlib.Path:
+    """Raises an error if the filename does not exist. Otherwise, the filename is returned.
+
+    Parameters
+    ----------
+    filename : pathlib.Path
+        Filename to check.
+
+    Returns
+    -------
+    pathlib.Path
+        The filename if it exists.
+
+    Raises
+    ------
+    FileNotFoundError
+        If the filename does not exist.
+    """
+    if not filename.exists():
+        raise FileNotFoundError('Filename does not exist. It might be moved or deleted!')
+    return filename
+
+
 def convert_strings_to_datetimes(array):
-    if np.issubdtype(array.dtype, np.str_):
-        return np.array([datetime.fromisoformat(date_str) for date_str in array.flat]).reshape(array.shape)
-    else:
-        return np.array([convert_strings_to_datetimes(subarray) for subarray in array])
+    assert np.issubdtype(array.dtype, np.str_), 'Unexpected array type'
+    return np.array([datetime.fromisoformat(date_str) for date_str in array.flat]).reshape(array.shape)
+    # else:
+    #     return np.array([convert_strings_to_datetimes(subarray) for subarray in array])
 
 
 def _pop_standard_attributes(kwargs, cache_entry) -> Tuple[Dict, Dict]:
     """Pop all standard attributes from kwargs and return them in a dict."""
     std_attrs = {}
     for k in cache_entry.keys():
         if k in kwargs:
@@ -59,40 +84,42 @@
     """Lower"""
 
     def __new__(cls, string):
         instance = super().__new__(cls, string.lower())
         return instance
 
 
-def lower(string: str) -> Lower:
+def lower(string: str) -> str:
     """return object Lower(string). Used when a dataset
     is called, but the upper/lower case should be irrelevant."""
     return Lower(string)
 
 
 def process_attributes(cls,
                        meth_name: str,
                        attrs: Dict,
                        kwargs: Dict,
                        name: str,
-                       existing_attrs: Tuple = None) -> Tuple[Dict, Dict, Dict]:
+                       existing_attrs: Optional[Tuple] = None) -> Tuple[Dict, Dict, Dict]:
     """Process attributes and kwargs for methods "create_dataset", "create_group" and "File.__init__" method.
 
     Parameters
     ----------
     cls : type
         Class of the method.
     meth_name : str
         Name of the method.
     attrs : Dict
         Attributes of the method.
     kwargs : Dict
         Keyword arguments of the method.
     name : str
         Name of the dataset or group to be created.
+    existing_attrs: Optional[Tuple]
+        Tuple of existing attributes. If an attribute is in this tuple, it is not considered as a standard attribute.
     """
     if existing_attrs is None:
         existing_attrs = list()
 
     curr_cv = convention.get_current_convention()
 
     # go through list of registered standard attributes, and check whether they are in kwargs:
@@ -168,103 +195,30 @@
     #                 f'You passed the standard attribute "{skey}" as a standard argument and it is '
     #                 f'also in the "attrs" argument. This is not allowed!')
 
     attrs.update(skwargs)
     return attrs, skwargs, kwargs
 
 
-class Core:
-    """Class inherited by File, Dataset and Group containing common methods."""
-
-    def __delattr__(self, item):
-        if self.standard_attributes.get(item, None):
-            if get_config('allow_deleting_standard_attributes'):
-                del self.attrs[item]
-                return
-            raise ValueError('Deleting standard attributes is not allowed based on the current configuration! '
-                             'You may change this by calling '
-                             '"h5tbx.set_config(allow_deleting_standard_attributes=True)".')
-        if item in self and get_config('natural_naming'):
-            del self[item]
+def _delattr(obj: protocols.H5TbxHLObject, item: str):
+    if obj.standard_attributes.get(item, None):
+        if get_config('allow_deleting_standard_attributes'):
+            del obj.attrs[item]
             return
-        super().__delattr__(item)
-
-    @property
-    def hdf_filename(self) -> pathlib.Path:
-        """The filename of the file, even if the HDF5 file is closed. Note, that
-        is not checked, if the file still exists!"""
-        return self._hdf_filename
-
-    @property
-    def convention(self):
-        """Return the convention currently enabled."""
-        return convention.get_current_convention()
-
-    @property
-    def standard_attributes(self) -> Dict:
-        """Return the standard attributes of the class."""
-        return self.convention.properties.get(self.__class__, {})
-
-    @property
-    def iri(self):
-        """Return IRI Manager"""
-        return iri.IRIManager(self.attrs)
-
-    @iri.setter
-    def iri(self, value):
-        """Sets an IRI to the group or dataset"""
-        iri.IRIManager(self.attrs).set_subject(value)
-
+        raise ValueError('Deleting standard attributes is not allowed based on the current configuration! '
+                         'You may change this by calling '
+                         '"h5tbx.set_config(allow_deleting_standard_attributes=True)".')
+    if item in obj and get_config('natural_naming'):
+        del obj[item]
+        return
+    del obj[item]
+    # super().__delattr__(item)
 
-class SpecialAttributeWriter:
-    """Accessor class, which provides methods to write special attributes to a dataset or group."""
-
-    def write_uuid(self, uuid: str = None, name='uuid', overwrite: bool = False) -> str:
-        """Write a uuid to the attribute of the object.
-
-        Parameters
-        ----------
-        uuid : str=None
-            The uuid to write. If None, a new uuid is generated.
-        name : str='uuid'
-            The name of the attribute. Default is "uuid".
-
-        Returns
-        -------
-        str
-            The uuid as string.
-        """
-        if name in self.attrs and not overwrite:
-            raise ValueError(f'The attribute "{name}" cannot be written. It already exists and '
-                             '"overwrite" is set to False')
-        if uuid is None:
-            from uuid import uuid4
-            uuid = uuid4()
-        suuid = str(uuid)
-        self.attrs[name] = suuid
-        return suuid
 
-    def write_iso_timestamp(self, name='timestamp', dt: datetime = None, overwrite: bool = False, **kwargs):
-        """Write the iso timestamp to the attribute of the object.
-
-        Parameters
-        --
-        """
-        if name in self.attrs and not overwrite:
-            raise ValueError(f'The attribute "{name}" cannot be written. It already exists and '
-                             '"overwrite" is set to False')
-        if dt is None:
-            dt = datetime.now()
-        else:
-            if not isinstance(dt, datetime):
-                raise TypeError(f'Invalid type for parameter "dt". Expected type datetime but got "{type(dt)}"')
-        self.attrs[name] = dt.isoformat(**kwargs)
-
-
-class Group(h5py.Group, SpecialAttributeWriter, Core):
+class Group(h5py.Group):
     """Inherited Group of the package h5py. Adds some useful methods on top
     of the underlying *h5py* package.
 
 
     .. note:: All features from h5py packages are preserved.
 
 
@@ -275,21 +229,26 @@
     * get_groups() - returns a list of groups in the group
     * get_tree_structure() - returns a tree structure of the group
     * create_string_dataset() - creates a dataset with string datatype
     * create_time_dataset() - creates a dataset with time datatype
 
     The following properties are added (or overwritten):
     * attrs - returns the *h5tbx* attribute manager, which is a subclass of the *h5py* attribute manager
-    * iri - returns the IRI Manager
+    * rdf - returns the RDF Manager
     * rootparent - returns the root group instance
     * basename - returns the basename of the group
     """
     hdfrepr = H5Repr()
 
     @property
+    def hdf_filename(self) -> pathlib.Path:
+        """The filename of the file, even if the HDF5 file is closed."""
+        return assert_filename_existence(self._hdf_filename)
+
+    @property
     def attrs(self):
         """Calls the wrapper attribute manager"""
         with phil:
             return WrapperAttributeManager(self)
 
     @property
     def rootparent(self):
@@ -306,56 +265,61 @@
     def get_datasets(self, pattern: str = '.*', recursive: bool = False) -> List[h5py.Dataset]:
         """Return list of datasets in the current group.
         If pattern is None, all groups are returned.
         If pattern is not None a regrex-match is performed
         on the basenames of the datasets."""
         if pattern == '.*' and not recursive:
             return [v for v in self.values() if isinstance(v, h5py.Dataset)]
-        grpDB = ObjDB(self)
-        return grpDB.find({'$name': {'$regex': pattern}}, '$Dataset', recursive=recursive)
+        return [self.rootparent[ds.name] for ds in
+                self.find({'$name': {'$regex': pattern}}, '$Dataset', recursive=recursive)]
 
-    def get_groups(self, pattern: str = '.*', recursive: bool = False) -> List[h5py.Group]:
+    def get_groups(self,
+                   pattern: str = '.*',
+                   recursive: bool = False) -> List[h5py.Group]:
         """Return list of groups in the current group.
         If pattern is None, all groups are returned.
         If pattern is not None a regrex-match is performed
         on the basenames of the groups."""
         if pattern == '.*' and not recursive:
             return [v for v in self.values() if isinstance(v, h5py.Group)]
-        return self.find({'$name': {'$regex': pattern}}, '$Group', recursive=recursive)
+        # if return_lazy:
+        #     return self.find({'$name': {'$regex': pattern}}, '$Group', recursive=recursive)
+        return [self.rootparent[g.name] for g in
+                self.find({'$name': {'$regex': pattern}}, '$Group', recursive=recursive)]
 
     def __init__(self, _id):
         if isinstance(_id, h5py.Group):
             _id = _id.id
         if isinstance(_id, h5py.h5g.GroupID):
             super().__init__(_id)
         else:
             raise ValueError('Could not initialize Group. A h5py.h5f.FileID object must be passed')
         self._hdf_filename = Path(self.file.filename)
 
     def __setitem__(self,
                     name: str,
-                    obj: Union[xr.DataArray, List, Tuple, Dict]) -> "Dataset":
+                    obj: Union[xr.DataArray, List, Tuple, Dict, h5py.ExternalLink]) -> protocols.H5TbxDataset:
         """
         Lazy creating datasets. More difficult than using h5py as mandatory
         parameters must be provided.
 
         Parameters
         ----------
         name: str
             Name of dataset
-        obj: xr.DataArray or Dict or List/Tuple of data and meta data-
-            If obj is not a xr.DataArray, data must be provided using a list or tuple.
-            See examples for possible ways to pass data.
+        obj: xr.DataArray or Dict or List/Tuple of data and metadata.
+                    If obj is not a xr.DataArray, data must be provided using a list or tuple.
+                    See examples for possible ways to pass data.
 
         Returns
         -------
         None
         """
         if isinstance(obj, xr.DataArray):
-            return obj.hdf.to_group(Group(self), name)
+            return Dataset(obj.hdf.to_group(Group(self), name).id)
         if isinstance(obj, (list, tuple)):
             if not isinstance(obj[1], dict):
                 raise TypeError(f'Second item must be type dict but is {type(obj[1])}')
             kwargs = obj[1]
             return self.create_dataset(name, data=obj[0], **kwargs)
         if isinstance(obj, dict):
             return self.create_dataset(name=name, **obj)
@@ -369,27 +333,27 @@
                     break
         ret = super().__getitem__(name)
         if isinstance(ret, h5py.Dataset):
             return self._h5ds(ret.id)
         if isinstance(ret, h5py.Group):
             return self._h5grp(ret.id)
 
-    def __getattr__(self, item):
-        standard_attributes = self.standard_attributes
+    def __getattr__(self, item: str):
+        standard_attributes: Dict = self.standard_attributes
         if standard_attributes:  # are there standard attributes registered?
-            standard_attribute = standard_attributes.get(item, None)
+            standard_attribute: Optional[protocols.StandardAttribute] = standard_attributes.get(item, None)
             if standard_attribute:  # is there an attribute requested with name=item available?
                 return standard_attribute.get(self)
 
         try:
             return super().__getattribute__(item)
         except (RuntimeError, AttributeError) as e:
             if not get_config('natural_naming'):
                 # raise an error if natural naming is NOT enabled
-                raise Exception(e)
+                raise AttributeError(e)
 
         # if item in self.__dict__:
         #     return super().__getattribute__(item)
         try:
             _item = item.replace('_', ' ')
             # item is a Group name?
             if item in [k for k, v in self.items() if isinstance(v, h5py.Group)]:
@@ -413,14 +377,43 @@
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __lt__(self, other):
         return self.name < other.name
 
+    def __delattr__(self, item):
+        _delattr(self, item)
+
+    @property
+    def convention(self):
+        """Return the convention currently enabled."""
+        return convention.get_current_convention()
+
+    @property
+    def standard_attributes(self) -> Dict:
+        """Return the standard attributes of the class."""
+        return self.convention.properties.get(self.__class__, {})
+
+    @property
+    def rdf(self):
+        """Return RDF Manager"""
+        return rdf.RDFManager(self.attrs)
+
+    @property
+    def iri(self):
+        """Deprecated. Use rdf instead."""
+        warnings.warn('Property "iri" is deprecated. Use "rdf" instead.', DeprecationWarning)
+        return rdf.RDFManager(self.attrs)
+
+    # @property
+    # def attrsdef(self) -> definition.DefinitionManager:
+    #     """Return DefinitionManager"""
+    #     return definition.DefinitionManager(self.attrs)
+
     def get_tree_structure(self, recursive=True, ignore_attrs: List[str] = None):
         """Return the tree (attributes, names, shapes) of the group and subgroups"""
         if ignore_attrs is None:
             ignore_attrs = H5PY_SPECIAL_ATTRIBUTES
         tree = dict(self.attrs.items())
         for k, v in self.items():
             if isinstance(v, h5py.Dataset):
@@ -435,15 +428,15 @@
                     tree[k] = v.get_tree_structure(recursive)
         return tree
 
     def create_group(self,
                      name: str,
                      overwrite: bool = None,
                      attrs: Dict = None,
-                     update_attrs: bool = False,
+                     update_attrs: Optional[bool] = False,
                      track_order=None,
                      **kwargs) -> "Group":
         """
         Overwrites parent methods. Additional parameters are "long_name" and "attrs".
         Besides, it does and behaves the same. Differently to dataset creating
         long_name is not mandatory (i.e. will not raise a warning).
 
@@ -455,14 +448,16 @@
             If the group does not already exist, the new group is written and this parameter has no effect.
             If the group exists and ...
             ... overwrite is None, then h5py behaviour is enabled meaning that if a group exists h5py will raise
             ... overwrite is True, then group is deleted and rewritten according to method parameters
             ... overwrite is False, then group creation has no effect. Existing group is returned.
         attrs : dict, optional
             Attributes of the group, default is None which is an empty dict
+        update_attrs: bool, optional
+            If overwrite is False, whether to update the attributes or not. Default is False.
         track_order : bool or None
             Track creation order under this group. Default is None.
         """
         if attrs is None:
             attrs = {}
 
         attrs, skwargs, kwargs = process_attributes(Group, 'create_group', attrs, kwargs, name)
@@ -499,24 +494,24 @@
                 except convention.standard_attributes.errors.StandardAttributeError as e:
                     del self[name]  # undo group creation
                     raise e
         return h5tbxgrp
 
     def create_time_dataset(self,
                             name: str,
-                            data: Union[datetime, List[datetime]],
+                            data: Union[datetime, List],
                             overwrite: bool = False,
                             attrs: Dict = None,
                             **kwargs):
         """Special creation function to create a time vector. Data is stored as a string dataset
         where each datetime is converted to a string with ISO format"""
         if attrs is None:
             attrs = {}
         attrs.update({'ISTIMEDS': 1,
-                      'TIMEFORMAT': 'ISO'})
+                      'TIMEFORMAT': 'ISO'})  # YYYY-MM-DDTHH:MM:SS.ffffff
         if isinstance(data, np.ndarray):
             return self.create_string_dataset(name, data=[t.astype(datetime).isoformat() for t in data],
                                               overwrite=overwrite, attrs=attrs, **kwargs)
         _data = np.asarray(data)
         _orig_shape = _data.shape
         _flat_data = _data.flatten()
         _flat_data = np.asarray([t.isoformat() for t in _flat_data])
@@ -546,19 +541,33 @@
         else:
             raise TypeError(f'Unexpected type for parameter "data": {type(data)}. Expected str or List/Tuple of str')
         dtype = f'S{max(1, n_letter)}'
         if name in self:
             if overwrite is True:
                 del self[name]  # delete existing dataset
             # else let h5py return the error
-        ds = super().create_dataset(name, dtype=dtype, data=data)
+
+        if isinstance(data, str):
+            compression = None
+            compression_opts = None
+        else:
+            compression = kwargs.pop('compression', get_config('hdf_compression'))
+            compression_opts = kwargs.pop('compression_opts', get_config('hdf_compression_opts'))
+
+        make_scale = kwargs.pop('make_scale', False)
+        ds = super().create_dataset(name, dtype=dtype, data=data, **kwargs,
+                                    compression=compression, compression_opts=compression_opts)
+        if make_scale:
+            if isinstance(data, str):
+                ds.make_scale(make_scale)
+            else:
+                ds.make_scale()
 
         for ak, av in attrs.items():
             ds.attrs[ak] = av
-        # TODO: H5StingDataset
         return self._h5ds(ds.id)
 
     def create_dataset(self,
                        name,
                        shape=None,
                        dtype=None,
                        data=None,
@@ -567,15 +576,15 @@
                        make_scale=False,
                        attach_data_scale=None,
                        attach_data_offset=None,
                        attach_scales=None,
                        ancillary_datasets=None,
                        attrs=None,
                        **kwargs  # standard attributes and other keyword arguments
-                       ):
+                       ) -> protocols.H5TbxDataset:
         """
         Creating a dataset. Allows attaching/making scale, overwriting and setting attributes simultaneously.
 
         Parameters
         ----------
         name : str
             Name of dataset
@@ -702,19 +711,20 @@
                     elif isinstance(scale, h5py.Dataset):
                         scale_name = scale.name
                         scale_data = scale[()]
                     else:
                         raise TypeError(f'Expecting type string or a h5py.Dataset for scale, not {type(scale)}')
                     data = data.rename({dim: scale_name}).assign_coords({scale_name: scale_data})
             attrs.update(data.attrs)
-            return data.hdf.to_group(self._h5grp(self), name=name,
+            xrds = data.hdf.to_group(self._h5grp(self), name=name,
                                      overwrite=overwrite,
                                      compression=compression,
                                      compression_opts=compression_opts,
                                      attrs=attrs)
+            return Dataset(xrds.id)
 
         if not isinstance(make_scale, (bool, str)):
             raise TypeError(f'Make scale must be a boolean or a string not {type(make_scale)}')
 
         if isinstance(shape, np.ndarray):  # needed if no keyword is used
             data = shape
             shape = None
@@ -728,22 +738,20 @@
             for anc_name, anc_ds in ancillary_datasets.items():
                 if not isinstance(anc_ds, h5py.Dataset):
                     raise TypeError(f'Expected ancillary dataset to be of type h5py.Dataset, '
                                     f'but got {type(anc_ds)}')
                 if anc_ds.shape != _data.shape:
                     raise ValueError(f'Associated dataset {anc_name} has shape {anc_ds.shape} '
                                      f'which does not match dataset shape {_data.shape}')
-            import json
             attrs[consts.ANCILLARY_DATASET] = json.dumps({k: v.name for k, v in ancillary_datasets.items()})
 
         _maxshape = kwargs.get('maxshape', shape)
 
-        logger.debug(
-            f'Creating dataset "{name}" in "{self.name}" with maxshape {_maxshape} " '
-            f'and using compression "{compression}" with opt "{compression_opts}"')
+        logger.debug(f'Creating dataset "{name}" in "{self.name}" with maxshape "{_maxshape}" '
+                     f'and using compression "{compression}" with opt "{compression_opts}"')
 
         # if possible, create dataset with shape first:
         if _data is not None:
             if _data.ndim == 0:
                 # create 0D dataset
                 _ds = super().create_dataset(name,
                                              shape=shape,
@@ -764,36 +772,37 @@
             # no data given, initialize with shape only
             _ds = super().create_dataset(name, shape=shape, dtype=dtype, data=_data,
                                          compression=compression,
                                          compression_opts=compression_opts,
                                          chunks=chunks,
                                          **kwargs)
 
-        ds = self._h5ds(_ds.id)
+        ds = Dataset(_ds.id)
+
         if attach_data_scale is not None or attach_data_offset is not None:
             units = attrs.get('units', None)
             if units:
                 ds.attrs['units'] = units
             ds.attach_data_scale_and_offset(attach_data_scale, attach_data_offset)
 
         # assign attributes, which may raise errors if attributes are standardized and not fulfill requirements:
         if attrs:
-            try:
-                for k, v in attrs.items():
+            for k, v in attrs.items():
+                try:
                     # call __setitem__ because then we can pass attrs which is needed by the potential validators of
                     # standard attributes
                     if isinstance(v, h5py.Dataset):
                         ds.attrs.__setitem__(k, v.name, attrs)
                     else:
                         ds.attrs.__setitem__(k, v, attrs)
-            except convention.standard_attributes.errors.StandardAttributeError as e:
-                logger.debug(f'Could not set attribute "{k}" with value "{v}" to dataset "{name}" for convention '
-                             f'{self.convention.name}. Orig err: "{e}"')
-                del self[name]
-                raise e
+                except convention.standard_attributes.errors.StandardAttributeError as e:
+                    logger.debug(f'Could not set attribute "{k}" with value "{v}" to dataset "{name}" for convention '
+                                 f'{self.convention.name}. Orig err: "{e}"')
+                    del self[name]
+                    raise e
 
         # what is this for? uncommented it in version v1.0.1
         # if isinstance(data, np.ndarray):
         #     if data is not None and data.ndim > 0:
         #         ds[()] = data
 
         # make scale
@@ -824,27 +833,62 @@
                         if not shape_of_axis_i == ds_to_attach.shape[0]:
                             del self[ds.name]
                             raise ValueError(f'Cannot assign {ds_to_attach.name} to {name} because it has '
                                              f'different shape {ds_to_attach.shape[0]} than {shape_of_axis_i}')
                         ds.dims[i].attach_scale(ds_to_attach)
         return ds
 
-    def find_one(self, flt: Union[Dict, str],
+    def find_one(self,
+                 flt: Union[Dict, str],
                  objfilter: Union[str, h5py.Dataset, h5py.Group, None] = None,
                  recursive: bool = True,
-                 ignore_attribute_error: bool = False):
-        """See find()"""
-        raise NotImplementedError('Move to database subpackage')
+                 ignore_attribute_error: bool = False) -> protocols.LazyObject:
+        """See ObjDB.find_one()"""
+        from h5rdmtoolbox.database import ObjDB
+        return ObjDB(self).find_one(flt, objfilter, recursive, ignore_attribute_error)
+
+    def find(self,
+             flt: Union[Dict, str, List[str]],
+             objfilter: Union[str, h5py.Dataset, h5py.Group, None] = None,
+             recursive: bool = True,
+             ignore_attribute_error: bool = False) -> List[protocols.LazyObject]:
+        """
+        Examples for filter parameters:
+        filter = {'long_name': 'any objects long name'} --> searches in attributes only
+        filter = {'$name': '/name'}  --> searches in groups and datasets for the (path)name
+        filter = {'$basename': 'name'}  --> searches in groups and datasets for the basename (without path)
+
+        Parameters
+        ----------
+        flt: Dict
+            Filter request
+        objfilter: str | h5py.Dataset | h5py.Group | None
+            Filter. Default is None. Otherwise, only dataset or group types are returned.
+        recursive: bool, optional
+            Recursive search. Default is True
+        ignore_attribute_error: bool, optional=False
+            If True, the KeyError normally raised when accessing hdf5 object attributes is ignored.
+            Otherwise, the KeyError is raised.
+
+        Returns
+        -------
+        h5obj: List[LazyObject]
+        """
+        from h5rdmtoolbox.database import ObjDB
+        return ObjDB(self).find(flt,
+                                objfilter,
+                                recursive=recursive,
+                                ignore_attribute_error=ignore_attribute_error)
 
     def create_dataset_from_csv(self, csv_filename: Union[str, pathlib.Path], *args, **kwargs):
         """Create datasets from a single csv file. Docstring: See File.create_datasets_from_csv()"""
         return self.create_datasets_from_csv(csv_filenames=[csv_filename, ], *args, **kwargs)
 
     def create_datasets_from_csv(self,
-                                 csv_filenames: Union[str, pathlib.Path],
+                                 csv_filenames: Union[str, pathlib.Path, List[str], List[pathlib.Path]],
                                  dimension: Union[int, str] = 0,
                                  shape=None,
                                  overwrite=False,
                                  combine_opt='stack',
                                  axis=0,
                                  chunks=None,
                                  attrs: Dict = None,
@@ -967,36 +1011,36 @@
             for name, value in df.items():
                 if shape is None:
                     data[name].append(value.values)
                 else:
                     data[name].append(value.values.reshape(shape))
 
         for name, value in data.items():
-            self.create_dataset(name=name,
+            self.create_dataset(name=str(name),
                                 data=np.stack(value, axis=axis),
                                 attrs=attrs.get(name, None),
                                 overwrite=overwrite,
                                 compression=compression,
                                 compression_opts=compression_opts,
                                 chunks=chunks)
 
     def create_dataset_from_image(self,
-                                  imgdata: Union[Callable, np.ndarray, List[np.ndarray]],
+                                  img_data: Union[Iterable, np.ndarray, List[np.ndarray]],
                                   name,
                                   chunks=None,
                                   dtype=None,
                                   axis=0,
                                   **kwargs):
         """
         Creates a dataset for a single or multiple files. If a list of filenames is passed
         All images are stacked (thus shape of all images must be equal!)
 
         Parameters
         ----------
-        imgdata : np.ndarray or list of np.ndarray
+        img_data : np.ndarray or list of np.ndarray
             Image filename or list of image file names. See also axis in case of multiple files
         name : str
             Name of create dataset
         chunks : Tuple or None
             Data chunking
         dtype : str
             Data type used for hdf dataset creation
@@ -1012,118 +1056,74 @@
 
         """
 
         # take compression from kwargs or config:
         _compression, _compression_opts = get_config('hdf_compression'), get_config('hdf_compression_opts')
         compression = kwargs.pop('compression', _compression)
         compression_opts = kwargs.pop('compression_opts', _compression_opts)
+        first_image = None
+        n = None
 
         if axis not in (0, -1):
-            raise ValueError(f'Value for parameter axis can only be 0 or 1 but not {axis}')
+            raise ValueError(f'Parameter for parameter axis can only be 0 or 1 but not {axis}')
+
+        iterable: bool = isinstance(img_data, Iterable)
+        if iterable:
+            # check if img_data has method __len__():
+            if not hasattr(img_data, '__len__'):
+                raise ValueError('img_data must have method __len__()')
+            n = len(img_data)
 
-        is_list_tuple_or_numpy = isinstance(imgdata, (list, tuple, np.ndarray))
-        if not is_list_tuple_or_numpy:
-            if not isinstance(imgdata, Iterable):
-                raise ValueError('imgdata must be iterable')
-            # check if imgdata has method __len__():
-            if not hasattr(imgdata, '__len__'):
-                raise ValueError('imgdata must have method __len__()')
-            # get first element of imgdata:
-            first_image = next(imgdata)
+            img_data = iter(img_data)
+
+            # get first element of img_data:
+            first_image = next(img_data)
             single_img_shape = first_image.shape
             if axis == 0:
-                shape = (len(imgdata), *single_img_shape)
+                shape = (n, *single_img_shape)
                 chunks = (1, *single_img_shape)
             else:
-                shape = (*single_img_shape, len(imgdata))
+                shape = (*single_img_shape, n)
                 chunks = (*single_img_shape, 1)
         else:
-            is_np_ndarray = isinstance(imgdata, np.ndarray)
-            if is_np_ndarray:
-                shape = imgdata.shape
+            if isinstance(img_data, np.ndarray):
+                shape = img_data.shape
             else:
-                single_img_shape = imgdata[0].shape
-                if not all([img.shape == single_img_shape for img in imgdata]):
-                    raise ValueError('All images must have the same shape to fit into the same dataset!')
-                if axis == 0:
-                    shape = (len(imgdata), *single_img_shape)
-                    if chunks is None:
-                        chunks = (1, *single_img_shape)
-                else:
-                    shape = (*single_img_shape, len(imgdata))
-                    if chunks is None:
-                        chunks = (*single_img_shape, 1)
+                shape = None
 
         ds = self.create_dataset(name=name,
                                  shape=shape,
                                  compression=compression,
                                  compression_opts=compression_opts,
                                  chunks=chunks,
                                  dtype=dtype,
                                  **kwargs)
-        if not is_list_tuple_or_numpy:
-            if axis == 0:
-                ds[0, ...] = first_image
-            else:
-                ds[..., 0] = first_image
-            for i, img in enumerate(imgdata):
-                if axis == 0:
-                    ds[i, ...] = img
-                else:
-                    ds[..., i] = img
+        if isinstance(img_data, np.ndarray):
+            ds[()] = img_data
             return ds
 
-        if is_np_ndarray:
-            ds[:] = imgdata
+        assert first_image is not None, 'First image is None. This should not happen!'
+        if axis == 0:
+            ds[0, ...] = first_image
         else:
-            ds[:] = np.stack(imgdata, axis=axis)
-        return ds
+            ds[..., 0] = first_image
 
-    # unused, but leave it for a while:
-    # def create_dataset_from_xarray_dataarray(self,
-    #                                          dataarr: xr.DataArray,
-    #                                          name: str = None,
-    #                                          overwrite: bool = False,
-    #                                          overwrite_coords: bool = False) -> None:
-    #     """create hdf dataset from xarray DataArray. All attributes are written to the
-    #     hdf dataset. If coordinates are present, they are written as dimension scales.
-    #     If only dimensions are present, the dim names are written as attributes using
-    #     `DIMS` as key."""
-    #     ds_coords = {}
-    #     attach_scales = [None] * dataarr.ndim
-    #     for idim, dim in enumerate(dataarr.dims):
-    #         if dim not in self or overwrite_coords:
-    #             ds = self.create_dataset(dim,
-    #                                      data=dataarr.coords[dim].values,
-    #                                      attrs=dataarr.coords[dim].attrs,
-    #                                      overwrite=overwrite_coords)
-    #             ds.make_scale()
-    #             ds_coords[dim] = ds
-    #         if dim in self:
-    #             attach_scales[idim] = dim
-    #     if name is None:
-    #         name = dataarr.name
-    #     if len(ds_coords) == 0:
-    #         dim_attr = {'DIMS': dataarr.dims}
-    #     else:
-    #         dim_attr = {}
-    #     dataarr.attrs.update(dim_attr)
-    #     ds = self.create_dataset(name,
-    #                              shape=dataarr.shape,
-    #                              attrs=dataarr.attrs,
-    #                              overwrite=overwrite,
-    #                              attach_scales=attach_scales)
-    #     ds[()] = dataarr.values
+        for i in range(1, n):
+            if axis == 0:
+                ds[i, ...] = next(img_data)
+            else:
+                ds[..., i] = next(img_data)
+        return ds
 
     def create_dataset_from_xarray_dataset(self, dataset: xr.Dataset) -> None:
         """creates the xr.DataArrays of the passed xr.Dataset, writes all attributes
         and handles the dimension scales."""
         ds_coords = {}
         for coord in dataset.coords.keys():
-            ds = self.create_dataset(coord,
+            ds = self.create_dataset(str(coord),
                                      data=dataset.coords[coord].values,
                                      attrs=dataset.coords[coord].attrs,
                                      overwrite=False)
             ds.make_scale()
             ds_coords[coord] = ds
         for data_var in dataset.data_vars.keys():
             ds = self.create_dataset(data_var,
@@ -1177,29 +1177,53 @@
         self[name] = h5py.ExternalLink(filename, path)
         return self[name]
 
     def create_from_yaml(self, yaml_filename: Path):
         """creates groups, datasets and attributes defined in a yaml file.
         Creation is performed relative to the current group level.
 
-        Note the required yaml file structure, e.g.
-        title='Title of the file'
-        contact='0000-1234-1234-1234'
-        grp/supgrp/y:
-          data: 2
-          overwrite: True
-          attrs:
-            units: 'm/s'
-        grp/supgrp:
-          attrs:
-            comment: This is a group comment
+        An example YAML file content could look like this:
+
+        >>> title: 'Title of the file'
+        >>> contact: '0000-1234-1234-1234'
+        >>> grp:
+        >>>   attrs:
+        >>>     comment: test
+        >>> grp/subgrp/y:
+        >>>   data: 2
+        >>>   overwrite: True
+        >>>   attrs:
+        >>>     units: 'm/s'
+        >>> grp/subgrp:
+        >>>   attrs:
+        >>>     comment: This is a group comment
+        >>>   velocity:
+        >>>     data: [3.4, 1.1]
+        >>>     overwrite: True
+        >>>     attrs:
+        >>>       units: 'm/s'
+
+        Examples
+        --------
+        >>> with h5tbx.File('test.h5', 'w') as h5:
+        >>>     h5.create_from_yaml('test.yaml')
         """
         from . import h5yaml
         h5yaml.H5Yaml(yaml_filename).write(self)
 
+    def create_from_dict(self, dictionary: Dict):
+        """Create groups and datasets based on a dictionary"""
+        from . import h5yaml
+        h5yaml.H5Dict(dictionary).write(self)
+
+    def create_from_jsonld(self, data: str, context: Optional[Dict] = None):
+        """Create groups/datasets from a jsonld string."""
+        from . import jsonld
+        jsonld.to_hdf(self, data=json.loads(data), context=context)
+
     def _get_obj_names(self, obj_type, recursive):
         """Return all names of specified object type
         in this group and if recursive==True also
         all below"""
         _names = []
 
         def _get_obj_name(name, node):
@@ -1243,17 +1267,17 @@
         if max_attr_length:
             self.hdfrepr.max_attr_length = max_attr_length
         return self.hdfrepr.__html__(self, collapsed=collapsed, chunks=chunks, maxshape=maxshape)
 
     def _repr_html_(self):
         return self.hdfrepr.__html__(self)
 
-    def sdump(self):
+    def sdump(self, hide_uri: bool = False):
         """string representation of group"""
-        return self.hdfrepr.str_repr(self)
+        return self.hdfrepr.str_repr(self, hide_uri=hide_uri)
 
     dumps = sdump
 
 
 class DatasetValues:
     """helper class to work around xarray"""
 
@@ -1266,22 +1290,22 @@
     def __setitem__(self, args, val):
         return self.h5dataset.__setitem__(args, val)
 
 
 def only_0d_and_1d(obj):
     """Decorator to check if the dataset is 1D"""
 
-    def wrapper(*args, **kwargs):
+    def wrapper(*args):
         if args[0].ndim > 1:
             raise ValueError('Only applicable to 0D and 1D datasets!')
 
     return obj
 
 
-class Dataset(h5py.Dataset, SpecialAttributeWriter, Core):
+class Dataset(h5py.Dataset):
     """Wrapper around the h5py.Dataset. Some useful methods are added on top of
     the underlying *h5py* package.
 
 
     .. note:: All features from h5py packages are preserved.
 
 
@@ -1294,26 +1318,24 @@
     * detach_data_offset(): Detach data offset from the current dataset.
     * detach_data_scale(): Detach data scale from the current dataset.
     * coords(): Return the coordinates of the current dataset similar to xarray.
     * dump(): Outputs xarray-inspired _html representation of the file content if a notebook environment is used.
     * dumps(): string representation of group
     * isel(): Select data by named dimension and index, mimics xarray.isel.
     * sel(): Select data by named dimension and values, mimics xarray.sel.
-    * to_units(): Convert the dataset to a new unit.
-    * write_iso_timestamp(): Write an ISO 8601 timestamp to the current dataset attribute.
 
     The following properties are added to the h5py.Dataset object:
 
     * rootparent: The root group of the file.
     * basename: The basename of the dataset.
     * values: Accessor to return numpy array of the dataset.
     """
 
     @only_0d_and_1d
-    def __lt__(self, other: Union[int, float]):
+    def __lt__(self, other: Union[int, float, protocols.H5TbxDataset]):
         if isinstance(other, (int, float)):
             data = self.values[()]
             if data.ndim == 1:
                 return np.where(data < other)[0]
             return data < other
         # to sort lists of datasets:
         return self.name < other.name
@@ -1360,23 +1382,52 @@
 
         raise ValueError(f'Unexpected type to compare to: "{type(other)}"')
 
     @with_phil
     def __hash__(self):
         return hash(self.id)
 
+    def __delattr__(self, item):
+        _delattr(self, item)
+
     @property
-    def attrs(self):
+    def convention(self):
+        """Return the convention currently enabled."""
+        return convention.get_current_convention()
+
+    @property
+    def standard_attributes(self) -> Dict:
+        """Return the standard attributes of the class."""
+        return self.convention.properties.get(self.__class__, {})
+
+    @property
+    def rdf(self):
+        """Return RDF Manager"""
+        return rdf.RDFManager(self.attrs)
+
+    @property
+    def iri(self):
+        """Deprecated. Use rdf instead."""
+        warnings.warn('Property "iri" is deprecated. Use "rdf" instead.', DeprecationWarning)
+        return rdf.RDFManager(self.attrs)
+
+    @property
+    def hdf_filename(self) -> pathlib.Path:
+        """The filename of the file, even if the HDF5 file is closed."""
+        return assert_filename_existence(self._hdf_filename)
+
+    @property
+    def attrs(self) -> protocols.H5TbxAttributeManager:
         """Exact copy of parent class:
         Attributes attached to this object """
         with phil:
             return WrapperAttributeManager(self)
 
     @property
-    def parent(self) -> "Group":
+    def parent(self) -> protocols.H5TbxGroup:
         """Return the parent group of this dataset
 
         Returns
         -------
         Group
             Parent group of this dataset"""
 
@@ -1454,19 +1505,14 @@
         if ancillary_dataset.shape != self.shape:
             raise ValueError('Shape of flag dataset does not match the shape of the current dataset!')
         ancillary_datasets = self.ancillary_datasets
         ancillary_datasets[ancillary_dataset.basename] = ancillary_dataset.name
         self.attrs[consts.ANCILLARY_DATASET] = ancillary_datasets
         return self
 
-    # @property
-    # def has_flag_data(self):
-    #     """Check if the dataset has a flag dataset attached."""
-    #     return ANCILLARY_DATASET in self.attrs and self.attrs[FLAG_DATASET_CONST] in self.parent
-
     def detach_data_scale(self):
         """Remove the attached data scale dataset from this dataset."""
         warnings.warn('Note, that detaching data scale may influence the correctness and traceability of your data',
                       UserWarning)
         self.attrs.pop('DATA_SCALE', None)
 
     def detach_data_offset(self):
@@ -1517,18 +1563,24 @@
         if 'DATA_OFFSET' in self.attrs:
             _src = self.attrs['DATA_OFFSET']
             if isinstance(_src, str):
                 return self.rootparent[_src]
             return self.rootparent[self.attrs['DATA_OFFSET'].name]
         return None
 
-    def coords(self) -> Dict[str, "Dataset"]:
+    def coords(self) -> Dict:
         """Return a dictionary of the dimension scales of the dataset.
         Corresponds to the xarray coordinates."""
-        return {d[0].name.rsplit('/')[-1]: d[0] for d in self.dims if len(d) > 0}
+        coords = {}
+        for dim in self.dims:
+            if len(dim) > 0:
+                for i, d in enumerate(dim):
+                    coords[dim[i].name.rsplit('/')[-1]] = dim[i]
+        return coords
+        # return {d[0].name.rsplit('/')[-1]: d[0] for d in self.dims if len(d) > 0}
 
     def isel(self, **indexers) -> xr.DataArray:
         """Index selection by providing the coordinate name.
 
         Parameters
         ----------
         indexers: Dict
@@ -1547,28 +1599,45 @@
         if len(indexers) == 0:
             return self[()]
         ds_coords = self.coords()
         if ds_coords:
             for cname in indexers.keys():
                 if cname not in ds_coords:
                     raise KeyError(f'Coordinate {cname} not in {list(ds_coords.keys())}')
-            sl = {cname: slice(None) for cname in ds_coords.keys()}
-            for cname, item in indexers.items():
+
+            sl = {cname: slice(None) for cname, _ in zip(ds_coords.keys(), range(self.ndim))}
+            for (cname, item), _ in zip(indexers.items(), range(self.ndim)):
                 sl[cname] = item
         else:
             # no indexers available. User must provide dim_<i> then!
             if not all([cname.startswith('dim_') for cname in indexers.keys()]):
                 raise KeyError(f'No coordinates available. Provide dim_<i> as key!')
             dim_dict = {f'dim_{i}': slice(None) for i in range(len(self.shape))}
             # indices = [int(cname.split('_')[1]) for cname in indexers.keys()]
-            sl = {cname: slice(None) for cname in dim_dict.keys()}
-            for cname, item in indexers.items():
+            sl = {cname: slice(None) for cname, _ in zip(dim_dict.keys(), range(self.ndim))}
+            for (cname, item), _ in zip(indexers.items(), range(self.ndim)):
                 sl[cname] = item
 
-        return self[tuple([v for v in sl.values()])]
+        def _make_ascending(_data):
+            if isinstance(_data, (np.ndarray, list)):
+                warnings.warn(
+                    'Only ascending order is supported for np.ndarray and list. Reducing the data to unique values'
+                )
+                unique_data = np.unique(_data)
+                _diff = np.diff(unique_data)
+                if np.all(_diff == 1):
+                    # more efficient to use slice
+                    return slice(unique_data[0], unique_data[-1] + 1, 1)
+                if np.all(_diff == 2):
+                    # more efficient to use slice
+                    return slice(unique_data[0], unique_data[-1] + 1, 2)
+                return unique_data
+            return _data
+
+        return self[tuple([_make_ascending(v) for v in sl.values()])]
 
     def sel(self, method=None, **coords):
         """Select data based on coordinates and specific value(s). This is useful if the index
         is not known. Only works for a single dimension and for method 'exact'."""
         av_coord_datasets = self.coords()
         isel = {}
         for coord_name, coord_values in coords.items():
@@ -1627,20 +1696,30 @@
         if isinstance(value, xr.DataArray):
             self.attrs.update(value.attrs)
             super().__setitem__(key, value.data)
         else:
             super().__setitem__(key, value)
 
     @dataset_value_decoder
-    def __getitem__(self, args, new_dtype=None, nparray=False) -> Union[xr.DataArray, np.ndarray]:
+    def __getitem__(self,
+                    args,
+                    new_dtype=None,
+                    nparray=False,
+                    links_as_strings: bool = False) -> Union[xr.DataArray, np.ndarray]:
         """Return sliced HDF dataset. If global setting `return_xarray`
         is set to True, a `xr.DataArray` is returned, otherwise the default
         behaviour of the h5p-package is used and a np.ndarray is returned.
         Note, that even if `return_xarray` is True, there is another way to
-        receive  numpy array. This is by calling .values[:] on the dataset."""
+        receive  numpy array. This is by calling .values[:] on the dataset.
+
+        Parameters
+        ----------
+        links_as_strings: bool
+            Attributes, that are links to other datasets or groups are returned as strings.
+        """
 
         args = args if isinstance(args, tuple) else (args,)
 
         if not get_config('return_xarray') or nparray:
             return super().__getitem__(args, new_dtype=new_dtype)
 
         # check if any entry in args is of type Ellipsis:
@@ -1650,15 +1729,24 @@
             ellipsis_index = args.index(Ellipsis)
             args.pop(ellipsis_index)
             args[ellipsis_index:ellipsis_index] = [slice(None)
                                                    for _ in range(self.ndim - len(args))]
             args = tuple(args)
 
         arr = super().__getitem__(args, new_dtype=new_dtype)
-        ds_attrs = self.attrs
+
+        if links_as_strings:
+            attrs = dict(self.attrs)
+            for k, v in attrs.copy().items():
+                if isinstance(v, (h5py.Group, h5py.Dataset)):
+                    attrs[k] = v.name
+            ds_attrs = attrs
+        else:
+            ds_attrs = self.attrs
+
         attrs = pop_hdf_attributes(ds_attrs)
 
         if 'DIMENSION_LIST' in ds_attrs:
             # there are coordinates to attach...
 
             myargs = [slice(None) for _ in range(self.ndim)]
             for ia, a in enumerate(args):
@@ -1709,22 +1797,22 @@
                             coords[coord_name] = xr.DataArray(name=coord_name, dims=(),
                                                               data=dim_ds_data,
                                                               attrs=dim_ds_attrs)
 
             used_dims = [dim_name for arg, dim_name in zip(
                 myargs, dims_names) if isinstance(arg, (slice, np.ndarray, list))]
 
-            COORDINATES = ds_attrs.get(protected_attributes.COORDINATES)
-            if COORDINATES is not None:
-                if isinstance(COORDINATES, str):
-                    COORDINATES = [COORDINATES, ]
+            coordinates: Optional[Union[str, List[str]]] = ds_attrs.get(protected_attributes.COORDINATES)
+            if coordinates is not None:
+                if isinstance(coordinates, str):
+                    coordinates = [coordinates, ]
                 else:
-                    COORDINATES = list(COORDINATES)
+                    coordinates = list(coordinates)
 
-                for c in COORDINATES:
+                for c in coordinates:
                     if c[0] == '/':
                         _data = self.rootparent[c]
                     else:
                         _data = self.parent[c]
                     _name = Path(c).stem
                     coords.update({_name: xr.DataArray(name=_name, dims=(),
                                                        data=_data,
@@ -1749,15 +1837,15 @@
                 else:  # _arr.ndim > 1:
                     orig_shape = _arr.shape
                     _flat_arr = np.asarray([datetime.fromisoformat(t) for t in _arr.flatten()])
                     _arr = _flat_arr.reshape(orig_shape)
                 return xr.DataArray(_arr, attrs=attrs)
             else:
                 if isinstance(_arr, np.ndarray):
-                    return tuple(_arr)
+                    return _arr
             return _arr
 
         return xr.DataArray(name=Path(self.name).stem, data=arr, attrs=attrs)
 
     def __repr__(self) -> str:
         r = super().__repr__()
         if not self:
@@ -1805,26 +1893,14 @@
         else:
             raise ValueError(f'Could not initialize Dataset with type(_id)={type(_id)}. '
                              'A h5py.h5f.FileID object must be passed')
 
         super().__init__(_id)
         self._hdf_filename = Path(self.file.filename)
 
-    def to_units(self, new_units: str, inplace: bool = False):
-        """Changes the physical unit of the dataset using pint_xarray.
-        If `inplace`=True, it loads to full dataset into RAM, which may
-        not recommended for very large datasets.
-        TODO: think about RAM check or perform it based on chunks"""
-        if inplace:
-            old_units = self[()].attrs['units']
-            self[()] = self[()].pint.quantify().pint.to(new_units).pint.dequantify()
-            new_units = self[()].attrs['units']
-            logger.debug(f'Changed units of {self.name} from {old_units} to {new_units}.')
-        return self[()].pint.quantify().pint.to(new_units).pint.dequantify()
-
     def set_primary_scale(self, axis, iscale: int):
         """Set the primary scale for a specific axis.
 
         Parameters
         ----------
         axis : int
             The axis index
@@ -1843,43 +1919,16 @@
         for _, ds in backup_scales:
             self.dims[axis].detach_scale(ds)
         ils = [iscale, *[i for i in range(nscales) if i != iscale]]
         for i in ils:
             self.dims[axis].attach_scale(backup_scales[i][1])
         logger.debug('new primary scale: %s', self.dims[axis][0])
 
-    def find(self, flt: Union[Dict, str],
-             objfilter: Union[str, h5py.Dataset, h5py.Group, None] = None,
-             ignore_attribute_error: bool = False) -> List:
-        """
-        Examples for filter parameters:
-        filter = {'long_name': 'any objects long name'} --> searches in attributes only
-        filter = {'$name': '/name'}  --> searches in groups and datasets for the (path)name
-        filter = {'$basename': 'name'}  --> searches in groups and datasets for the basename (without path)
 
-        Parameters
-        ----------
-        flt: Dict
-            Filter request
-        objfilter: str | h5py.Dataset | h5py.Group | None
-            Filter. Default is None. Otherwise, only dataset or group types are returned.
-        recursive: bool, optional
-            Recursive search. Default is True
-        ignore_attribute_error: bool, optional=False
-            If True, the KeyError normally raised when accessing hdf5 object attributess is ignored.
-            Otherwise, the KeyError is raised.
-
-        Returns
-        -------
-        h5obj: h5py.Dataset or h5py.Group
-        """
-        raise NotImplementedError('Move to database subpackage')
-
-
-class File(h5py.File, Group, SpecialAttributeWriter, Core):
+class File(h5py.File, Group):
     """Main wrapper around h5py.File.
 
     Adds additional features and methods to h5py.File in order to streamline the work with
     HDF5 files and to incorporate usage of metadata (attribute naming) convention.
     An additional argument is added to the h5py.
 
 
@@ -1903,15 +1952,15 @@
 
     * moveto(): Move the file to a new location.
     * saveas(): Save the file to a new location.
     * reopen(): Reopen the closed file.
 
     The following attributes are added to the h5py.File object:
 
-    * iri: IRI Manager
+    * rdf: RDF Manager
     * hdf_filename: (pathlib.Path) The name of the file, accessible even if the file is closed.
     * version: (str) The version of the package used to create the file.
     * modification_time: (datetime) The modification time of the file.
     * creation_time: (datetime) The creation time of the file.
     * filesize: (int) The size of the file in bytes.
 
     .. seealso:: :class:`h5rdmtoolbox.core.Group`
@@ -1923,15 +1972,15 @@
         with phil:
             return WrapperAttributeManager(self)
 
     @property
     def version(self) -> str:
         """Return version stored in file, which is the package version used at the time of creation.
         Not necessarily the current version of the package."""
-        return self.attrs.get('__h5rdmtoolbox_version__')
+        return self.get('h5rdmtoolbox', {}).attrs.get('__h5rdmtoolbox_version__')
 
     @property
     def modification_time(self) -> datetime:
         """Return the modification from the file. Not stored as an attribute!"""
         return datetime.fromtimestamp(self._hdf_filename.stat().st_mtime,
                                       tz=timezone.utc).astimezone()
 
@@ -1966,15 +2015,14 @@
                 kwargs, _ = _pop_standard_attributes(
                     kwargs, cache_entry=convention.get_current_convention().methods[self.__class__]["__init__"]
                 )
             super(File, self).__init__(name, mode, **kwargs)
             self._hdf_filename = Path(self.filename)
             return
 
-        fname = None
         # name is path or None:
         if name is None:
             _tmp_init = True
             logger.debug("An empty File class is initialized")
             name = utils.touch_tmp_hdf5_file()
             if mode is None:
                 mode = 'r+'
@@ -1989,16 +2037,16 @@
                 # file does exist and mode not given --> read only!
                 if fname.exists():
                     mode = 'r'
                     logger.debug('Mode is set to "r" because file exists and mode was not given.')
 
                 # file does not exist and mode is not given--> write!
                 elif not fname.exists():
-                    mode = 'w'
-                    logger.debug('Mode is set to "w" because file does not exist and mode was not given.')
+                    raise FileNotFoundError(f'File "{fname}" does not exist and mode is not given.')
+
             elif mode == 'w' and fname.exists():
                 fname.unlink()
                 logger.debug('File exists and mode is set to "w". Deleting file first.')
             # else mode is given, so just continue... may be correct, may be not... let h5py find out
 
         if mode is None:
             logger.debug('Mode not set. Set it to "r" by default')
@@ -2007,15 +2055,15 @@
             raise ValueError(
                 f'It seems that no proper file name is passed: type of "{name}" is {type(name)}'
             )
         else:
             if mode == 'r+':
                 if not Path(name).exists():
                     _tmp_init = True
-                    mode = 'r+'
+                    # mode = 'r+'
                     # "touch" the file, so it exists
                     _h5pykwargs = kwargs.copy()
                     for k in list(kwargs.keys()):
                         if k not in H5KWARGS:
                             _h5pykwargs.pop(k, None)
                     with h5py.File(name, mode='w', **_h5pykwargs) as _h5:
                         pass  # just touching the file
@@ -2056,16 +2104,21 @@
         super().__init__(name=name,
                          mode=mode,
                          **kwargs)
         self._hdf_filename = Path(self.filename)
 
         if self.mode != 'r':
             # update file toolbox version, wrapper version
-            if '__h5rdmtoolbox_version__' not in self.attrs:
-                self.attrs['__h5rdmtoolbox_version__', consts.VERSION_IRI] = __version__
+            if get_config('auto_create_h5tbx_version'):
+                if 'h5rdmtoolbox' not in self and get_config('auto_create_h5tbx_version'):
+                    utils.create_h5tbx_version_grp(self)
+                    # logger.debug('Creating group "h5rdmtoolbox" with attribute "__h5rdmtoolbox_version__" in file')
+                    # _tbx_grp = self.create_group('h5rdmtoolbox')
+                    # _tbx_grp.rdf.subject = 'https://schema.org/SoftwareSourceCode'
+                    # _tbx_grp.attrs['__h5rdmtoolbox_version__', 'https://schema.org/softwareVersion'] = __version__
             for k, v in attrs.items():
                 self.attrs[k] = v
 
     def __setattr__(self, key, value):
         props = self.convention.properties.get(self.__class__, None)
         if props:
             prop = props.get(key, None)
@@ -2079,14 +2132,43 @@
     def __repr__(self) -> str:
         r = super().__repr__()
         return r.replace('HDF5', f'HDF5 (convention: "{convention.get_current_convention().name}")')
 
     def __str__(self) -> str:
         return f'<class "{self.__class__.__name__}" convention: "{convention.get_current_convention().name}">'
 
+    def __delattr__(self, item):
+        _delattr(self, item)
+
+    @property
+    def convention(self):
+        """Return the convention currently enabled."""
+        return convention.get_current_convention()
+
+    @property
+    def standard_attributes(self) -> Dict:
+        """Return the standard attributes of the class."""
+        return self.convention.properties.get(self.__class__, {})
+
+    @property
+    def rdf(self):
+        """Return RDF Manager"""
+        return rdf.RDFManager(self.attrs)
+
+    @property
+    def iri(self):
+        """Deprecated. Use rdf instead."""
+        warnings.warn('Property "iri" is deprecated. Use "rdf" instead.', DeprecationWarning)
+        return rdf.RDFManager(self.attrs)
+
+    # @property
+    # def attrsdef(self) -> definition.DefinitionManager:
+    #     """Return DefinitionManager"""
+    #     return definition.DefinitionManager(self.attrs)
+
     def moveto(self, destination: Path, overwrite: bool = False) -> Path:
         """Move the opened file to a new destination.
 
         Parameters
         ----------
         destination : Path
             New filename.
@@ -2172,13 +2254,28 @@
 
         Returns
         -------
         Subclass of File
         """
         return File(filename, mode)
 
+    def dump_jsonld(self,
+                    skipND: int = 1,
+                    structural: bool = True,
+                    semantic: bool = True,
+                    resolve_keys: bool = False,
+                    **kwargs) -> str:
+        """Dump the file content as JSON-LD string"""
+        from .. import dump_jsonld
+        return dump_jsonld(self.hdf_filename,
+                           skipND=skipND,
+                           structural=structural,
+                           semantic=semantic,
+                           resolve_keys=resolve_keys,
+                           **kwargs)
+
 
 Dataset._h5grp = Group
 Dataset._h5ds = Dataset
 
 Group._h5grp = Group
 Group._h5ds = Dataset
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/ds_decoder.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/ds_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 def dataset_value_decoder(func):
     """decorator during slicing of dataset"""
 
     def wrapper(*args, **kwargs):
         """wrapper that decodes the xarray.DataArray object"""
         ds = args[0]
         assert isinstance(ds, h5py.Dataset)
+        kwargs.update(links_as_strings=True)
         xarr = func(*args, **kwargs)
 
         parent_slice = args[1]
 
         if not isinstance(xarr, xr.DataArray):
             return xarr
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/h5attr.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5attr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,108 @@
+"""Attribute module"""
 import ast
 import h5py
 import json
+import logging
 import numpy as np
 import pint
+import pydantic
 import rdflib
+import warnings
+from datetime import datetime
+from h5py._hl.attrs import AttributeManager
 from h5py._hl.base import with_phil
-from h5py._objects import ObjectID
-from typing import Dict, Union
+from h5py._objects import ObjectID, phil
+from pydantic import HttpUrl
+from typing import Dict, Union, Tuple, Optional, Any
 
-from . import logger
 from .h5utils import get_rootparent
 from .. import errors
 from .. import get_config, convention, utils
 from .. import get_ureg
 from .. import protected_attributes
 from ..convention import consts
 
+logger = logging.getLogger('h5rdmtoolbox')
 H5_DIM_ATTRS = protected_attributes.h5rdmtoolbox
 
 
+class AttrDescriptionError(Exception):
+    """Generic attribute description error"""
+    pass
+
+
+class Attribute:
+    """Helper class for quick assignment of RDF attributes to the HDF5 file.
+
+    Examples
+    --------
+    >>> import h5rdmtoolbox as h5tbx
+    >>> from ontolutils import M4I
+    >>> rdf_attr = h5tbx.Attribute('0000-0001-8729-0482', rdf_predicate=M4I.orcidId,
+    ...                            rdf_object='https://orcid.org/0000-0001-8729-0482')
+    >>> with h5tbx.File('test.h5', 'w') as h5:
+    ...     grp = h5.create_group('person')
+    ...     grp.attrs['orcid'] = rdf_attr
+    ...     # equal to:
+    ...     # grp.attrs['orcid'] = '0000-0001-8729-0482'
+    ...     # grp.rdf.predicate['orcid'] = str(M4I.orcidId)
+    ...     # grp.rdf.object['orcid'] = 'https://orcid.org/0000-0001-8729-0482'
+    """
+
+    def __init__(self,
+                 value, *,
+                 definition: Optional[str] = None,
+                 rdf_predicate=None,
+                 rdf_object=None):
+        self.value = value
+        if not isinstance(value, str):
+            raise TypeError(f'Attribute value must be a string but got {type(value)}')
+        self.definition = definition  # skos:definition
+        self.rdf_predicate = self._validate_rdf(rdf_predicate)
+        self.rdf_object = self._validate_rdf(rdf_object)
+
+    @staticmethod
+    def _validate_rdf(value):
+        if value is None:
+            return
+        try:
+            str(HttpUrl(value))
+        except pydantic.ValidationError as e:
+            raise AttrDescriptionError(
+                f'Invalid URL: "{value}". This was validated with pydantic. Pydantic error: {e}'
+            )
+        return value
+
+    def __repr__(self) -> str:
+        out = f'{self.__class__.__name__}({self.value}'
+        if self.rdf_predicate is not None:
+            out += f', rdf_predicate={self.rdf_predicate}'
+        if self.rdf_object is not None:
+            out += f', rdf_object={self.rdf_object}'
+        if self.definition is not None:
+            out += f', definition={self.definition}'
+        out += ')'
+        return out
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
+
+# def Attribute(value, definition: Optional[str] = None,
+#               rdf_predicate=None, rdf_object=None) -> AttributeValue:
+#     """attribute interface function"""
+#     return AttributeValue(
+#         value,
+#         definition,
+#         rdf_predicate,
+#         rdf_object
+#     )
+
+
 def pop_hdf_attributes(attrs: Dict) -> Dict:
     """Remove HDF attributes like NAME, CLASS, .... from the input dictionary
 
     Parameters
     ----------
     attrs: Dict
         Input dictionary
@@ -50,15 +130,15 @@
 
     def to_pint(self) -> "pint.util.Quantity":
         """Returns a pint.Quantity object"""
         assert get_ureg().default_format == get_config('ureg_format')
         return get_ureg()(self)
 
 
-class WrapperAttributeManager(h5py.AttributeManager):
+class WrapperAttributeManager(AttributeManager):
     """
     Subclass of h5py's Attribute Manager.
     Allows storing dictionaries as json strings and to store a dataset or a group as an
     attribute. The latter uses the name of the object. When __getitem__() is called and
     the name (string) is identified as a dataset or group, then this object is returned.
     """
 
@@ -120,65 +200,128 @@
             vstr = str(ret.tolist())
             if '<HDF5 object reference>' in vstr:
                 return ret
             return WrapperAttributeManager._parse_return_value(_id, vstr)
         return ret
 
     @with_phil
-    def __getitem__(self, name):
+    def __getitem__(self, name: str):
 
         ret = super(WrapperAttributeManager, self).__getitem__(name)
         parent = self._parent
 
         if get_config(
                 'expose_user_prop_to_attrs') and parent.__class__ in convention.get_current_convention().properties:
             if name in convention.get_current_convention().properties[parent.__class__]:
                 return convention.get_current_convention().properties[parent.__class__][name].get(parent)
         return WrapperAttributeManager._parse_return_value(self._id, ret)
 
     def create(self,
                name,
                data,
                shape=None, dtype=None,
-               predicate: Union[str, rdflib.URIRef] = None,
-               object: Union[str, rdflib.URIRef] = None):
+               rdf_predicate: Union[str, rdflib.URIRef] = None,
+               rdf_object: Optional[Union[str, rdflib.URIRef]] = None,
+               definition: Optional[str] = None,
+               **kwargs) -> Any:
+        """
+        Create a new attribute.
+
+        .. note:: Via the config setting "ignore_none" (`h5tbx.set_config(ignore_none=True)`) attribute values, that are None are not written.
+
+
+        Parameters
+        ----------
+        name: str
+            Name of the attribute.
+        data: any
+            Attribute value.
+        shape: tuple, optional
+            Shape of the attribute. If None, the shape is determined from the data.
+        dtype:
+            Data type of the attribute. If None, the data type is determined from the data.
+        rdf_predicate: Union[str, rdflib.URIRef], optional
+            IRI of the predicate
+        rdf_object: Union[str, rdflib.URIRef], optional
+            IRI of the object
+        """
+        if data is None and get_config('ignore_none'):
+            logger.debug(f'Attribute "{name}" is None and "ignore_none" in config is True. Attribute is not created.')
+            return
         r = super().create(name,
                            utils.parse_object_for_attribute_setting(data),
                            shape, dtype)
-        if predicate is not None:
-            self._parent.iri.predicate[name] = predicate
-        if object is not None:
-            self._parent.iri.object[name] = object
+        _predicate = kwargs.get('predicate', None)
+        if _predicate is not None:
+            rdf_predicate = _predicate
+            warnings.warn('The "predicate" argument is deprecated. Use "rdf_predicate" instead.', DeprecationWarning)
+        _object = kwargs.get('predicate', None)
+        if _object is not None:
+            rdf_object = _object
+            warnings.warn('The "object" argument is deprecated. Use "rdf_object" instead.', DeprecationWarning)
+
+        if rdf_predicate is not None:
+            self._parent.rdf.predicate[name] = rdf_predicate
+        if rdf_object is not None:
+            self._parent.rdf.object[name] = rdf_object
+        if definition is not None:
+            self._parent.rdf[name].definition = definition
         return r
 
     @with_phil
-    def __setitem__(self, name, value, attrs=None):
+    def __setitem__(self,
+                    name: Union[str, Tuple[str, str]],
+                    value, attrs: Optional[Dict] = None):
         """ Set a new attribute, overwriting any existing attribute.
 
         The type and shape of the attribute are determined from the data.  To
         use a specific type or shape, or to preserve the type of attribute,
         use the methods create() and modify().
 
         Parameters
         ----------
-        name : str
-            Name of the attribute.
+        name : Union[str, Tuple[str, str]]
+            Name of the attribute. If it is a tuple, the second element is the IRI of the attribute.
         value : any
-            Attribute value.
+            Attribute value. Can also be type `AttributeValue` to set a value and its object IRI.
         """
         if name == '_parent':
             return
+
+        if isinstance(value, Attribute):
+            object_iri = value.rdf_object
+            predicate_iri = value.rdf_predicate
+            attr_def = value.definition
+            value = value.value
+
+            if not isinstance(name, tuple):
+                self.create(name,
+                            value,
+                            rdf_predicate=predicate_iri,
+                            rdf_object=object_iri,
+                            definition=attr_def)
+
+        else:
+            object_iri = None
+            predicate_iri = None
+            attr_def = None
+
         if isinstance(name, tuple):
             # length must be 2, second element must be a IRI (not checked though)
             if not len(name) == 2:
                 raise ValueError('Tuple must have length 2 in order to interpret it as an'
                                  'attribute name and its IRI')
-            _name, _iri = name
-            self.create(_name, value)
-            self._parent.iri.predicate[_name] = _iri
+            if predicate_iri is not None:
+                raise ValueError('You cannot set the predicate iri at the same time by RDFAttribute and through '
+                                 'the tuple syntax.')
+            _name, predicate_iri = name
+            self.create(_name, value,
+                        rdf_predicate=predicate_iri,
+                        rdf_object=object_iri,
+                        definition=attr_def)
             return
 
         if not isinstance(name, str):
             raise TypeError(f'Attribute name must be a str but got {type(name)}')
 
         curr_cv = convention.get_current_convention()
 
@@ -282,33 +425,62 @@
         for k, v in adict.items():
             if not show_private:
                 if k.startswith('__') and k.endswith('__'):
                     continue
             print(f'{k:{keylen}}:  {v}')
 
     @property
-    def raw(self) -> "h5py.AttributeManager":
+    def raw(self) -> AttributeManager:
         """Return the original h5py attribute object manager"""
-        from h5py._hl import attrs
-        from h5py._objects import phil
         with phil:
-            return attrs.AttributeManager(self._parent)
+            return AttributeManager(self._parent)
+
+    def write_uuid(self, uuid: Optional[str] = None,
+                   name: Optional[str] = None,
+                   overwrite: bool = False) -> str:
+        """Write an uuid to the attribute of the object.
 
-# class IRIAttr:
-#     """Helper class to write attributes together with an IRI
-#
-#     Examples
-#     --------
-#     >>> import h5rdmtoolbox as h5tbx
-#     >>> hasKQ = namespace.M4I.hasKindOfQuantity
-#     >>> Velocity = 'https://qudt.org/vocab/quantitykind/Velocity'
-#     >>>
-#     >>> with h5tbx('test.h5') as h5:
-#     ...     h5.u.attrs['qK', hasKQ] = h5tbx.IRIAttr(value='Velocity', iri=Velocity)
-#     """
-#
-#     def __init__(self, value, iri):
-#         self.value = value
-#         self.iri = iri
-#
-#     def __repr__(self):
-#         return f'{self.__class__.__name__}({self.value} iri={self.iri})'
+        Parameters
+        ----------
+        uuid : str=None
+            The uuid to write. If None, a new uuid is generated.
+        name: str=None
+            Name of the attribute. If None, the default name is taken from the configuration.
+        overwrite: bool=False
+            If the attribute already exists, it is not overwritten if overwrite is False.
+
+        Returns
+        -------
+        str
+            The uuid as string.
+        """
+        if name is None:
+            name = get_config('uuid_name')
+
+        if name in self and not overwrite:
+            raise ValueError(f'The attribute "{name}" cannot be written. It already exists and '
+                             '"overwrite" is set to False')
+        if uuid is None:
+            from uuid import uuid4
+            uuid = uuid4()
+        suuid = str(uuid)
+        self.create(name=name, data=suuid)
+        return suuid
+
+    def write_iso_timestamp(self,
+                            name='timestamp',
+                            dt: Optional[datetime] = None,
+                            overwrite: bool = False, **kwargs):
+        """Write the iso timestamp to the attribute of the object.
+
+        Parameters
+        --
+        """
+        if name in self and not overwrite:
+            raise ValueError(f'The attribute "{name}" cannot be written. It already exists and '
+                             '"overwrite" is set to False')
+        if dt is None:
+            dt = datetime.now()
+        else:
+            if not isinstance(dt, datetime):
+                raise TypeError(f'Invalid type for parameter "dt". Expected type datetime but got "{type(dt)}"')
+        self.create(name=name, data=dt.isoformat(**kwargs))
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/h5utils.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
         def search(parent):
             global found
             parent = parent.parent
             if parent.name == '/':
                 found = parent
             else:
-                _ = search(parent)
+                search(parent)
 
         search(parent)
         return found
 
     if obj.name == '/':
         return obj
     return get_root(obj.parent)
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/h5yaml.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5yaml.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 import h5py
 import pathlib
 import yaml
 from typing import Dict
+from typing import Protocol
 
 
-class H5Yaml:
-    """Interface class to yaml files which allow to create HDF5
-    objects from a yaml file definition"""
-
-    def __init__(self, filename):
-        self.filename = pathlib.Path(filename)
-        if not self.filename.exists():
-            raise FileNotFoundError(f'File not found: {self.filename}')
-        if not self.filename.is_file():
-            raise FileExistsError(f'Not a file: {self.filename}')
-        self._data = None
+class _H5DictDataInterface(Protocol):
 
     @property
     def data(self) -> Dict:
-        if self._data is None:
-            with open(self.filename, 'r') as f:
-                self._data = yaml.safe_load(f)
-        return self._data
+        """Return data"""
+        ...
 
     def write(self, h5: h5py.Group):
         data = self.data
         for k, v in data.items():
             if not isinstance(v, dict):
                 # is an attribute of the grou
                 h5.attrs[k] = v
             else:
                 # can be dataset or group
                 if H5Yaml.is_dataset(v):
                     v.pop('type', None)
                     if 'name' not in v:
                         v['name'] = k
-
-                    h5.create_dataset(**v)
+                    # units = v.pop('units', None)
+                    # standard_name = v.pop('standard_name', None)
+                    # TODO remove the following hotfix
+                    name = v.pop('name')
+                    data = v.pop('data')
+                    try:
+                        h5.create_dataset(name, data=data, **v)
+                    except (TypeError,) as e:
+                        raise RuntimeError('Could not create dataset. Please check the yaml file. The orig. '
+                                           f'error is "{e}"')
+                    # if isinstance(data, str):
+                    #     ds = h5.create_string_dataset(name, data=data,
+                    #                                   **v)
+                    # else:
+                    #     ds = h5.create_dataset(name=name, data=data)
+                    # for ak, av in v.items():
+                    #     ds.attrs[ak] = av
+                    # if units:
+                    #     ds.attrs['units'] = units
+                    # if standard_name:
+                    #     ds.attrs['standard_name'] = standard_name
                 elif H5Yaml.is_group(v):
                     v.pop('type', None)
 
                     group_data = v.copy()
 
                     datasets = {_k: group_data.pop(_k) for _k, _v in v.items() if H5Yaml.is_dataset(_v)}
 
-                    group_data['overwrite'] = group_data.get('overwrite', False)
+                    group_data['overwrite'] = group_data.get('overwrite', None)
                     group_data['update_attrs'] = group_data.get('update_attrs', True)
 
                     if 'name' not in group_data:
                         group_data['name'] = k
 
                     g = h5.create_group(**group_data)
 
@@ -72,7 +80,38 @@
         if isinstance(item, dict):
             for n, v in item.items():
                 if isinstance(v, dict):
                     return True
                 break
             return not H5Yaml.is_dataset(item)
         return False
+
+
+class H5Dict(_H5DictDataInterface):
+
+    def __init__(self, data):
+        self._data = data
+
+    @property
+    def data(self) -> Dict:
+        return self._data
+
+
+class H5Yaml(_H5DictDataInterface):
+    """Interface class to yaml files which allow to create HDF5
+    objects from a yaml file definition"""
+
+    def __init__(self, filename):
+        self.filename = pathlib.Path(filename)
+        if not self.filename.exists():
+            raise FileNotFoundError(f'File not found: {self.filename}')
+        if not self.filename.is_file():
+            raise FileExistsError(f'Not a file: {self.filename}')
+        self._data = None
+
+    @property
+    def data(self) -> Dict:
+        """Return data"""
+        if self._data is None:
+            with open(self.filename, 'r') as f:
+                self._data = yaml.safe_load(f)
+        return self._data
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox/wrapper/xr2hdf.py` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/xr2hdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,101 +1,103 @@
 import h5py
 import numpy as np
 import xarray as xr
+
 from .. import protected_attributes
 
+
 @xr.register_dataarray_accessor("hdf")
 class HDFArrayAccessor:
     """Accessor class that allows to write a Data Array to an HDF5 group"""
 
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
-    def to_group(self, h5group: h5py.Group, name=None, overwrite: bool = False, **kwargs) -> h5py.Dataset:
+    def to_group(self, group: h5py.Group, name=None, overwrite: bool = False, **kwargs) -> h5py.Dataset:
         """Saves the xarray DataArray in a group.
         Parameters
         ----------
-        h5group: h5py.Group
+        group: h5py.Group
             HDF5 group to write dataset into
         name: str, optional=None
             Name of hdf dataset. overwrites name of xr.DataArray
         overwrite: bool, optional=False
             Whether to overwrite an existing dataset with that name
         """
         # h5group = h5py.Group(h5group.id)
         if not self._obj.name and name is None:
             raise AttributeError('Data Array has no name and no name is passed as function parameter.')
         if self._obj.name and name is None:
             name = self._obj.name
-        if name in h5group and overwrite:
-            del h5group[name]
-        elif name in h5group and not overwrite:
+        if name in group and overwrite:
+            del group[name]
+        elif name in group and not overwrite:
             raise ValueError('A dataset with that name already exists and overwrite is set to false.')
 
         ds_attrs = kwargs.pop('attrs', {})
         ds_attrs.update(self._obj.attrs)
 
         for coord in self._obj.coords:
-            if coord in h5group:  # coordinate already exists:
+            if coord in group:  # coordinate already exists:
                 _raise = False
-                if h5group[coord].ndim == 0:
-                    if float(h5group[coord][()]) != float(self._obj.coords[coord][()]):
+                if group[coord].ndim == 0:
+                    if float(group[coord][()]) != float(self._obj.coords[coord][()]):
                         _raise = True
                 else:
-                    if not np.array_equal(h5group[coord][()], self._obj.coords[coord]):
+                    if not np.array_equal(group[coord][()], self._obj.coords[coord]):
                         _raise = True
                 if _raise:
                     raise ValueError(f'The xarray coordinate "{coord}" exists already '
-                                     f'in the HDF group "{h5group.name}" with that name but with '
+                                     f'in the HDF group "{group.name}" with that name but with '
                                      'different values. \nCannot create the dataset '
                                      f'"{name}". Either delete the existing coordinate dataset '
                                      'or write the dataset to a different group.')
 
         attach_scales = []
         coordinates_0dim = []
 
         for coord in self._obj.coords:
-            if coord not in h5group:
+            if coord not in group:
                 _data = self._obj.coords[coord].values
                 coord_attrs = self._obj.coords[coord].attrs
                 if _data.ndim == 0:
                     _ = kwargs.pop('compression_opts', None)
                     _ = kwargs.pop('compression', None)
-                    cds = h5group.create_dataset(coord,
-                                                 data=self._obj.coords[coord].values,
-                                                 attrs=coord_attrs, **kwargs)
+                    cds = group.create_dataset(coord,
+                                               data=self._obj.coords[coord].values,
+                                               attrs=coord_attrs, **kwargs)
                 else:
-                    cds = h5group.create_dataset(coord,
-                                                 data=self._obj.coords[coord].values,
-                                                 attrs=coord_attrs, **kwargs)
+                    cds = group.create_dataset(coord,
+                                               data=self._obj.coords[coord].values,
+                                               attrs=coord_attrs, **kwargs)
                 for k, v in self._obj.coords[coord].attrs.items():
                     cds.attrs[k] = v
                 cds.make_scale()
 
-            if 'REFERENCE_LIST' not in h5group[coord].attrs:
-                h5group[coord].make_scale()
+            if 'REFERENCE_LIST' not in group[coord].attrs:
+                group[coord].make_scale()
 
             if self._obj.coords[coord].ndim == 0:
                 coordinates_0dim.append(coord)  # will be written to attribute "COORDINATES"
             else:
                 attach_scales.append(coord)
 
-        dset = h5group.create_dataset(name, data=self._obj.data, attrs=ds_attrs, **kwargs)
+        dset = group.create_dataset(name, data=self._obj.data, attrs=ds_attrs, **kwargs)
         # for k, v in ds_attrs.items():
         #     try:
         #         if isinstance(v, str):
         #             dset.attrs[k] = str(v)
         #         else:
         #             dset.attrs[k] = v
         #     except Exception as e:
         #         raise Exception(f'Error setting attribute to HDF dataset {dset}:'
         #                         f'\n  name: {k}\n  value: {v} \n  type: {type(v)}\n'
         #                         f'Original error: {e}')
 
         # TODO check that there are "intermediate" coords like ix(x), iy(y)
         for i, s in enumerate(self._obj.dims):
             if s in self._obj.coords:
-                dset.dims[i].attach_scale(h5group[s])
+                dset.dims[i].attach_scale(group[s])
 
         if coordinates_0dim:
             dset.attrs[protected_attributes.COORDINATES] = coordinates_0dim
         return dset
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/PKG-INFO` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5rdmtoolbox
-Version: 1.2.2
+Version: 1.3.0a1
 Summary: Supporting a FAIR Research Data lifecycle using Python and HDF5.
 Home-page: https://h5rdmtoolbox.readthedocs.io/en/latest/
 Author: Matthias Probst
 Author-email: matthias.probst@kit.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,27 +25,32 @@
 Requires-Dist: IPython>=7.34.0
 Requires-Dist: pyyaml>6.0
 Requires-Dist: xarray>=2022.3.0
 Requires-Dist: pint==0.21.1
 Requires-Dist: pint_xarray
 Requires-Dist: regex
 Requires-Dist: packaging
+Requires-Dist: ontolutils>=0.2.20
 Requires-Dist: python-forge
 Requires-Dist: requests
 Requires-Dist: pydantic>=2.3.0
 Requires-Dist: rdflib
 Provides-Extra: database
 Requires-Dist: pymongo; extra == "database"
+Provides-Extra: layout-validation
+Requires-Dist: tabulate; extra == "layout-validation"
 Provides-Extra: csv
 Requires-Dist: pandas; extra == "csv"
 Provides-Extra: snt
 Requires-Dist: xmltodict; extra == "snt"
 Requires-Dist: tabulate; extra == "snt"
 Requires-Dist: python-gitlab; extra == "snt"
 Requires-Dist: pypandoc; extra == "snt"
+Provides-Extra: gui
+Requires-Dist: PyQt5; extra == "gui"
 Provides-Extra: test
 Requires-Dist: pytest>=7.1.2; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: xmltodict; extra == "test"
 Requires-Dist: scipy; extra == "test"
 Requires-Dist: pandas; extra == "test"
@@ -78,15 +83,17 @@
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: scikit-image; extra == "docs"
 Requires-Dist: scikit-learn; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: simplejson; extra == "docs"
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: kglab; extra == "docs"
 Provides-Extra: complete
+Requires-Dist: PyQt5; extra == "complete"
 Requires-Dist: pytest>=7.1.2; extra == "complete"
 Requires-Dist: pytest-cov; extra == "complete"
 Requires-Dist: pylint; extra == "complete"
 Requires-Dist: xmltodict; extra == "complete"
 Requires-Dist: scipy; extra == "complete"
 Requires-Dist: pandas; extra == "complete"
 Requires-Dist: xmltodict; extra == "complete"
@@ -117,36 +124,37 @@
 Requires-Dist: sphinx-copybutton; extra == "complete"
 Requires-Dist: scikit-image; extra == "complete"
 Requires-Dist: scikit-learn; extra == "complete"
 Requires-Dist: sphinx-design; extra == "complete"
 Requires-Dist: simplejson; extra == "complete"
 Requires-Dist: myst-nb; extra == "complete"
 Requires-Dist: sphinxcontrib-bibtex; extra == "complete"
+Requires-Dist: kglab; extra == "complete"
 
 # HDF5 Research Data Management Toolbox
 
 ![Tests](https://github.com/matthiasprobst/h5RDMtoolbox/actions/workflows/tests.yml/badge.svg)
 ![DOCS](https://codecov.io/gh/matthiasprobst/h5RDMtoolbox/branch/dev/graph/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/h5rdmtoolbox/badge/?version=latest)](https://h5rdmtoolbox.readthedocs.io/en/latest/?badge=latest)
 ![pyvers](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 
 *Note, that the project is still under development!*
 
-The "HDF5 Research Data Management Toolbox" (h5RDMtoolbox) is a python package supporting everybody who is working with
+The "HDF5 Research Data Management Toolbox" (h5RDMtoolbox) is a Python package supporting everybody who is working with
 HDF5 to achieve a sustainable data lifecycle which follows
 the [FAIR (Findable, Accessible, Interoperable, Reusable)](https://www.nature.com/articles/sdata201618)
 principles. It specifically supports the five main steps of *planning*, *collecting*, *analyzing*, *sharing* and
 *reusing* data. Please visit the [documentation](https://h5rdmtoolbox.readthedocs.io/en/latest/) for detailed
 information of try the [quickstart using colab](#quickstart).
 
 ## Highlights
 
 - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to allow easy access to metadata and data during
   analysis and processing (
-  see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface).
+  see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface)).
 - Assigning [metadata with "globally unique and persistent identifiers"]() as required
   by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/)
   . This "remove[s] ambiguity in the meaning of your published data...".
 - Define standard attributes through
   [conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/convention/index.html) and enforce users to use
   them
 - Upload HDF5 files directly
@@ -254,17 +262,21 @@
 - `h5py=3.7.0`: HDF5 file interface
 - `xarray>=2022.3.0`: Working with scientific arrays in combination with attributes. Allows carrying metadata from HDF5
   to user
 - `pint>=0.19.2`: Allows working with units
 - `pint_xarray>=0.2.1`: Working with units for usage with xarray
 - `python-forge==18.6.0`: Used to update function signatures when using
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
+- `pydantic`: Used to validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
 - `pyyaml>6.0.0`: Reading and writing of yaml files, e.g. metadata definitions (conventions). Note, lower versions
   collide with python 3.11
 - `requests`: Used to download files from the internet or validate URLs, e.g. metadata definitions (conventions)
+- `rdflib`: Used to enable working with RDF
+- `ontolutils`: Required to work with RDF and derive semantic description of HDF5 file content
+
 
 #### Optional dependencies
 
 To run unit tests or to enable certain features, additional dependencies must be installed.
 
 Install optional dependencies by specifying them in square brackets after the package name, e.g.:
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/SOURCES.txt` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,141 +4,139 @@
 setup.cfg
 setup.py
 h5rdmtoolbox/__init__.py
 h5rdmtoolbox/_cfg.py
 h5rdmtoolbox/_repr.py
 h5rdmtoolbox/_user.py
 h5rdmtoolbox/_version.py
-h5rdmtoolbox/cache.py
+h5rdmtoolbox/cli.py
 h5rdmtoolbox/consts.py
+h5rdmtoolbox/dev.py
 h5rdmtoolbox/errors.py
-h5rdmtoolbox/hdfgui.py
 h5rdmtoolbox/identifiers.py
-h5rdmtoolbox/namespace.py
 h5rdmtoolbox/plotting.py
 h5rdmtoolbox/protected_attributes.py
+h5rdmtoolbox/protocols.py
 h5rdmtoolbox/tutorial.py
 h5rdmtoolbox/utils.py
 h5rdmtoolbox/warnings.py
 h5rdmtoolbox.egg-info/PKG-INFO
 h5rdmtoolbox.egg-info/SOURCES.txt
 h5rdmtoolbox.egg-info/dependency_links.txt
+h5rdmtoolbox.egg-info/entry_points.txt
 h5rdmtoolbox.egg-info/requires.txt
 h5rdmtoolbox.egg-info/top_level.txt
 h5rdmtoolbox/convention/__init__.py
-h5rdmtoolbox/convention/_h5tbx.py
-h5rdmtoolbox/convention/_m4i_namespace.py
-h5rdmtoolbox/convention/_obo_namespace.py
 h5rdmtoolbox/convention/cfg.py
 h5rdmtoolbox/convention/consts.py
 h5rdmtoolbox/convention/core.py
+h5rdmtoolbox/convention/definition.py
 h5rdmtoolbox/convention/errors.py
 h5rdmtoolbox/convention/generate.py
+h5rdmtoolbox/convention/hdf_ontology.py
 h5rdmtoolbox/convention/references.py
 h5rdmtoolbox/convention/standard_attributes.py
 h5rdmtoolbox/convention/toolbox_validators.py
 h5rdmtoolbox/convention/utils.py
 h5rdmtoolbox/convention/warnings.py
+h5rdmtoolbox/convention/ontology/__init__.py
+h5rdmtoolbox/convention/ontology/h5namespace.py
+h5rdmtoolbox/convention/ontology/h5ontocls.py
 h5rdmtoolbox/convention/standard_names/__init__.py
 h5rdmtoolbox/convention/standard_names/accessor.py
 h5rdmtoolbox/convention/standard_names/affixes.py
 h5rdmtoolbox/convention/standard_names/cache.py
 h5rdmtoolbox/convention/standard_names/consts.py
 h5rdmtoolbox/convention/standard_names/h5interface.py
 h5rdmtoolbox/convention/standard_names/name.py
 h5rdmtoolbox/convention/standard_names/table.py
 h5rdmtoolbox/convention/standard_names/transformation.py
 h5rdmtoolbox/convention/standard_names/utils.py
-h5rdmtoolbox/data/__init__.py
+h5rdmtoolbox/data/def_icon.png
 h5rdmtoolbox/data/fluid-v1.yml
 h5rdmtoolbox/data/h5tbx.yaml
+h5rdmtoolbox/data/id_icon.png
+h5rdmtoolbox/data/iri_icon.png
 h5rdmtoolbox/data/piv-v1.yml
 h5rdmtoolbox/data/style.css
 h5rdmtoolbox/data/tutorial_convention.yaml
 h5rdmtoolbox/data/tutorial_standard_name_table.yaml
+h5rdmtoolbox/data/type_icon.png
 h5rdmtoolbox/database/__init__.py
-h5rdmtoolbox/database/lazy.py
+h5rdmtoolbox/database/interface.py
 h5rdmtoolbox/database/mongo.py
-h5rdmtoolbox/database/template.py
 h5rdmtoolbox/database/hdfdb/__init__.py
 h5rdmtoolbox/database/hdfdb/filedb.py
-h5rdmtoolbox/database/hdfdb/nonsearchable.py
 h5rdmtoolbox/database/hdfdb/objdb.py
 h5rdmtoolbox/database/hdfdb/query.py
 h5rdmtoolbox/database/hdfdb/utils.py
 h5rdmtoolbox/extensions/__init__.py
-h5rdmtoolbox/extensions/dataset.py
-h5rdmtoolbox/extensions/ipyvolume.py
 h5rdmtoolbox/extensions/magnitude.py
 h5rdmtoolbox/extensions/normalize.py
-h5rdmtoolbox/extensions/scatterhist.py
 h5rdmtoolbox/extensions/units.py
 h5rdmtoolbox/extensions/vector.py
 h5rdmtoolbox/layout/__init__.py
 h5rdmtoolbox/layout/core.py
 h5rdmtoolbox/repository/__init__.py
-h5rdmtoolbox/repository/h5metamapper.py
 h5rdmtoolbox/repository/interface.py
 h5rdmtoolbox/repository/zenodo/__init__.py
 h5rdmtoolbox/repository/zenodo/core.py
 h5rdmtoolbox/repository/zenodo/metadata.py
 h5rdmtoolbox/repository/zenodo/tokens.py
 h5rdmtoolbox/repository/zenodo/utils.py
 h5rdmtoolbox/wrapper/__init__.py
-h5rdmtoolbox/wrapper/accessory.py
+h5rdmtoolbox/wrapper/accessor.py
 h5rdmtoolbox/wrapper/core.py
 h5rdmtoolbox/wrapper/ds_decoder.py
 h5rdmtoolbox/wrapper/h5attr.py
 h5rdmtoolbox/wrapper/h5ext.py
 h5rdmtoolbox/wrapper/h5utils.py
 h5rdmtoolbox/wrapper/h5yaml.py
-h5rdmtoolbox/wrapper/iri.py
 h5rdmtoolbox/wrapper/jsonld.py
+h5rdmtoolbox/wrapper/lazy.py
+h5rdmtoolbox/wrapper/rdf.py
 h5rdmtoolbox/wrapper/xr2hdf.py
-h5rdmtoolbox/wrapper/namespaces/__init__.py
-h5rdmtoolbox/wrapper/namespaces/_build.py
-h5rdmtoolbox/wrapper/namespaces/_codemeta_namespace.py
-h5rdmtoolbox/wrapper/namespaces/_m4i_namespace.py
-h5rdmtoolbox/wrapper/namespaces/_obo_namespace.py
-h5rdmtoolbox/wrapper/namespaces/_qudt_quantitykind_namespace.py
-h5rdmtoolbox/wrapper/namespaces/_qudt_unit_namespace.py
 tests/__init__.py
 tests/clean_zenodo_sandbox.py
 tests/test_config.py
 tests/test_extensions.py
 tests/test_identifiers.py
-tests/test_logger.py
 tests/test_plotting.py
 tests/test_repr.py
 tests/test_user.py
 tests/test_utils.py
 tests/test_version.py
 tests/test_xarray_export.py
 tests/conventions/__init__.py
 tests/conventions/test_conventions.py
+tests/conventions/test_engmeta.py
+tests/conventions/test_ontology.py
 tests/conventions/test_references.py
 tests/conventions/test_toolbox_validators.py
 tests/conventions/test_utils.py
 tests/conventions/standard_attributes/__init__.py
 tests/conventions/standard_attributes/test_standard_attributes.py
 tests/conventions/standard_attributes/test_standard_names.py
 tests/conventions/standard_attributes/standard_names/__init__.py
 tests/conventions/standard_attributes/standard_names/test_interface.py
 tests/conventions/standard_attributes/standard_names/test_provenance.py
 tests/conventions/standard_attributes/standard_names/test_snt.py
 tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py
 tests/database/__init__.py
-tests/database/notest_mongo_old.py
+tests/database/test_find_rdf.py
 tests/database/test_hdfDB.py
 tests/database/test_mongo.py
 tests/layouts/__init__.py
 tests/layouts/test_core.py
+tests/layouts/test_docs.py
 tests/repository/__init__.py
-tests/repository/test_metadatamapper.py
 tests/repository/test_zenodo.py
 tests/wrapper/__init__.py
 tests/wrapper/test_core.py
 tests/wrapper/test_dump.py
 tests/wrapper/test_file.py
 tests/wrapper/test_h5ext.py
+tests/wrapper/test_jsonld.py
+tests/wrapper/test_lazy.py
 tests/wrapper/test_namespaces.py
+tests/wrapper/test_rdf.py
 tests/wrapper/test_xr2df.py
```

### Comparing `h5rdmtoolbox-1.2.2/h5rdmtoolbox.egg-info/requires.txt` & `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 IPython>=7.34.0
 pyyaml>6.0
 xarray>=2022.3.0
 pint==0.21.1
 pint_xarray
 regex
 packaging
+ontolutils>=0.2.20
 python-forge
 requests
 pydantic>=2.3.0
 rdflib
 
 [complete]
+PyQt5
 pytest>=7.1.2
 pytest-cov
 pylint
 xmltodict
 scipy
 pandas
 tabulate
@@ -32,14 +34,15 @@
 sphinx-copybutton
 scikit-image
 scikit-learn
 sphinx-design
 simplejson
 myst-nb
 sphinxcontrib-bibtex
+kglab
 
 [csv]
 pandas
 
 [database]
 pymongo
 
@@ -60,14 +63,21 @@
 sphinx-copybutton
 scikit-image
 scikit-learn
 sphinx-design
 simplejson
 myst-nb
 sphinxcontrib-bibtex
+kglab
+
+[gui]
+PyQt5
+
+[layout_validation]
+tabulate
 
 [snt]
 xmltodict
 tabulate
 python-gitlab
 pypandoc
```

### Comparing `h5rdmtoolbox-1.2.2/setup.cfg` & `h5rdmtoolbox-1.3.0a1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,154 +1,142 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 3572 646d 746f 6f6c 626f 780d   = h5rdmtoolbox.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e32 2e32  .version = 1.2.2
-00000030: 0d0a 6175 7468 6f72 203d 204d 6174 7468  ..author = Matth
-00000040: 6961 7320 5072 6f62 7374 0d0a 6175 7468  ias Probst..auth
-00000050: 6f72 5f65 6d61 696c 203d 206d 6174 7468  or_email = matth
-00000060: 6961 732e 7072 6f62 7374 406b 6974 2e65  ias.probst@kit.e
-00000070: 6475 0d0a 6465 7363 7269 7074 696f 6e20  du..description 
-00000080: 3d20 5375 7070 6f72 7469 6e67 2061 2046  = Supporting a F
-00000090: 4149 5220 5265 7365 6172 6368 2044 6174  AIR Research Dat
-000000a0: 6120 6c69 6665 6379 636c 6520 7573 696e  a lifecycle usin
-000000b0: 6720 5079 7468 6f6e 2061 6e64 2048 4446  g Python and HDF
-000000c0: 352e 0d0a 6c6f 6e67 5f64 6573 6372 6970  5...long_descrip
-000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-000000e0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000120: 7073 3a2f 2f68 3572 646d 746f 6f6c 626f  ps://h5rdmtoolbo
-00000130: 782e 7265 6164 7468 6564 6f63 732e 696f  x.readthedocs.io
-00000140: 2f65 6e2f 6c61 7465 7374 2f0d 0a63 6c61  /en/latest/..cla
-00000150: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-00000160: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000170: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000180: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
-00000190: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001a0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
-000001b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001d0: 332e 3130 0d0a 0950 726f 6772 616d 6d69  3.10...Programmi
-000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001f0: 7974 686f 6e20 3a3a 2033 2e31 310d 0a09  ython :: 3.11...
-00000200: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000210: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000220: 3a20 332e 3132 0d0a 094c 6963 656e 7365  : 3.12...License
-00000230: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000240: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-00000250: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000260: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000270: 6465 6e74 0d0a 0944 6576 656c 6f70 6d65  dent...Developme
-00000280: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
-00000290: 2042 6574 610d 0a09 546f 7069 6320 3a3a   Beta...Topic ::
-000002a0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-000002b0: 6e65 6572 696e 670d 0a0d 0a5b 6f70 7469  neering....[opti
-000002c0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
-000002d0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-000002e0: 6571 7569 7265 7320 3d20 3e3d 332e 382c  equires = >=3.8,
-000002f0: 203c 332e 3133 0d0a 696e 636c 7564 655f   <3.13..include_
-00000300: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000310: 7275 650d 0a69 6e73 7461 6c6c 5f72 6571  rue..install_req
-00000320: 7569 7265 7320 3d20 0d0a 0961 7070 6469  uires = ...appdi
-00000330: 7273 203e 3d20 312e 342e 340d 0a09 696d  rs >= 1.4.4...im
-00000340: 706f 7274 6c69 625f 7265 736f 7572 6365  portlib_resource
-00000350: 730d 0a09 6e75 6d70 7920 3e3d 2031 2e32  s...numpy >= 1.2
-00000360: 300d 0a09 6835 7079 203e 2033 2e37 2e30  0...h5py > 3.7.0
-00000370: 0d0a 096d 6174 706c 6f74 6c69 6220 3e3d  ...matplotlib >=
-00000380: 2033 2e35 2e32 0d0a 0949 5079 7468 6f6e   3.5.2...IPython
-00000390: 203e 3d20 372e 3334 2e30 2020 2320 636f   >= 7.34.0  # co
-000003a0: 6c61 6220 7761 6e74 7320 372e 3334 2e30  lab wants 7.34.0
-000003b0: 0d0a 0970 7979 616d 6c20 3e20 362e 3020  ...pyyaml > 6.0 
-000003c0: 2023 2035 2e34 2064 6f65 7320 6e6f 7420   # 5.4 does not 
-000003d0: 776f 726b 2077 6974 6820 7079 7468 6f6e  work with python
-000003e0: 2033 2e31 3121 0d0a 0978 6172 7261 7920   3.11!...xarray 
-000003f0: 3e3d 2032 3032 322e 332e 300d 0a09 7069  >= 2022.3.0...pi
-00000400: 6e74 203d 3d20 302e 3231 2e31 2020 2320  nt == 0.21.1  # 
-00000410: 7069 6e74 203e 3d20 302e 3139 2e32 3c30  pint >= 0.19.2<0
-00000420: 2e32 322e 3020 4e6f 7465 3a20 302e 3232  .22.0 Note: 0.22
-00000430: 2e30 2073 686f 7773 2062 6164 2073 7472  .0 shows bad str
-00000440: 2d6f 7574 7075 7420 666f 7220 7175 616e  -output for quan
-00000450: 7469 7469 6573 2077 6974 6820 666f 726d  tities with form
-00000460: 6174 204c 787e 0d0a 0970 696e 745f 7861  at Lx~...pint_xa
-00000470: 7272 6179 2023 203e 3d20 302e 322e 310d  rray # >= 0.2.1.
-00000480: 0a09 7265 6765 7820 2320 3e3d 2032 3032  ..regex # >= 202
-00000490: 330d 0a09 7061 636b 6167 696e 670d 0a09  3...packaging...
-000004a0: 7079 7468 6f6e 2d66 6f72 6765 2023 203d  python-forge # =
-000004b0: 3d20 3138 2e36 2e30 0d0a 0972 6571 7565  = 18.6.0...reque
-000004c0: 7374 730d 0a09 7079 6461 6e74 6963 203e  sts...pydantic >
-000004d0: 3d20 322e 332e 300d 0a09 7264 666c 6962  = 2.3.0...rdflib
-000004e0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
-000004f0: 7261 735f 7265 7175 6972 655d 0d0a 6461  ras_require]..da
-00000500: 7461 6261 7365 203d 200d 0a09 7079 6d6f  tabase = ...pymo
-00000510: 6e67 6f20 2320 3e3d 2034 2e32 2e30 0d0a  ngo # >= 4.2.0..
-00000520: 6373 7620 3d20 0d0a 0970 616e 6461 7320  csv = ...pandas 
-00000530: 2320 3e3d 2031 2e34 2e33 0d0a 736e 7420  # >= 1.4.3..snt 
-00000540: 3d20 0d0a 0978 6d6c 746f 6469 6374 0d0a  = ...xmltodict..
-00000550: 0974 6162 756c 6174 6520 2320 3e3d 2030  .tabulate # >= 0
-00000560: 2e38 2e31 300d 0a09 7079 7468 6f6e 2d67  .8.10...python-g
-00000570: 6974 6c61 620d 0a09 7079 7061 6e64 6f63  itlab...pypandoc
-00000580: 2023 203e 3d20 312e 3131 0d0a 7465 7374   # >= 1.11..test
-00000590: 203d 200d 0a09 7079 7465 7374 203e 3d20   = ...pytest >= 
-000005a0: 372e 312e 320d 0a09 7079 7465 7374 2d63  7.1.2...pytest-c
-000005b0: 6f76 0d0a 0970 796c 696e 740d 0a09 786d  ov...pylint...xm
-000005c0: 6c74 6f64 6963 740d 0a09 7363 6970 7920  ltodict...scipy 
-000005d0: 2023 2070 726f 7669 6465 7320 6e65 7463   # provides netc
-000005e0: 6466 340d 0a09 2528 6373 7629 730d 0a09  df4...%(csv)s...
-000005f0: 2528 736e 7429 730d 0a09 2528 6461 7461  %(snt)s...%(data
-00000600: 6261 7365 2973 0d0a 646f 6373 203d 200d  base)s..docs = .
-00000610: 0a09 2528 6373 7629 730d 0a09 2528 736e  ..%(csv)s...%(sn
-00000620: 7429 730d 0a09 2528 6461 7461 6261 7365  t)s...%(database
-00000630: 2973 0d0a 0925 2874 6573 7429 730d 0a09  )s...%(test)s...
-00000640: 6a75 7079 7465 726c 6162 0d0a 0953 7068  jupyterlab...Sph
-00000650: 696e 7820 3e3d 2033 2c3c 350d 0a09 7370  inx >= 3,<5...sp
-00000660: 6869 6e78 5f62 6f6f 6b5f 7468 656d 6520  hinx_book_theme 
-00000670: 3d3d 2030 2e33 2e33 0d0a 0973 7068 696e  == 0.3.3...sphin
-00000680: 782d 636f 7079 6275 7474 6f6e 0d0a 0973  x-copybutton...s
-00000690: 6369 6b69 742d 696d 6167 650d 0a09 7363  cikit-image...sc
-000006a0: 696b 6974 2d6c 6561 726e 0d0a 0973 7068  ikit-learn...sph
-000006b0: 696e 782d 6465 7369 676e 0d0a 0973 696d  inx-design...sim
-000006c0: 706c 656a 736f 6e0d 0a09 6d79 7374 2d6e  plejson...myst-n
-000006d0: 620d 0a09 7370 6869 6e78 636f 6e74 7269  b...sphinxcontri
-000006e0: 622d 6269 6274 6578 0d0a 636f 6d70 6c65  b-bibtex..comple
-000006f0: 7465 203d 200d 0a09 2528 7465 7374 2973  te = ...%(test)s
-00000700: 0d0a 0925 2864 6f63 7329 730d 0a0d 0a5b  ...%(docs)s....[
-00000710: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-00000720: 6461 7461 5d0d 0a68 3572 646d 746f 6f6c  data]..h5rdmtool
-00000730: 626f 7820 3d20 0d0a 0964 6174 612f 2a2e  box = ...data/*.
-00000740: 7961 6d6c 0d0a 0964 6174 612f 2a2e 796d  yaml...data/*.ym
-00000750: 6c0d 0a09 6461 7461 2f54 6278 4c61 796f  l...data/TbxLayo
-00000760: 7574 2e68 6466 0d0a 0964 6174 612f 456d  ut.hdf...data/Em
-00000770: 7074 794c 6179 6f75 742e 6864 660d 0a09  ptyLayout.hdf...
-00000780: 6461 7461 2f73 7479 6c65 2e63 7373 0d0a  data/style.css..
-00000790: 0974 6573 7473 2f64 6174 612f 2a0d 0a09  .tests/data/*...
-000007a0: 636f 6e76 656e 7469 6f6e 732f 6874 6d6c  conventions/html
-000007b0: 2f74 656d 706c 6174 652e 6874 6d6c 0d0a  /template.html..
-000007c0: 0d0a 5b74 6f6f 6c3a 7079 7465 7374 5d0d  ..[tool:pytest].
-000007d0: 0a70 7974 686f 6e5f 6669 6c65 7320 3d20  .python_files = 
-000007e0: 7465 7374 5f2a 2e70 790d 0a74 6573 7470  test_*.py..testp
-000007f0: 6174 6873 203d 2074 6573 7473 0d0a 0d0a  aths = tests....
-00000800: 5b63 6f76 6572 6167 653a 7061 7468 735d  [coverage:paths]
-00000810: 0d0a 736f 7572 6365 203d 200d 0a09 7465  ..source = ...te
-00000820: 7374 730d 0a0d 0a5b 636f 7665 7261 6765  sts....[coverage
-00000830: 3a72 756e 5d0d 0a72 656c 6174 6976 655f  :run]..relative_
-00000840: 6669 6c65 7320 3d20 6661 6c73 650d 0a0d  files = false...
-00000850: 0a5b 636f 7665 7261 6765 3a72 6570 6f72  .[coverage:repor
-00000860: 745d 0d0a 6578 636c 7564 655f 6c69 6e65  t]..exclude_line
-00000870: 7320 3d20 0d0a 0970 7261 676d 613a 206e  s = ...pragma: n
-00000880: 6f20 636f 7665 720d 0a09 6465 6620 5f5f  o cover...def __
-00000890: 7265 7072 5f5f 0d0a 0940 6174 6578 6974  repr__...@atexit
-000008a0: 2e72 6567 6973 7465 720d 0a09 6578 6365  .register...exce
-000008b0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
-000008c0: 720d 0a09 7261 6973 6520 4e6f 7449 6d70  r...raise NotImp
-000008d0: 6c65 6d65 6e74 6564 4572 726f 720d 0a09  lementedError...
-000008e0: 6578 6365 7074 2054 7970 6545 7272 6f72  except TypeError
-000008f0: 0d0a 0972 6574 7572 6e20 6622 7b62 636f  ...return f"{bco
-00000900: 6c6f 7273 2e2a 0d0a 0964 6566 205f 6174  lors.*...def _at
-00000910: 7472 6962 7574 655f 7265 7072 5f68 746d  tribute_repr_htm
-00000920: 6c0d 0a09 6465 6620 5f67 726f 7570 5f72  l...def _group_r
-00000930: 6570 725f 6874 6d6c 0d0a 0964 6566 205f  epr_html...def _
-00000940: 6874 6d6c 5f72 6570 725f 6461 7461 7365  html_repr_datase
-00000950: 740d 0a09 6465 6620 6835 6669 6c65 5f68  t...def h5file_h
-00000960: 746d 6c5f 7265 7072 0d0a 0d0a 5b65 6767  tml_repr....[egg
-00000970: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000980: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000990: 2030 0d0a 0d0a                            0....
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e33 2e30  .version = 1.3.0
+00000030: 6131 0d0a 6175 7468 6f72 203d 204d 6174  a1..author = Mat
+00000040: 7468 6961 7320 5072 6f62 7374 0d0a 6175  thias Probst..au
+00000050: 7468 6f72 5f65 6d61 696c 203d 206d 6174  thor_email = mat
+00000060: 7468 6961 732e 7072 6f62 7374 406b 6974  thias.probst@kit
+00000070: 2e65 6475 0d0a 6465 7363 7269 7074 696f  .edu..descriptio
+00000080: 6e20 3d20 5375 7070 6f72 7469 6e67 2061  n = Supporting a
+00000090: 2046 4149 5220 5265 7365 6172 6368 2044   FAIR Research D
+000000a0: 6174 6120 6c69 6665 6379 636c 6520 7573  ata lifecycle us
+000000b0: 696e 6720 5079 7468 6f6e 2061 6e64 2048  ing Python and H
+000000c0: 4446 352e 0d0a 6c6f 6e67 5f64 6573 6372  DF5...long_descr
+000000d0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000e0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+000000f0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000100: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000110: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000120: 7474 7073 3a2f 2f68 3572 646d 746f 6f6c  ttps://h5rdmtool
+00000130: 626f 782e 7265 6164 7468 6564 6f63 732e  box.readthedocs.
+00000140: 696f 2f65 6e2f 6c61 7465 7374 2f0d 0a63  io/en/latest/..c
+00000150: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+00000160: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000170: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000180: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001a0: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001d0: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
+000001e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001f0: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
+00000200: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000220: 203a 3a20 332e 3132 0d0a 094c 6963 656e   :: 3.12...Licen
+00000230: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000240: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000250: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+00000260: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000270: 656e 6465 6e74 0d0a 0944 6576 656c 6f70  endent...Develop
+00000280: 6d65 6e74 2053 7461 7475 7320 3a3a 2034  ment Status :: 4
+00000290: 202d 2042 6574 610d 0a09 546f 7069 6320   - Beta...Topic 
+000002a0: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+000002b0: 6769 6e65 6572 696e 670d 0a0d 0a5b 6f70  gineering....[op
+000002c0: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
+000002d0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+000002e0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+000002f0: 382c 203c 332e 3133 0d0a 696e 636c 7564  8, <3.13..includ
+00000300: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+00000310: 2054 7275 650d 0a69 6e73 7461 6c6c 5f72   True..install_r
+00000320: 6571 7569 7265 7320 3d20 0d0a 0961 7070  equires = ...app
+00000330: 6469 7273 203e 3d20 312e 342e 340d 0a09  dirs >= 1.4.4...
+00000340: 696d 706f 7274 6c69 625f 7265 736f 7572  importlib_resour
+00000350: 6365 730d 0a09 6e75 6d70 7920 3e3d 2031  ces...numpy >= 1
+00000360: 2e32 300d 0a09 6835 7079 203e 2033 2e37  .20...h5py > 3.7
+00000370: 2e30 0d0a 096d 6174 706c 6f74 6c69 6220  .0...matplotlib 
+00000380: 3e3d 2033 2e35 2e32 0d0a 0949 5079 7468  >= 3.5.2...IPyth
+00000390: 6f6e 203e 3d20 372e 3334 2e30 2020 2320  on >= 7.34.0  # 
+000003a0: 636f 6c61 6220 7761 6e74 7320 372e 3334  colab wants 7.34
+000003b0: 2e30 0d0a 0970 7979 616d 6c20 3e20 362e  .0...pyyaml > 6.
+000003c0: 3020 2023 2035 2e34 2064 6f65 7320 6e6f  0  # 5.4 does no
+000003d0: 7420 776f 726b 2077 6974 6820 7079 7468  t work with pyth
+000003e0: 6f6e 2033 2e31 3121 0d0a 0978 6172 7261  on 3.11!...xarra
+000003f0: 7920 3e3d 2032 3032 322e 332e 300d 0a09  y >= 2022.3.0...
+00000400: 7069 6e74 203d 3d20 302e 3231 2e31 2020  pint == 0.21.1  
+00000410: 2320 7069 6e74 203e 3d20 302e 3139 2e32  # pint >= 0.19.2
+00000420: 3c30 2e32 322e 3020 4e6f 7465 3a20 302e  <0.22.0 Note: 0.
+00000430: 3232 2e30 2073 686f 7773 2062 6164 2073  22.0 shows bad s
+00000440: 7472 2d6f 7574 7075 7420 666f 7220 7175  tr-output for qu
+00000450: 616e 7469 7469 6573 2077 6974 6820 666f  antities with fo
+00000460: 726d 6174 204c 787e 0d0a 0970 696e 745f  rmat Lx~...pint_
+00000470: 7861 7272 6179 2023 203e 3d20 302e 322e  xarray # >= 0.2.
+00000480: 310d 0a09 7265 6765 7820 2320 3e3d 2032  1...regex # >= 2
+00000490: 3032 330d 0a09 7061 636b 6167 696e 670d  023...packaging.
+000004a0: 0a09 6f6e 746f 6c75 7469 6c73 3e3d 302e  ..ontolutils>=0.
+000004b0: 322e 3230 0d0a 0970 7974 686f 6e2d 666f  2.20...python-fo
+000004c0: 7267 6520 2320 3d3d 2031 382e 362e 300d  rge # == 18.6.0.
+000004d0: 0a09 7265 7175 6573 7473 0d0a 0970 7964  ..requests...pyd
+000004e0: 616e 7469 6320 3e3d 2032 2e33 2e30 0d0a  antic >= 2.3.0..
+000004f0: 0972 6466 6c69 620d 0a0d 0a5b 6f70 7469  .rdflib....[opti
+00000500: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+00000510: 7265 5d0d 0a64 6174 6162 6173 6520 3d20  re]..database = 
+00000520: 0d0a 0970 796d 6f6e 676f 2023 203e 3d20  ...pymongo # >= 
+00000530: 342e 322e 300d 0a6c 6179 6f75 745f 7661  4.2.0..layout_va
+00000540: 6c69 6461 7469 6f6e 203d 200d 0a09 7461  lidation = ...ta
+00000550: 6275 6c61 7465 0d0a 6373 7620 3d20 0d0a  bulate..csv = ..
+00000560: 0970 616e 6461 7320 2320 3e3d 2031 2e34  .pandas # >= 1.4
+00000570: 2e33 0d0a 736e 7420 3d20 0d0a 0978 6d6c  .3..snt = ...xml
+00000580: 746f 6469 6374 0d0a 0974 6162 756c 6174  todict...tabulat
+00000590: 6520 2320 3e3d 2030 2e38 2e31 300d 0a09  e # >= 0.8.10...
+000005a0: 7079 7468 6f6e 2d67 6974 6c61 620d 0a09  python-gitlab...
+000005b0: 7079 7061 6e64 6f63 2023 203e 3d20 312e  pypandoc # >= 1.
+000005c0: 3131 0d0a 6775 6920 3d20 0d0a 0950 7951  11..gui = ...PyQ
+000005d0: 7435 0d0a 7465 7374 203d 200d 0a09 7079  t5..test = ...py
+000005e0: 7465 7374 203e 3d20 372e 312e 320d 0a09  test >= 7.1.2...
+000005f0: 7079 7465 7374 2d63 6f76 0d0a 0970 796c  pytest-cov...pyl
+00000600: 696e 740d 0a09 786d 6c74 6f64 6963 740d  int...xmltodict.
+00000610: 0a09 7363 6970 7920 2023 2070 726f 7669  ..scipy  # provi
+00000620: 6465 7320 6e65 7463 6466 340d 0a09 2528  des netcdf4...%(
+00000630: 6373 7629 730d 0a09 2528 736e 7429 730d  csv)s...%(snt)s.
+00000640: 0a09 2528 6461 7461 6261 7365 2973 0d0a  ..%(database)s..
+00000650: 646f 6373 203d 200d 0a09 2528 6373 7629  docs = ...%(csv)
+00000660: 730d 0a09 2528 736e 7429 730d 0a09 2528  s...%(snt)s...%(
+00000670: 6461 7461 6261 7365 2973 0d0a 0925 2874  database)s...%(t
+00000680: 6573 7429 730d 0a09 6a75 7079 7465 726c  est)s...jupyterl
+00000690: 6162 0d0a 0953 7068 696e 7820 3e3d 2033  ab...Sphinx >= 3
+000006a0: 2c3c 350d 0a09 7370 6869 6e78 5f62 6f6f  ,<5...sphinx_boo
+000006b0: 6b5f 7468 656d 6520 3d3d 2030 2e33 2e33  k_theme == 0.3.3
+000006c0: 0d0a 0973 7068 696e 782d 636f 7079 6275  ...sphinx-copybu
+000006d0: 7474 6f6e 0d0a 0973 6369 6b69 742d 696d  tton...scikit-im
+000006e0: 6167 650d 0a09 7363 696b 6974 2d6c 6561  age...scikit-lea
+000006f0: 726e 0d0a 0973 7068 696e 782d 6465 7369  rn...sphinx-desi
+00000700: 676e 0d0a 0973 696d 706c 656a 736f 6e0d  gn...simplejson.
+00000710: 0a09 6d79 7374 2d6e 620d 0a09 7370 6869  ..myst-nb...sphi
+00000720: 6e78 636f 6e74 7269 622d 6269 6274 6578  nxcontrib-bibtex
+00000730: 0d0a 096b 676c 6162 0d0a 636f 6d70 6c65  ...kglab..comple
+00000740: 7465 203d 200d 0a09 2528 6775 6929 730d  te = ...%(gui)s.
+00000750: 0a09 2528 7465 7374 2973 0d0a 0925 2864  ..%(test)s...%(d
+00000760: 6f63 7329 730d 0a0d 0a5b 6f70 7469 6f6e  ocs)s....[option
+00000770: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
+00000780: 0a68 3572 646d 746f 6f6c 626f 7820 3d20  .h5rdmtoolbox = 
+00000790: 0d0a 0964 6174 612f 2a2e 7961 6d6c 0d0a  ...data/*.yaml..
+000007a0: 0964 6174 612f 2a2e 796d 6c0d 0a09 6461  .data/*.yml...da
+000007b0: 7461 2f2a 2e70 6e67 0d0a 0964 6174 612f  ta/*.png...data/
+000007c0: 5462 784c 6179 6f75 742e 6864 660d 0a09  TbxLayout.hdf...
+000007d0: 6461 7461 2f45 6d70 7479 4c61 796f 7574  data/EmptyLayout
+000007e0: 2e68 6466 0d0a 0964 6174 612f 7374 796c  .hdf...data/styl
+000007f0: 652e 6373 730d 0a09 7465 7374 732f 6461  e.css...tests/da
+00000800: 7461 2f2a 0d0a 0963 6f6e 7665 6e74 696f  ta/*...conventio
+00000810: 6e73 2f68 746d 6c2f 7465 6d70 6c61 7465  ns/html/template
+00000820: 2e68 746d 6c0d 0a0d 0a5b 746f 6f6c 3a70  .html....[tool:p
+00000830: 7974 6573 745d 0d0a 7079 7468 6f6e 5f66  ytest]..python_f
+00000840: 696c 6573 203d 2074 6573 745f 2a2e 7079  iles = test_*.py
+00000850: 0d0a 7465 7374 7061 7468 7320 3d20 7465  ..testpaths = te
+00000860: 7374 730d 0a0d 0a5b 6f70 7469 6f6e 732e  sts....[options.
+00000870: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+00000880: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+00000890: 200d 0a09 6835 7462 7820 3d20 6835 7264   ...h5tbx = h5rd
+000008a0: 6d74 6f6f 6c62 6f78 2e63 6c69 3a6d 6169  mtoolbox.cli:mai
+000008b0: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
+000008c0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000008d0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_interface.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import unittest
 import xarray as xr
-from h5rdmtoolbox.repository import zenodo
 
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox.convention.standard_names import HDF5StandardNameInterface
+from h5rdmtoolbox.repository import zenodo
 
 
 class TestStandardAttributes(unittest.TestCase):
 
     def setUp(self) -> None:
-        # cv = h5tbx.convention.from_zenodo(doi_or_recid=10156750, overwrite=True)
-        repo = zenodo.ZenodoRecord(10156750)
+        # cv = h5tbx.convention.from_zenodo(doi_or_recid=10428822, overwrite=True)
+        repo = zenodo.ZenodoRecord(10428822)
         cv = h5tbx.convention.from_repo(repo,
-                                         name='tutorial_convention.yaml',
-                                         take_existing=True)
+                                        name='tutorial_convention.yaml',
+                                        take_existing=True)
         cv.properties[h5tbx.File]['data_type'].make_optional()
         cv.properties[h5tbx.File]['contact'].make_optional()
         h5tbx.use(cv)
 
     def tearDown(self) -> None:
         h5tbx.use(None)
 
@@ -82,15 +82,15 @@
                               attach_scales=('y', 'x'))
             h5.create_dataset('grp/v', data=np.random.rand(3, 5),
                               standard_name='y_velocity',
                               units='m/s',
                               attach_scales=('y', 'x'))
         h5sni = HDF5StandardNameInterface.from_hdf(h5.hdf_filename)
         for c in h5sni.coordinate:
-            self.assertIsInstance(c, h5tbx.database.lazy.LDataset)
+            self.assertIsInstance(c, h5tbx.wrapper.lazy.LDataset)
         self.assertEqual(h5sni.coordinate.x, h5sni.coordinate[0])
         self.assertEqual(h5sni.coordinate.y, h5sni.coordinate[1])
         self.assertDictEqual({'x': 5, 'y': 3}, h5sni.coordinate.shape)
         self.assertEqual(2, h5sni.velocity.ndim)
 
     def test_interface_with_coords(self):
         with h5tbx.File(contact=h5tbx.__author_orcid__) as h5:
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_provenance.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_provenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
         except (requests.ConnectionError,
                 requests.Timeout) as e:
             self.connected = False
             warnings.warn('No internet connection', UserWarning)
 
         h5tbx.use(None)
 
-        # cv = h5tbx.convention.from_zenodo('https://zenodo.org/record/10156750',
+        # cv = h5tbx.convention.from_zenodo('https://zenodo.org/record/10428822',
         #                                    overwrite=True,
         #                                    force_download=True)
         from h5rdmtoolbox.repository.zenodo import ZenodoRecord
-        repo = ZenodoRecord(10156750)
+        repo = ZenodoRecord(10428822)
         cv = h5tbx.convention.from_repo(repo,
                                          name='tutorial_convention.yaml',
                                          take_existing=True,
                                          force_download=True)
-        # cv = h5tbx.convention.from_zenodo('https://zenodo.org/record/10156750',
+        # cv = h5tbx.convention.from_zenodo('https://zenodo.org/record/10428822',
         #                                    overwrite=True,
         #                                    force_download=True)
 
         h5tbx.use(cv)
         with h5tbx.File(data_type='experimental', contact=h5tbx.__author_orcid__) as h5:
             h5.create_dataset('time', data=np.linspace(0, 5, 5), standard_name='time', units='s', make_scale=True)
             h5.create_dataset('y', data=np.linspace(0, 10, 10), standard_name='y_coordinate', units='m',
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_snt.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_snt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+import pydantic
 import requests
 import unittest
 import warnings
+from pydantic import BaseModel
 
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox import tutorial
 from h5rdmtoolbox.convention.errors import StandardNameError
 from h5rdmtoolbox.convention.standard_names import parse_snt
 from h5rdmtoolbox.convention.standard_names.name import StandardName
-from h5rdmtoolbox.convention.standard_names.table import StandardNameTable
+from h5rdmtoolbox.convention.standard_names.table import StandardNameTable, parse_version
+from h5rdmtoolbox.convention.toolbox_validators import standardNameTableType
+from h5rdmtoolbox.convention.toolbox_validators import standardNameType
 
 
 class TestStandardAttributes(unittest.TestCase):
 
     def setUp(self) -> None:
         h5tbx.use(None)
         try:
-            requests.get('https://git.scc.kit.edu', timeout=5)
+            requests.get('https://www.google.com/', timeout=5)
             self.connected = True
         except (requests.ConnectionError,
                 requests.Timeout) as e:
             self.connected = False
             warnings.warn('No internet connection', UserWarning)
 
         self.snt = h5tbx.tutorial.get_standard_name_table()
@@ -45,14 +49,28 @@
             StandardName.check_syntax('123')
         self.assertDictEqual({'name': 'x_velocity', 'units': 'm/s', 'description': 'Velocity in x-direction.'},
                              sn.to_dict())
         self.assertFalse(sn.is_vector())
         snt = parse_snt(h5tbx.tutorial.get_standard_name_table_yaml_file())
         self.assertTrue(sn.check(snt))
 
+        class MyStandardName(BaseModel):
+            sn: standardNameType
+
+        with self.assertRaises(pydantic.ValidationError):
+            my_sn = MyStandardName(sn='x_velocity')
+        with self.assertRaises(TypeError):
+            my_sn = MyStandardName(sn=1.2)
+
+    def test_parse_version(self):
+        self.assertEqual(parse_version('v1.0.0'), 'v1.0.0')
+        self.assertEqual(parse_version('1.0.0'), '1.0.0')
+        self.assertEqual(parse_version('78'), '78.0.0')
+        self.assertEqual(parse_version('invalid'), 'invalid')
+
     def test_parse_snt(self):
         with self.assertRaises(TypeError):
             parse_snt(None)
         with self.assertRaises(TypeError):
             parse_snt(3.4)
         snt = parse_snt(self.snt)
         self.assertIsInstance(snt, StandardNameTable)
@@ -62,16 +80,15 @@
         self.assertIsInstance(snt, StandardNameTable)
         snt = parse_snt(str(h5tbx.tutorial.get_standard_name_table_yaml_file()))
         self.assertIsInstance(snt, StandardNameTable)
 
     def test_snt_cache(self):
         """caching of SNTs only works if they are zenodo references"""
         cv = h5tbx.convention.Convention(name='test', contact='me', institution='mine', decoders=())
-        from h5rdmtoolbox.convention.toolbox_validators import standardNameTableType
-        from pydantic import BaseModel
+
         class standard_name_table_validator(BaseModel):
             """The standard name table of the convention."""
             value: standardNameTableType
 
         sa = h5tbx.convention.standard_attributes.StandardAttribute(
             name='snt',
             validator=standard_name_table_validator,
@@ -100,14 +117,15 @@
                               })
 
         snt = StandardNameTable('test', version='v1.0.0', meta={},
                                 standard_names={'x_velocity': {
                                     'units': 'm/s', 'description': 'x velocity.', 'alias': 'u'},
                                     'y_velocity': {'canonical_units': 'm/s', 'description': 'y velocity', 'alias': 'v'}
                                 })
+        self.assertListEqual(snt.names, ['x_velocity', 'y_velocity'])
         self.assertEqual('x velocity.', snt['x_velocity'].description)
         self.assertEqual('y velocity.', snt['y_velocity'].description)
 
         self.assertEqual({'u': 'x_velocity', 'v': 'y_velocity'}, snt.aliases)
         self.assertEqual('v1.0.0', snt.version)
 
         self.assertIn('x_velocity', snt)
@@ -213,14 +231,26 @@
                                                         'z': {'description': 'z coordinate'}}),
                                 meta=dict(institution='my_institution',
                                           contact='https://orcid.org/0000-0001-8729-0482'))
         snt_dict = snt.to_dict()
         self.assertIn('standard_names', snt_dict)
         self.assertIn('affixes', snt_dict)
 
+    def test_to_markdown(self):
+        with open(self.snt.to_markdown(h5tbx.utils.generate_temporary_filename(suffix='.md'))) as f:
+            lines = f.readlines()
+        for line in lines:
+            print(line.strip())
+        self.assertEqual(lines[1].strip(), 'title: Standard Name Table for Fan simulations and measurements')
+        self.assertEqual(lines[6].strip(), '| Standard Name |     units     | Description |')
+        self.assertEqual(lines[8].strip(),
+                         '| time | s | Time refers to the relative time since start of data acquisition. |')
+        for line in lines:
+            (line.strip())
+
     def test_to_from_yaml(self):
         snt = StandardNameTable(name='test_snt',
                                 standard_names={'x_velocity': {'units': 'm/s', 'description': 'x velocity'}},
                                 version='v1.0.0-beta',
                                 affixes=dict(component={'description': 'test component',
                                                         'x': {'description': 'x coordinate'},
                                                         'y': {'description': 'y coordinate'},
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/test_standard_attributes.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_attributes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Testing the standard attributes"""
 import pint
 import unittest
 from typing import Union
 
 import h5rdmtoolbox as h5tbx
+from h5rdmtoolbox.convention.consts import DefaultValue
 from h5rdmtoolbox.convention.standard_attributes import StandardAttribute
 
 
 class TestStandardAttributes(unittest.TestCase):
 
     @staticmethod
     def assertPintUnitEqual(unit1: [str, pint.Unit], unit2: Union[str, pint.Unit]):
@@ -21,12 +22,39 @@
         self.assertIsInstance(sa.name, str)
         self.assertIsInstance(sa.description, str)
         self.assertIsInstance(sa.is_positional(), bool)
         self.assertIsInstance(sa.target_method, str)
 
     def test_standard_attribute_basics(self):
         with self.assertRaises(TypeError):
-            test = StandardAttribute('test',
-                                     validator={'$type': 'string'},
-                                     target_method='create_dataset',
-                                     description='A test',
-                                     )
+            StandardAttribute('test',
+                              validator={'$type': 'string'},
+                              target_method=3.4,
+                              description='A test',
+                              )
+
+        with self.assertRaises(ValueError):
+            StandardAttribute('test',
+                              validator={'$type': 'string'},
+                              target_method='create_dataset2',
+                              description='A test',
+                              )
+
+        test = StandardAttribute('test',
+                                 validator={'$type': 'string'},
+                                 target_method='create_dataset',
+                                 description='A test',
+                                 default_value='none'
+                                 )
+        self.assertEqual(test.default_value, None)
+
+        test = StandardAttribute('test',
+                                 validator={'$type': 'string'},
+                                 target_method='create_dataset',
+                                 description='A test',
+                                 alternative_standard_attribute='alternative',
+                                 default_value='$empty'
+                                 )
+        self.assertEqual(test.default_value, DefaultValue.EMPTY)
+        self.assertEqual(test.alternative_standard_attribute, 'alternative')
+
+        self.assertFalse(test.is_obligatory())
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/standard_attributes/test_standard_names.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         self.assertTrue(table['velocity'].is_vector())
         with self.assertRaises(h5tbx.errors.StandardNameError):
             table['x_pressure']
         self.assertIsInstance(table['derivative_of_x_coordinate_wrt_x_velocity'], StandardName)
 
         table['x_velocity_in_stationary_frame']
 
-
     def test_StandardNameTableFromWeb(self):
         try:
             import xmltodict
             xmltodict_exists = True
         except ImportError:
             xmltodict_exists = False
             warnings.warn('xmltodict not installed. Cannot test "test_StandardNameTableFromWeb"', UserWarning)
@@ -220,15 +219,15 @@
 
     def test_from_zenodo(self):
         if self.connected:
             snt = StandardNameTable.from_zenodo(doi_or_recid=10428795)
             self.assertIsInstance(snt, StandardNameTable)
             filename = h5tbx.UserDir['standard_name_tables'] / f'10428795.yaml'
             self.assertTrue(filename.exists())
-            filename.unlink(missing_ok=True)
+            # filename.unlink(missing_ok=True)
 
     def test_from_yaml(self):
         cv = h5tbx.convention.from_yaml(tutorial.get_standard_attribute_yaml_filename(), overwrite=True)
         h5tbx.use(cv)
 
         with h5tbx.File(contact='https://orcid.org/0000-0001-8729-0482', data_type='numerical') as h5:
             with self.assertRaises(StandardAttributeError):
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/test_conventions.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/test_conventions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import appdirs
 import h5py
+import logging
 import pathlib
 import pint
 import requests
 import shutil
 import sys
 import unittest
 import warnings
@@ -11,37 +12,37 @@
 from datetime import datetime
 
 import h5rdmtoolbox
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox import convention
 from h5rdmtoolbox import tutorial
 from h5rdmtoolbox.convention import core
-from h5rdmtoolbox.convention.core import InvalidAttribute
-from h5rdmtoolbox.convention.core import MissingAttribute
+from h5rdmtoolbox.convention.core import InvalidAttribute, MissingAttribute
 from h5rdmtoolbox.convention.standard_names.table import StandardNameTable
 from h5rdmtoolbox.repository.zenodo import ZenodoSandboxDeposit
 from h5rdmtoolbox.repository.zenodo.metadata import Metadata, Creator
 
+logger = logging.getLogger('h5rdmtoolbox')
+# setting logger to debug:
+logger.setLevel('DEBUG')
 __this_dir__ = pathlib.Path(__file__).parent
 
 
 class TestConventions(unittest.TestCase):
 
     def setUp(self) -> None:
         try:
             requests.get('https://git.scc.kit.edu', timeout=5)
             self.connected = True
         except (requests.ConnectionError,
                 requests.Timeout) as e:
             self.connected = False
             warnings.warn('No internet connection', UserWarning)
 
-        # setting logger to debug:
-        from h5rdmtoolbox.convention import logger
-        logger.setLevel('DEBUG')
+
 
     def test_list_of_validators(self):
         lov = convention.get_list_of_validators()
         self.assertIsInstance(lov, dict)
         self.assertTrue(len(lov) > 0)
 
     def test_create_with_code(self):
@@ -154,15 +155,15 @@
         r = extract_function_info(tree)
         with self.assertRaises(ValueError):
             validate_specialtype_functions({r[0][0]: r[0][1]})
 
     def test_h5tbx(self):
         f = h5tbx.UserDir['convention'] / 'h5tbx' / 'h5tbx.py'
         f.unlink(missing_ok=True)
-        from h5rdmtoolbox.convention._h5tbx import build_convention
+        from h5rdmtoolbox.convention import build_convention
         build_convention()
 
         h5tbx.use('h5tbx')
         cv = h5tbx.convention.get_current_convention()
 
         self.assertEqual('h5tbx', h5tbx.convention.get_current_convention().name)
 
@@ -207,15 +208,15 @@
         self.assertTupleEqual(('scale_and_offset',), cv.decoders)
         self.assertIn('comment', cv.properties[h5tbx.File])
         self.assertIn('comment', cv.properties[h5tbx.Group])
 
     def test_overwrite_existing_file(self):
         if self.connected:
             # delete an existing convention like this first:
-            h5tbx.convention.from_zenodo(doi_or_recid='10156750', overwrite=False)
+            h5tbx.convention.from_zenodo(doi_or_recid='10428822', overwrite=False)
             # h5tbx.convention.from_yaml('test_convention.yaml')
             h5tbx.use('h5rdmtoolbox-tutorial-convention')
 
             with h5tbx.File(mode='w',
                             attrs=dict(
                                 data_type='experimental',
                                 contact='https://orcid.org/0000-0001-8729-0482'),
@@ -528,37 +529,14 @@
                 h5.contact  # takes a bit because validated online!
                 snt = h5.standard_name_table
                 self.assertIsInstance(snt, h5tbx.convention.standard_names.StandardNameTable)
                 for sa in h5.standard_attributes:
                     self.assertFalse('-' in sa)
                 self.assertNotEqual(h5.standard_attributes['comment'].description,
                                     h5['test'].standard_attributes['comment'].description)
-            if False:
-                self.assertEqual(cv.name, 'h5rdmtoolbox-tutorial-convention')
-                self.assertEqual(
-                    h5tbx.convention.standard_attributes.DefaultValue.EMPTY,
-                    cv.properties[h5tbx.File]['data_type'].default_value
-                )
-                cv.properties[h5tbx.File]['data_type'].make_optional()
-                self.assertEqual(
-                    h5tbx.convention.standard_attributes.DefaultValue.NONE,
-                    cv.properties[h5tbx.File]['data_type'].default_value
-                )
-
-                # we can download from zenodo by passing the short or full DOI or the URL:
-
-                dois = ('10156750', '10.5281/zenodo.10156750', 'https://zenodo.org/record/10156750',
-                        'https://doi.org/10.5281/zenodo.10156750')
-                h5tbx.UserDir.clear_cache()
-                with self.assertRaises(ValueError):  # because it is not a standard attribute YAML file!
-                    cv = h5tbx.convention.from_zenodo(doi=10428795)
-
-                for doi in dois:
-                    cv = h5tbx.convention.from_zenodo(doi=doi)
-                    self.assertEqual(cv.name, 'h5rdmtoolbox-tutorial-convention')
 
     def test_default_value(self):
         from h5rdmtoolbox.convention.consts import DefaultValue
         d = DefaultValue('$none')
         self.assertEqual(d.value, DefaultValue.NONE)
         d = DefaultValue('$empty')
         self.assertEqual(d.value, DefaultValue.EMPTY)
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/test_references.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/test_references.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/test_toolbox_validators.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/test_toolbox_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,23 +59,25 @@
         self.assertEqual(r'"^[a-zA-Z0-9_]*$"', rp.re_pattern)
 
         rp = RegexProcessor({r'validator': r'$regex(^[a-zA-Z].*(?<!\s)$)'})
         self.assertEqual(r'^[a-zA-Z].*(?<!\s)$', rp.re_pattern)
 
     def test_validate_identifier(self):
         class Identifier(BaseModel):
-            ident: toolbox_validators.identifierType
+            identifier: toolbox_validators.identifierType
 
         with self.assertRaises(ValueError):
             Identifier(orcid=3.4)
+        with self.assertRaises(TypeError):
+            Identifier(identifier=3.4)
         with self.assertRaises(pydantic.ValidationError):
-            Identifier(ident='0000-0001-8729-0482')
-        Identifier(ident='https://orcid.org/0000-0002-1825-0097')
+            Identifier(identifier='0000-0001-8729-0482')
+        Identifier(identifier='https://orcid.org/0000-0002-1825-0097')
         with self.assertRaises(pydantic.ValidationError):
-            Identifier(ident='https://orcid.org/0000-0002-1825-0096')  # invalid orcid due to checksum
+            Identifier(identifier='https://orcid.org/0000-0002-1825-0096')  # invalid orcid due to checksum
 
     def test_validate_orcid(self):
         class Validator(BaseModel):
             orcid: toolbox_validators.orcidType
 
         with self.assertRaises(TypeError):
             Validator(orcid=3.4)
@@ -107,23 +109,30 @@
             quantity: toolbox_validators.quantityType
 
         Validator(quantity=pint.Quantity(3.4, 'm'))
         self.assertIsInstance(Validator(quantity=pint.Quantity(3.4, 'm')).quantity, pint.Quantity)
         self.assertIsInstance(Validator(quantity='3.3 m').quantity, pint.Quantity)
         self.assertEqual(Validator(quantity='3.3 m').quantity.magnitude, 3.3)
 
+        with self.assertRaises(ValueError):
+            Validator(quantity='3.4 kilo meter')
+
     def test_validate_units(self):
         class Validator(BaseModel):
             units: toolbox_validators.unitsType
 
         Validator(units=pint.Unit('m'))
         self.assertIsInstance(Validator(units=pint.Unit('m')).units, pint.Unit)
         self.assertIsInstance(Validator(units='m').units, pint.Unit)
 
+        with self.assertRaises(pydantic.ValidationError):
+            Validator(units={'unit': 'm'})
+
     def test_date_format(self):
         class Validator(BaseModel):
             date: toolbox_validators.dateFormatType
 
         self.assertIsInstance(Validator(date='2021-01-01').date,
                               datetime.datetime)
+
         with self.assertRaises(TypeError):
             Validator(date=3.4)
```

### Comparing `h5rdmtoolbox-1.2.2/tests/conventions/test_utils.py` & `h5rdmtoolbox-1.3.0a1/tests/conventions/test_utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/tests/database/notest_mongo_old.py` & `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,253 +1,394 @@
-import datetime
+"""test_file.py"""
+import h5py
 import numpy as np
+import pathlib
+import time
 import unittest
-import warnings
+import uuid
+import yaml
+from datetime import datetime
+from pathlib import Path
 
 import h5rdmtoolbox as h5tbx
-from h5rdmtoolbox import File
 from h5rdmtoolbox import tutorial
 from h5rdmtoolbox import use
+from h5rdmtoolbox.utils import generate_temporary_filename
+from h5rdmtoolbox.wrapper.core import File
 
-try:
-    # noinspection PyUnresolvedReferences
-    from h5rdmtoolbox.database import mongo
-    import pymongo.collection
-    from pymongo import MongoClient
-
-    mongo_installed = True
-except ImportError:
-    mongo_installed = False
-from h5rdmtoolbox.database.mongo import make_dict_mongo_compatible, type2mongo
-
-if mongo_installed:
-    class TestH5Mongo(unittest.TestCase):
-
-        def setUp(self) -> None:
-            use(None)
-            self.mongodb_running = True
-            try:
-                client = MongoClient(serverSelectionTimeoutMS=1.)
-                client.server_info()
-                mongodb_av = True
-            except pymongo.errors.ServerSelectionTimeoutError as err:
-                mongodb_av = False
-                warnings.warn('Cannot test mongoDB features as no mongodb server is running!')
-
-            if mongodb_av:
-                db = client['h5tbx_test_db']
-                collection = db['test']
-                self.collection = collection
-            else:
-                self.mongodb_running = False
-
-        def test_make_dict_mongo_compatible(self):
-            self.assertDictEqual({'a': 4.3}, make_dict_mongo_compatible({'a': 4.3}))
-            self.assertDictEqual({'a': 4}, make_dict_mongo_compatible({'a': 4}))
-            self.assertDictEqual({'a': None}, make_dict_mongo_compatible({'a': None}))
-            self.assertDictEqual({'a': {'b': 5.3}}, make_dict_mongo_compatible({'a': {'b': 5.3}}))
-            self.assertDictEqual({'a': {'b': 6.3}}, make_dict_mongo_compatible({'a': {'b': float(6.3)}}))
-
-        def test_type2mongo(self):
-            self.assertEqual(None, type2mongo(None))
-            self.assertEqual(4.3, type2mongo(float(4.3)))
-            self.assertEqual([2.3], type2mongo(np.array([2.3])))
-            self.assertEqual([5, ], type2mongo(np.array([5])))
-
-        def test_insert_relative_filename(self):
-            if self.mongodb_running:
-                self.collection.drop()
-                with File() as h5:
-                    h5tbx.MongoDB.insert_group()
-                    h5.mongo.insert(collection=self.collection)
-                    self.assertEqual(self.collection.find_one({})['filename'], h5.filename)
-                    self.collection.drop()
-                with File() as h5:
-                    h5.mongo.insert(collection=self.collection, use_relative_filename=True)
-                    self.assertEqual(self.collection.find_one({})['filename'], h5.filename)
-
-        def test_coordinates(self):
-            if self.mongodb_running:
-                self.collection.drop()
-                with File() as h5:
-                    h5.create_dataset('x', data=np.arange(0, 4, 1), dtype=int,
-                                      attrs=dict(units='', long_name='x_coordinate'), make_scale=True)
-                    h5.create_dataset('y', data=np.arange(0, 4, 1), dtype=int,
-                                      attrs=dict(units='', long_name='y_coordinate'), make_scale=True)
-                    h5.create_dataset('z', data=2, dtype=int,
-                                      attrs=dict(units='', long_name='z_coordinate'))
-                    h5.create_dataset('images', data=np.random.random((4, 4, 4)),
-                                      attrs=dict(units='counts', long_name='a long name'),
-                                      attach_scales=([h5['x'], h5['y']], None, None))
-                    h5['images'].attrs['COORDINATES'] = ['/z', ]
-                    h5.images.mongo.insert(collection=self.collection, axis=None)
-
-        def test_insert_tree_structure(self):
-            if self.mongodb_running:
-                self.collection.drop()
-                with File() as h5:
-                    h5.create_dataset('ds_at_root', data=np.random.random((2, 10, 8)),
-                                      attrs=dict(units='',
-                                                 long_name='ds_at_root'))
-                    g = h5.create_group('group1')
-                    g.create_dataset('ds1', data=np.random.random((2, 10, 8)),
-                                     attrs=dict(units='',
-                                                long_name='ds_at_group1'))
-                    g2 = g.create_group('group2')
-                    g2.create_dataset('ds2', data=np.random.random((2, 10, 8)),
-                                      attrs=dict(units='',
-                                                 long_name='ds_at_group2'))
-                    h5.mongo.insert(collection=self.collection, flatten_tree=False, recursive=True)
-                    self.assertDictEqual(list(self.collection.find({}))[0]['group1'], {'ds1': {'shape': [2, 10, 8],
-                                                                                               'ndim': 3,
-                                                                                               'long_name': 'ds_at_group1',
-                                                                                               'units': ''},
-                                                                                       'group2': {
-                                                                                           'ds2': {'shape': [2, 10, 8],
-                                                                                                   'ndim': 3,
-                                                                                                   'long_name': 'ds_at_group2',
-                                                                                                   'units': ''}}})
-
-        def test_tree_to_mongo(self):
-            if self.mongodb_running:
-                self.collection.drop()
-
-                usernames = ('Allen', 'Mike', 'Ellen', 'Elliot')
-                company = ('bikeCompany', 'shoeCompany', 'bikeCompany', 'shoeCompany')
-                filenames = []
-                for i, (username, company) in enumerate(zip(usernames, company)):
-                    with File(h5tbx.utils.generate_temporary_filename(), 'w') as h5:
-                        filenames.append(h5.hdf_filename)
-                        h5.attrs['username'] = username
-                        h5.attrs['company'] = company
-                        h5.attrs['meta'] = {'day': 'monday', 'iday': 0}
-                        h5.create_dataset('ds_at_root', data=np.random.random((2, 10, 8)),
-                                          attrs=dict(units='',
-                                                     long_name='ds_at_root'))
-                        h5['ds_at_root'].make_scale()
-                        g = h5.create_group('idgroup')
-                        ds = g.create_dataset('ds_at_subgroup', data=np.random.random((2, 10, 13)),
-                                              attrs=dict(units='',
-                                                         long_name='ds_at_subgroup'))
-                        ds.dims[0].attach_scale(h5['ds_at_root'])
-                        ds.attrs['id'] = i
-
-                with File(filenames[0]) as h5:
-                    tree = h5.get_tree_structure(True)
-                self.collection.insert_one(make_dict_mongo_compatible(tree))
-
-        def test_insert_dataset(self):
-            if self.mongodb_running:
-                self.collection.drop()
-                with File() as h5:
-                    hdf_filename = h5.hdf_filename
-                    h5.create_dataset('z', data=2, dtype=int,
-                                      attrs=dict(units='', long_name='z_coordinate'))
-                    h5.create_dataset('index', data=np.arange(0, 4, 1), dtype=int,
-                                      attrs=dict(units='', long_name='index'), make_scale=True)
-                    h5.create_dataset('index2', data=np.arange(0, 4, 1), dtype=int,
-                                      attrs=dict(units='', long_name='index'), make_scale=True)
-                    h5.create_dataset('index3', data=np.arange(0, 4, 1), dtype=int,
-                                      attrs=dict(units='', long_name='index'), make_scale=False)
-                    h5.create_dataset('images', data=np.random.random((4, 11, 21)),
-                                      attrs=dict(units='counts', long_name='a long name'),
-                                      attach_scales=([h5['index'], h5['index2']], None, None))
-                    h5['images'].attrs['COORDINATES'] = ['/z', ]
-                    h5['images'].attrs['None'] = None
-                    h5.attrs['np_ndarray'] = np.array([1.2, -2.3])
-                    h5['images'].attrs['np_ndarray'] = np.array([1.2, -2.3])
-                    h5['images'].attrs['float'] = 1.2
-                    h5['images'].attrs['np_float'] = np.float64(1.2)
-
-                    h5.images.mongo.insert(axis=0, collection=self.collection)
-
-                res = self.collection.find()
-
-                now = datetime.datetime.utcnow()
-
-                for r in res:
-                    if r['name'] == 'images':
-                        self.assertEqual(r['filename'], str(hdf_filename))
-                        for k in (
-                                'filename', 'path', 'shape', 'ndim', 'slice', 'index', 'index2', 'z', 'long_name',
-                                'units'):
-                            self.assertIn(k, r.keys())
-
-                    self.assertTrue((now - r['file_creation_time']).total_seconds() < 1)
-
-                self.collection.drop()
-                with File(hdf_filename) as h5:
-                    h5.images.mongo.insert(axis=0, collection=self.collection, dims=(h5['/index'],))
-                res = self.collection.find()
-                for r in res:
-                    self.assertIn('index', r.keys())
-                    self.assertIn('index2', r.keys())
-                    self.assertNotIn('index3', r.keys())
-
-                self.collection.drop()
-                with File(hdf_filename) as h5:
-                    h5.images.mongo.insert(axis=0, collection=self.collection, dims=(h5['/index'], h5['/index2']))
-                res = self.collection.find()
-                for r in res:
-                    self.assertIn('index', r.keys())
-                    self.assertIn('index2', r.keys())
-                    self.assertNotIn('index3', r.keys())
-
-                self.collection.drop()
-                with File(hdf_filename) as h5:
-                    h5.images.mongo.insert(axis=0, collection=self.collection, dims=(h5['/index3'],))
-                res = self.collection.find()
-                for r in res:
-                    self.assertIn('index', r.keys())
-                    self.assertIn('index2', r.keys())
-                    self.assertIn('index3', r.keys())
-
-        def test_insert_dataset_update(self):
-            if self.mongodb_running:
-                self.collection.drop()
-                with File() as h5:
-                    hdf_filename = h5.hdf_filename
-                    h5.create_dataset('z', data=2, dtype=int,
-                                      attrs=dict(units='', long_name='z_coordinate'))
-                    for i in range(3):
-                        h5.z.mongo.insert(axis=None, collection=self.collection, update=True)
-                    self.assertEqual(self.collection.count_documents({}), 1)
-                    for i in range(3):
-                        h5.z.mongo.insert(axis=None, collection=self.collection, update=False)
-                    self.assertEqual(self.collection.count_documents({}), 4)
-                    for r in self.collection.find({}):
-                        self.assertEqual(r['filename'], str(h5.hdf_filename))
-                        self.assertEqual(r['name'], '/z')
-
-        def test_insert_group(self):
-            if self.mongodb_running:
-                self.collection.drop()
-                with File() as h5:
-                    h5.attrs['rootatr'] = 1
-                    h5.attrs['str'] = 'test'
-
-                    h5.create_dataset('dataset', data=[1, 2, 3],
-                                      attrs=dict(units='m/s', long_name='a velocity'))
-
-                    g = h5.create_group('a_group')
-                    g.attrs['a'] = 1
-                    g.attrs['str'] = 'test'
-
-                    self.collection.drop()
-                    h5.mongo.insert(self.collection)
-
-                    self.assertEqual(self.collection.count_documents({}), 2)
-                    now = datetime.datetime.now()
-                    for r in self.collection.find({}):
-                        self.assertTrue((now - r['file_creation_time']).total_seconds() < 1)
-
-        def test_insert_group_flatten(self):
-            if self.mongodb_running:
-                self.collection.drop()
-
-                repo_filenames = tutorial.database.generate_test_files()
-                for fname in repo_filenames:
-                    with File(fname) as h5:
-                        h5.mongo.insert(collection=self.collection, recursive=True, flatten_tree=True)
-                now = datetime.datetime.now() - datetime.timedelta(minutes=1)
-                for r in self.collection.find({}):
-                    self.assertTrue((now - r['file_creation_time']).total_seconds() < 20)
+
+class TestFile(unittest.TestCase):
+
+    def setUp(self) -> None:
+        """setup"""
+        use(None)
+        with File(mode='w') as h5:
+            h5.attrs['one'] = 1
+            g = h5.create_group('grp_1')
+            g.attrs['one'] = 1
+            h5.attrs['two'] = 2
+            h5.attrs['three'] = 3
+            h5.create_dataset('ds', shape=(4,), attrs=dict(one=1))
+            h5.create_group('grp_2')
+            h5.create_group('grp_3')
+            h5.create_group('grp_X')
+            h5.create_dataset('ds1', shape=(3,))
+            h5.create_dataset('ds2', shape=(3,))
+            h5.create_dataset('dsY', shape=(3,))
+            self.test_filename = h5.hdf_filename
+
+        self.lay_filename = generate_temporary_filename(prefix='lay', suffix='.hdf')
+        self.other_filename = generate_temporary_filename(prefix='other', suffix='.hdf')
+
+    def tearDown(self) -> None:
+        for fname in Path(__file__).parent.glob('*'):
+            if fname.suffix not in ('py', '.py', '.yaml'):
+                if fname.is_file():
+                    fname.unlink()
+
+    def test_filename(self):
+        with h5tbx.File() as h5:
+            with self.assertRaises(AttributeError):
+                h5.hdf_filename = 3
+        self.assertIsInstance(h5.hdf_filename, pathlib.Path)
+        self.assertTrue(h5.hdf_filename.exists())
+        h5tbx.clean_temp_data()
+        with self.assertRaises(FileNotFoundError):
+            h5.hdf_filename.exists()
+
+        if pathlib.Path('test.hdf').exists():
+            # just in case ...
+            pathlib.Path('test.hdf').unlink()
+        with h5tbx.File('test.hdf', 'w') as h5:
+            self.assertEqual('r+', h5.mode)
+            self.assertEqual('test.hdf', h5.hdf_filename.name)
+        if h5.hdf_filename.exists():
+            h5.hdf_filename.unlink()
+
+    def test_reopen_file(self):
+        cv_yaml_filename = tutorial.get_standard_attribute_yaml_filename()
+        cv = h5tbx.convention.from_yaml(cv_yaml_filename, overwrite=True)
+        h5tbx.use(cv)
+        with h5tbx.File(data_type='experimental',
+                        contact=h5tbx.__author_orcid__) as h5:
+            pass
+        # reopen file with read-only mode works fine
+        with h5tbx.File(h5.hdf_filename, 'r') as h5:
+            self.assertTrue('data_type' in h5.attrs.raw)
+            self.assertTrue('contact' in h5.attrs.raw)
+
+        # reopen file with read-write mode must also. the mandatory root attributes are set earlier...
+        with h5tbx.File(h5.hdf_filename, 'r+') as h5:
+            self.assertTrue('data_type' in h5.attrs.raw)
+            self.assertTrue('contact' in h5.attrs.raw)
+
+    def test_dumps(self):
+        with h5tbx.File() as h5:
+            h5.dumps()
+
+    def test_create_dataset(self):
+        """File has more parameters to pass as H5Base"""
+        with File() as h5:
+            ds = h5.create_dataset('u', shape=())
+            self.assertEqual(ds.name, '/u')
+
+    def test_uuid4(self):
+        with File() as h5:
+            uuid4 = uuid.uuid4()
+            h5.attrs.write_uuid(uuid4)
+            self.assertEqual(h5.attrs['uuid'], str(uuid4))
+            h5.attrs.write_uuid(uuid4, name='uuid4')
+            self.assertEqual(h5.attrs['uuid4'], str(uuid4))
+            with self.assertRaises(ValueError):
+                h5.attrs.write_uuid(overwrite=False)
+            with self.assertRaises(ValueError):
+                h5.attrs.write_uuid(uuid4, name='uuid4', overwrite=False)
+            uuid4new = uuid.uuid4()
+            h5.attrs.write_uuid(uuid4new, name='uuid4', overwrite=True)
+            self.assertNotEqual(h5.attrs['uuid4'], str(uuid4))
+            self.assertEqual(h5.attrs['uuid4'], str(uuid4new))
+            h5.attrs.write_uuid(overwrite=True)
+            self.assertNotEqual(h5.attrs['uuid'], str(uuid4))
+            self.assertNotEqual(h5.attrs['uuid'], str(uuid4new))
+
+    def test_timestamp(self):
+        with File() as h5:
+            h5.attrs.write_iso_timestamp()
+            self.assertIsInstance(h5.attrs['timestamp'], str)
+            h5.attrs.write_iso_timestamp(name='timestamp2')
+            dt2 = h5.attrs['timestamp2']
+            self.assertIsInstance(dt2, str)
+            with self.assertRaises(ValueError):
+                h5.attrs.write_iso_timestamp(name='timestamp2', overwrite=False)
+            time.sleep(0.01)
+            h5.attrs.write_iso_timestamp(name='timestamp2', overwrite=True)
+            self.assertNotEqual(dt2, h5.attrs['timestamp2'])
+
+            dtnow = datetime.now()
+            dtnow_iso = dtnow.isoformat()
+            time.sleep(0.01)
+            h5.attrs.write_iso_timestamp(name='now', dt=dtnow)
+            self.assertEqual(h5.attrs['now'], dtnow_iso)
+
+    def test_attrs1(self):
+        with File(mode='w') as h5:
+            h5.create_dataset('ds', shape=(), attrs={'mean': 1.2})
+
+            h5tbx.set_config(natural_naming=False)
+
+            h5tbx.set_config(natural_naming=True)
+            self.assertEqual(h5tbx.get_config('natural_naming'), True)
+            with h5tbx.set_config(natural_naming=False):
+                self.assertEqual(h5tbx.get_config('natural_naming'), False)
+                with self.assertRaises(AttributeError):
+                    self.assertEqual(h5.attrs.mean, 1.2)
+            self.assertEqual(h5tbx.get_config('natural_naming'), True)
+
+            h5.attrs.title = 'title of file'
+            self.assertEqual(h5.attrs['title'], 'title of file')
+
+            dset = h5.create_dataset('ds', data=1,
+                                     attrs={
+                                         'long_name': 'a long name',
+                                         'a1': 1, 'a2': 'str', 'a3': {'a': 2}
+                                     },
+                                     overwrite=True)
+            self.assertEqual(dset.attrs.get('a1'), 1)
+            self.assertEqual(dset.attrs.get('a2'), 'str')
+
+            h5.attrs['a dict'] = {'key1': 'value1', 'key2': 1239.2}
+            self.assertDictEqual(h5.attrs['a dict'], {'key1': 'value1', 'key2': 1239.2})
+
+            dset.attrs['a dict'] = {'key1': 'value1', 'key2': 1239.2, 'subdict': {'subkey': 99}}
+            self.assertDictEqual(dset.attrs['a dict'], {'key1': 'value1', 'key2': 1239.2, 'subdict': {'subkey': 99}})
+
+    def test_attrs2(self):
+        """test attrs manager"""
+        with File(mode='w') as h5:
+            h5tbx.set_config(natural_naming=False)
+
+            with self.assertRaises(AttributeError):
+                self.assertEqual(h5.attrs.mean, 1.2)
+
+            h5tbx.set_config(natural_naming=True)
+
+            h5.attrs.title = 'title of file'
+
+            self.assertEqual(h5.attrs['title'], 'title of file')
+            #
+            # h5.attrs['gr'] = h5['/']
+            # self.assertEqual(h5.attrs['gr'].name, '/')
+
+            # h5.attrs.gr2 = h5['/']
+            # self.assertEqual(h5.attrs['gr2'].name, '/')
+
+            dset = h5.create_dataset('ds', data=1,
+                                     attrs={'a1': 1, 'a2': 'str',
+                                            'a3': {'a': 2}})
+            self.assertEqual(dset.attrs.get('a1'), 1)
+            self.assertEqual(dset.attrs.get('a2'), 'str')
+
+            h5.attrs['dsref'] = dset
+            self.assertEqual(h5.attrs.raw['dsref'], dset.name)
+            self.assertEqual(h5.attrs['dsref'], dset)
+
+            h5.attrs['dsref2'] = dset.name
+            self.assertEqual(h5.attrs.raw['dsref'], dset.name)
+            self.assertEqual(h5.attrs['dsref2'], dset)
+
+            h5.attrs['a dict'] = {'key1': 'value1', 'key2': 1239.2}
+            self.assertDictEqual(h5.attrs['a dict'], {'key1': 'value1', 'key2': 1239.2})
+
+            dset.attrs['a dict'] = {'key1': 'value1', 'key2': 1239.2}
+            self.assertDictEqual(dset.attrs['a dict'], {'key1': 'value1', 'key2': 1239.2})
+
+    def test_hdf_filename(self):
+        with File() as h5:
+            self.assertIsInstance(h5.hdf_filename, pathlib.Path)
+            self.assertTrue(h5.hdf_filename.exists())
+            self.assertIsInstance(h5.hdf_filename, pathlib.Path)
+
+            h5.create_group('grp')
+            h5.create_dataset('ds', shape=(2, 3))
+
+            self.assertEqual(h5.grp.hdf_filename, h5.hdf_filename)
+            self.assertEqual(h5.ds.hdf_filename, h5.hdf_filename)
+
+            self.assertEqual(h5.grp.hdf_filename, h5['grp'].hdf_filename)
+            self.assertEqual(h5.ds.hdf_filename, h5['ds'].hdf_filename)
+
+    def test_open(self):
+        with File(mode='w') as h5:
+            h5.attrs['one'] = 1
+        with File(h5.hdf_filename, mode='w') as h5:
+            self.assertTrue('one' not in h5.attrs)
+            h5.attrs['one'] = 1
+        with File(h5.hdf_filename, mode='r+') as h5:
+            self.assertTrue('one' in h5.attrs)
+            h5.attrs['two'] = 2
+            self.assertTrue('two' in h5.attrs)
+
+        with File(mode='w') as h5:
+            pass
+        h5.reopen('r+')
+        self.assertEqual(h5.mode, 'r+')
+        h5.close()
+
+    def test_tree_structure(self):
+        with File() as h5:
+            h5.attrs['one'] = 1
+            h5.attrs['two'] = 2
+            h5.create_dataset('root_ds', shape=(2, 40, 3))
+            grp = h5.create_group('grp',
+                                  attrs={'description': 'group description'})
+            grp.create_dataset('grp_ds',
+                               shape=(2, 40, 3))
+            sub_grp = grp.create_group('sub_grp',
+                                       attrs={'description': 'sub group description'})
+            sub_grp.create_dataset('sub_grp_ds',
+                                   shape=(2, 40, 3))
+            tree = h5.get_tree_structure()
+
+            # TODO: there is a branch with improved tree structure code. however, the monogoDB scripts depend on it and nee to be changed accordingly first!
+
+            # self.assertTrue('/' in tree)
+            # self.assertTrue('grp' in tree)
+            # self.assertTrue('root_ds' in tree)
+
+            # self.assertFalse('sub_grp' in tree)
+            # self.assertFalse('sub_grp' in tree['/'])
+            #
+            # self.assertTrue('sub_grp' in tree['grp'])
+            # self.assertTrue('sub_grp' in tree['grp'])
+
+    def test_dimension_scales(self):
+        with File(mode='w') as h5:
+            _ = h5.create_dataset('x', data=[1, 2, 3], make_scale=True)
+            with self.assertRaises(ValueError):  # because name already exists
+                _ = h5.create_dataset('x', data=[1, 2, 3], make_scale=True)
+            del h5['x']
+            with self.assertRaises(TypeError):
+                _ = h5.create_dataset('x', data=[1, 2, 3], make_scale=[1, 2])
+
+    def test_scale_manipulation(self):
+        with File(mode='w') as h5:
+            h5.create_dataset('x',
+                              data=np.random.rand(10),
+                              attrs=dict(long_name='x-coordinate',
+                                         units='m', ), )
+            h5.create_dataset('time', data=np.random.rand(10), attrs=dict(long_name='time', units='s'))
+            h5.create_dataset('temp', data=np.random.rand(10), attrs=dict(long_name='temperature', units='K'),
+                              attach_scale=((h5['x'], h5['time']),))
+            self.assertTrue(h5['temp'].dims[0])
+            h5['temp'].set_primary_scale(0, 1)
+
+    def test_xr_dataset(self):
+        import xarray as xr
+        # from https://docs.xarray.dev/en/v0.9.5/examples/quick-overview.html#datasets
+        ds = xr.Dataset({'foo': [1, 2, 3], 'bar': ('x', [1, 2]), 'baz': np.pi})
+        ds.foo.attrs['units'] = 'm'
+        ds.foo.attrs['long_name'] = 'foo'
+
+        ds.bar.attrs['units'] = 'm'
+        ds.bar.attrs['long_name'] = 'bar'
+
+        ds.baz.attrs['units'] = 'm'
+        ds.baz.attrs['long_name'] = 'baz'
+
+        with File() as h5:
+            h5.create_dataset_from_xarray_dataset(ds)
+
+    def test_data_scale_and_offset(self):
+        with h5tbx.use('h5tbx') as cv5:
+            with File(mode='w') as h5:
+                ds = h5.create_dataset('ds', data=np.arange(10), attrs=dict(units='V'))
+                ds_scale = h5.create_dataset('ds_scale', data=1, attrs=dict(units='m/s/V'))
+                # ds_scale.make_data_scale()
+                ds.attach_data_scale_and_offset(ds_scale, None)
+                self.assertEqual(ds_scale, ds.get_data_scale())
+                self.assertEqual('m/s', ds[()].units)
+
+                ds.detach_data_scale()
+                self.assertEqual('V', str(ds[()].units))
+
+    def test_assign_data_to_existing_dset(self):
+        h5tbx.set_config(natural_naming=True)
+        with File(mode='w') as h5:
+            ds = h5.create_dataset('ds', shape=(2, 3))
+            ds[0, 0] = 5
+            self.assertEqual(ds[0, 0], 5)
+
+    def test_from_yaml_to_hdf(self):
+        dictionary = {
+            'boundary/outlet boundary/y':
+                {'data': 2, 'attrs': {'units': 'm', 'standard_name': 'y_coordinate',
+                                      'comment': 'test', 'another_attr': 100.2,
+                                      'array': [1, 2, 3]}},
+            'test/grp': {'attrs': {'long_name': 'a test group'}}
+        }
+        yaml_file = generate_temporary_filename(suffix='.yaml')
+        with open(yaml_file, 'w') as f:
+            yaml.safe_dump(dictionary, f)
+
+        hdf_filename = generate_temporary_filename(suffix='.hdf')
+        with File(hdf_filename, 'w') as h5:
+            h5.create_from_yaml(yaml_file)
+            self.assertIn('test/grp', h5)
+            self.assertIn('boundary/outlet boundary/y', h5)
+            self.assertTrue(h5['boundary/outlet boundary/y'].attrs['units'], 'm')
+
+    def test_dataset_value_comparison(self):
+        with File(mode='w') as h5:
+            ds1 = h5.create_dataset('ds1', data=4.4)
+            ds2 = h5.create_dataset('ds2', data=4.5)
+            self.assertEqual(0, ds1.ndim)
+            self.assertEqual(0, ds2.ndim)
+            self.assertTrue(ds1 < float(ds2[()]))
+            self.assertFalse(ds1 > float(ds2[()]))
+            self.assertFalse(ds1 == float(ds2[()]))
+
+    def test_get_group_names(self):
+        with h5tbx.set_config(auto_create_h5tbx_version=False):
+            with File(mode='w') as h5:
+                g = h5.create_group('one', 'one')
+                g.create_group('two', 'two')
+
+                g = g.create_group('three', 'three')
+                g.create_group('four', 'four')
+                self.assertEqual(h5['one'].get_group_names(), ['three', 'three/four', 'two'])
+                self.assertEqual(sorted(h5['one'].get_group_names(recursive=False)), sorted(['two', 'three']))
+                self.assertEqual(sorted(h5['/'].get_group_names(recursive=False)), sorted(['one', ]))
+                self.assertEqual(sorted(h5.get_group_names(recursive=False)), sorted(['one', ]))
+
+    def test_get_dataset_names(self):
+        with File(mode='w') as h5:
+            h5.create_dataset('one', data=1, attrs=dict(long_name='long name', units=''))
+            h5.create_dataset('two', data=1, attrs=dict(long_name='long name', units=''))
+            h5.create_dataset('grp/three', data=1, attrs=dict(long_name='long name', units=''))
+            h5.create_dataset('grp/two', data=1, attrs=dict(long_name='long name', units=''))
+            self.assertEqual(h5.get_dataset_names(),
+                             ['grp/three', 'grp/two', 'one', 'two'])
+
+    def test_multi_dim_scales(self):
+        fname = generate_temporary_filename(suffix='.hdf')
+        with h5py.File(fname, 'w') as h5:
+            x = h5.create_dataset('x', data=[0.0, 10.5, 20.13])
+            ix = h5.create_dataset('ix', data=[0, 16, 32])
+            y = h5.create_dataset('y', data=[0.0, 4.5, 23.13])
+            iy = h5.create_dataset('iy', data=[0, 16, 32])
+
+            signal = h5.create_dataset('signal', data=np.ones((3, 3)))
+
+            x.make_scale('x')
+            ix.make_scale('ix')
+            y.make_scale('y')
+            iy.make_scale('iy')
+
+            signal.dims[0].attach_scale(h5['x'])
+            signal.dims[0].attach_scale(h5['ix'])
+            signal.dims[1].attach_scale(h5['y'])
+            signal.dims[1].attach_scale(h5['iy'])
+
+        with File(fname) as h5:
+            x = h5['x'][:]
+            ix = h5['ix'][:]
+            s = h5['signal'][:, :]
```

### Comparing `h5rdmtoolbox-1.2.2/tests/repository/test_zenodo.py` & `h5rdmtoolbox-1.3.0a1/tests/repository/test_zenodo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import json
 import logging
 import os
 import pathlib
-import pydantic
 import unittest
 from datetime import datetime
 
+import pydantic
+
 import h5rdmtoolbox as h5tbx
+from h5rdmtoolbox import UserDir
 from h5rdmtoolbox.repository import zenodo, upload_file
-from h5rdmtoolbox.repository.h5metamapper import hdf2json
 from h5rdmtoolbox.repository.zenodo.metadata import Metadata, Creator, Contributor
 from h5rdmtoolbox.repository.zenodo.tokens import get_api_token, set_api_token
+from h5rdmtoolbox.wrapper.jsonld import dump_file
 
 logger = logging.getLogger(__name__)
 
 
 class TestConfig(unittest.TestCase):
 
-    # def test_max_requests(self):
-    #     """The number of requests per minute is limited to X (~100) per minute and Y (~5000) per hour.
-    #     It the number is exceeded, a 429 error is returned."""
-    #     from h5rdmtoolbox.repository.zenodo.core import logger
-    #     logger.setLevel(logging.DEBUG)
-    #     z = zenodo.ZenodoSandboxDeposit(8561)
-    #     for i in range(200):
-    #         r = z.get()
-    #         print(i+1, r.status_code)
-    #         filenames = z.download_files()
-    #         assert len(filenames) == 1
-    #         h5tbx.convention.from_yaml(filenames[0])
-    #         for f in filenames:
-    #             f.unlink()
+    # def tearDown(self):
+    #     depositions_url = 'https://sandbox.zenodo.org/api/deposit/depositions?'
+    #
+    #     response = requests.get(depositions_url, params={'access_token': get_api_token(sandbox=True)}).json()
+    #     n_unsubmitted = sum([not hit['submitted'] for hit in response])
+    #     while n_unsubmitted > 0:
+    #         for hit in response:
+    #             if not hit['submitted']:
+    #                 delete_response = requests.delete(hit['links']['latest_draft'],
+    #                                                   params={'access_token': get_api_token(sandbox=True)})
+    #                 delete_response.raise_for_status()
+    #         response = requests.get(depositions_url, params={'access_token': get_api_token(sandbox=True)}).json()
+    #         n_unsubmitted = sum([not hit['submitted'] for hit in response])
 
     def test_creator(self):
         from h5rdmtoolbox.repository.zenodo.metadata import Creator
         with self.assertRaises(ValueError):
             creator = Creator(name='John Doe', affiliation='University of Nowhere')
         creator = Creator(name='Doe, John')
         self.assertEqual(creator.name, 'Doe, John')
@@ -131,44 +132,49 @@
                                 keywords=['hdf5', 'research data management', 'rdm'],
                                 upload_type='publication',
                                 publication_type='other',
                                 access_right='embargoed',
                                 embargo_date='01-2022-01',  # wrong format!
                                 publication_date='2023-01-01')
 
-
     def test_get_api(self):
         self.assertIsInstance(get_api_token(sandbox=True), str)
 
         from h5rdmtoolbox.repository.zenodo.tokens import _parse_ini_file
         import appdirs
         fname = pathlib.Path(appdirs.user_data_dir('h5rdmtoolbox')) / 'zenodo.ini'
         if fname.exists():
             bak_fname = fname.rename(fname.with_suffix('.bak'))
         else:
             bak_fname = None
 
+        zenodo_ini_filename = UserDir['repository'] / 'zenodo.ini'
+        if zenodo_ini_filename.exists():
+            tmp_zenodo_ini_filename = zenodo_ini_filename.rename(zenodo_ini_filename.with_suffix('.ini_bak'))
+        else:
+            tmp_zenodo_ini_filename = None
+
         with self.assertRaises(FileNotFoundError):
             _parse_ini_file(None)
 
         with self.assertRaises(FileNotFoundError):
             _parse_ini_file('invalid.ini')
 
-        with self.assertRaises(FileNotFoundError):
-            _parse_ini_file(None)
-
         if bak_fname:
             bak_fname.rename(fname)
 
         tmp_ini_file = h5tbx.utils.generate_temporary_filename(suffix='.ini', touch=True)
         ini_filename = _parse_ini_file(tmp_ini_file)
         self.assertEqual(ini_filename, tmp_ini_file)
         self.assertTrue(ini_filename.exists())
         ini_filename.unlink()
 
+        if tmp_zenodo_ini_filename:
+            tmp_zenodo_ini_filename.rename(tmp_zenodo_ini_filename.with_suffix('.ini'))
+
     def test_get_api_token(self):
         env_token_sb = os.environ.pop('ZENODO_SANDBOX_API_TOKEN', None)
         env_token = os.environ.pop('ZENODO_API_TOKEN', None)
         test_ini_filename = pathlib.Path(__file__).parent / 'test.ini'
         self.assertEqual(get_api_token(sandbox=True, zenodo_ini_filename=test_ini_filename), '123')
         self.assertEqual(get_api_token(sandbox=False, zenodo_ini_filename=test_ini_filename), '456')
 
@@ -179,17 +185,22 @@
         self.assertEqual('def', os.environ.get('ZENODO_API_TOKEN', None))
         self.assertEqual(get_api_token(sandbox=False, zenodo_ini_filename=test_ini_filename), 'def')
         os.environ.pop('ZENODO_API_TOKEN', None)
 
         # reset environment variable
         if env_token_sb is not None:
             os.environ['ZENODO_SANDBOX_API_TOKEN'] = env_token_sb
-        self.assertEqual(env_token_sb, os.environ.get('ZENODO_SANDBOX_API_TOKEN', None))
+            self.assertEqual(env_token_sb, os.environ.get('ZENODO_SANDBOX_API_TOKEN', None))
+        else:
+            os.environ.pop('ZENODO_SANDBOX_API_TOKEN')
+
         if env_token is not None:
             os.environ['ZENODO_API_TOKEN'] = env_token
+        else:
+            os.environ.pop('ZENODO_API_TOKEN', None)
         self.assertEqual(env_token, os.environ.get('ZENODO_API_TOKEN', None))
 
     def test_set_api_token(self):
 
         env_token_sb = os.environ.pop('ZENODO_SANDBOX_API_TOKEN', None)
         env_token = os.environ.pop('ZENODO_API_TOKEN', None)
 
@@ -215,33 +226,44 @@
 
         if env_token_sb is not None:
             os.environ['ZENODO_SANDBOX_API_TOKEN'] = env_token_sb
         self.assertEqual(env_token_sb, os.environ.get('ZENODO_SANDBOX_API_TOKEN', None))
         if env_token is not None:
             os.environ['ZENODO_API_TOKEN'] = env_token
 
+
+
     def test_upload_hdf(self):
         z = zenodo.ZenodoSandboxDeposit(None)
 
         with h5tbx.File() as h5:
             h5.attrs['long_name'] = 'root'
             h5.create_dataset('test', data=1, attrs={'units': 'm/s', 'long_name': 'dataset 1'})
             h5.create_dataset('grp1/test2', data=2, attrs={'test': 1, 'long_name': 'dataset 2'})
 
             orig_hdf_filename = h5.hdf_filename
         hdf_file_name = orig_hdf_filename.name
         json_name = hdf_file_name.replace('.hdf', '.json')
 
+        def hdf2json(hdf_filename: pathlib.Path) -> pathlib.Path:
+            json_ld_filename = hdf_filename.with_suffix('.json')
+            with open(json_ld_filename, 'w') as f:
+                f.write(dump_file(hdf_filename, skipND=1))
+            return json_ld_filename
+
         z.upload_hdf_file(orig_hdf_filename, metamapper=hdf2json)
         filenames = z.get_filenames()
         self.assertIn(hdf_file_name, filenames)
         self.assertIn(json_name, filenames)
         with self.assertRaises(KeyError):
             _ = z.download_file('invalid.hdf')
 
+        hdf_filenames = z.get_filenames(suffix='.hdf')
+        self.assertEqual(len(hdf_filenames), 1)
+
         hdf_filename = z.download_file(hdf_file_name)
 
         self.assertTrue(hdf_filename.exists())
 
         with h5tbx.File(hdf_filename) as h5:
             self.assertEqual(h5.attrs['long_name'], 'root')
             self.assertEqual(h5['test'].attrs['units'], 'm/s')
@@ -250,43 +272,52 @@
             self.assertEqual(h5['grp1/test2'].attrs['long_name'], 'dataset 2')
 
         json_filename = z.download_file(json_name)
         self.assertTrue(json_filename.exists())
         with open(json_filename) as f:
             json_dict = json.loads(f.read())
 
-        from h5rdmtoolbox import consts
-        self.assertEqual(json_dict['attrs'],
-                         {'__h5rdmtoolbox_version__': h5tbx.__version__,
-                          'long_name': 'root',
-                          'IRI_PREDICATE': json.dumps({'__h5rdmtoolbox_version__': consts.VERSION_IRI})})
-        z.delete()
+        self.assertTrue('@context' in json_dict)
+        self.assertEqual(json_dict['@type'], 'hdf5:File')
+
+        #
+        # print(json_dict['h5rdmtoolbox']['attrs'])
+        # self.assertDictEqual(
+        #     json_dict['h5rdmtoolbox']['attrs'],
+        #     {
+        #         '@type': 'https://schema.org/SoftwareSourceCode',
+        #         rdf.RDF_PREDICATE_ATTR_NAME: '{"__h5rdmtoolbox_version__": "https://schema.org/softwareVersion"}',
+        #         '__h5rdmtoolbox_version__': h5tbx.__version__
+        #     }
+        # )
+        # z.delete()
 
     def test_ZenodoSandboxDeposit(self):
         z = zenodo.ZenodoSandboxDeposit(None)
-        self.assertIsInstance(z.metadata, dict)
+        self.assertIsInstance(z.get_metadata(), dict)
         self.assertEqual(z.get_doi(), f'10.5281/zenodo.{z.rec_id}')
-        self.assertIn('access_right', z.metadata)
-        self.assertIn('prereserve_doi', z.metadata)
-        self.assertEqual('open', z.metadata['access_right'])
-        self.assertEqual(z.rec_id, z.metadata['prereserve_doi']['recid'])
+        self.assertIn('access_right', z.get_metadata())
+        self.assertIn('prereserve_doi', z.get_metadata())
+        self.assertEqual('open', z.get_metadata()['access_right'])
+        self.assertEqual(z.rec_id, z.get_metadata()['prereserve_doi']['recid'])
         self.assertTrue(z.exists())
+        self.assertFalse(z.is_published())
 
         old_rec_id = z.rec_id
 
-        z.delete()
+        # z.delete()
 
         with self.assertRaises(ValueError):
-            _ = zenodo.ZenodoSandboxDeposit(old_rec_id)
+            _ = zenodo.ZenodoSandboxDeposit('123123123123')
 
         z = zenodo.ZenodoSandboxDeposit(None)
         self.assertNotEqual(old_rec_id, z.rec_id)
 
-        with self.assertRaises(TypeError):
-            z.metadata = {'access_right': 'closed'}
+        # with self.assertRaises(TypeError):
+        #     z.metadata = {'access_right': 'closed'}
 
         meta = Metadata(
             version="0.1.0-rc.1+build.1",
             title='[deleteme]h5tbxZenodoInterface',
             description='A toolbox for managing HDF5-based research data management',
             creators=[Creator(name="Probst, Matthias",
                               affiliation="KIT - ITS",
@@ -299,25 +330,32 @@
             image_type='photo',
             access_right='open',
             keywords=['hdf5', 'research data management', 'rdm'],
             publication_date=datetime.now(),
             embargo_date='2020'
         )
 
-        z.metadata = meta
-        ret_metadata = z.metadata
+        with self.assertRaises(TypeError):
+            z.set_metadata(12)
+
+        z.set_metadata(meta.model_dump())
+        z.set_metadata(meta)
+        ret_metadata = z.get_metadata()
         self.assertEqual(ret_metadata['upload_type'],
                          meta.model_dump()['upload_type'])
         self.assertListEqual(ret_metadata['keywords'],
                              meta.model_dump()['keywords'])
 
         # add file:
         tmpfile = pathlib.Path('testfile.txt')
         with open(tmpfile, 'w') as f:
             f.write('This is a test file.')
+
+        with self.assertRaises(FileNotFoundError):
+            z.upload_file('doesNotExist.txt', overwrite=True)
         z.upload_file(tmpfile, overwrite=True)
         self.assertIn('testfile.txt', z.get_filenames())
 
         with self.assertWarns(UserWarning):
             z.upload_file('testfile.txt', overwrite=False)
 
         upload_file(z, tmpfile, overwrite=True)
@@ -328,18 +366,36 @@
         # delete file locally:
         tmpfile.unlink()
         self.assertFalse(tmpfile.exists())
 
         filename = z.download_file('testfile.txt', target_folder='.')
         self.assertIsInstance(filename, pathlib.Path)
         self.assertTrue(filename.exists())
+        with open(filename, 'r') as f:
+            self.assertEqual(f.read(), 'This is a test file.')
         filename.unlink()
 
         filenames = z.download_files(target_folder='.')
+
         self.assertIsInstance(filenames, list)
         self.assertIsInstance(filenames[0], pathlib.Path)
         for filename in filenames:
             self.assertTrue(filename.exists())
             filename.unlink()
 
-        z.delete()
-        self.assertFalse(z.exists())
+        hdf5_filenames = z.download_files(target_folder='.', suffix='.hdf')
+        self.assertIsInstance(hdf5_filenames, list)
+        self.assertEqual(len(hdf5_filenames), 0)
+
+        txt_filenames = z.download_files(target_folder='.', suffix='.txt')
+        self.assertIsInstance(txt_filenames, list)
+        self.assertEqual(len(txt_filenames), 1)
+        self.assertEqual(txt_filenames[0].suffix, '.txt')
+
+        hdf_and_txt_filenames = z.download_files(target_folder='.', suffix=['.txt', '.hdf'])
+        self.assertIsInstance(hdf_and_txt_filenames, list)
+        self.assertEqual(len(hdf_and_txt_filenames), 1)
+        self.assertEqual(hdf_and_txt_filenames[0].suffix, '.txt')
+
+        self.assertTrue(z.exists())
+        # z.delete()
+        # self.assertFalse(z.exists())
```

### Comparing `h5rdmtoolbox-1.2.2/tests/test_config.py` & `h5rdmtoolbox-1.3.0a1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/tests/test_identifiers.py` & `h5rdmtoolbox-1.3.0a1/tests/test_identifiers.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,47 +15,61 @@
     def test_rorid(self):
         self.assertTrue(identifiers.RORID('https://ror.org/04wxnsj81').validate())
         self.assertFalse(identifiers.RORID('https://ror.org/?4wxnsj82').validate())
         self.assertTrue(identifiers.RORID('04wxnsj81').validate())
         self.assertEqual(str(identifiers.RORID('04wxnsj81')), 'https://ror.org/04wxnsj81')
         self.assertFalse(identifiers.RORID('https://orcid.org/0000-0002-1825-0097').validate())
 
+        with self.assertRaises(NotImplementedError):
+            identifiers.RORID('04wxnsj81').check_checksum()
+
     def test_from_url(self):
         self.assertIsInstance(identifiers.from_url('https://orcid.org/0000-0002-1825-0097'),
                               identifiers.ORCID)
         # self.assertIsInstance(identifiers.from_url('https://ror.org/04t3en479'),
         #                       identifiers.RORID)
 
     # def test_gnd(self):
     #     self.assertTrue(identifiers.GND('118540268').validate())
     #     self.assertFalse(identifiers.GND('118540269').validate())
 
     def test_isbn(self):
         self.assertTrue(identifiers.ISBN10('80-85892-15-4').validate())
         self.assertFalse(identifiers.ISBN10('80/85892-15-4').validate())
         self.assertFalse(identifiers.ISBN10('80-85892-15-8').validate())
+        self.assertFalse(identifiers.ISBN10('80-85892-15-X').validate())
         self.assertTrue(identifiers.ISBN13('978-80-85892-15-4').validate())
         self.assertFalse(identifiers.ISBN13('978-80-85892-15-8').validate())
         self.assertFalse(identifiers.ISBN13('978/80-85892-15-4').validate())
 
     def test_orcid(self):
+        self.assertTrue(identifiers.ORCID('https://orcid.org/0000-0002-1825-0097').exists())
+        self.assertFalse(identifiers.ORCID('https://orcid.org/1111-0002-1825-0097').exists())
         self.assertTrue(identifiers.ORCID('https://orcid.org/0000-0002-1825-0097').validate())
         self.assertFalse(identifiers.ORCID('https://orcid.org/0000-0002-1825-0096').validate())
         self.assertTrue(identifiers.ORCID('0000-0002-1825-0097').validate())
         self.assertTrue(identifiers.ORCID('https://orcid.org/0000-0001-5109-3700').validate())
         self.assertTrue(identifiers.ORCID('https://orcid.org/0000-0002-1694-233X').validate())
 
-    # def test_orcid(self):
-    #     o = h5tbx.orcid.KnownOrcids()
-    #     o._filename = h5tbx.utils.generate_temporary_filename()
-    #     o.load()
-    #     self.assertEqual([], o._orcids)
-    #     o._orcids = ['1', '2']
-    #     o.save()
-    #     self.assertTrue(o.filename.exists())
+    def test_orcid_cache(self):
+        identifiers.KNOWN_ORCID_FILENAME.unlink(missing_ok=True)
+        self.assertEqual(len(identifiers.ORCID.get_existing_orcids()), 0)
+        identifiers.ORCID('https://orcid.org/0000-0002-1825-0097').exists()
+        print(identifiers.ORCID.get_existing_orcids())
+        self.assertEqual(len(identifiers.ORCID.get_existing_orcids()), 1)
+        self.assertEqual(identifiers.ORCID.get_existing_orcids()[0], 'https://orcid.org/0000-0002-1825-0097')
+
+    # def test_orcid_exists(self):
+    # o = h5tbx.orcid.KnownOrcids()
+    # o._filename = h5tbx.utils.generate_temporary_filename()
+    # o.load()
+    # self.assertEqual([], o._orcids)
+    # o._orcids = ['1', '2']
+    # o.save()
+    # self.assertTrue(o.filename.exists())
     #
     #     o.add('3')
     #     self.assertEqual(['1', '2', '3'], o.orcids)
     #
     #     o = h5tbx.orcid.ORCID([h5tbx.__author_orcid__])
     #     self.assertIsInstance(o, h5tbx.orcid.ORCID)
     #
```

### Comparing `h5rdmtoolbox-1.2.2/tests/test_plotting.py` & `h5rdmtoolbox-1.3.0a1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/tests/test_utils.py` & `h5rdmtoolbox-1.3.0a1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-import appdirs
 import datetime
 import h5py
 import pathlib
 import unittest
 
 import h5rdmtoolbox as h5tbx
 
 __this_dir__ = pathlib.Path(__file__).parent
 
 
 class TestUtils(unittest.TestCase):
 
+    def test_hash(self):
+        with h5tbx.File() as h5:
+            pass
+        self.assertEqual(h5tbx.get_checksum(h5.hdf_filename),
+                         '6781e0baec8d65b9a95a3e879a5098d1')
+
+
     def test_touch_tmp_hdf5_file(self):
-        now = datetime.datetime.now()
-        tmp_hdf5file = h5tbx.utils.touch_tmp_hdf5_file(touch=True,
-                                                       attrs={'dtime': now})
-        self.assertTrue(h5tbx.UserDir['tmp'] in tmp_hdf5file.parents)
-
-        self.assertEqual(h5tbx.utils.get_filesize(tmp_hdf5file).magnitude, 6144)
-        self.assertEqual(h5tbx.utils.get_filesize(tmp_hdf5file).units, h5tbx.get_ureg().Unit('byte'))
-
-    def test_create_tbx_logger(self):
-        logger = h5tbx.utils.create_tbx_logger('test')
-        self.assertEqual(pathlib.Path(appdirs.user_log_dir('h5rdmtoolbox')), logger._directory)
-        self.assertEqual(pathlib.Path(appdirs.user_log_dir('h5rdmtoolbox')) / 'test.log',
-                         pathlib.Path(logger.handlers[0].baseFilename))
+        with h5tbx.set_config(auto_create_h5tbx_version=False):
+            now = datetime.datetime.now()
+            tmp_hdf5file = h5tbx.utils.touch_tmp_hdf5_file(touch=True,
+                                                           attrs={'dtime': now})
+            self.assertTrue(h5tbx.UserDir['tmp'] in tmp_hdf5file.parents)
+            self.assertEqual(h5tbx.utils.get_filesize(tmp_hdf5file).magnitude, 6144)
+            self.assertEqual(h5tbx.get_filesize(tmp_hdf5file).magnitude, 6144)
+            self.assertEqual(h5tbx.utils.get_filesize(tmp_hdf5file).units, h5tbx.get_ureg().Unit('byte'))
 
     def test_remove_special_chars(self):
         self.assertEqual('test123_', h5tbx.utils.remove_special_chars('test123&%$#_'))
         self.assertEqual('test123', h5tbx.utils.remove_special_chars('test123&%$#_', keep_special=''))
         self.assertEqual('test123&', h5tbx.utils.remove_special_chars('test123&%$#_', keep_special='&'))
 
     def test_generate_temporary_filename(self):
@@ -81,17 +82,18 @@
         dsp = h5tbx.utils.DocStringParser(_test)
         self.assertEqual('test', dsp.get_original_doc_string())
         self.assertEqual((None, [], [], []), h5tbx.utils.DocStringParser.parse_docstring(dsp.get_original_doc_string()))
         self.assertEqual((None, [], [], []), h5tbx.utils.DocStringParser.parse_docstring(''))
 
     def test_has_datasets(self):
         with h5tbx.use(None):
-            with h5tbx.File() as h5:
-                self.assertFalse(h5tbx.utils.has_datasets(h5))
-                h5.create_dataset('test', data=1)
-                self.assertTrue(h5tbx.utils.has_datasets(h5))
-                self.assertFalse(h5tbx.utils.has_groups(h5))
-                h5.create_group('testgroup')
-                self.assertTrue(h5tbx.utils.has_groups(h5))
+            with h5tbx.set_config(auto_create_h5tbx_version=False):
+                with h5tbx.File() as h5:
+                    self.assertFalse(h5tbx.utils.has_datasets(h5))
+                    h5.create_dataset('test', data=1)
+                    self.assertTrue(h5tbx.utils.has_datasets(h5))
+                    self.assertFalse(h5tbx.utils.has_groups(h5))
+                    h5.create_group('testgroup')
+                    self.assertTrue(h5tbx.utils.has_groups(h5))
 
-            self.assertTrue(h5tbx.utils.has_datasets(h5.hdf_filename))
-            self.assertTrue(h5tbx.utils.has_groups(h5.hdf_filename))
+                self.assertTrue(h5tbx.utils.has_datasets(h5.hdf_filename))
+                self.assertTrue(h5tbx.utils.has_groups(h5.hdf_filename))
```

### Comparing `h5rdmtoolbox-1.2.2/tests/test_version.py` & `h5rdmtoolbox-1.3.0a1/tests/test_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import json
 import pathlib
 import unittest
 
-import h5rdmtoolbox as h5tbx
+from h5rdmtoolbox import __version__, get_package_meta
 
 __this_dir__ = pathlib.Path(__file__).parent
 
 
 class TestVersion(unittest.TestCase):
 
     def test_version(self):
         this_version = 'x.x.x'
         setupcfg_filename = __this_dir__ / '../setup.cfg'
         with open(setupcfg_filename, 'r') as f:
             lines = f.readlines()
             for line in lines:
                 if 'version' in line:
                     this_version = line.split(' = ')[-1].strip()
-        self.assertEqual(h5tbx.__version__, this_version)
+        self.assertEqual(__version__, this_version)
 
     def test_codemeta(self):
         """checking if the version in codemeta.json is the same as the one of the toolbox"""
 
-        with open(__this_dir__ / '../codemeta.json', 'r') as f:
-            codemeta = json.loads(f.read())
+        codemeta = get_package_meta()
 
-        assert codemeta['version'] == h5tbx.__version__
+        assert codemeta['version'] == __version__
```

### Comparing `h5rdmtoolbox-1.2.2/tests/test_xarray_export.py` & `h5rdmtoolbox-1.3.0a1/tests/test_xarray_export.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/tests/wrapper/test_core.py` & `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,44 +3,70 @@
 import json
 import numpy as np
 import pandas as pd
 import pathlib
 import unittest
 import xarray as xr
 from datetime import datetime, timedelta
+from dateutil.parser import parse
 from numpy import linspace as ls
 
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox import __version__
 from h5rdmtoolbox.wrapper import h5yaml
 from h5rdmtoolbox.wrapper.h5attr import AttributeString
 
-logger = h5tbx.logger
-# logger.setLevel('ERROR')
+logger = h5tbx.set_loglevel('ERROR')
+
 __this_dir__ = pathlib.Path(__file__).parent
 
 
 class TestCore(unittest.TestCase):
 
     def setUp(self) -> None:
         h5tbx.use(None)
 
-    def test_logger(self):
-        from h5rdmtoolbox.utils import ToolboxLogger
-        self.assertIsInstance(logger, ToolboxLogger)
-
     def test_lower(self):
         self.assertEqual(h5tbx.Lower('Hello'), 'hello')
         self.assertIsInstance(h5tbx.lower('Hello'), h5tbx.Lower)
 
+    @classmethod
+    def tearDownClass(cls) -> None:
+        h5tbx.set_config(auto_create_h5tbx_version=False)
+
     def test_File(self):
         self.assertEqual(str(h5tbx.File), "<class 'h5rdmtoolbox.wrapper.core.File'>")
+        h5tbx.set_config(auto_create_h5tbx_version=False)
+        self.assertEqual(h5tbx.get_config('auto_create_h5tbx_version'), False)
+        with h5tbx.File() as h5:
+            self.assertTrue('h5rdmtoolbox' not in h5)
+            self.assertEqual(h5.__str__(), '<class "File" convention: "h5py">')
+
+        h5tbx.set_config(auto_create_h5tbx_version=True)
+        self.assertEqual(h5tbx.get_config('auto_create_h5tbx_version'), True)
         with h5tbx.File() as h5:
+            self.assertFalse('h5rdmtoolbox' not in h5)
             self.assertEqual(h5.__str__(), '<class "File" convention: "h5py">')
 
+        with h5tbx.set_config(auto_create_h5tbx_version=False):
+            with h5tbx.File() as h5:
+                self.assertTrue('h5rdmtoolbox' not in h5)
+                self.assertEqual(h5.__str__(), '<class "File" convention: "h5py">')
+
+        with h5tbx.File() as h5:
+            self.assertFalse('h5rdmtoolbox' not in h5)
+            self.assertEqual(h5.__str__(), '<class "File" convention: "h5py">')
+
+        assert h5.hdf_filename.exists()
+        _h5_filename = h5.hdf_filename
+
+        _h5_filename.rename(_h5_filename.with_suffix('.h5'))
+        with self.assertRaises(FileNotFoundError):
+            h5.hdf_filename
+
     def test_dump(self):
         # all following should not raise an error...
         with h5tbx.File() as h5:
             pass
         h5tbx.dump(h5.hdf_filename)
         h5tbx.dump(h5)
         h5tbx.dump(str(h5.hdf_filename))
@@ -79,52 +105,71 @@
                 with self.assertRaises(AttributeError):
                     with h5tbx.set_config(natural_naming=False):
                         del ds.ds
 
                 del h5.ds
                 self.assertTrue('ds' not in h5)
 
+    def test_delattr(self):
+        with h5tbx.File() as h5:
+            h5.attrs['test'] = 'test'
+            del h5.attrs['test']
+            h5.create_dataset('ds',
+                              data=np.arange(10),
+                              # units='m/s',
+                              attrs={'comment': 'test'})
+            self.assertIn('ds', h5)
+            del h5.ds
+            self.assertNotIn('ds', h5)
+
+        with h5tbx.File() as h5:
+            h5.attrs['test'] = 'test'
+            h5.create_dataset('ds',
+                              data=np.arange(10),
+                              # units='m/s',
+                              attrs={'comment': 'test'})
+            with h5tbx.set_config(natural_naming=False):
+                del h5.ds
+
     def test_setattr(self):
         with h5tbx.File() as h5:
             with self.assertRaises(AttributeError):
                 h5.smth = 10
             h5._smth = 10
             self.assertEqual(10, h5._smth)
 
+            h5tbx.set_config(ignore_none=True)
+            h5.attrs['none_attr'] = None
+            self.assertFalse('none_attr' in h5)
+            h5tbx.set_config(ignore_none=False)
+            h5.attrs['none_attr'] = None
+            self.assertEqual(h5.attrs['none_attr'], 'None')
+
     def test_rootparent(self):
         with h5tbx.File() as h5:
             g = h5.create_group('g')
             self.assertEqual(h5, g.rootparent)
             self.assertEqual(h5, h5['g'].rootparent)
             self.assertEqual(h5, h5.rootparent)
 
             grp = h5.create_group('grp1/grp2/grp3')
             self.assertEqual(grp.rootparent, h5)
             dset = grp.create_dataset('test', data=1)
             self.assertEqual(dset.rootparent, h5)
 
             self.assertEqual(dset.rootparent, h5)
 
-    # def test_basename(self):
-    #     with h5tbx.File() as h5:
-    #         h5.create_dataset('ds', data=np.arange(10))
-    #         self.assertEqual(h5['ds'].basename, 'ds')
-    #         h5.create_dataset('a/b/ds', data=np.arange(10))
-    #         self.assertEqual(h5['a/b/ds'].basename, 'ds')
-    #         self.assertEqual(h5['a'].basename, 'a')
-    #         self.assertEqual(h5['a/b'].basename, 'b')
-
     def test_write_iso_timestamp(self):
         with h5tbx.File() as h5:
             now = datetime.now()
-            h5.write_iso_timestamp('timestamp', dt=now)
+            h5.attrs.write_iso_timestamp('timestamp', dt=now)
             self.assertIsInstance(h5.attrs['timestamp'], str)
             self.assertEqual(h5.attrs['timestamp'], str(now.isoformat()))
             with self.assertRaises(TypeError):
-                h5.write_iso_timestamp('timestamp', dt='now', overwrite=True)
+                h5.attrs.write_iso_timestamp('timestamp', dt='now', overwrite=True)
 
     def test_create_dataset(self):
         with h5tbx.File() as h5:
             h5.create_dataset('ds', data=np.arange(10))
             np.testing.assert_equal(h5['ds'][:], np.arange(10))
 
             h5.create_dataset('ds2', shape=(10,), dtype=np.float32)
@@ -137,15 +182,21 @@
             np.testing.assert_equal(h5['ds3'][:], np.arange(10))
 
             h5.create_dataset('ds4', np.arange(20))
             np.testing.assert_equal(h5['ds4'][:], np.arange(20))
 
     def test_create_datasets_from_csv(self):
         df = pd.DataFrame({'x': [1, 5, 10, 0], 'y': [-3, 20, 0, 11.5]})
-        csv_filename1 = h5tbx.utils.generate_temporary_filename(suffix='.csv')
+        csv_filename1 = h5tbx.utils.generate_temporary_filename(suffix='.csv', touch=False)
+        self.assertEqual(csv_filename1.suffix, '.csv')
+        self.assertFalse(csv_filename1.exists())
+        csv_filename1 = h5tbx.utils.generate_temporary_filename(suffix='.csv', touch=True)
+        self.assertEqual(csv_filename1.suffix, '.csv')
+        self.assertTrue(csv_filename1.exists())
+
         df.to_csv(csv_filename1, index=None)
 
         with h5tbx.File() as h5:
             with self.assertRaises(ValueError):
                 h5.create_datasets_from_csv(csv_filenames=csv_filename1, combine_opt='invlaid')
             h5.create_datasets_from_csv(csv_filenames=csv_filename1)
             self.assertEqual(h5['x'].shape, (4,))
@@ -292,16 +343,17 @@
             self.assertEqual(list(grp.get_datasets('dat*')), [grp['data'], ])
             self.assertEqual(sorted(grp.get_datasets('.*')), [grp['data'], ])
             self.assertEqual(list(grp.get_datasets('idat*')), [])
             with self.assertRaises(ValueError):
                 h5tbx.Group(4.3)
             with self.assertRaises(TypeError):
                 h5.grp['New'] = (4.3, int)
-            h5.grp['New'] = dict(data=np.random.rand(10, 20, 30))
 
+            h5.grp['New'] = np.random.rand(10, 20, 30), dict(attrs=dict(name='my_dataset'))
+            self.assertEqual(h5.grp['New'].attrs['name'], 'my_dataset')
             newds = h5.grp['New']
             self.assertEqual(newds.name, '/grp/New')
 
             from h5rdmtoolbox.wrapper.core import Lower
             newds = h5.grp[Lower('new')]
             self.assertEqual(newds.name, '/grp/New')
 
@@ -326,74 +378,94 @@
 
             h5.create_string_dataset('str', 'test', attrs={'a': 'b'})
             self.assertTrue('str' in h5)
             self.assertEqual(h5['str'].attrs['a'], 'b')
             self.assertTrue(h5['str'].name, '/str')
             self.assertEqual(h5['str'][()], 'test')
 
+            h5.create_string_dataset('arr_str', ['word1', 'word2'], attrs={'a': 'b'})
+            self.assertTrue('arr_str' in h5)
+            self.assertEqual(h5['arr_str'][0], 'word1')
+            self.assertEqual(h5['arr_str'][1], 'word2')
+
             h5.create_string_dataset('str2', ('a', 'b', 'c'))
             self.assertTrue(h5['str2'].name, '/str2')
-            self.assertEqual(h5['str2'][()], ('a', 'b', 'c'))
+            self.assertEqual(tuple(h5['str2'][()]), ('a', 'b', 'c'))
 
             h5.create_string_dataset('str2', ('a', 'bb', 'c', 'd'), overwrite=True)
             self.assertTrue(h5['str2'].name, '/str2')
-            self.assertEqual(h5['str2'][()], ('a', 'bb', 'c', 'd'))
+            self.assertEqual(tuple(h5['str2'][()]), ('a', 'bb', 'c', 'd'))
             self.assertTrue(h5['str2'].size, 2)
 
             h5.create_string_dataset('str2', ('a', 'b', 'c', 'dddd'), overwrite=True, attrs={'a': 'b'})
             self.assertTrue(h5['str2'].name, '/str2')
-            self.assertEqual(h5['str2'][()], ('a', 'b', 'c', 'dddd'))
+            self.assertEqual(tuple(h5['str2'][()]), ('a', 'b', 'c', 'dddd'))
             self.assertTrue(h5['str2'].size, 4)
 
             self.assertEqual('/grp', h5['grp'].name)
 
     # ---------------------------------------------------------------------------
     # special dataset creation methods:
     # ---------------------------------------------------------------------------
     def test_create_img_dataset(self):
 
         # Iterable class:
         class ImgReader:
+            """DummyReader"""
+
             def __init__(self, imgdir):
                 self._imgdir = imgdir
                 self._index = 0
                 self._size = 5
-
-            def read_img(self):
-                return np.random.random((20, 10))
+                self._dummy_array = np.ones(shape=(5, 20, 10))
+                self._dummy_array[0, ...] = 10
+                self._dummy_array[1, ...] = 20
+                self._dummy_array[2, ...] = 30
+                self._dummy_array[3, ...] = 40
+                self._dummy_array[4, ...] = 50
 
             def __iter__(self):
                 return self
 
             def __len__(self):
                 return self._size
 
             def __next__(self):
                 if self._index < self._size:
+                    arr = self._dummy_array[self._index]
                     self._index += 1
-                    return self.read_img()
+                    return arr
                 raise StopIteration
 
         imgreader = ImgReader('testdir')
         with h5tbx.File() as h5:
             ds = h5.create_dataset_from_image(imgreader, 'testimg', axis=0)
             self.assertEqual(ds.shape, (5, 20, 10))
             self.assertEqual(ds.chunks, (1, 20, 10))
+            for i in range(5):
+                np.testing.assert_equal(ds.values[i, ...],
+                                        np.ones(shape=(20, 10)) * (i + 1) * 10)
             # reset imgreader
             imgreader._index = 0
             ds = h5.create_dataset_from_image(imgreader, 'testimg2', axis=-1)
             self.assertEqual(ds.shape, (20, 10, 5))
             self.assertEqual(ds.chunks, (20, 10, 1))
+            for i in range(5):
+                np.testing.assert_equal(ds.values[..., i],
+                                        np.ones(shape=(20, 10)) * (i + 1) * 10)
 
         # write more tests for create_dataset_from_image:
         with h5tbx.File() as h5:
-            ds = h5.create_dataset_from_image([np.random.random((20, 10))] * 5,
+            arr_list = [np.random.random((20, 10)).astype('float32')] * 5
+            ds = h5.create_dataset_from_image(arr_list,
                                               'testimg', axis=0)
             self.assertEqual(ds.shape, (5, 20, 10))
             self.assertEqual(ds.chunks, (1, 20, 10))
+            for i in range(5):
+                np.testing.assert_array_almost_equal(ds.values[i, ...], arr_list[i], decimal=5)
 
         imgreader._index = 0
         h5tbx.use('h5py')
         with h5tbx.File() as h5:
             ds = h5.create_dataset_from_image(imgreader, 'testimg', axis=0,
                                               attrs=dict(units='', long_name='test'))
             self.assertEqual(ds.shape, (5, 20, 10))
@@ -404,25 +476,29 @@
                                               attrs=dict(units='', long_name='test'))
             self.assertEqual(ds.shape, (20, 10, 5))
             self.assertEqual(ds.chunks, (20, 10, 1))
 
         # write more tests for create_dataset_from_image:
         with h5tbx.File() as h5:
             ds = h5.create_dataset_from_image([np.random.random((20, 10))] * 5,
-                                              'testimg', axis=0, attrs=dict(units='', long_name='test'))
+                                              'testimg', axis=0,
+                                              attrs=dict(units='', long_name='test'))
             self.assertEqual(ds.shape, (5, 20, 10))
             self.assertEqual(ds.chunks, (1, 20, 10))
+            self.assertEqual(ds.attrs['units'], '')
+            self.assertEqual(ds.attrs['long_name'], 'test')
+            self.assertEqual(ds.name, '/testimg')
 
     def test_properties(self):
         with h5tbx.File() as h5:
             self.assertIsInstance(h5.creation_time, datetime)
             now = datetime.now().astimezone()
             file_now = h5.creation_time
             self.assertTrue(abs((file_now - now).total_seconds()) < 1)
-            self.assertTrue('__h5rdmtoolbox_version__' in h5.attrs)
+            self.assertTrue('__h5rdmtoolbox_version__' in h5['h5rdmtoolbox'].attrs)
             self.assertEqual(h5.version, __version__)
             self.assertEqual(h5.filesize.units, h5tbx.get_ureg().byte)
             self.assertIsInstance(h5.hdf_filename, pathlib.Path)
 
     def test_special_attribute_types(self):
         with h5tbx.File() as h5:
             ds = h5.create_dataset('test', data=np.random.random((10, 10)))
@@ -482,14 +558,15 @@
 
     def test_create_from_yaml(self):
 
         h5y = h5yaml.H5Yaml(__this_dir__ / '../data/from_yaml.yaml')
         with h5tbx.File() as h5:
             h5y.write(h5)
             self.assertIn('grp', h5)
+            self.assertEqual(h5.grp.attrs['comment'], 'test')
             self.assertIn('grp/supgrp', h5)
             self.assertIn('velocity', h5['grp/supgrp'])
             self.assertEqual('Title of the file', h5.attrs['title'])
             self.assertEqual('0000-1234-1234-1234', h5.attrs['contact'])
 
         with h5tbx.File() as h5:
             h5.create_from_yaml(__this_dir__ / '../data/from_yaml.yaml')
@@ -593,14 +670,22 @@
             h5.create_dataset('vel', data=[1.5, 2.5, 3.5], attach_scales='time')
             h5.create_dataset('vel_no_scale', data=[1.5, 2.5, 3.5])
             self.assertIsInstance(h5['vel'].coords(), dict)
             self.assertEqual('time', list(h5['vel'].coords().keys())[0])
             self.assertEqual({'time': h5['time']}, h5['vel'].coords())
             self.assertEqual({}, h5['vel_no_scale'].coords())
 
+        # multiple dims:
+        with h5tbx.File() as h5:
+            h5.create_dataset('x1', data=[1, 2, 3], make_scale=True)
+            h5.create_dataset('x2', data=[10, 20, 30], make_scale=True)
+            h5.create_dataset('data', data=[-1, 0, 1], attach_scales=('x1',))
+            h5['data'].dims[0].attach_scale(h5['x2'])
+            self.assertEqual({'x1': h5['x1'], 'x2': h5['x2']}, h5['data'].coords())
+
     def test_isel_sel(self):
         with h5tbx.File() as h5:
             h5.create_dataset('time', data=[1, 2, 3], make_scale=True)
             h5.create_dataset('vel', data=[1.5, 2.5, 3.5], attach_scales='time')
             np.testing.assert_equal(h5['vel'].values[0:2], h5['vel'].isel(time=slice(0, 2)).values)
             self.assertEqual(3.5, float(h5['vel'].isel(time=2)))
             with self.assertRaises(KeyError):
@@ -609,14 +694,32 @@
             self.assertEqual(2.5, float(h5['vel'].sel(time=2.0)))
             with self.assertRaises(ValueError):
                 h5['vel'].sel(time=1.2)
             with self.assertRaises(NotImplementedError):
                 h5['vel'].sel(time=1.2, method='invalid')
             self.assertEqual(1.5, float(h5['vel'].sel(time=1.2, method='nearest')))
 
+    def test_unit_conversion_interface(self):
+        with h5tbx.File() as h5:
+            h5.create_dataset('time', data=[1, 2, 3], attrs=dict(units='s'), make_scale=True)
+            h5.create_dataset('vel', data=[1.5, 2.5, 3.5], attrs=dict(units='m/s'), attach_scales='time')
+            # print(h5['vel'].to_units('m/s', time='h'))
+            ret = h5['vel'].to_units('mm/s', time='h').sel(time=1.2, method='nearest')
+            self.assertEqual(1.5 * 1000, float(ret))
+            self.assertEqual('mm/s', ret.attrs['units'])
+            self.assertEqual('h', ret.coords['time'].units)
+
+            time_h = h5.time.to_units('h')[()]
+            self.assertEqual(time_h.units, 'h')
+            np.testing.assert_almost_equal(time_h.values, np.array([1, 2, 3]) / 60 / 60)
+
+            time_h = h5.vel.to_units('mm/s').isel(time=1)
+            self.assertEqual(time_h.units, 'mm/s')
+            self.assertEqual(time_h.values, 2.5 * 1000)
+
     def test_multi_isel_and_sel(self):
         with h5tbx.File() as h5:
             time = h5.create_dataset('time', data=ls(0, 1, 10), make_scale=True)
             y = h5.create_dataset('y', data=ls(0, 1, 5), make_scale=True)
             x = h5.create_dataset('x', data=ls(0, 10, 7), make_scale=True)
             h5.create_dataset('data',
                               shape=(10, 5, 7), attach_scales=('time', 'y', 'x'))
@@ -629,14 +732,24 @@
         filename = h5.hdf_filename
 
         with h5tbx.File(filename) as h5:
             d = h5['data'].sel(
                 x=[4.3, 10.9],
                 time=0.2,
                 method='nearest')
+            np.testing.assert_equal(d.x.data, [5, 10])
+
+            d = h5['data'].sel(
+                x=np.linspace(4.3, 10.9, 100),
+                time=0.2,
+                method='nearest')
+            np.testing.assert_array_almost_equal(d.x.data, [5, 6.666667, 8.333333, 10])
+
+            d = h5['data'].isel(x=[0, 1])
+            self.assertEqual(float(d.x[0]), float(h5.x[0]))
 
     def test_create_dataset_with_ancillary_ds(self):
         with h5tbx.File() as h5:
             h5.create_dataset('flag', data=[1, 0, 1], dtype='int8')
             self.assertEqual(h5['flag'].dtype, np.dtype('int8'))
             h5.create_dataset('flag2', data=[0, 0], dtype='int8', make_scale='the_flag_2')
 
@@ -668,17 +781,26 @@
                 h5.create_dataset('vel3', data=[1.5, 2.5], attach_scale='3D')
 
     def test_time(self):
         tdata = [datetime.now(),
                  (datetime.now() + timedelta(hours=1))]
         tdata_np = np.asarray(tdata, dtype=np.datetime64)
         with h5tbx.File() as h5:
-            h5.create_string_dataset('time', data=[t.isoformat() for t in tdata],
-                                     attrs={'ISTIMEDS': 1,
-                                            'TIMEFORMAT': 'ISO'})
+            with h5tbx.set_config(hdf_compression='gzip', hdf_compression_opts=5):
+                h5.create_string_dataset('time', data=[t.isoformat() for t in tdata],
+                                         attrs={'ISTIMEDS': 1,
+                                                'TIMEFORMAT': 'ISO'})
+                self.assertEqual(h5['time'].compression, 'gzip')
+                self.assertEqual(h5['time'].compression_opts, 5)
+                h5.create_string_dataset('single_time', data=tdata[0].isoformat(),
+                                         attrs={'ISTIMEDS': 1,
+                                                'TIMEFORMAT': 'ISO'})
+                self.assertEqual(h5['single_time'].compression, None)
+                self.assertEqual(h5['single_time'].compression_opts, None)
+
             tds = h5['time'][()]
 
             h5.create_time_dataset('time2', data=tdata)
             tds2 = h5['time2'][()]
 
             h5.create_time_dataset('time3', data=tdata_np,
                                    attrs={'ISTIMEDS': 1,
@@ -703,22 +825,62 @@
                                                  datetime.now() + timedelta(hours=1),
                                                  datetime.now() + timedelta(hours=3)],
                                    attrs={'ISTIMEDS': 1,
                                           'TIMEFORMAT': 'ISO'}, make_scale=True)
             h5.create_dataset('vel', data=[1, 2, -3], attach_scale='time')
             v = h5.vel[()]
 
+        with h5tbx.File() as h5:
+            t1 = [datetime.now(),
+                  datetime.now() + timedelta(hours=1),
+                  datetime.now() + timedelta(hours=3)]
+            h5.create_time_dataset('time1', data=t1,
+                                   attrs={'ISTIMEDS': 1,
+                                          'TIMEFORMAT': 'ISO'}, make_scale=True)
+            t2 = [datetime.now(),
+                  datetime.now() + timedelta(days=1),
+                  datetime.now() + timedelta(days=3)]
+            h5.create_time_dataset('time2', data=t2,
+                                   attrs={'ISTIMEDS': 1,
+                                          'TIMEFORMAT': 'ISO'}, make_scale=True)
+            h5.create_dataset('vel', data=[[1, 2, -3],
+                                           [1, 2, -3],
+                                           [1, 2, -3]], attach_scale=('time1', 'time2'))
+            v = h5.vel[()]
+            self.assertEqual(v.shape, (3, 3))
+            self.assertEqual(v.dims[0], 'time1')
+            self.assertEqual(v.dims[1], 'time2')
+            self.assertEqual(parse(str(v.time1[0].data).strip('0')),
+                             parse(str(t1[0]).strip('0')))
+            self.assertEqual(parse(str(v.time2[0].data).strip('0')),
+                             parse(str(t2[0]).strip('0')))
+
     def test_multidim_time_ds(self):
         with h5tbx.File() as h5:
-            h5.create_time_dataset('time', data=[[datetime.now(),
-                                                  datetime.now() + timedelta(hours=1),
-                                                  datetime.now() + timedelta(hours=3)],
-                                                 [datetime.now(),
-                                                  datetime.now() + timedelta(hours=6),
-                                                  datetime.now() + timedelta(hours=10)]
-                                                 ],
+            h5.create_time_dataset('time',
+                                   data=[[datetime.now(),
+                                          datetime.now() + timedelta(hours=1),
+                                          datetime.now() + timedelta(hours=3)],
+                                         [datetime.now(),
+                                          datetime.now() + timedelta(hours=6),
+                                          datetime.now() + timedelta(hours=10)]
+                                         ],
                                    attrs={'ISTIMEDS': 1,
                                           'TIMEFORMAT': 'ISO'})
             t = h5.time[()]
             self.assertIsInstance(t, xr.DataArray)
             self.assertEqual(t.shape, (2, 3))
             self.assertIsInstance(t[0, 0].values, np.datetime64)
+
+    def test_attr_group_link_and_xarray(self):
+        with h5tbx.File() as h5:
+            grp = h5.create_group('my_grp')
+            ds = h5.create_dataset(name='ds', data=4)
+
+            ds.attrs['link to grp'] = grp
+
+            self.assertIsInstance(ds.attrs['link to grp'], h5py.Group)
+
+            da = ds[()]
+            self.assertIsInstance(da, xr.DataArray)
+            self.assertIsInstance(da.attrs['link to grp'], str)
+            print(da)
```

### Comparing `h5rdmtoolbox-1.2.2/tests/wrapper/test_h5ext.py` & `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_h5ext.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.2.2/tests/wrapper/test_xr2df.py` & `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_xr2df.py`

 * *Files identical despite different names*

