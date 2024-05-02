# Comparing `tmp/xcoll-0.3.5.tar.gz` & `tmp/xcoll-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcoll-0.3.5.tar", max compression
+gzip compressed data, was "xcoll-0.3.6.tar", max compression
```

## Comparing `xcoll-0.3.5.tar` & `xcoll-0.3.6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    11357 2024-03-03 12:36:30.690976 xcoll-0.3.5/LICENSE
--rw-r--r--   0        0        0       74 2024-03-03 12:36:30.690976 xcoll-0.3.5/NOTICE
--rw-r--r--   0        0        0     1713 2024-03-03 12:36:30.690976 xcoll-0.3.5/README.md
--rw-r--r--   0        0        0      996 2024-04-04 13:58:03.585707 xcoll-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      642 2024-04-04 13:56:34.025164 xcoll-0.3.5/xcoll/__init__.py
--rw-r--r--   0        0        0      776 2024-04-04 13:56:34.025164 xcoll-0.3.5/xcoll/beam_elements/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-04 13:56:34.025164 xcoll-0.3.5/xcoll/beam_elements/absorber.py
--rw-r--r--   0        0        0    15785 2024-04-04 13:58:03.586707 xcoll-0.3.5/xcoll/beam_elements/base.py
--rw-r--r--   0        0        0     5502 2024-04-04 13:56:34.025164 xcoll-0.3.5/xcoll/beam_elements/collimators_src/absorber.h
--rw-r--r--   0        0        0     5596 2024-03-21 14:40:13.321383 xcoll-0.3.5/xcoll/beam_elements/collimators_src/everest_block.h
--rw-r--r--   0        0        0     6296 2024-04-04 13:56:34.025164 xcoll-0.3.5/xcoll/beam_elements/collimators_src/everest_collimator.h
--rw-r--r--   0        0        0     5164 2024-04-04 13:56:34.026164 xcoll-0.3.5/xcoll/beam_elements/collimators_src/everest_crystal.h
--rw-r--r--   0        0        0    11369 2024-04-04 13:56:34.026164 xcoll-0.3.5/xcoll/beam_elements/everest.py
--rw-r--r--   0        0        0    49476 2024-04-04 13:58:03.586707 xcoll-0.3.5/xcoll/colldb.py
--rw-r--r--   0        0        0    17015 2024-04-04 13:56:34.026164 xcoll-0.3.5/xcoll/collimator_settings.py
--rw-r--r--   0        0        0      525 2024-04-04 13:58:03.587707 xcoll-0.3.5/xcoll/general.py
--rw-r--r--   0        0        0     1586 2024-04-04 13:56:34.027164 xcoll-0.3.5/xcoll/headers/checks.h
--rw-r--r--   0        0        0      844 2024-03-21 14:40:13.322383 xcoll-0.3.5/xcoll/headers/particle_states.h
--rw-r--r--   0        0        0       39 2024-03-05 09:07:52.886116 xcoll-0.3.5/xcoll/impacts/__init__.py
--rw-r--r--   0        0        0     3953 2024-04-04 13:56:34.027164 xcoll-0.3.5/xcoll/impacts/impacts.py
--rw-r--r--   0        0        0     5950 2024-04-04 13:56:34.027164 xcoll-0.3.5/xcoll/impacts/impacts_src/impacts.h
--rw-r--r--   0        0        0     2493 2024-03-03 12:36:55.658772 xcoll-0.3.5/xcoll/impacts/interaction_types.py
--rw-r--r--   0        0        0    45052 2024-04-04 13:58:03.587707 xcoll-0.3.5/xcoll/manager.py
--rw-r--r--   0        0        0     8936 2024-04-04 13:58:03.587707 xcoll-0.3.5/xcoll/rf_sweep.py
--rw-r--r--   0        0        0      286 2024-04-04 13:56:34.028164 xcoll-0.3.5/xcoll/scattering_routines/everest/__init__.py
--rw-r--r--   0        0        0     1390 2024-03-03 12:36:55.662773 xcoll-0.3.5/xcoll/scattering_routines/everest/constants.h
--rw-r--r--   0        0        0    54119 2024-04-04 13:56:34.028164 xcoll-0.3.5/xcoll/scattering_routines/everest/crystal.h
--rw-r--r--   0        0        0     3743 2024-03-21 14:52:35.463362 xcoll-0.3.5/xcoll/scattering_routines/everest/everest.h
--rw-r--r--   0        0        0     1306 2024-04-04 13:56:34.028164 xcoll-0.3.5/xcoll/scattering_routines/everest/everest.py
--rw-r--r--   0        0        0     7308 2024-03-21 14:54:10.742593 xcoll-0.3.5/xcoll/scattering_routines/everest/jaw.h
--rw-r--r--   0        0        0     9410 2024-03-21 14:55:02.260178 xcoll-0.3.5/xcoll/scattering_routines/everest/materials.py
--rw-r--r--   0        0        0     4518 2024-03-21 14:40:13.323383 xcoll-0.3.5/xcoll/scattering_routines/everest/multiple_coulomb_scattering.h
--rw-r--r--   0        0        0     6585 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/everest/properties.h
--rw-r--r--   0        0        0     6333 2024-03-21 14:55:26.497982 xcoll-0.3.5/xcoll/scattering_routines/everest/scatter.h
--rw-r--r--   0        0        0     9455 2024-04-04 13:56:34.028164 xcoll-0.3.5/xcoll/scattering_routines/everest/scatter_crystal.h
--rw-r--r--   0        0        0     2270 2024-03-04 18:43:20.880294 xcoll-0.3.5/xcoll/scattering_routines/fluka/build_fluka_input.py
--rw-r--r--   0        0        0       73 2024-03-02 17:23:41.394367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/.git
--rw-r--r--   0        0        0       12 2024-03-02 17:23:41.402367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/.gitignore
--rw-r--r--   0        0        0      591 2024-03-02 17:23:41.402367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt
--rw-r--r--   0        0        0     5951 2024-03-02 17:23:41.402367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile
--rw-r--r--   0        0        0     3404 2024-03-02 17:23:41.402367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/Makefile
--rw-r--r--   0        0        0      611 2024-03-02 17:23:41.402367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/README
--rw-r--r--   0        0        0    65455 2024-03-02 17:23:41.403367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile
--rw-r--r--   0        0        0    45517 2024-03-02 17:23:41.403367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc
--rw-r--r--   0        0        0   138089 2024-03-02 17:23:41.403367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub
--rw-r--r--   0        0        0    74567 2024-03-02 17:23:41.403367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html
--rw-r--r--   0        0        0   233955 2024-03-02 17:23:41.404367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf
--rw-r--r--   0        0        0    36021 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png
--rw-r--r--   0        0        0     2904 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png
--rw-r--r--   0        0        0    23826 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png
--rw-r--r--   0        0        0     3956 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png
--rw-r--r--   0        0        0     7017 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png
--rw-r--r--   0        0        0    33614 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png
--rw-r--r--   0        0        0    51182 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png
--rw-r--r--   0        0        0      146 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/Makefile
--rw-r--r--   0        0        0    74068 2024-03-02 17:23:41.405367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl
--rw-r--r--   0        0        0     2793 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/Connection.h
--rw-r--r--   0        0        0     1976 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h
--rw-r--r--   0        0        0      757 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h
--rw-r--r--   0        0        0     5954 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h
--rw-r--r--   0        0        0     1731 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/Message.h
--rw-r--r--   0        0        0     1328 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h
--rw-r--r--   0        0        0    82884 2024-03-02 17:23:41.756364 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a
--rwxr-xr-x   0        0        0    66688 2024-03-02 17:23:41.780364 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so
--rw-r--r--   0        0        0     2907 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c
--rw-r--r--   0        0        0     2330 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c
--rw-r--r--   0        0        0     3629 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f
--rw-r--r--   0        0        0     2995 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f
--rw-r--r--   0        0        0     5769 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/Connection.c
--rw-r--r--   0        0        0     5882 2024-03-02 17:23:41.434367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/Connection.d
--rw-r--r--   0        0        0    13008 2024-03-02 17:23:41.473366 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/Connection.o
--rw-r--r--   0        0        0     4804 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c
--rw-r--r--   0        0        0     3829 2024-03-02 17:23:41.487366 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d
--rw-r--r--   0        0        0    12440 2024-03-02 17:23:41.517366 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o
--rw-r--r--   0        0        0     1541 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c
--rw-r--r--   0        0        0     2445 2024-03-02 17:23:41.529366 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d
--rw-r--r--   0        0        0      288 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.h
--rw-r--r--   0        0        0     7664 2024-03-02 17:23:41.549366 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o
--rw-r--r--   0        0        0     1925 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c
--rw-r--r--   0        0        0     5905 2024-03-02 17:23:41.566365 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d
--rw-r--r--   0        0        0     7536 2024-03-02 17:23:41.597365 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o
--rw-r--r--   0        0        0      396 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer_private.h
--rw-r--r--   0        0        0      421 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO_private.h
--rw-r--r--   0        0        0    11512 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c
--rw-r--r--   0        0        0     3240 2024-03-02 17:23:41.610365 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d
--rw-r--r--   0        0        0    23400 2024-03-02 17:23:41.654365 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o
--rw-r--r--   0        0        0     6361 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c
--rw-r--r--   0        0        0     5716 2024-03-02 17:23:41.671365 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d
--rw-r--r--   0        0        0      902 2024-03-03 12:36:55.663772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h
--rw-r--r--   0        0        0    16816 2024-03-02 17:23:41.710364 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o
--rw-r--r--   0        0        0    14484 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/tags
--rw-r--r--   0        0        0      166 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/AllTests.cpp
--rw-r--r--   0        0        0      152 2024-03-03 12:36:55.664772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/CommonTest.h
--rw-r--r--   0        0        0     2464 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp
--rw-r--r--   0        0        0     1851 2024-03-02 17:23:41.406367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp
--rw-r--r--   0        0        0    11293 2024-03-02 17:23:41.407367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp
--rw-r--r--   0        0        0    14331 2024-03-02 17:23:41.407367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp
--rw-r--r--   0        0        0      526 2024-03-02 17:23:41.407367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c
--rw-r--r--   0        0        0      226 2024-03-03 12:36:55.664772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.h
--rw-r--r--   0        0        0     2244 2024-03-02 17:23:41.407367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c
--rw-r--r--   0        0        0     1660 2024-03-03 12:36:55.664772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h
--rw-r--r--   0        0        0      549 2024-03-02 17:23:41.407367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c
--rw-r--r--   0        0        0      395 2024-03-03 12:36:55.664772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.h
--rw-r--r--   0        0        0      360 2024-03-02 17:23:41.407367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.c
--rw-r--r--   0        0        0      280 2024-03-03 12:36:55.664772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.h
--rw-r--r--   0        0        0      330 2024-03-03 12:36:55.664772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFortranFlukaIO.h
--rw-r--r--   0        0        0     1452 2024-03-02 17:23:41.407367 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c
--rw-r--r--   0        0        0      906 2024-03-03 12:36:55.664772 xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h
--rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 xcoll-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-03 12:36:30.690976 xcoll-0.3.6/LICENSE
+-rw-r--r--   0        0        0       74 2024-03-03 12:36:30.690976 xcoll-0.3.6/NOTICE
+-rw-r--r--   0        0        0     1713 2024-03-03 12:36:30.690976 xcoll-0.3.6/README.md
+-rw-r--r--   0        0        0      996 2024-05-02 14:27:33.660461 xcoll-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      642 2024-05-02 14:14:15.108567 xcoll-0.3.6/xcoll/__init__.py
+-rw-r--r--   0        0        0      776 2024-05-02 14:14:15.108567 xcoll-0.3.6/xcoll/beam_elements/__init__.py
+-rw-r--r--   0        0        0     1260 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/absorber.py
+-rw-r--r--   0        0        0    15785 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/base.py
+-rw-r--r--   0        0        0     5502 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/absorber.h
+-rw-r--r--   0        0        0     5596 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_block.h
+-rw-r--r--   0        0        0     6296 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_collimator.h
+-rw-r--r--   0        0        0     5164 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_crystal.h
+-rw-r--r--   0        0        0    11369 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/everest.py
+-rw-r--r--   0        0        0    49476 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/colldb.py
+-rw-r--r--   0        0        0    17015 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/collimator_settings.py
+-rw-r--r--   0        0        0      525 2024-05-02 14:27:33.660461 xcoll-0.3.6/xcoll/general.py
+-rw-r--r--   0        0        0     1586 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/headers/checks.h
+-rw-r--r--   0        0        0      844 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/headers/particle_states.h
+-rw-r--r--   0        0        0       39 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/__init__.py
+-rw-r--r--   0        0        0     3953 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/impacts.py
+-rw-r--r--   0        0        0     5950 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/impacts_src/impacts.h
+-rw-r--r--   0        0        0     2493 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/interaction_types.py
+-rw-r--r--   0        0        0    45052 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/manager.py
+-rw-r--r--   0        0        0     8936 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/rf_sweep.py
+-rw-r--r--   0        0        0      286 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/scattering_routines/everest/__init__.py
+-rw-r--r--   0        0        0     1390 2024-04-29 13:36:30.200438 xcoll-0.3.6/xcoll/scattering_routines/everest/constants.h
+-rw-r--r--   0        0        0    54119 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/crystal.h
+-rw-r--r--   0        0        0     3743 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/everest.h
+-rw-r--r--   0        0        0     1306 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/everest.py
+-rw-r--r--   0        0        0     7308 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/everest/jaw.h
+-rw-r--r--   0        0        0     9410 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/scattering_routines/everest/materials.py
+-rw-r--r--   0        0        0     4518 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/everest/multiple_coulomb_scattering.h
+-rw-r--r--   0        0        0     6585 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/everest/properties.h
+-rw-r--r--   0        0        0     6333 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/scatter.h
+-rw-r--r--   0        0        0     9455 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/scatter_crystal.h
+-rw-r--r--   0        0        0     2270 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/scattering_routines/fluka/build_fluka_input.py
+-rw-r--r--   0        0        0       73 2024-03-02 17:23:41.394367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/.git
+-rw-r--r--   0        0        0       12 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/.gitignore
+-rw-r--r--   0        0        0      591 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt
+-rw-r--r--   0        0        0     5951 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile
+-rw-r--r--   0        0        0     3404 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/Makefile
+-rw-r--r--   0        0        0      611 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/README
+-rw-r--r--   0        0        0    65455 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile
+-rw-r--r--   0        0        0    45517 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc
+-rw-r--r--   0        0        0   138089 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub
+-rw-r--r--   0        0        0    74567 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html
+-rw-r--r--   0        0        0   233955 2024-03-02 17:23:41.404367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf
+-rw-r--r--   0        0        0    36021 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png
+-rw-r--r--   0        0        0     2904 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png
+-rw-r--r--   0        0        0    23826 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png
+-rw-r--r--   0        0        0     3956 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png
+-rw-r--r--   0        0        0     7017 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png
+-rw-r--r--   0        0        0    33614 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png
+-rw-r--r--   0        0        0    51182 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png
+-rw-r--r--   0        0        0      146 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/Makefile
+-rw-r--r--   0        0        0    74068 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl
+-rw-r--r--   0        0        0     2793 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Connection.h
+-rw-r--r--   0        0        0     1976 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h
+-rw-r--r--   0        0        0      757 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h
+-rw-r--r--   0        0        0     5954 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h
+-rw-r--r--   0        0        0     1731 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Message.h
+-rw-r--r--   0        0        0     1328 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h
+-rw-r--r--   0        0        0    82884 2024-03-02 17:23:41.756364 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a
+-rwxr-xr-x   0        0        0    66688 2024-03-02 17:23:41.780364 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so
+-rw-r--r--   0        0        0     2907 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c
+-rw-r--r--   0        0        0     2330 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c
+-rw-r--r--   0        0        0     3629 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f
+-rw-r--r--   0        0        0     2995 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f
+-rw-r--r--   0        0        0     5769 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.c
+-rw-r--r--   0        0        0     5882 2024-03-02 17:23:41.434367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.d
+-rw-r--r--   0        0        0    13008 2024-03-02 17:23:41.473366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.o
+-rw-r--r--   0        0        0     4804 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c
+-rw-r--r--   0        0        0     3829 2024-03-02 17:23:41.487366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d
+-rw-r--r--   0        0        0    12440 2024-03-02 17:23:41.517366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o
+-rw-r--r--   0        0        0     1541 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c
+-rw-r--r--   0        0        0     2445 2024-03-02 17:23:41.529366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d
+-rw-r--r--   0        0        0      288 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.h
+-rw-r--r--   0        0        0     7664 2024-03-02 17:23:41.549366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o
+-rw-r--r--   0        0        0     1925 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c
+-rw-r--r--   0        0        0     5905 2024-03-02 17:23:41.566365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d
+-rw-r--r--   0        0        0     7536 2024-03-02 17:23:41.597365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o
+-rw-r--r--   0        0        0      396 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer_private.h
+-rw-r--r--   0        0        0      421 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO_private.h
+-rw-r--r--   0        0        0    11512 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c
+-rw-r--r--   0        0        0     3240 2024-03-02 17:23:41.610365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d
+-rw-r--r--   0        0        0    23400 2024-03-02 17:23:41.654365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o
+-rw-r--r--   0        0        0     6361 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c
+-rw-r--r--   0        0        0     5716 2024-03-02 17:23:41.671365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d
+-rw-r--r--   0        0        0      902 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h
+-rw-r--r--   0        0        0    16816 2024-03-02 17:23:41.710364 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o
+-rw-r--r--   0        0        0    14484 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/tags
+-rw-r--r--   0        0        0      166 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/AllTests.cpp
+-rw-r--r--   0        0        0      152 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/CommonTest.h
+-rw-r--r--   0        0        0     2464 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp
+-rw-r--r--   0        0        0     1851 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp
+-rw-r--r--   0        0        0    11293 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp
+-rw-r--r--   0        0        0    14331 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp
+-rw-r--r--   0        0        0      526 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c
+-rw-r--r--   0        0        0      226 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.h
+-rw-r--r--   0        0        0     2244 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c
+-rw-r--r--   0        0        0     1660 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h
+-rw-r--r--   0        0        0      549 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c
+-rw-r--r--   0        0        0      395 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.h
+-rw-r--r--   0        0        0      360 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.c
+-rw-r--r--   0        0        0      280 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.h
+-rw-r--r--   0        0        0      330 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFortranFlukaIO.h
+-rw-r--r--   0        0        0     1452 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c
+-rw-r--r--   0        0        0      906 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 xcoll-0.3.6/PKG-INFO
```

### Comparing `xcoll-0.3.5/LICENSE` & `xcoll-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/README.md` & `xcoll-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/pyproject.toml` & `xcoll-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcoll"
-version = "0.3.5"
+version = "0.3.6"
 description = "Xsuite collimation package"
 homepage = "https://github.com/xsuite/xcoll"
 repository = "https://github.com/xsuite/xcoll"
 authors = [
            "Frederik F. Van der Veken <frederik@cern.ch>",
            "Despina Demetriadou <despina.demetriadou@cern.ch>",
            "Andrey Abramov <andrey.abramov@cern.ch>",
```

### Comparing `xcoll-0.3.5/xcoll/__init__.py` & `xcoll-0.3.6/xcoll/__init__.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/__init__.py` & `xcoll-0.3.6/xcoll/beam_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/absorber.py` & `xcoll-0.3.6/xcoll/beam_elements/absorber.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/base.py` & `xcoll-0.3.6/xcoll/beam_elements/base.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/collimators_src/absorber.h` & `xcoll-0.3.6/xcoll/beam_elements/collimators_src/absorber.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/collimators_src/everest_block.h` & `xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_block.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/collimators_src/everest_collimator.h` & `xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_collimator.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/collimators_src/everest_crystal.h` & `xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/beam_elements/everest.py` & `xcoll-0.3.6/xcoll/beam_elements/everest.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/colldb.py` & `xcoll-0.3.6/xcoll/colldb.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/collimator_settings.py` & `xcoll-0.3.6/xcoll/collimator_settings.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/general.py` & `xcoll-0.3.6/xcoll/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 _pkg_root = Path(__file__).parent.absolute()
 
 citation = "F.F. Van der Veken, et al.: Recent Developments with the New Tools for Collimation Simulations in Xsuite, Proceedings of HB2023, Geneva, Switzerland."
 
 # ===================
 # Do not change
 # ===================
-__version__ = '0.3.5'
+__version__ = '0.3.6'
 # ===================
```

### Comparing `xcoll-0.3.5/xcoll/headers/checks.h` & `xcoll-0.3.6/xcoll/headers/checks.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/headers/particle_states.h` & `xcoll-0.3.6/xcoll/headers/particle_states.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/impacts/impacts.py` & `xcoll-0.3.6/xcoll/impacts/impacts.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/impacts/impacts_src/impacts.h` & `xcoll-0.3.6/xcoll/impacts/impacts_src/impacts.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/impacts/interaction_types.py` & `xcoll-0.3.6/xcoll/impacts/interaction_types.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/manager.py` & `xcoll-0.3.6/xcoll/manager.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/rf_sweep.py` & `xcoll-0.3.6/xcoll/rf_sweep.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/constants.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/constants.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/crystal.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/everest.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/everest.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/everest.py` & `xcoll-0.3.6/xcoll/scattering_routines/everest/everest.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/jaw.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/jaw.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/materials.py` & `xcoll-0.3.6/xcoll/scattering_routines/everest/materials.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/multiple_coulomb_scattering.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/multiple_coulomb_scattering.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/properties.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/properties.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/scatter.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/scatter.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/everest/scatter_crystal.h` & `xcoll-0.3.6/xcoll/scattering_routines/everest/scatter_crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/build_fluka_input.py` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/build_fluka_input.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/Makefile` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/Makefile`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/README` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/README`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/Connection.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Connection.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/Message.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Message.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/Connection.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/Connection.d` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/Connection.o` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/src/tags` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/tags`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h` & `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.5/PKG-INFO` & `xcoll-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcoll
-Version: 0.3.5
+Version: 0.3.6
 Summary: Xsuite collimation package
 Home-page: https://github.com/xsuite/xcoll
 License: Apache 2.0
 Author: Frederik F. Van der Veken
 Author-email: frederik@cern.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
```

