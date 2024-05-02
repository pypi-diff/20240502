# Comparing `tmp/quark-engine-24.4.1.tar.gz` & `tmp/quark_engine-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quark-engine-24.4.1.tar", last modified: Wed Apr  3 06:23:47 2024, max compression
+gzip compressed data, was "quark_engine-24.5.1.tar", last modified: Thu May  2 09:27:06 2024, max compression
```

## Comparing `quark-engine-24.4.1.tar` & `quark_engine-24.5.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.005511 quark-engine-24.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 06:23:32.000000 quark-engine-24.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-03 06:23:47.005511 quark-engine-24.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-03 06:23:32.000000 quark-engine-24.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:46.997511 quark-engine-24.4.1/quark/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:46.997511 quark-engine-24.4.1/quark/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/apkinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:46.997511 quark-engine-24.4.1/quark/core/axmlreader/
--rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/axmlreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/axmlreader/axml_definition
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:46.997511 quark-engine-24.4.1/quark/core/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/interface/baseapkinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/parallelquark.py
--rw-r--r--   0 runner    (1001) docker     (127)    30370 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/quark.py
--rw-r--r--   0 runner    (1001) docker     (127)    23110 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/r2apkinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    19911 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/rzapkinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.001511 quark-engine-24.4.1/quark/core/struct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/struct/bytecodeobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/struct/methodobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/struct/registerobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/struct/ruleobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/core/struct/tableobject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.001511 quark-engine-24.4.1/quark/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/evaluator/pyeval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.001511 quark-engine-24.4.1/quark/forensic/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/forensic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/forensic/forensic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/forensic/vt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/freshquark.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/radiocontrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/rulegeneration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.001511 quark-engine-24.4.1/quark/script/
--rw-r--r--   0 runner    (1001) docker     (127)    21288 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/script/ciphey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.001511 quark-engine-24.4.1/quark/script/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/script/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/script/frida/agent.js
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/script/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/script/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.001511 quark-engine-24.4.1/quark/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/utils/weight.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.005511 quark-engine-24.4.1/quark/webreport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/webreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21921 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/webreport/analysis_report_layout.html
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/webreport/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    24449 2024-04-03 06:23:32.000000 quark-engine-24.4.1/quark/webreport/genrule_report_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.005511 quark-engine-24.4.1/quark_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-03 06:23:46.000000 quark-engine-24.4.1/quark_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-03 06:23:46.000000 quark-engine-24.4.1/quark_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:23:46.000000 quark-engine-24.4.1/quark_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 06:23:46.000000 quark-engine-24.4.1/quark_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 06:23:46.000000 quark-engine-24.4.1/quark_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 06:23:46.000000 quark-engine-24.4.1/quark_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:23:47.005511 quark-engine-24.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-03 06:23:32.000000 quark-engine-24.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:23:47.005511 quark-engine-24.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-03 06:23:32.000000 quark-engine-24.4.1/tests/test_freshquark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-03 06:23:32.000000 quark-engine-24.4.1/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.260493 quark_engine-24.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 09:26:58.000000 quark_engine-24.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-02 09:27:06.260493 quark_engine-24.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-05-02 09:26:58.000000 quark_engine-24.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.252493 quark_engine-24.5.1/quark/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.252493 quark_engine-24.5.1/quark/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/apkinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.252493 quark_engine-24.5.1/quark/core/axmlreader/
+-rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/axmlreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/axmlreader/axml_definition
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.252493 quark_engine-24.5.1/quark/core/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/interface/baseapkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/parallelquark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30370 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/quark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23110 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/r2apkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19911 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/rzapkinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.256493 quark_engine-24.5.1/quark/core/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/struct/bytecodeobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/struct/methodobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/struct/registerobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/struct/ruleobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/core/struct/tableobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.256493 quark_engine-24.5.1/quark/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/evaluator/pyeval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.256493 quark_engine-24.5.1/quark/forensic/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/forensic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/forensic/forensic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/forensic/vt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/freshquark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/radiocontrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/rulegeneration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.256493 quark_engine-24.5.1/quark/script/
+-rw-r--r--   0 runner    (1001) docker     (127)    21288 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/script/ciphey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.256493 quark_engine-24.5.1/quark/script/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/script/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/script/frida/agent.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/script/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/script/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.256493 quark_engine-24.5.1/quark/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/utils/weight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.256493 quark_engine-24.5.1/quark/webreport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/webreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21921 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/webreport/analysis_report_layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/webreport/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24449 2024-05-02 09:26:58.000000 quark_engine-24.5.1/quark/webreport/genrule_report_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.260493 quark_engine-24.5.1/quark_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-02 09:27:06.000000 quark_engine-24.5.1/quark_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-02 09:27:06.000000 quark_engine-24.5.1/quark_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:27:06.000000 quark_engine-24.5.1/quark_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 09:27:06.000000 quark_engine-24.5.1/quark_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 09:27:06.000000 quark_engine-24.5.1/quark_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:27:06.000000 quark_engine-24.5.1/quark_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:27:06.260493 quark_engine-24.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-02 09:26:58.000000 quark_engine-24.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:27:06.260493 quark_engine-24.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-02 09:26:58.000000 quark_engine-24.5.1/tests/test_freshquark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-02 09:26:58.000000 quark_engine-24.5.1/tests/test_report.py
```

### Comparing `quark-engine-24.4.1/LICENSE` & `quark_engine-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/PKG-INFO` & `quark_engine-24.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quark-engine
-Version: 24.4.1
+Version: 24.5.1
 Summary: An Obfuscation-Neglect Android Malware Scoring System
 Home-page: https://github.com/quark-engine/quark-engine
 Author: YuShiang Dang, ShengFeng Lu, KunYu Chen
 Author-email: pulorsok@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quark-engine Version: 24.4.1 Summary: An
+Metadata-Version: 2.1 Name: quark-engine Version: 24.5.1 Summary: An
 Obfuscation-Neglect Android Malware Scoring System Home-page: https://
 github.com/quark-engine/quark-engine Author: YuShiang Dang, ShengFeng Lu, KunYu
 Chen Author-email: pulorsok@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Topic ::
 Security Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: prettytable>=1.0.0 Requires-Dist:
```

### Comparing `quark-engine-24.4.1/README.md` & `quark_engine-24.5.1/README.md`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/cli.py` & `quark_engine-24.5.1/quark/cli.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/analysis.py` & `quark_engine-24.5.1/quark/core/analysis.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/apkinfo.py` & `quark_engine-24.5.1/quark/core/apkinfo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/axmlreader/__init__.py` & `quark_engine-24.5.1/quark/core/axmlreader/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/axmlreader/axml_definition` & `quark_engine-24.5.1/quark/core/axmlreader/axml_definition`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/interface/baseapkinfo.py` & `quark_engine-24.5.1/quark/core/interface/baseapkinfo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/parallelquark.py` & `quark_engine-24.5.1/quark/core/parallelquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/quark.py` & `quark_engine-24.5.1/quark/core/quark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/r2apkinfo.py` & `quark_engine-24.5.1/quark/core/r2apkinfo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/rzapkinfo.py` & `quark_engine-24.5.1/quark/core/rzapkinfo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/struct/bytecodeobject.py` & `quark_engine-24.5.1/quark/core/struct/bytecodeobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/struct/methodobject.py` & `quark_engine-24.5.1/quark/core/struct/methodobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/struct/registerobject.py` & `quark_engine-24.5.1/quark/core/struct/registerobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/struct/ruleobject.py` & `quark_engine-24.5.1/quark/core/struct/ruleobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/core/struct/tableobject.py` & `quark_engine-24.5.1/quark/core/struct/tableobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/evaluator/pyeval.py` & `quark_engine-24.5.1/quark/evaluator/pyeval.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/forensic/forensic.py` & `quark_engine-24.5.1/quark/forensic/forensic.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/forensic/vt_analysis.py` & `quark_engine-24.5.1/quark/forensic/vt_analysis.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/freshquark.py` & `quark_engine-24.5.1/quark/freshquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/logo.py` & `quark_engine-24.5.1/quark/logo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/radiocontrast.py` & `quark_engine-24.5.1/quark/radiocontrast.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/report.py` & `quark_engine-24.5.1/quark/report.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/rulegeneration.py` & `quark_engine-24.5.1/quark/rulegeneration.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/script/__init__.py` & `quark_engine-24.5.1/quark/script/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/script/ciphey.py` & `quark_engine-24.5.1/quark/script/ciphey.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/script/frida/__init__.py` & `quark_engine-24.5.1/quark/script/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/script/frida/agent.js` & `quark_engine-24.5.1/quark/script/frida/agent.js`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/script/objection.py` & `quark_engine-24.5.1/quark/script/objection.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/utils/colors.py` & `quark_engine-24.5.1/quark/utils/colors.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/utils/graph.py` & `quark_engine-24.5.1/quark/utils/graph.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/utils/output.py` & `quark_engine-24.5.1/quark/utils/output.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/utils/pprint.py` & `quark_engine-24.5.1/quark/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/utils/regex.py` & `quark_engine-24.5.1/quark/utils/regex.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/utils/tools.py` & `quark_engine-24.5.1/quark/utils/tools.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/utils/weight.py` & `quark_engine-24.5.1/quark/utils/weight.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/webreport/analysis_report_layout.html` & `quark_engine-24.5.1/quark/webreport/analysis_report_layout.html`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/webreport/generate.py` & `quark_engine-24.5.1/quark/webreport/generate.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark/webreport/genrule_report_layout.html` & `quark_engine-24.5.1/quark/webreport/genrule_report_layout.html`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/quark_engine.egg-info/PKG-INFO` & `quark_engine-24.5.1/quark_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quark-engine
-Version: 24.4.1
+Version: 24.5.1
 Summary: An Obfuscation-Neglect Android Malware Scoring System
 Home-page: https://github.com/quark-engine/quark-engine
 Author: YuShiang Dang, ShengFeng Lu, KunYu Chen
 Author-email: pulorsok@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quark-engine Version: 24.4.1 Summary: An
+Metadata-Version: 2.1 Name: quark-engine Version: 24.5.1 Summary: An
 Obfuscation-Neglect Android Malware Scoring System Home-page: https://
 github.com/quark-engine/quark-engine Author: YuShiang Dang, ShengFeng Lu, KunYu
 Chen Author-email: pulorsok@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Topic ::
 Security Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: prettytable>=1.0.0 Requires-Dist:
```

### Comparing `quark-engine-24.4.1/quark_engine.egg-info/SOURCES.txt` & `quark_engine-24.5.1/quark_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/setup.py` & `quark_engine-24.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/tests/test_freshquark.py` & `quark_engine-24.5.1/tests/test_freshquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-24.4.1/tests/test_report.py` & `quark_engine-24.5.1/tests/test_report.py`

 * *Files identical despite different names*

