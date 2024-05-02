# Comparing `tmp/flightanalysis-0.2.6.tar.gz` & `tmp/flightanalysis-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightanalysis-0.2.6.tar", last modified: Thu Apr 18 12:15:24 2024, max compression
+gzip compressed data, was "flightanalysis-0.2.7.tar", last modified: Wed May  1 09:30:12 2024, max compression
```

## Comparing `flightanalysis-0.2.6.tar` & `flightanalysis-0.2.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.035287 flightanalysis-0.2.6/flightanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.035287 flightanalysis-0.2.6/flightanalysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/el_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.035287 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/complete.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/scored.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/sch_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.039287 flightanalysis-0.2.6/flightanalysis/data/
--rw-r--r--   0 runner    (1001) docker     (127)    72721 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/IMAC_Unlimited2024_schedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60591 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_a25_schedule.json
--rw-r--r--   0 runner    (1001) docker     (127)   100154 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_f25_schedule.json
--rw-r--r--   0 runner    (1001) docker     (127)    87050 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_p23_schedule.json
--rw-r--r--   0 runner    (1001) docker     (127)   101042 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_p25_schedule.json
--rw-r--r--   0 runner    (1001) docker     (127)    45110 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3auk_clubman_schedule.json
--rw-r--r--   0 runner    (1001) docker     (127)    40407 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3auk_inter_schedule.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.039287 flightanalysis-0.2.6/flightanalysis/definition/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.039287 flightanalysis-0.2.6/flightanalysis/definition/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/elbuilders.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/manbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/collectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/eldef.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/mandef.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/maninfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/manoption.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/manparm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/definition/operations/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/funopp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/itemopp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/mathopp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/scheddef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/scheduleinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/autorotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/nose_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/pitch_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/stall_turn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/manoeuvre.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/scoring/criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/f3a_criteria.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/combination.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/bounded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/downgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/flightanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/scripts/batch_analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/scripts/collect_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/tests/test_criiteria.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/tests/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.689256 flightanalysis-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 09:30:12.689256 flightanalysis-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.673256 flightanalysis-0.2.7/flightanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.677256 flightanalysis-0.2.7/flightanalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/el_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.677256 flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/scored.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/analysis/sch_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.681256 flightanalysis-0.2.7/flightanalysis/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    72721 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/IMAC_Unlimited2024_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60591 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/f3a_a25_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)   100154 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/f3a_f25_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    87050 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/f3a_p23_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)   101042 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/f3a_p25_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45110 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/f3auk_clubman_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40407 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/data/f3auk_inter_schedule.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.681256 flightanalysis-0.2.7/flightanalysis/definition/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.681256 flightanalysis-0.2.7/flightanalysis/definition/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/builders/elbuilders.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/builders/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/builders/manbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/eldef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/mandef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/maninfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/manoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/manparm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.681256 flightanalysis-0.2.7/flightanalysis/definition/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/operations/funopp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/operations/itemopp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/operations/mathopp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/scheddef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/definition/scheduleinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.685256 flightanalysis-0.2.7/flightanalysis/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/autorotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/nose_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/pitch_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/elements/stall_turn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/manoeuvre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.685256 flightanalysis-0.2.7/flightanalysis/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.685256 flightanalysis-0.2.7/flightanalysis/scoring/criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/f3a_criteria.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.685256 flightanalysis-0.2.7/flightanalysis/scoring/criteria/inter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/inter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/inter/combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/inter/comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.689256 flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/bounded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/downgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/flightanalysis/scoring/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.689256 flightanalysis-0.2.7/flightanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 09:30:12.000000 flightanalysis-0.2.7/flightanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-01 09:30:12.000000 flightanalysis-0.2.7/flightanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:30:12.000000 flightanalysis-0.2.7/flightanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 09:30:12.000000 flightanalysis-0.2.7/flightanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 09:30:12.000000 flightanalysis-0.2.7/flightanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.689256 flightanalysis-0.2.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/scripts/batch_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/scripts/collect_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-01 09:30:12.689256 flightanalysis-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:30:12.689256 flightanalysis-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/tests/test_criiteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 09:29:39.000000 flightanalysis-0.2.7/tests/test_data.py
```

### Comparing `flightanalysis-0.2.6/LICENSE` & `flightanalysis-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/PKG-INFO` & `flightanalysis-0.2.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: fastdtw
 Requires-Dist: simplejson
-Requires-Dist: pfc-geometry>=0.2.4
-Requires-Dist: flightdata>=0.2.6
+Requires-Dist: pfc-geometry>=0.2.5
+Requires-Dist: flightdata>=0.2.7
 
 # FlightAnalysis
 
 This package contains tools for analysing recorded flight log data.The main objective is 
 to facilitate automated judging for precision aerobatic competitions.
```

### Comparing `flightanalysis-0.2.6/flightanalysis/analysis/el_analysis.py` & `flightanalysis-0.2.7/flightanalysis/analysis/el_analysis.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/alignment.py` & `flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/alignment.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,67 +5,77 @@
 from loguru import logger
 from .basic import AlinmentStage, Basic
 from flightanalysis.definition import ManDef
 
 
 @dataclass
 class Alignment(Basic):
+    dist: float
     manoeuvre: Manoeuvre
     template: State
 
-    def run_all(self):
+    def run_all(self, optimise_aligment=True):
+        new = self
         while self.__class__.__name__ != 'Scored':
-            new = self.run()
+            new = self.run(optimise_aligment)
             if new.__class__.__name__ == self.__class__.__name__:
                 break
             self = new
         return new
     
     @staticmethod
     def from_dict(data: dict, fallback=True):
         ia = Basic.from_dict(data)
         try:    
             ia = Alignment(
+                dist=data['dist'] if 'dist' in data else 0,
                 manoeuvre=Manoeuvre.from_dict(data['manoeuvre']),
                 template=State.from_dict(data['template']),
                 **ia.__dict__
             )
         except Exception as e:
             if fallback:
                 logger.debug(f'Failed to parse Alignment {repr(e)}')
             else:
                 raise e
         return ia
 
     def alignment(self, radius=10):
         assert self.stage < AlinmentStage.SECONDARY
         logger.debug(f'Running alignment stage {self.stage}')
-        aligned = State.align(self.flown, self.template, radius, self.stage==AlinmentStage.SETUP)[1]
+        dist, aligned = State.align(self.flown, self.template, radius, self.stage==AlinmentStage.SETUP)
         return Alignment(
-            self.mdef, aligned, self.direction, self.stage + 1,
+            self.mdef, aligned, self.direction, self.stage + 1, dist,
             *self.manoeuvre.match_intention(self.template[0], aligned)
         )
+    
 
     def run_alignment(self, radius=10):
+        if self.stage > AlinmentStage.SETUP:
+            self = Alignment(
+                self.mdef, self.flown, self.direction, self.stage + 1, self.dist,
+                *self.manoeuvre.match_intention(self.template[0], self.flown)
+            )
         while self.stage < AlinmentStage.SECONDARY:
             try:
                 self = self.alignment(radius)
             except Exception as ex:
                 logger.exception(f'Error running alignment stage {self.stage}, {ex}')
                 break
         return self
 
-    def run(self) -> Complete:
+    def run(self, optimise_aligment=True) -> Complete:
         self = self.run_alignment()
+
         if self.stage < AlinmentStage.SECONDARY:
             return self
         else:
             mdef = ManDef(self.mdef.info, self.mdef.mps.update_defaults(self.manoeuvre), self.mdef.eds)
             correction = mdef.create(self.template[0].transform).add_lines()
 
             return Complete(
                 mdef, self.flown, self.direction, AlinmentStage.SECONDARY, 
-                self.manoeuvre, self.template, correction, 
+                self.dist, self.manoeuvre, self.template, correction, 
                 correction.create_template(self.template[0], self.flown)
             )
 
 from .complete import Complete  # noqa: E402
```

### Comparing `flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/basic.py` & `flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from flightdata import State, Flight, Origin
 from flightanalysis.definition import ManDef, SchedDef, ManOption
 import geometry as g
 from json import load
 from .analysis import AlinmentStage, Analysis
+import numpy as np
 
 
 @dataclass
 class Basic(Analysis):
     mdef: ManDef | ManOption
     flown: State
     direction: int
     stage: AlinmentStage
 
     @property
     def name(self):
         return self.mdef.uid
 
-    def run_all(self):
-        res = [s for s in [s.run_all() for s in self.run()] if isinstance(s, Scored)]
-        
-        if len(res) == 0:
-            return self
-                
-        min_dg = None
-        for n in res:
-            if hasattr(n, 'scores'):
-                if min_dg is None or n.scores.intra.total < min_dg:
-                    min_dg = n.scores.intra.total
-                    self = n 
+    def run_all(self, optimise_aligment=True):
+        res = [s.run_all(False) for s in self.run(False)]
+        self = res[0]
+        if len(res) > 1:
+            for r in res[1:]:
+                if r.stage < self.stage:
+                    continue
+                if r.dist < self.dist:
+                    self = r
+
+        if isinstance(self, Scored) and optimise_aligment:
+            self.stage = AlinmentStage.SECONDARY
+            self = self.run(True)
                    
         return self
         
-
     @classmethod
     def from_dict(Cls, data:dict) -> Basic:
         return Basic(
             ManDef.from_dict(data["mdef"]),
             State.from_dict(data["flown"]),
             data['direction'],
             data['stage']
@@ -61,23 +62,23 @@
         state = State.from_flight(flight, box).splitter_labels(
             data["mans"],
             [m.info.short_name for m in sdef]
         )
         mdef= sdef[mid]
         return Basic(mdef, state.get_manoeuvre(mdef.uid), AlinmentStage.SETUP)
 
-    def run(self) -> list[Alignment]:
+    def run(self, optimise_aligment=True) -> list[Alignment]:
         itrans = self.create_itrans()
         mopt = ManOption([self.mdef]) if isinstance(self.mdef, ManDef) else self.mdef
 
         als = []        
         for mdef in mopt:
             man = mdef.create(itrans).add_lines()
             als.append(Alignment(
                 mdef, self.flown, self.direction, AlinmentStage.SETUP, 
-                man, man.create_template(itrans)
+                1e9, man, man.create_template(itrans)
             ))
         return als
 
 
 from .alignment import Alignment  # noqa: E402
 from .scored import Scored  # noqa: E402
```

### Comparing `flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/complete.py` & `flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/complete.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,18 @@
         except Exception as e:
             if fallback:
                 logger.debug(f"Failed to parse Complete: {repr(e)}")
             else:
                 raise e
         return pa
 
-    def run(self) -> Scored:
-        if self.stage < AlinmentStage.OPTIMISED:
+    def run(self, optimise_aligment=True) -> Scored:
+        if self.stage < AlinmentStage.OPTIMISED and optimise_aligment:
             self = self.optimise_alignment()
+        self = self.update_templates()
         return Scored(**self.__dict__, 
             scores=ManoeuvreResults(self.inter(), self.intra(), self.positioning())
         )
 
     @property
     def elnames(self):
         return list(self.mdef.eds.data.keys())
@@ -58,24 +59,30 @@
 
     def get_ea(self, edef):
         el = getattr(self.manoeuvre.all_elements(), edef.name)
         st = el.get_data(self.flown)
         tp = el.get_data(self.template).relocate(st.pos[0])
         return ElementAnalysis(edef, self.mdef.mps, el, st, tp, el.ref_frame(tp))
 
+    def update_templates(self):
+        if not np.all(self.flown.element == self.template.element):    
+            manoeuvre, template = self.manoeuvre.match_intention(self.template[0], self.flown)
+            mdef = ManDef(self.mdef.info, self.mdef.mps.update_defaults(self.manoeuvre), self.mdef.eds)
+            correction = mdef.create(self.template[0].transform).add_lines()
+
+            return Complete(
+                mdef, self.flown, self.direction, AlinmentStage.OPTIMISED, self.dist,
+                manoeuvre, template, correction, correction.create_template(template[0])
+            )
+        else:
+            return self
+    
     def optimise_alignment(self):
-        aligned = self.manoeuvre.optimise_alignment(self.template, self.flown)
-        manoeuvre, template = self.manoeuvre.match_intention(self.template[0], aligned)
-        mdef = ManDef(self.mdef.info, self.mdef.mps.update_defaults(self.manoeuvre), self.mdef.eds)
-        correction = mdef.create(self.template[0].transform).add_lines()
-
-        return Complete(
-            mdef, aligned, self.direction, AlinmentStage.OPTIMISED, 
-            manoeuvre, template, correction, correction.create_template(template[0])
-        )
+        self.flown = self.manoeuvre.optimise_alignment(self.template, self.flown)
+        return self.update_templates()
     
     def side_box(self):
         return F3A.intra.box(
             'side box', 
             Measurement.side_box(self.flown)
         )
```

### Comparing `flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/scored.py` & `flightanalysis-0.2.7/flightanalysis/analysis/manoeuvre_analysis/scored.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,9 +19,9 @@
         except Exception as e:
             if fallback:
                 logger.debug(f"Failed to read scores, {repr(e)}")
             else:
                 raise e
         return ca
     
-    def run(self):
+    def run(self, optimise_alignment=True):
         return self
```

### Comparing `flightanalysis-0.2.6/flightanalysis/analysis/sch_analysis.py` & `flightanalysis-0.2.7/flightanalysis/analysis/sch_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         
 
         state = State.from_flight(flight, box).splitter_labels(
             data["mans"],
             sdef.uids
         )#.move(g.Transformation(g.Point(-data['parameters']['moveEast'], -data['parameters']['moveNorth'], 0)))
 
-        direction = -state.get_manoeuvre(0)[0].direction()[0]
+        direction = -state.get_manoeuvre(1)[0].direction()[0]
 
         return ScheduleAnalysis(
             [analysis.Basic(
                 mdef, 
                 state.get_manoeuvre(mdef.uid), 
                 direction,
                 analysis.AlinmentStage.SETUP
```

### Comparing `flightanalysis-0.2.6/flightanalysis/data/IMAC_Unlimited2024_schedule.json` & `flightanalysis-0.2.7/flightanalysis/data/IMAC_Unlimited2024_schedule.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/data/f3a_a25_schedule.json` & `flightanalysis-0.2.7/flightanalysis/data/f3a_a25_schedule.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/data/f3a_f25_schedule.json` & `flightanalysis-0.2.7/flightanalysis/data/f3a_f25_schedule.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/data/f3a_p23_schedule.json` & `flightanalysis-0.2.7/flightanalysis/data/f3a_p23_schedule.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/data/f3a_p25_schedule.json` & `flightanalysis-0.2.7/flightanalysis/data/f3a_p25_schedule.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/data/f3auk_clubman_schedule.json` & `flightanalysis-0.2.7/flightanalysis/data/f3auk_clubman_schedule.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/data/f3auk_inter_schedule.json` & `flightanalysis-0.2.7/flightanalysis/data/f3auk_inter_schedule.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/__init__.py` & `flightanalysis-0.2.7/flightanalysis/definition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/builders/elbuilders.py` & `flightanalysis-0.2.7/flightanalysis/definition/builders/elbuilders.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/builders/manbuilder.py` & `flightanalysis-0.2.7/flightanalysis/definition/builders/manbuilder.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/collectors.py` & `flightanalysis-0.2.7/flightanalysis/definition/collectors.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/eldef.py` & `flightanalysis-0.2.7/flightanalysis/definition/eldef.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/mandef.py` & `flightanalysis-0.2.7/flightanalysis/definition/mandef.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/maninfo.py` & `flightanalysis-0.2.7/flightanalysis/definition/maninfo.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/manoption.py` & `flightanalysis-0.2.7/flightanalysis/definition/manoption.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/manparm.py` & `flightanalysis-0.2.7/flightanalysis/definition/manparm.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/operations/funopp.py` & `flightanalysis-0.2.7/flightanalysis/definition/operations/funopp.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/operations/itemopp.py` & `flightanalysis-0.2.7/flightanalysis/definition/operations/itemopp.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/operations/mathopp.py` & `flightanalysis-0.2.7/flightanalysis/definition/operations/mathopp.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/operations/operation.py` & `flightanalysis-0.2.7/flightanalysis/definition/operations/operation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/scheddef.py` & `flightanalysis-0.2.7/flightanalysis/definition/scheddef.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/definition/scheduleinfo.py` & `flightanalysis-0.2.7/flightanalysis/definition/scheduleinfo.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/autorotation.py` & `flightanalysis-0.2.7/flightanalysis/elements/autorotation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/element.py` & `flightanalysis-0.2.7/flightanalysis/elements/element.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/line.py` & `flightanalysis-0.2.7/flightanalysis/elements/line.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/loop.py` & `flightanalysis-0.2.7/flightanalysis/elements/loop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/nose_drop.py` & `flightanalysis-0.2.7/flightanalysis/elements/nose_drop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/pitch_break.py` & `flightanalysis-0.2.7/flightanalysis/elements/pitch_break.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/recovery.py` & `flightanalysis-0.2.7/flightanalysis/elements/recovery.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/elements/stall_turn.py` & `flightanalysis-0.2.7/flightanalysis/elements/stall_turn.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/manoeuvre.py` & `flightanalysis-0.2.7/flightanalysis/manoeuvre.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/schedule.py` & `flightanalysis-0.2.7/flightanalysis/schedule.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/criteria/criteria.py` & `flightanalysis-0.2.7/flightanalysis/scoring/criteria/criteria.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/criteria/exponential.py` & `flightanalysis-0.2.7/flightanalysis/scoring/criteria/exponential.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/criteria/f3a_criteria.py` & `flightanalysis-0.2.7/flightanalysis/scoring/criteria/f3a_criteria.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/combination.py` & `flightanalysis-0.2.7/flightanalysis/scoring/criteria/inter/combination.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/bounded.py` & `flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/bounded.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/continuous.py` & `flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/continuous.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,32 +48,30 @@
 
     @staticmethod
     def convolve(data, width):
         kernel = np.ones(width) / width
         outd = np.full(len(data), np.nan)
         conv = np.convolve(data, kernel, mode='valid')
         ld = (len(data) - len(conv))/2
-        outd[int(np.ceil(ld)):-int(np.floor(ld))] = conv
-        outd[:width//2] = np.linspace(np.mean(data[0:width//4]), outd[width//2],width//2)
-        outd[-width//2:] = np.linspace(outd[-width//2], np.mean(data[-1-width//4:-1]),width//2)
+        ldc = int(np.ceil(ld))
+        ldf = int(np.floor(ld))
+        outd[ldf:-ldc] = conv
+        outd[:ldf] = np.linspace(np.mean(data[:ldf]), conv[0],ldf+1)[:-1]
+        outd[-ldc:] = np.linspace(conv[-1], np.mean(data[-ldc:]), ldc+1)[1:]
         return outd
 
 
 class ContAbs(Continuous):
-#    def prepare(self, value: npt.NDArray, expected: float):
-#        
-#        return  value - expected
-
     def prepare(self, values: npt.NDArray, expected: float):
-        window = 30
+#        window = 30
         sample = values - expected
-        if len(sample) <= window:
+        if len(sample) <= 8:
             return np.linspace(values[0],values[-1], len(sample))
         else:
-            return Continuous.convolve(sample, window)
+            return Continuous.convolve(sample, min(len(values)//3, 40))
 
     @staticmethod
     def mistakes(data, peaks, troughs):
         '''All increases away from zero are downgraded (only peaks)'''
         last_trough = -1 if troughs[-1] else None
         first_peak = 1 if peaks[0] else 0
         return np.abs(data[first_peak:][peaks[first_peak:]] - data[:last_trough][troughs[:last_trough]])
@@ -83,23 +81,23 @@
         first_peak = 1 if peaks[0] else 0
         return ids[first_peak:][peaks[first_peak:]]
 
 
 class ContRat(Continuous):
     
     def prepare(self, values: npt.NDArray, expected: float):
-        window = 40
-        if len(values) <= window:
+        #window = 40
+        if len(values) <= 8:
             return np.abs(np.linspace(
                 np.mean(values[:1+len(values)//3]), 
                 np.mean(values[-1-len(values)//3:]), 
                 len(values)
             ))
         else:
-            return np.abs(Continuous.convolve(values, window))
+            return np.abs(Continuous.convolve(values, min(len(values)//3, 40)))
             
     @staticmethod
     def mistakes(data, peaks, troughs):
         '''All changes are downgraded (peaks and troughs)'''
         values = data[peaks + troughs]
         return np.maximum(values[:-1], values[1:]) / np.minimum(values[:-1], values[1:]) - 1
```

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/single.py` & `flightanalysis-0.2.7/flightanalysis/scoring/criteria/intra/single.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/downgrade.py` & `flightanalysis-0.2.7/flightanalysis/scoring/downgrade.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/measurement.py` & `flightanalysis-0.2.7/flightanalysis/scoring/measurement.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,19 +70,31 @@
     @staticmethod
     def _vector_vis(direction: Point, loc: Point) -> Union[Point, npt.NDArray]:
         #a vector error is more visible if it is perpendicular to the viewing vector
         # 0 to np.pi, pi/2 gives max, 0&np.pi give min
         return direction,  (1 - 0.8* np.abs(Point.cos_angle_between(loc, direction))) * Measurement._pos_vis(loc)
 
     @staticmethod
-    def _roll_vis(loc: Point, att: Quaternion) -> Union[Point, npt.NDArray]:
-        #a roll error is more visible if the movement of the wing tips is perpendicular to the view vector
-        #the wing tips move in the local body Z axis
-        world_tip_movement_direction = att.transform_point(PZ()) 
-        return world_tip_movement_direction, (1-0.8*np.abs(Point.cos_angle_between(loc, world_tip_movement_direction))) * Measurement._pos_vis(loc)
+    def _roll_vis(fl: State, tp: State) -> Union[Point, npt.NDArray]:
+        
+        
+        afl = Point.cos_angle_between(fl.pos, fl.att.transform_point(PZ()))
+        atp = Point.cos_angle_between(tp.pos, tp.att.transform_point(PZ()))
+
+        azfl = np.cos(fl.att.inverse().transform_point(-fl.pos).planar_angles().x)
+        aztp = np.cos(tp.att.inverse().transform_point(-tp.pos).planar_angles().x)
+
+        ao = afl.copy()
+
+        ao[np.abs(afl) > np.abs(atp)] = atp[np.abs(afl) > np.abs(atp)]
+        ao[np.sign(azfl) != np.sign(aztp)] = 0 # wings have passed through the view vector
+
+        rvis = (1-0.8*np.abs(ao))
+        
+        return fl.att.transform_point(PZ()), rvis * Measurement._pos_vis(fl.pos)
 
     @staticmethod
     def _rad_vis(loc:Point, axial_dir: Point) -> Union[Point, npt.NDArray]:
         #radial error more visible if axis is parallel to the view vector
         return axial_dir, (0.2+0.8*np.abs(Point.cos_angle_between(loc, axial_dir))) * Measurement._pos_vis(loc)
 
     @staticmethod
@@ -111,15 +123,15 @@
         """direction is the body X axis, value is equal to the roll angle difference from template"""
         body_roll_error = Quaternion.body_axis_rates(tp.att, fl.att) * PX()
         world_roll_error = fl.att.transform_point(body_roll_error)
 
         return Measurement(
             np.unwrap(abs(world_roll_error) * np.sign(body_roll_error.x)), 
             0, 
-            *Measurement._roll_vis(fl.pos, fl.att)
+            *Measurement._roll_vis(fl, tp)
         )
 
     @staticmethod
     def roll_angle_proj(fl: State, tp: State, proj: Point) -> Self:
         """Direction is the body X axis, value is equal to the roll angle error.
         roll angle error is the angle between the body proj vector axis and the 
         reference frame proj vector. 
@@ -136,15 +148,15 @@
 
         flturns = np.sum(Point.scalar_projection(fl.rvel, fl.vel) * fl.dt) / (2*np.pi)
         tpturns = np.sum(Point.scalar_projection(tp.rvel, tp.vel) * tp.dt) / (2*np.pi)
 
         return Measurement(
             int(flturns - tpturns) * 2 * np.pi + fl_roll_angle - tp_roll_angle,
             0, 
-            *Measurement._roll_vis(fl.pos, fl.att)
+            *Measurement._roll_vis(fl, tp)
         )
 
     @staticmethod
     def roll_angle_y(fl: State, tp: State) -> Self:
         return Measurement.roll_angle_proj(fl, tp, PY())
 
     @staticmethod
@@ -164,22 +176,29 @@
             *Measurement._vector_vis(ref_frame.q.transform_point(distance), fl.pos)
         )
             
     @staticmethod
     def roll_rate(fl: State, tp: State) -> Measurement:
         """vector in the body X axis, length is equal to the roll rate"""
         wrvel = fl.att.transform_point(fl.p * PX())
-        return Measurement(abs(wrvel) * np.sign(fl.p), np.mean(tp.p), *Measurement._roll_vis(fl.pos, fl.att))
+        return Measurement(
+            abs(wrvel) * np.sign(fl.p), 
+            np.mean(tp.p), 
+            *Measurement._roll_vis(fl, tp)
+        )
     
     @staticmethod
     def nose_drop(fl: State, tp: State) -> Measurement:
         """Check the change in body pitch angle between the start and end of the element"""
         flpit = Quaternion.body_axis_rates(fl.att[0], fl.att[-1]).y
-                
-        return Measurement(flpit, np.array([0]), *Measurement._roll_vis(fl.pos[-1], fl.att[-1]))
+        return Measurement(
+            flpit, 
+            np.array([0]), 
+            *Measurement._roll_vis(fl[-1], tp[-1])
+        )
     
     @staticmethod
     def track_proj(fl: State, tp: State, proj: Point, fix='ang'):
         """
         Direction is the world frame scalar rejection of the velocity difference onto the template velocity 
         vector.
         proj defines the axis in the ref_frame (tp[0].transform) to work on.
@@ -188,15 +207,18 @@
         """
         ref_frame = tp[0].transform
         tr = ref_frame.q.inverse()
 
         fwvel = fl.att.transform_point(fl.vel)
         twvel = tp.att.transform_point(tp.vel)
 
-        direction, vis = Measurement._vector_vis(Point.vector_rejection(fwvel, twvel).unit(), fl.pos)
+        direction, vis = Measurement._vector_vis(
+            Point.vector_rejection(fwvel, twvel).unit(), 
+            fl.pos
+        )
         
         fcvel = tr.transform_point(fwvel)
         tcvel = tr.transform_point(twvel)
         
         if fix == 'vel':
             verr = Point.vector_projection(fcvel, proj)
             sign = -np.ones_like(verr.x)
```

### Comparing `flightanalysis-0.2.6/flightanalysis/scoring/results.py` & `flightanalysis-0.2.7/flightanalysis/scoring/results.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/flightanalysis.egg-info/PKG-INFO` & `flightanalysis-0.2.7/flightanalysis.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: fastdtw
 Requires-Dist: simplejson
-Requires-Dist: pfc-geometry>=0.2.4
-Requires-Dist: flightdata>=0.2.6
+Requires-Dist: pfc-geometry>=0.2.5
+Requires-Dist: flightdata>=0.2.7
 
 # FlightAnalysis
 
 This package contains tools for analysing recorded flight log data.The main objective is 
 to facilitate automated judging for precision aerobatic competitions.
```

### Comparing `flightanalysis-0.2.6/flightanalysis.egg-info/SOURCES.txt` & `flightanalysis-0.2.7/flightanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/scripts/batch_analyse.py` & `flightanalysis-0.2.7/scripts/batch_analyse.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/scripts/collect_scores.py` & `flightanalysis-0.2.7/scripts/collect_scores.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/setup.cfg` & `flightanalysis-0.2.7/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = flightanalysis
 author = Thomas David
 author_email = thomasdavid0@gmail.com
 description = A package for analysing flight data
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.2.6
+version = 0.2.7
 url = https://github.com/PyFlightCoach/FlightAnalysis
 
 [options]
 include_package_data = True
 package_dir = 
 	flightanalysis = flightanalysis
 	scripts = scripts
@@ -18,14 +18,14 @@
 	scripts/batch_analyse.py
 install_requires = 
 	numpy
 	pandas
 	scipy
 	fastdtw
 	simplejson
-	pfc-geometry>=0.2.4
-	flightdata>=0.2.6
+	pfc-geometry>=0.2.5
+	flightdata>=0.2.7
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `flightanalysis-0.2.6/setup.py` & `flightanalysis-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.6/tests/test_criiteria.py` & `flightanalysis-0.2.7/tests/test_criiteria.py`

 * *Files identical despite different names*

