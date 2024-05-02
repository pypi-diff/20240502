# Comparing `tmp/enigmapython-0.1.4.tar.gz` & `tmp/enigmapython-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigmapython-0.1.4.tar", last modified: Thu May  2 08:36:56 2024, max compression
+gzip compressed data, was "enigmapython-0.1.5.tar", last modified: Thu May  2 08:40:32 2024, max compression
```

## Comparing `enigmapython-0.1.4.tar` & `enigmapython-0.1.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:36:56.302993 enigmapython-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-02 08:36:56.302993 enigmapython-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:36:56.298993 enigmapython-0.1.4/enigmapython/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Enigma.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaI.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorway.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaINorwayRotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaIRotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonder.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonderRotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonderRotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaISonderRotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorVI.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorVII.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM3RotorVIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorBeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorGamma.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorI.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorII.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorIV.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorV.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorVI.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorVII.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EnigmaM4RotorVIII.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Etw.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/EtwPassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Observable.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Observer.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Plugboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/PlugboardPassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Reflector.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorNorwayUKW.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorSonderUKW.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWA.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWB.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWBThin.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWC.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/ReflectorUKWCThin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Rotor.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/SwappablePlugboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-02 08:36:52.000000 enigmapython-0.1.4/enigmapython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:36:56.302993 enigmapython-0.1.4/enigmapython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 08:36:56.000000 enigmapython-0.1.4/enigmapython.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:36:56.302993 enigmapython-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 08:36:52.000000 enigmapython-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:40:32.883189 enigmapython-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-02 08:40:32.883189 enigmapython-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:40:32.883189 enigmapython-0.1.5/enigmapython/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Enigma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaINorway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaINorwayRotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaINorwayRotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaINorwayRotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaINorwayRotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaINorwayRotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaIRotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaIRotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaIRotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaIRotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaIRotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaISonder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaISonderRotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaISonderRotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaISonderRotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorVI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorVII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM3RotorVIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorBeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorGamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorIV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorVI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorVII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EnigmaM4RotorVIII.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Etw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/EtwPassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Plugboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/PlugboardPassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Reflector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/ReflectorNorwayUKW.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/ReflectorSonderUKW.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/ReflectorUKWA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/ReflectorUKWB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/ReflectorUKWBThin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/ReflectorUKWC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/ReflectorUKWCThin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Rotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/SwappablePlugboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-02 08:40:26.000000 enigmapython-0.1.5/enigmapython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:40:32.883189 enigmapython-0.1.5/enigmapython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-02 08:40:32.000000 enigmapython-0.1.5/enigmapython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-02 08:40:32.000000 enigmapython-0.1.5/enigmapython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:40:32.000000 enigmapython-0.1.5/enigmapython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 08:40:32.000000 enigmapython-0.1.5/enigmapython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:40:32.883189 enigmapython-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 08:40:26.000000 enigmapython-0.1.5/setup.py
```

### Comparing `enigmapython-0.1.4/PKG-INFO` & `enigmapython-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: enigmapython
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple yet faithful library to emulate different Enigma machines models using Python
 Home-page: https://github.com/denismaggior8/enigma-python
 Author: Denis Maggiorotto
 Description-Content-Type: text/markdown
 
 # Enigma Python library
 
 ![](img/logo.jpg)
 
 ## About
 
-Welcome to **enigma-python**, a Python package designed to emulate the legendary Enigma cryptographic machine used during World War II. enigma-python provides a faithful implementation of the Enigma machine, allowing users to explore and understand the workings of this historic device.
+Welcome to **enigmapython**, a Python package designed to emulate the legendary Enigma cryptographic machine used during World War II. **enigmapython** provides a faithful implementation of the Enigma machine, allowing users to explore and understand the workings of this historic device.
 
 ## Key Features
 
-- **Flexible Configuration**: enigma-python allows customization of the Enigma machine configuration, enabling users to experiment with different rotor settings, reflectors, and ring positions.
-- **Easy Extension**: enigma-python is designed to be easily extensible, allowing developers to add new features or enhance the existing implementation.
-- **Simple yet faithful**: don't be fooled by its simplicity; enigma-python implements 100% the algorithms of many Enigma machine models, allowing to decode a message that has been encoded by a real Enigma machine and also the contrary.
+- **Flexible Configuration**: **enigmapython** allows customization of the Enigma machine configuration, enabling users to experiment with different rotor settings, reflectors, and ring positions.
+- **Easy Extension**: **enigmapython** is designed to be easily extensible, allowing developers to add new features or enhance the existing implementation.
+- **Simple yet faithful**: don't be fooled by its simplicity; **enigmapython** implements 100% the algorithms of many Enigma machine models, allowing to decode a message that has been encoded by a real Enigma machine and also the contrary.
 
 ## Machines implementations
 
 The following Enigma machine models (along with their rotors, reflectors and plugboards) have been implemented:
 
 ### Enigma I
```

### Comparing `enigmapython-0.1.4/enigmapython/Enigma.py` & `enigmapython-0.1.5/enigmapython/Enigma.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.4/enigmapython/Rotor.py` & `enigmapython-0.1.5/enigmapython/Rotor.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.4/enigmapython/SwappablePlugboard.py` & `enigmapython-0.1.5/enigmapython/SwappablePlugboard.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.4/enigmapython/Utils.py` & `enigmapython-0.1.5/enigmapython/Utils.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.4/enigmapython/__init__.py` & `enigmapython-0.1.5/enigmapython/__init__.py`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.4/enigmapython.egg-info/PKG-INFO` & `enigmapython-0.1.5/enigmapython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: enigmapython
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple yet faithful library to emulate different Enigma machines models using Python
 Home-page: https://github.com/denismaggior8/enigma-python
 Author: Denis Maggiorotto
 Description-Content-Type: text/markdown
 
 # Enigma Python library
 
 ![](img/logo.jpg)
 
 ## About
 
-Welcome to **enigma-python**, a Python package designed to emulate the legendary Enigma cryptographic machine used during World War II. enigma-python provides a faithful implementation of the Enigma machine, allowing users to explore and understand the workings of this historic device.
+Welcome to **enigmapython**, a Python package designed to emulate the legendary Enigma cryptographic machine used during World War II. **enigmapython** provides a faithful implementation of the Enigma machine, allowing users to explore and understand the workings of this historic device.
 
 ## Key Features
 
-- **Flexible Configuration**: enigma-python allows customization of the Enigma machine configuration, enabling users to experiment with different rotor settings, reflectors, and ring positions.
-- **Easy Extension**: enigma-python is designed to be easily extensible, allowing developers to add new features or enhance the existing implementation.
-- **Simple yet faithful**: don't be fooled by its simplicity; enigma-python implements 100% the algorithms of many Enigma machine models, allowing to decode a message that has been encoded by a real Enigma machine and also the contrary.
+- **Flexible Configuration**: **enigmapython** allows customization of the Enigma machine configuration, enabling users to experiment with different rotor settings, reflectors, and ring positions.
+- **Easy Extension**: **enigmapython** is designed to be easily extensible, allowing developers to add new features or enhance the existing implementation.
+- **Simple yet faithful**: don't be fooled by its simplicity; **enigmapython** implements 100% the algorithms of many Enigma machine models, allowing to decode a message that has been encoded by a real Enigma machine and also the contrary.
 
 ## Machines implementations
 
 The following Enigma machine models (along with their rotors, reflectors and plugboards) have been implemented:
 
 ### Enigma I
```

### Comparing `enigmapython-0.1.4/enigmapython.egg-info/SOURCES.txt` & `enigmapython-0.1.5/enigmapython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enigmapython-0.1.4/setup.py` & `enigmapython-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     author="Denis Maggiorotto",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/denismaggior8/enigma-python",
     name="enigmapython",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(
         # All keyword arguments below are optional:
         where='.',  # '.' by default
         include=['enigmapython'],  # ['*'] by default
     ),
     description="A simple yet faithful library to emulate different Enigma machines models using Python"
 )
```

