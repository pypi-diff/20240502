# Comparing `tmp/emmet-api-0.83.0.tar.gz` & `tmp/emmet-api-0.83.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.83.0.tar", last modified: Tue Apr 30 20:52:42 2024, max compression
+gzip compressed data, was "emmet-api-0.83.1.tar", last modified: Thu May  2 21:38:16 2024, max compression
```

## Comparing `emmet-api-0.83.0.tar` & `emmet-api-0.83.1.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.823714 emmet-api-0.83.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-30 20:52:37.000000 emmet-api-0.83.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 20:52:42.823714 emmet-api-0.83.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 20:52:37.000000 emmet-api-0.83.0/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.779714 emmet-api-0.83.0/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.787714 emmet-api-0.83.0/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/_messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_messages/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/_messages/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.791714 emmet-api-0.83.0/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/conversion_electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/conversion_electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/conversion_electrodes/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.795714 emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13458 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.799714 emmet-api-0.83.0/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.803714 emmet-api-0.83.0/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/metal_binding/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/metal_binding/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.807714 emmet-api-0.83.0/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 20:52:37.000000 emmet-api-0.83.0/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 20:52:42.000000 emmet-api-0.83.0/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-30 20:52:42.000000 emmet-api-0.83.0/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:52:42.000000 emmet-api-0.83.0/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:52:42.000000 emmet-api-0.83.0/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-30 20:52:42.000000 emmet-api-0.83.0/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 20:52:42.000000 emmet-api-0.83.0/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13875 2024-04-30 20:52:37.000000 emmet-api-0.83.0/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-30 20:52:37.000000 emmet-api-0.83.0/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-30 20:52:37.000000 emmet-api-0.83.0/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-30 20:52:37.000000 emmet-api-0.83.0/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-30 20:52:37.000000 emmet-api-0.83.0/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-30 20:52:37.000000 emmet-api-0.83.0/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-30 20:52:37.000000 emmet-api-0.83.0/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-30 20:52:37.000000 emmet-api-0.83.0/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-30 20:52:37.000000 emmet-api-0.83.0/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:52:42.823714 emmet-api-0.83.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-30 20:52:37.000000 emmet-api-0.83.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 20:52:37.000000 emmet-api-0.83.0/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.783714 emmet-api-0.83.0/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.787714 emmet-api-0.83.0/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.811714 emmet-api-0.83.0/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.815714 emmet-api-0.83.0/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/metal_binding/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.819714 emmet-api-0.83.0/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.823714 emmet-api-0.83.0/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:42.823714 emmet-api-0.83.0/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-30 20:52:37.000000 emmet-api-0.83.0/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.136979 emmet-api-0.83.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-02 21:38:07.000000 emmet-api-0.83.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-02 21:38:16.136979 emmet-api-0.83.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 21:38:07.000000 emmet-api-0.83.1/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.092979 emmet-api-0.83.1/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.100979 emmet-api-0.83.1/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.100979 emmet-api-0.83.1/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_messages/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/_messages/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.104979 emmet-api-0.83.1/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/conversion_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/conversion_electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/conversion_electrodes/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.108979 emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13458 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.112979 emmet-api-0.83.1/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.116979 emmet-api-0.83.1/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/metal_binding/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/metal_binding/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.120979 emmet-api-0.83.1/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-02 21:38:07.000000 emmet-api-0.83.1/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-02 21:38:15.000000 emmet-api-0.83.1/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-02 21:38:16.000000 emmet-api-0.83.1/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:38:15.000000 emmet-api-0.83.1/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:38:15.000000 emmet-api-0.83.1/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-02 21:38:15.000000 emmet-api-0.83.1/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 21:38:15.000000 emmet-api-0.83.1/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13875 2024-05-02 21:38:07.000000 emmet-api-0.83.1/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-02 21:38:07.000000 emmet-api-0.83.1/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-02 21:38:07.000000 emmet-api-0.83.1/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-02 21:38:07.000000 emmet-api-0.83.1/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-02 21:38:07.000000 emmet-api-0.83.1/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-02 21:38:07.000000 emmet-api-0.83.1/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-02 21:38:07.000000 emmet-api-0.83.1/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-02 21:38:07.000000 emmet-api-0.83.1/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-02 21:38:07.000000 emmet-api-0.83.1/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:38:16.136979 emmet-api-0.83.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 21:38:07.000000 emmet-api-0.83.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-02 21:38:07.000000 emmet-api-0.83.1/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.124979 emmet-api-0.83.1/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.096979 emmet-api-0.83.1/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.100979 emmet-api-0.83.1/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.128979 emmet-api-0.83.1/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.132979 emmet-api-0.83.1/tests/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/metal_binding/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.136979 emmet-api-0.83.1/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.136979 emmet-api-0.83.1/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.136979 emmet-api-0.83.1/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.136979 emmet-api-0.83.1/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.136979 emmet-api-0.83.1/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:16.136979 emmet-api-0.83.1/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-02 21:38:07.000000 emmet-api-0.83.1/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.83.0/Dockerfile` & `emmet-api-0.83.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/app.py` & `emmet-api-0.83.1/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/core/api.py` & `emmet-api-0.83.1/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.83.1/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.83.1/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/core/documentation.py` & `emmet-api-0.83.1/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/core/global_header.py` & `emmet-api-0.83.1/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/core/settings.py` & `emmet-api-0.83.1/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.83.1/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.83.1/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.83.1/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.83.1/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/_messages/query_operator.py` & `emmet-api-0.83.1/emmet/api/routes/_messages/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/_messages/resources.py` & `emmet-api-0.83.1/emmet/api/routes/_messages/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/dois/resources.py` & `emmet-api-0.83.1/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.83.1/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/conversion_electrodes/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/conversion_electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/insertion_electrodes/utils.py` & `emmet-api-0.83.1/emmet/api/routes/materials/insertion_electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.83.1/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.83.1/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.83.1/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.83.1/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.83.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.83.1/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.83.1/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.83.1/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.83.1/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/metal_binding/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/metal_binding/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/metal_binding/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/metal_binding/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/tasks/utils.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/utils.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.83.1/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.83.1/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/material_resources.py` & `emmet-api-0.83.1/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/molecule_resources.py` & `emmet-api-0.83.1/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/requirements/deployment.txt` & `emmet-api-0.83.1/requirements/deployment.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.83.1/requirements/ubuntu-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
-blinker==1.7.0
+blinker==1.8.1
     # via flask
-boto3==1.34.85
+boto3==1.34.95
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.85
+botocore==1.34.95
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -53,41 +53,41 @@
     # via matplotlib
 cryptography==42.0.5
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.1
+ddtrace==2.8.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.1
+emmet-core==0.83.0
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.110.1
+fastapi==0.110.3
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
-gunicorn==21.2.0
+gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 idna==3.7
     # via
     #   anyio
     #   requests
@@ -99,35 +99,35 @@
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 joblib==1.4.0
     # via pymatgen
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.64.1
+maggma==0.66.0
     # via emmet-api (setup.py)
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
 matplotlib==3.8.4
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.3.31
+monty==2024.4.17
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -158,45 +158,45 @@
     # via pymatgen
 pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
-plotly==5.20.0
+plotly==5.21.0
     # via pymatgen
 protobuf==5.26.1
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
-pydash==8.0.0
+pydash==8.0.1
     # via maggma
 pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymongo==4.6.3
+pymongo==4.7.1
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
@@ -208,17 +208,17 @@
     #   pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via pybtex
-pyzmq==26.0.0
+pyzmq==26.0.2
     # via maggma
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
@@ -236,15 +236,15 @@
     # via boto3
 scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
-shapely==2.0.3
+shapely==2.0.4
     # via
     #   emmet-api (setup.py)
     #   pymatgen-analysis-alloys
 six==1.16.0
     # via
     #   ddsketch
     #   ddtrace
```

### Comparing `emmet-api-0.83.0/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.83.1/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via starlette
@@ -18,21 +18,21 @@
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
-blinker==1.7.0
+blinker==1.8.1
     # via flask
-boto3==1.34.85
+boto3==1.34.95
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.85
+botocore==1.34.95
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -55,75 +55,85 @@
     #   mkdocstrings
     #   mongogrant
     #   uvicorn
 colorama==0.4.6
     # via griffe
 contourpy==1.2.1
     # via matplotlib
-coverage[toml]==7.4.4
+coverage[toml]==7.5.0
     # via pytest-cov
 cryptography==42.0.5
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.1
+ddtrace==2.8.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.1
+emmet-core==0.83.0
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.110.1
+fastapi==0.110.3
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.13.4
+filelock==3.14.0
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.2
+griffe==0.44.0
     # via mkdocstrings-python
-gunicorn==21.2.0
+gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
 idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocs-get-deps
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==6.4.0
+    # via
+    #   matplotlib
+    #   spglib
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via
     #   emmet-api (setup.py)
@@ -135,25 +145,25 @@
     # via
     #   boto3
     #   botocore
 joblib==1.4.0
     # via pymatgen
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.64.1
+maggma==0.66.0
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -166,66 +176,70 @@
     #   mkdocstrings
     #   werkzeug
 matplotlib==3.8.4
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.5.3
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==1.0.1
     # via mkdocstrings
 mkdocs-awesome-pages-plugin==2.9.2
     # via emmet-api (setup.py)
+mkdocs-get-deps==0.2.0
+    # via mkdocs
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.3.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.24.3
+mkdocstrings[python]==0.25.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.9.2
+mkdocstrings-python==1.10.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.3.31
+monty==2024.4.17
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via maggma
-mypy==1.9.0
+mypy==1.10.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.4.0
     # via mkdocs-awesome-pages-plugin
-networkx==3.3
+networkx==3.2.1
     # via pymatgen
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
     # via
     #   contourpy
     #   maggma
@@ -253,22 +267,22 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
-    #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
     #   virtualenv
-plotly==5.20.0
+plotly==5.21.0
     # via pymatgen
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pre-commit==3.7.0
     # via emmet-api (setup.py)
 protobuf==5.26.1
     # via ddtrace
 pybtex==0.24.0
     # via
@@ -276,53 +290,53 @@
     #   pymatgen
 pycodestyle==2.11.1
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
-pydash==8.0.0
+pydash==8.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via mkdocs-material
 pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymdown-extensions==10.7.1
+pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
-pymongo==4.6.3
+pymongo==4.7.1
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==5.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.9.0.post0
     # via
@@ -334,24 +348,25 @@
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-pyzmq==26.0.0
+pyzmq==26.0.2
     # via maggma
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
@@ -369,15 +384,15 @@
     # via boto3
 scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
-shapely==2.0.3
+shapely==2.0.4
     # via
     #   emmet-api (setup.py)
     #   pymatgen-analysis-alloys
 six==1.16.0
     # via
     #   ddsketch
     #   ddtrace
@@ -409,54 +424,61 @@
     #   pytest
 tornado==6.4
     # via livereload
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-types-requests==2.31.0.20240406
+types-requests==2.31.0.6
     # via emmet-api (setup.py)
-types-setuptools==69.5.0.20240415
+types-setuptools==69.5.0.20240423
     # via emmet-api (setup.py)
+types-urllib3==1.26.25.14
+    # via types-requests
 typing-extensions==4.11.0
     # via
+    #   aioitertools
     #   anyio
     #   asgiref
+    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
+    #   mkdocstrings
     #   mypy
     #   pydantic
     #   pydantic-core
     #   pydash
+    #   starlette
     #   uvicorn
 tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==2.2.1
+urllib3==1.26.18
     # via
     #   botocore
     #   requests
-    #   types-requests
 uvicorn==0.29.0
     # via maggma
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via pre-commit
 watchdog==4.0.0
     # via mkdocs
 wcmatch==8.5.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==3.0.2
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.18.1
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.0/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.83.1/requirements/ubuntu-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
-blinker==1.7.0
+blinker==1.8.1
     # via flask
-boto3==1.34.85
+boto3==1.34.95
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.85
+botocore==1.34.95
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -53,37 +53,37 @@
     # via matplotlib
 cryptography==42.0.5
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.1
+ddtrace==2.8.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.1
+emmet-core==0.83.0
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-fastapi==0.110.1
+fastapi==0.110.3
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
-gunicorn==21.2.0
+gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 idna==3.7
     # via
     #   anyio
     #   requests
@@ -95,35 +95,35 @@
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 joblib==1.4.0
     # via pymatgen
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.64.1
+maggma==0.66.0
     # via emmet-api (setup.py)
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
 matplotlib==3.8.4
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.3.31
+monty==2024.4.17
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -154,45 +154,45 @@
     # via pymatgen
 pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
-plotly==5.20.0
+plotly==5.21.0
     # via pymatgen
 protobuf==5.26.1
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
-pydash==8.0.0
+pydash==8.0.1
     # via maggma
 pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymongo==4.6.3
+pymongo==4.7.1
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
@@ -204,17 +204,17 @@
     #   pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via pybtex
-pyzmq==26.0.0
+pyzmq==26.0.2
     # via maggma
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
@@ -232,15 +232,15 @@
     # via boto3
 scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
-shapely==2.0.3
+shapely==2.0.4
     # via
     #   emmet-api (setup.py)
     #   pymatgen-analysis-alloys
 six==1.16.0
     # via
     #   ddsketch
     #   ddtrace
```

### Comparing `emmet-api-0.83.0/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.83.1/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
-blinker==1.7.0
+blinker==1.8.1
     # via flask
-boto3==1.34.85
+boto3==1.34.95
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.85
+botocore==1.34.95
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -55,63 +55,63 @@
     #   mkdocstrings
     #   mongogrant
     #   uvicorn
 colorama==0.4.6
     # via griffe
 contourpy==1.2.1
     # via matplotlib
-coverage[toml]==7.4.4
+coverage[toml]==7.5.0
     # via pytest-cov
 cryptography==42.0.5
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.1
+ddtrace==2.8.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.1
+emmet-core==0.83.0
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-fastapi==0.110.1
+fastapi==0.110.3
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.13.4
+filelock==3.14.0
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.2
+griffe==0.44.0
     # via mkdocstrings-python
-gunicorn==21.2.0
+gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
 idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
     # via opentelemetry-api
@@ -130,25 +130,25 @@
     # via
     #   boto3
     #   botocore
 joblib==1.4.0
     # via pymatgen
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.64.1
+maggma==0.66.0
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -161,58 +161,62 @@
     #   mkdocstrings
     #   werkzeug
 matplotlib==3.8.4
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.5.3
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==1.0.1
     # via mkdocstrings
 mkdocs-awesome-pages-plugin==2.9.2
     # via emmet-api (setup.py)
+mkdocs-get-deps==0.2.0
+    # via mkdocs
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.3.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.24.3
+mkdocstrings[python]==0.25.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.9.2
+mkdocstrings-python==1.10.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.3.31
+monty==2024.4.17
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via maggma
-mypy==1.9.0
+mypy==1.10.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.4.0
     # via mkdocs-awesome-pages-plugin
@@ -248,22 +252,22 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
-    #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
     #   virtualenv
-plotly==5.20.0
+plotly==5.21.0
     # via pymatgen
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pre-commit==3.7.0
     # via emmet-api (setup.py)
 protobuf==5.26.1
     # via ddtrace
 pybtex==0.24.0
     # via
@@ -271,53 +275,53 @@
     #   pymatgen
 pycodestyle==2.11.1
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
-pydash==8.0.0
+pydash==8.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via mkdocs-material
 pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymdown-extensions==10.7.1
+pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
-pymongo==4.6.3
+pymongo==4.7.1
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==5.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.9.0.post0
     # via
@@ -329,24 +333,25 @@
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-pyzmq==26.0.0
+pyzmq==26.0.2
     # via maggma
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
@@ -364,15 +369,15 @@
     # via boto3
 scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
-shapely==2.0.3
+shapely==2.0.4
     # via
     #   emmet-api (setup.py)
     #   pymatgen-analysis-alloys
 six==1.16.0
     # via
     #   ddsketch
     #   ddtrace
@@ -401,15 +406,15 @@
     # via livereload
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
 types-requests==2.31.0.20240406
     # via emmet-api (setup.py)
-types-setuptools==69.5.0.20240415
+types-setuptools==69.5.0.20240423
     # via emmet-api (setup.py)
 typing-extensions==4.11.0
     # via
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   mypy
@@ -423,15 +428,15 @@
 urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   types-requests
 uvicorn==0.29.0
     # via maggma
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via pre-commit
 watchdog==4.0.0
     # via mkdocs
 wcmatch==8.5.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==3.0.2
     # via flask
```

### Comparing `emmet-api-0.83.0/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.83.1/requirements/ubuntu-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
-blinker==1.7.0
+blinker==1.8.1
     # via flask
-boto3==1.34.85
+boto3==1.34.95
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.85
+botocore==1.34.95
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -53,41 +53,41 @@
     # via matplotlib
 cryptography==42.0.5
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.1
+ddtrace==2.8.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.1
+emmet-core==0.83.0
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.110.1
+fastapi==0.110.3
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
-gunicorn==21.2.0
+gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 idna==3.7
     # via
     #   anyio
     #   requests
@@ -105,35 +105,35 @@
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 joblib==1.4.0
     # via pymatgen
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.64.1
+maggma==0.66.0
     # via emmet-api (setup.py)
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
 matplotlib==3.8.4
     # via pymatgen
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.3.31
+monty==2024.4.17
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -164,45 +164,45 @@
     # via pymatgen
 pandas==2.2.2
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
-plotly==5.20.0
+plotly==5.21.0
     # via pymatgen
 protobuf==5.26.1
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
-pydash==8.0.0
+pydash==8.0.1
     # via maggma
 pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymongo==4.6.3
+pymongo==4.7.1
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
@@ -214,17 +214,17 @@
     #   pandas
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via pybtex
-pyzmq==26.0.0
+pyzmq==26.0.2
     # via maggma
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
@@ -242,15 +242,15 @@
     # via boto3
 scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
-shapely==2.0.3
+shapely==2.0.4
     # via
     #   emmet-api (setup.py)
     #   pymatgen-analysis-alloys
 six==1.16.0
     # via
     #   ddsketch
     #   ddtrace
```

### Comparing `emmet-api-0.83.0/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.83.1/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via starlette
@@ -18,21 +18,21 @@
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.2
     # via paramiko
-blinker==1.7.0
+blinker==1.8.1
     # via flask
-boto3==1.34.85
+boto3==1.34.95
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.85
+botocore==1.34.95
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -55,84 +55,75 @@
     #   mkdocstrings
     #   mongogrant
     #   uvicorn
 colorama==0.4.6
     # via griffe
 contourpy==1.2.1
     # via matplotlib
-coverage[toml]==7.4.4
+coverage[toml]==7.5.0
     # via pytest-cov
 cryptography==42.0.5
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.1
+ddtrace==2.8.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
     #   maggma
     #   pymongo
-emmet-core==0.82.1
+emmet-core==0.83.0
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.110.1
+fastapi==0.110.3
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.13.4
+filelock==3.14.0
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.2
+griffe==0.44.0
     # via mkdocstrings-python
-gunicorn==21.2.0
+gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
 idna==3.7
     # via
     #   anyio
     #   requests
 importlib-metadata==7.0.0
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   mkdocstrings
-    #   opentelemetry-api
-importlib-resources==6.4.0
-    # via
-    #   matplotlib
-    #   spglib
+    # via opentelemetry-api
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.2.0
     # via flask
 jinja2==3.1.3
     # via
     #   emmet-api (setup.py)
@@ -144,25 +135,25 @@
     # via
     #   boto3
     #   botocore
 joblib==1.4.0
     # via pymatgen
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.64.1
+maggma==0.66.0
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -175,66 +166,70 @@
     #   mkdocstrings
     #   werkzeug
 matplotlib==3.8.4
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.5.3
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
     #   mkdocstrings
 mkdocs-autorefs==1.0.1
     # via mkdocstrings
 mkdocs-awesome-pages-plugin==2.9.2
     # via emmet-api (setup.py)
+mkdocs-get-deps==0.2.0
+    # via mkdocs
 mkdocs-markdownextradata-plugin==0.2.5
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.3.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.24.3
+mkdocstrings[python]==0.25.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.9.2
+mkdocstrings-python==1.10.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.3.31
+monty==2024.4.17
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via maggma
-mypy==1.9.0
+mypy==1.10.0
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.4.0
     # via mkdocs-awesome-pages-plugin
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
     # via
     #   contourpy
     #   maggma
@@ -262,22 +257,22 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
-    #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
     #   virtualenv
-plotly==5.20.0
+plotly==5.21.0
     # via pymatgen
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pre-commit==3.7.0
     # via emmet-api (setup.py)
 protobuf==5.26.1
     # via ddtrace
 pybtex==0.24.0
     # via
@@ -285,53 +280,53 @@
     #   pymatgen
 pycodestyle==2.11.1
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   emmet-core
     #   fastapi
     #   maggma
     #   pydantic-settings
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via
     #   emmet-core
     #   maggma
-pydash==8.0.0
+pydash==8.0.1
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via mkdocs-material
 pymatgen==2024.4.13
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymdown-extensions==10.7.1
+pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
-pymongo==4.6.3
+pymongo==4.7.1
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==5.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.9.0.post0
     # via
@@ -343,24 +338,25 @@
 python-dotenv==1.0.1
     # via pydantic-settings
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-pyzmq==26.0.0
+pyzmq==26.0.2
     # via maggma
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   mongogrant
     #   pymatgen
@@ -378,15 +374,15 @@
     # via boto3
 scipy==1.13.0
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
-shapely==2.0.3
+shapely==2.0.4
     # via
     #   emmet-api (setup.py)
     #   pymatgen-analysis-alloys
 six==1.16.0
     # via
     #   ddsketch
     #   ddtrace
@@ -418,61 +414,54 @@
     #   pytest
 tornado==6.4
     # via livereload
 tqdm==4.66.2
     # via
     #   maggma
     #   pymatgen
-types-requests==2.31.0.6
+types-requests==2.31.0.20240406
     # via emmet-api (setup.py)
-types-setuptools==69.5.0.20240415
+types-setuptools==69.5.0.20240423
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.14
-    # via types-requests
 typing-extensions==4.11.0
     # via
-    #   aioitertools
     #   anyio
     #   asgiref
-    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
-    #   mkdocstrings
     #   mypy
     #   pydantic
     #   pydantic-core
     #   pydash
-    #   starlette
     #   uvicorn
 tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
+    #   types-requests
 uvicorn==0.29.0
     # via maggma
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via pre-commit
 watchdog==4.0.0
     # via mkdocs
 wcmatch==8.5.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==3.0.2
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.18.1
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.0/setup.py` & `emmet-api-0.83.1/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/start.sh` & `emmet-api-0.83.1/start.sh`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/_consumer/test_query_operators.py` & `emmet-api-0.83.1/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/_general_store/test_query_operators.py` & `emmet-api-0.83.1/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/core/test_mapi.py` & `emmet-api-0.83.1/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.83.1/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/electrodes/test_utils.py` & `emmet-api-0.83.1/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/materials/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/materials/test_utils.py` & `emmet-api-0.83.1/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/summary/test_hint_scheme.py` & `emmet-api-0.83.1/tests/materials/summary/test_hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/summary/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.83.1/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.83.1/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/synthesis/test_utils.py` & `emmet-api-0.83.1/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/tasks/test_utils.py` & `emmet-api-0.83.1/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/materials/xas/test_query_operators.py` & `emmet-api-0.83.1/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/metal_binding/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/metal_binding/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/tasks/test_utils.py` & `emmet-api-0.83.1/tests/molecules/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.0/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.83.1/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

