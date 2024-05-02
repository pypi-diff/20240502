# Comparing `tmp/collective.tiles.carousel-1.0.3.tar.gz` & `tmp/collective_tiles_carousel-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.tiles.carousel-1.0.3.tar", last modified: Fri Nov  3 08:32:59 2023, max compression
+gzip compressed data, was "collective_tiles_carousel-1.0.4.tar", last modified: Thu May  2 14:15:03 2024, max compression
```

## Comparing `collective.tiles.carousel-1.0.3.tar` & `collective_tiles_carousel-1.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.516007 collective.tiles.carousel-1.0.3/
--rw-r--r--   0 peterm     (501) staff       (20)      488 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/CHANGES.rst
--rw-r--r--   0 peterm     (501) staff       (20)      110 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/CONTRIBUTORS.rst
--rw-r--r--   0 peterm     (501) staff       (20)      521 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/DEVELOP.rst
--rw-r--r--   0 peterm     (501) staff       (20)    18092 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)      668 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/LICENSE.rst
--rw-r--r--   0 peterm     (501) staff       (20)     3148 2023-11-03 08:32:59.515885 collective.tiles.carousel-1.0.3/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     1331 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/README.rst
--rw-r--r--   0 peterm     (501) staff       (20)       58 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/constraints.txt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.511439 collective.tiles.carousel-1.0.3/docs/
--rw-r--r--   0 peterm     (501) staff       (20)     7981 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/docs/conf.py
--rw-r--r--   0 peterm     (501) staff       (20)      112 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/docs/index.rst
--rw-r--r--   0 peterm     (501) staff       (20)      123 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/requirements.txt
--rw-r--r--   0 peterm     (501) staff       (20)       38 2023-11-03 08:32:59.516044 collective.tiles.carousel-1.0.3/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     2793 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/setup.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.509304 collective.tiles.carousel-1.0.3/src/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.511542 collective.tiles.carousel-1.0.3/src/collective/
--rw-r--r--   0 peterm     (501) staff       (20)       56 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.512557 collective.tiles.carousel-1.0.3/src/collective/tiles/
--rw-r--r--   0 peterm     (501) staff       (20)       56 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.513442 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/
--rw-r--r--   0 peterm     (501) staff       (20)      118 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     1783 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)      249 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/interfaces.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.513953 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/
--rw-r--r--   0 peterm     (501) staff       (20)      611 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/README.rst
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/collective.tiles.carousel.pot
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.509616 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/en/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.514184 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/en/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)       28 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/en/LC_MESSAGES/collective.tiles.carousel.mo
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/en/LC_MESSAGES/collective.tiles.carousel.po
--rw-r--r--   0 peterm     (501) staff       (20)     1726 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/update.py
--rwxr-xr-x   0 peterm     (501) staff       (20)      512 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/update.sh
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.509857 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.514385 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)      193 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/default/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      185 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/default/metadata.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.514503 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/default/registry/
--rw-r--r--   0 peterm     (501) staff       (20)     2282 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/default/registry/mosaic.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.514611 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      128 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      586 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/setuphandlers.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.515242 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)      871 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)       91 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/slide_full_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)      230 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/slide_full_view.py
--rw-r--r--   0 peterm     (501) staff       (20)      540 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/slide_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)     3132 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/slide_view.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.515349 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/static/
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/static/.gitkeep
--rw-r--r--   0 peterm     (501) staff       (20)     1685 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/testing.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.515622 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.515731 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/robot/
--rw-r--r--   0 peterm     (501) staff       (20)     2032 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/robot/test_example.robot
--rw-r--r--   0 peterm     (501) staff       (20)      947 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/test_robot.py
--rw-r--r--   0 peterm     (501) staff       (20)     2220 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/test_setup.py
--rw-r--r--   0 peterm     (501) staff       (20)     4737 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tile.pt
--rw-r--r--   0 peterm     (501) staff       (20)    13295 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tile.py
--rw-r--r--   0 peterm     (501) staff       (20)     1176 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/utils.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-11-03 08:32:59.512441 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)     3148 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     2234 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)      130 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       28 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)      364 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)       11 2023-11-03 08:32:59.000000 collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/top_level.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.435635 collective_tiles_carousel-1.0.4/
+-rw-r--r--   0 peterm     (501) staff       (20)      589 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/CHANGES.rst
+-rw-r--r--   0 peterm     (501) staff       (20)      110 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/CONTRIBUTORS.rst
+-rw-r--r--   0 peterm     (501) staff       (20)      521 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/DEVELOP.rst
+-rw-r--r--   0 peterm     (501) staff       (20)    18092 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      668 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/LICENSE.rst
+-rw-r--r--   0 peterm     (501) staff       (20)     4022 2024-05-02 14:15:03.435398 collective_tiles_carousel-1.0.4/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     1331 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/README.rst
+-rw-r--r--   0 peterm     (501) staff       (20)       58 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/constraints.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.429928 collective_tiles_carousel-1.0.4/docs/
+-rw-r--r--   0 peterm     (501) staff       (20)     7981 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/docs/conf.py
+-rw-r--r--   0 peterm     (501) staff       (20)      112 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/docs/index.rst
+-rw-r--r--   0 peterm     (501) staff       (20)      123 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/requirements.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       38 2024-05-02 14:15:03.435674 collective_tiles_carousel-1.0.4/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     2793 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.427495 collective_tiles_carousel-1.0.4/src/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.430048 collective_tiles_carousel-1.0.4/src/collective/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.431131 collective_tiles_carousel-1.0.4/src/collective/tiles/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.432134 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/
+-rw-r--r--   0 peterm     (501) staff       (20)      119 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1783 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      249 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/interfaces.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.432683 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/
+-rw-r--r--   0 peterm     (501) staff       (20)      611 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/README.rst
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/collective.tiles.carousel.pot
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.427850 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/en/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.432936 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/en/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)       28 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/en/LC_MESSAGES/collective.tiles.carousel.mo
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/en/LC_MESSAGES/collective.tiles.carousel.po
+-rw-r--r--   0 peterm     (501) staff       (20)     1726 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/update.py
+-rwxr-xr-x   0 peterm     (501) staff       (20)      512 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/update.sh
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.428148 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.433166 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      193 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/default/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      185 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/default/metadata.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.433293 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/default/registry/
+-rw-r--r--   0 peterm     (501) staff       (20)     2282 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/default/registry/mosaic.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.433426 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      128 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      586 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/setuphandlers.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.434132 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      871 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)       91 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/slide_full_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      230 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/slide_full_view.py
+-rw-r--r--   0 peterm     (501) staff       (20)      540 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/slide_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     3132 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/slide_view.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.434249 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/static/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/static/.gitkeep
+-rw-r--r--   0 peterm     (501) staff       (20)     1685 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/testing.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.434565 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.434680 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/robot/
+-rw-r--r--   0 peterm     (501) staff       (20)     2032 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/robot/test_example.robot
+-rw-r--r--   0 peterm     (501) staff       (20)      947 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/test_robot.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2221 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4737 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tile.pt
+-rw-r--r--   0 peterm     (501) staff       (20)    12230 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tile.py
+-rw-r--r--   0 peterm     (501) staff       (20)      550 2024-05-02 14:15:02.000000 collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/utils.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2024-05-02 14:15:03.434859 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)     4022 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     2234 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      130 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       28 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      364 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2024-05-02 14:15:03.000000 collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/top_level.txt
```

### Comparing `collective.tiles.carousel-1.0.3/DEVELOP.rst` & `collective_tiles_carousel-1.0.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/LICENSE.GPL` & `collective_tiles_carousel-1.0.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/LICENSE.rst` & `collective_tiles_carousel-1.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/README.rst` & `collective_tiles_carousel-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/docs/conf.py` & `collective_tiles_carousel-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/setup.py` & `collective_tiles_carousel-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.tiles.carousel",
-    version="1.0.3",
+    version="1.0.4",
     description="Slider for plone.app.mosaic based on Bootstrap 5",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/configure.zcml` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/README.rst` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/update.py` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/locales/update.sh` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/profiles/default/registry/mosaic.xml` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/profiles/default/registry/mosaic.xml`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/setuphandlers.py` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/configure.zcml` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/slide_view.pt` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/slide_view.pt`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/slides/slide_view.py` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/slides/slide_view.py`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/testing.py` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/testing.py`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/robot/test_example.robot` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/test_robot.py` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tests/test_setup.py` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tests/test_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Setup tests for this package."""
+
 from collective.tiles.carousel.testing import (
     COLLECTIVE_TILES_CAROUSEL_INTEGRATION_TESTING,
 )
 from plone import api
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.base.utils import get_installer
```

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tile.pt` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tile.pt`

 * *Files identical despite different names*

### Comparing `collective.tiles.carousel-1.0.3/src/collective/tiles/carousel/tile.py` & `collective_tiles_carousel-1.0.4/src/collective/tiles/carousel/tile.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 from collective.tiles.carousel.interfaces import ICollectiveTilesCarouselLayer
 from collective.tiles.carousel.utils import parse_query_from_data
 from operator import itemgetter
 from plone import api
 from plone.app.contenttypes.browser.link_redirect_view import NON_RESOLVABLE_URL_SCHEMES
 from plone.app.contenttypes.interfaces import ICollection
 from plone.app.contenttypes.utils import replace_link_variables_by_paths
-from plone.app.querystring import queryparser
-from plone.app.querystring.interfaces import IParsedQueryIndexModifier
 from plone.app.z3cform.widgets.querystring import QueryStringFieldWidget
 from plone.app.z3cform.widgets.relateditems import RelatedItemsFieldWidget
 from plone.autoform import directives as form
 from plone.dexterity.interfaces import IDexterityContainer
 from plone.memoize import view
 from plone.registry.interfaces import IRegistry
 from plone.supermodel.model import Schema
 from plone.tiles import Tile
 from plone.tiles.interfaces import IPersistentTile
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope import schema
 from zope.component import getMultiAdapter
-from zope.component import getUtilitiesFor
 from zope.component import getUtility
 from zope.interface import alsoProvides
 from zope.interface import implementer
 from zope.interface import provider
 from zope.schema.interfaces import IContextSourceBinder
 from zope.schema.interfaces import IVocabularyFactory
 from zope.schema.vocabulary import SimpleTerm
@@ -244,45 +241,18 @@
             name="plone.allowed_sizes",
         )
         for allowed_size in allowed_sizes:
             name = allowed_size.split()[0]
             values.append(name)
         return values
 
-    def parse_query_from_data(data, context=None):
-        """Parse query from data dictionary"""
-        if context is None:
-            context = api.portal.get()
-        query = data.get("query", {}) or {}
-        try:
-            parsed = queryparser.parseFormquery(context, query)
-        except KeyError:
-            parsed = {}
-
-        index_modifiers = getUtilitiesFor(IParsedQueryIndexModifier)
-        for name, modifier in index_modifiers:
-            if name in parsed:
-                new_name, query = modifier(parsed[name])
-                parsed[name] = query
-                # if a new index name has been returned, we need to replace
-                # the native ones
-                if name != new_name:
-                    del parsed[name]
-                    parsed[new_name] = query
-
-        if data.get("sort_on"):
-            parsed["sort_on"] = data["sort_on"]
-        if data.get("sort_reversed", False):
-            parsed["sort_order"] = "reverse"
-        return parsed
-
     @property
     def items(self):
         items = OrderedDict()
-        if "carousel_items" in self.data:
+        if len(self.data.get("carousel_items") or []):
             for item in self.data["carousel_items"]:
                 if ICollection.providedBy(item.to_object):
                     items.update(
                         OrderedDict.fromkeys(
                             [
                                 x.getObject()
                                 for x in item.to_object.results(
@@ -305,24 +275,27 @@
                             ]
                         )
                     )
                     continue
                 else:
                     items[item.to_object] = None
 
-        if getattr(self, "query", None):
+        query = self.query
+        if query:
             items.update(
-                OrderedDict.fromkeys(
-                    [x.getObject() for x in api.content.find(**self.query)]
-                )
+                OrderedDict.fromkeys([x.getObject() for x in self.catalog(**query)])
             )
+
         result = []
-        for obj in items.keys():
+        limit = self.data.get("limit") or 12
+        for count, obj in enumerate(items.keys(), 1):
             result.append(obj)
-        ips = self.data.get("items_per_slide", 1)
+            if count >= limit:
+                break
+        ips = self.data.get("items_per_slide", 1) or 1
         slides = [
             result[i : i + ips]
             for i in [x * ips for x in range(0, int(len(result) / ips) + int(1))]
         ]
         return [x for x in slides if x]
 
     def item_view(self, item, data):
```

### Comparing `collective.tiles.carousel-1.0.3/src/collective.tiles.carousel.egg-info/SOURCES.txt` & `collective_tiles_carousel-1.0.4/src/collective.tiles.carousel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

