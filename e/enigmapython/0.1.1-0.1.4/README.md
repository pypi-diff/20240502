# Comparing `tmp/enigmapython-0.1.1.tar.gz` & `tmp/enigmapython-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigmapython-0.1.1.tar", last modified: Thu May  2 08:24:21 2024, max compression
+gzip compressed data, was "enigmapython-0.1.4.tar", last modified: Thu May  2 08:36:56 2024, max compression
```

## Comparing `enigmapython-0.1.1.tar` & `enigmapython-0.1.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:24:21.128412 enigmapython-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:24:21.128412 enigmapython-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:24:21.128412 enigmapython-0.1.1/enigmapython/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Enigma.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaI.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaINorway.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaINorwayRotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaINorwayRotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaINorwayRotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaINorwayRotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaINorwayRotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaIRotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaIRotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaIRotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaIRotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaIRotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaISonder.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaISonderRotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaISonderRotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaISonderRotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorVI.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorVII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM3RotorVIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorBeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorGamma.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorVI.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorVII.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EnigmaM4RotorVIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Etw.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/EtwPassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Observable.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Observer.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Plugboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/PlugboardPassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Reflector.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/ReflectorNorwayUKW.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/ReflectorSonderUKW.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/ReflectorUKWA.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/ReflectorUKWB.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/ReflectorUKWBThin.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/ReflectorUKWC.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/ReflectorUKWCThin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Rotor.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/SwappablePlugboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-02 08:24:12.000000 enigmapython-0.1.1/enigmapython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:24:21.128412 enigmapython-0.1.1/enigmapython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:24:21.000000 enigmapython-0.1.1/enigmapython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-02 08:24:21.000000 enigmapython-0.1.1/enigmapython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:24:21.000000 enigmapython-0.1.1/enigmapython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 08:24:21.000000 enigmapython-0.1.1/enigmapython.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:24:21.128412 enigmapython-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 08:24:12.000000 enigmapython-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:36:56.302993 enigmapython-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-02 08:36:56.302993 enigmapython-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:36:56.298993 enigmapython-0.1.4/enigmapython/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Enigma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonderRotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonderRotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonderRotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorVI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorVII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorVIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorBeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorGamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorVI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorVII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorVIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Etw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EtwPassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Plugboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/PlugboardPassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Reflector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorNorwayUKW.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorSonderUKW.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWBThin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWCThin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Rotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/SwappablePlugboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:36:56.302993 enigmapython-0.1.4/enigmapython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:36:56.302993 enigmapython-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 08:36:52.000000 enigmapython-0.1.4/setup.py
```

### Comparing `enigmapython-0.1.1/enigmapython/Enigma.py` & `enigmapython-0.1.4/enigmapython/Enigma.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.1/enigmapython/Rotor.py` & `enigmapython-0.1.4/enigmapython/Rotor.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.1/enigmapython/SwappablePlugboard.py` & `enigmapython-0.1.4/enigmapython/SwappablePlugboard.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.1/enigmapython/Utils.py` & `enigmapython-0.1.4/enigmapython/Utils.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.1/enigmapython/__init__.py` & `enigmapython-0.1.4/enigmapython/__init__.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.1/enigmapython.egg-info/SOURCES.txt` & `enigmapython-0.1.4/enigmapython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

