# Comparing `tmp/dials_data-2.4.85.tar.gz` & `tmp/dials_data-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dials_data-2.4.85.tar", last modified: Thu May  2 08:33:23 2024, max compression
+gzip compressed data, was "dials_data-2.4.9.tar", last modified: Tue Mar  8 09:34:37 2022, max compression
```

## Comparing `dials_data-2.4.85.tar` & `dials_data-2.4.9.tar`

### file list

```diff
@@ -1,128 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:23.620383 dials_data-2.4.85/
--rw-r--r--   0 vsts      (1001) docker     (127)     3357 2024-05-02 08:33:12.000000 dials_data-2.4.85/CONTRIBUTING.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     2485 2024-05-02 08:33:12.000000 dials_data-2.4.85/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     1486 2024-05-02 08:33:12.000000 dials_data-2.4.85/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      296 2024-05-02 08:33:12.000000 dials_data-2.4.85/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     6092 2024-05-02 08:33:23.620383 dials_data-2.4.85/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2491 2024-05-02 08:33:12.000000 dials_data-2.4.85/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:23.580382 dials_data-2.4.85/dials_data/
--rw-r--r--   0 vsts      (1001) docker     (127)      353 2024-05-02 08:33:20.000000 dials_data-2.4.85/dials_data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4848 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/cli.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5214 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/datasets.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:23.596382 dials_data-2.4.85/dials_data/definitions/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/4fluoro_cxi.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/MyD88_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/aluminium_standard.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2511 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/blend_tutorial.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     4110 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/centroid_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1101 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/cspad_metrology.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1216 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/cunir_serial.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1618 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/cunir_serial_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1078 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/dtpb_serial_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2094 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/four_circle_eiger.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    10198 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/fumarase.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      687 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/i19_1_pdteet_index.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2388 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/image_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      821 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/indexing_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     3659 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/insulin.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1962 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/insulin_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      800 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/isis_sxd_example_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      730 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/isis_sxd_nacl_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1492 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/iterative_cspad_refinement.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1397 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    10657 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/l_cysteine_dials_output.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      725 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/lcls_rayonix_kapton.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/lysozyme_JF16M_4img.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/lysozyme_JF16M_4img_spectra.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/lysozyme_electron_diffraction.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      924 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/mpro_x0305_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    11627 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/mpro_x0692.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1810 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/multi_crystal_proteinase_k.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    11610 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/polyhedra_narrow_wedges.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      761 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/pycbf.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/pychef.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2403 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/quartz_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     3419 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/refinement_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    20032 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/relion_tutorial_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      935 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/semisynthetic_multilattice.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    83017 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/small_molecule_example.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1279 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/spring8_ccp4_2018.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      594 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/thaumatin_eiger_screen.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2750 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/thaumatin_grid_scan.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    45846 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/thaumatin_i04.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2479 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/trypsin_multi_lattice.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2459 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/vmxi_proteinase_k_sweeps.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      651 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/vmxi_thaumatin.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/vmxi_thaumatin_grid_index.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     7832 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/x4wide.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      755 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/definitions/x4wide_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    12537 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/download.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:23.616383 dials_data-2.4.85/dials_data/hashinfo/
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/4fluoro_cxi.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      276 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/MyD88_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/aluminium_standard.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2566 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/blend_tutorial.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2642 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/centroid_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      364 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/cspad_metrology.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      812 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/cunir_serial.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      800 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/cunir_serial_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/dtpb_serial_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/four_circle_eiger.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    10782 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/fumarase.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      279 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/i19_1_pdteet_index.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/image_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      536 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/indexing_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     4152 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/insulin.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/insulin_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/isis_sxd_example_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      453 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/iterative_cspad_refinement.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      634 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     7029 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/l_cysteine_dials_output.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/lcls_rayonix_kapton.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      280 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/lysozyme_JF16M_4img.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/lysozyme_JF16M_4img_spectra.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/lysozyme_electron_diffraction.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      456 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/mpro_x0305_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/mpro_x0692.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1590 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/multi_crystal_proteinase_k.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     7126 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/polyhedra_narrow_wedges.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      369 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/pycbf.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/pychef.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1408 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/quartz_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1862 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/refinement_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/relion_tutorial_data.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      454 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/semisynthetic_multilattice.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    79302 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/small_molecule_example.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/spring8_ccp4_2018.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      454 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/thaumatin_eiger_screen.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1793 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/thaumatin_grid_scan.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    48162 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/thaumatin_i04.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2504 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/trypsin_multi_lattice.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1526 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/vmxi_thaumatin.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      278 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/vmxi_thaumatin_grid_index.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     8112 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/x4wide.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      456 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/hashinfo/x4wide_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1049 2024-05-02 08:33:12.000000 dials_data-2.4.85/dials_data/pytest11.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:23.620383 dials_data-2.4.85/dials_data.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     6092 2024-05-02 08:33:23.000000 dials_data-2.4.85/dials_data.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4659 2024-05-02 08:33:23.000000 dials_data-2.4.85/dials_data.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-02 08:33:23.000000 dials_data-2.4.85/dials_data.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      192 2024-05-02 08:33:23.000000 dials_data-2.4.85/dials_data.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-02 08:33:23.000000 dials_data-2.4.85/dials_data.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-05-02 08:33:23.000000 dials_data-2.4.85/dials_data.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-02 08:33:23.000000 dials_data-2.4.85/dials_data.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:23.620383 dials_data-2.4.85/docs/
--rwxr-xr-x   0 vsts      (1001) docker     (127)     4880 2024-05-02 08:33:12.000000 dials_data-2.4.85/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-05-02 08:33:12.000000 dials_data-2.4.85/docs/contributing.rst
--rw-r--r--   0 vsts      (1001) docker     (127)       28 2024-05-02 08:33:12.000000 dials_data-2.4.85/docs/history.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     1997 2024-05-02 08:33:12.000000 dials_data-2.4.85/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     5127 2024-05-02 08:33:12.000000 dials_data-2.4.85/docs/installation.rst
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-02 08:33:12.000000 dials_data-2.4.85/docs/readme.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3976 2024-05-02 08:33:12.000000 dials_data-2.4.85/docs/why.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     2537 2024-05-02 08:33:20.000000 dials_data-2.4.85/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-02 08:33:23.624383 dials_data-2.4.85/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 08:33:23.620383 dials_data-2.4.85/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     2549 2024-05-02 08:33:12.000000 dials_data-2.4.85/tests/test_dials_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2325 2024-05-02 08:33:12.000000 dials_data-2.4.85/tests/test_yaml_files.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3357 2022-03-08 09:34:30.000000 dials_data-2.4.9/CONTRIBUTING.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     2146 2022-03-08 09:34:30.000000 dials_data-2.4.9/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1486 2022-03-08 09:34:30.000000 dials_data-2.4.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      296 2022-03-08 09:34:30.000000 dials_data-2.4.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     5635 2022-03-08 09:34:37.645043 dials_data-2.4.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     2491 2022-03-08 09:34:30.000000 dials_data-2.4.9/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.633043 dials_data-2.4.9/dials_data/
+-rw-r--r--   0 vsts      (1001) docker     (121)      352 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4870 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5214 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/datasets.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.637043 dials_data-2.4.9/dials_data/definitions/
+-rw-r--r--   0 vsts      (1001) docker     (121)      987 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/MyD88_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1364 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/aluminium_standard.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2511 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/blend_tutorial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     4110 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/centroid_test_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      903 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/cunir_serial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1279 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/cunir_serial_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2094 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/four_circle_eiger.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    10198 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/fumarase.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      687 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/i19_1_pdteet_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2228 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/image_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     3659 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/insulin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/insulin_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      800 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/isis_sxd_example_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1397 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    10657 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/l_cysteine_dials_output.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      725 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/lcls_rayonix_kapton.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/lysozyme_electron_diffraction.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/mpro_x0305_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    11627 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/mpro_x0692.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1761 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/multi_crystal_proteinase_k.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      761 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/pycbf.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      150 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/pychef.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2403 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/quartz_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    20032 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/relion_tutorial_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    83017 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/small_molecule_example.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1279 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/spring8_ccp4_2018.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/thaumatin_eiger_screen.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2750 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/thaumatin_grid_scan.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    45846 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/thaumatin_i04.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2479 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/trypsin_multi_lattice.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2459 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/vmxi_proteinase_k_sweeps.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      645 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin_grid_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     7832 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/x4wide.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      755 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/x4wide_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    11892 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/download.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/dials_data/hashinfo/
+-rw-r--r--   0 vsts      (1001) docker     (121)      276 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/MyD88_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/aluminium_standard.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2566 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/blend_tutorial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2642 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/centroid_test_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      547 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/cunir_serial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      624 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/cunir_serial_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      375 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/four_circle_eiger.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    10782 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/fumarase.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      279 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/i19_1_pdteet_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1340 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/image_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     4152 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/insulin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1162 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/insulin_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      642 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/isis_sxd_example_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      634 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     7029 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/l_cysteine_dials_output.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      366 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/lcls_rayonix_kapton.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      275 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/lysozyme_electron_diffraction.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/mpro_x0305_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/mpro_x0692.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1502 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/multi_crystal_proteinase_k.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      369 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/pycbf.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/pychef.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/relion_tutorial_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    79302 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/small_molecule_example.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/spring8_ccp4_2018.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/thaumatin_eiger_screen.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1793 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/thaumatin_grid_scan.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    48162 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/thaumatin_i04.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2504 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/trypsin_multi_lattice.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1526 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/vmxi_thaumatin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      278 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/vmxi_thaumatin_grid_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     8112 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/x4wide.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/x4wide_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/pytest11.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.633043 dials_data-2.4.9/dials_data.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5635 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     3624 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       48 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/docs/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     4880 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       33 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/contributing.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)       28 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/history.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1997 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     5127 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/installation.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)       27 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/readme.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     3976 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/why.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      217 2022-03-08 09:34:30.000000 dials_data-2.4.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1618 2022-03-08 09:34:37.645043 dials_data-2.4.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      128 2022-03-08 09:34:30.000000 dials_data-2.4.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2468 2022-03-08 09:34:30.000000 dials_data-2.4.9/tests/test_dials_data.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2325 2022-03-08 09:34:30.000000 dials_data-2.4.9/tests/test_yaml_files.py
```

### Comparing `dials_data-2.4.85/CONTRIBUTING.rst` & `dials_data-2.4.9/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
 
 Get Started!
 ------------
 
-Ready to contribute? Here's how to set up `dials-data` for local development.
+Ready to contribute? Here's how to set up `dials_data` for local development.
 
 1. Fork the `dials/data` `repository on GitHub <https://github.com/dials/data>`__.
 2. Clone your fork locally::
 
     $ git clone git@github.com:your_name_here/data.git
 
 3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
```

### Comparing `dials_data-2.4.85/HISTORY.rst` & `dials_data-2.4.9/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 =======
 History
 =======
 
 2.5 (????-??-??)
 ^^^^^^^^^^^^^^^^
 
-* Fix permission generation when extracting tar archives. Files extracted will be created with
-  default permissions, instead of what has been packed in with the archive. This solves the issue
-  of shared data stores becoming inaccessible to some users.
-* ``DataFetcher``: new parameter verify=True to verify download hashinfo by default.
 
 2.4 (2022-03-07)
 ^^^^^^^^^^^^^^^^
 
 * dials_data no longer uses ``py.path`` internally.
 * dials_data now includes type checking with mypy.
 * We started using the ``requests`` library for faster downloads.
```

### Comparing `dials_data-2.4.85/LICENSE` & `dials_data-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/PKG-INFO` & `dials_data-2.4.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: dials_data
-Version: 2.4.85
+Version: 2.4.9
 Summary: DIALS Regression Data Manager
-Author-email: DIALS development team <dials-support@lists.sourceforge.net>
+Home-page: https://github.com/dials/data
+Author: DIALS development team
+Author-email: dials-support@lists.sourceforge.net
 License: BSD 3-Clause License
-Project-URL: Homepage, https://github.com/dials/data
 Project-URL: Bug Tracker, https://github.com/dials/data/issues
 Project-URL: Documentation, https://dials-data.readthedocs.io/
 Project-URL: Source Code, https://github.com/dials/data
 Keywords: dials,dials_data
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: importlib_resources!=6.2,!=6.3.0,!=6.3.1,>=1.1
-Requires-Dist: pytest
-Requires-Dist: pyyaml
-Requires-Dist: requests
 
 =============================
 DIALS Regression Data Manager
 =============================
 
 .. image:: https://img.shields.io/pypi/v/dials_data.svg
         :target: https://pypi.python.org/pypi/dials_data
@@ -65,34 +63,34 @@
 .. image:: https://img.shields.io/pypi/l/dials_data.svg
         :target: https://pypi.python.org/pypi/dials_data
         :alt: BSD license
 
 A python package providing data files used for regression tests in
 DIALS_, dxtbx_, xia2_ and related packages.
 
-If you want to know more about what ``dials-data`` is you can
+If you want to know more about what ``dials_data`` is you can
 have a read through the `background information <https://dials-data.readthedocs.io/en/latest/why.html>`__.
 
 For everything else `the main documentation <https://dials-data.readthedocs.io/>`__ is probably the best start.
 
 
 Installation
 ^^^^^^^^^^^^
 
 To install this package in a normal Python environment, run::
 
-    pip install dials-data
+    pip install dials_data
 
 and then you can use it with::
 
     dials.data
 
 If you are in a conda environment you can instead run::
 
-    conda install -c conda-forge dials-data
+    conda install -c conda-forge dials_data
 
 For more details please take a look at the
 `installation and usage page <https://dials-data.readthedocs.io/en/latest/installation.html>`__.
 
 
 .. _DIALS: https://dials.github.io
 .. _dxtbx: https://github.com/cctbx/cctbx_project/tree/master/dxtbx
@@ -101,18 +99,14 @@
 =======
 History
 =======
 
 2.5 (????-??-??)
 ^^^^^^^^^^^^^^^^
 
-* Fix permission generation when extracting tar archives. Files extracted will be created with
-  default permissions, instead of what has been packed in with the archive. This solves the issue
-  of shared data stores becoming inaccessible to some users.
-* ``DataFetcher``: new parameter verify=True to verify download hashinfo by default.
 
 2.4 (2022-03-07)
 ^^^^^^^^^^^^^^^^
 
 * dials_data no longer uses ``py.path`` internally.
 * dials_data now includes type checking with mypy.
 * We started using the ``requests`` library for faster downloads.
@@ -188,7 +182,9 @@
 * pytest fixture
 
 
 0.1 (2018-11-02)
 ^^^^^^^^^^^^^^^^
 
 * First automatic deployment and release on PyPI
+
+
```

### Comparing `dials_data-2.4.85/README.rst` & `dials_data-2.4.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -37,34 +37,34 @@
 .. image:: https://img.shields.io/pypi/l/dials_data.svg
         :target: https://pypi.python.org/pypi/dials_data
         :alt: BSD license
 
 A python package providing data files used for regression tests in
 DIALS_, dxtbx_, xia2_ and related packages.
 
-If you want to know more about what ``dials-data`` is you can
+If you want to know more about what ``dials_data`` is you can
 have a read through the `background information <https://dials-data.readthedocs.io/en/latest/why.html>`__.
 
 For everything else `the main documentation <https://dials-data.readthedocs.io/>`__ is probably the best start.
 
 
 Installation
 ^^^^^^^^^^^^
 
 To install this package in a normal Python environment, run::
 
-    pip install dials-data
+    pip install dials_data
 
 and then you can use it with::
 
     dials.data
 
 If you are in a conda environment you can instead run::
 
-    conda install -c conda-forge dials-data
+    conda install -c conda-forge dials_data
 
 For more details please take a look at the
 `installation and usage page <https://dials-data.readthedocs.io/en/latest/installation.html>`__.
 
 
 .. _DIALS: https://dials.github.io
 .. _dxtbx: https://github.com/cctbx/cctbx_project/tree/master/dxtbx
```

### Comparing `dials_data-2.4.85/dials_data/cli.py` & `dials_data-2.4.9/dials_data/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,17 @@
 The most commonly used commands are:
    list     List available datasets
    get      Download datasets
 
 Each command has its own set of parameters, and you can get more information
 by running dials.data <command> --help
 
-""".format(version=version),
+""".format(
+            version=version
+        ),
         formatter_class=argparse.RawTextHelpFormatter,
     )
     parser.add_argument("subcommand", help=argparse.SUPPRESS)
     # parse_args defaults to [1:] for args, but need to
     # exclude the rest of the args too, or validation will fail
     parameters = sys.argv[1:2]
     if not parameters:
```

### Comparing `dials_data-2.4.85/dials_data/datasets.py` & `dials_data-2.4.9/dials_data/datasets.py`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/MyD88_processed.yml` & `dials_data-2.4.9/dials_data/definitions/MyD88_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/aluminium_standard.yml` & `dials_data-2.4.9/dials_data/definitions/aluminium_standard.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 name: Aluminium standard
 author: Elena Pascal, Yun Song (2021)
 license: CC-BY 4.0
 description: >
   Powder diffraction data collected by Yun Song at DLS on eBIC's Talos Arctica (m12).
   The sample is a polycrystalline aluminium standard.
 
-  `imported.expt` was generated with:
+  imported.expt was generated with
     $ dials.import $(dials.data get -q aluminium_standard)/0p67_5s_0000.mrc
 
-  `eyeballed.expt` was generated with: 
-    $ dials.powder_calibrate imported.expt standard="Al" coarse_geom="eyeballed.expt"
-
-  `calibrated.expt` was generated without using the wizard with:
-    $ dials.powder_calibrate eyeballed.expt standard="Al" eyeball=False
+  eyeballed.expt was generated with dials.powder_calibrate_widget
 
+  calibrated.expt was generated with
+    starting_file = "eyeballed.expt"
+    test_args = [starting_file, "standard=Al", "eyeball=False"]
+    expt_parameters, user_arguments = parse_args(args=test_args)
+    calibrator = PowderCalibrator(expt_params=expt_parameters, user_args=user_arguments)
+    calibrator.calibrate_with_calibrant(verbose=True)
   
   Used for powder geometry calibration testing.
 
 data:
 
   - url: https://raw.githubusercontent.com/dials/data-files/35addc5660df90b3b9579bc932e95a9aa01389fe/aluminium_standard/0p67_5s_0000.mrc
   - url: https://raw.githubusercontent.com/dials/data-files/35addc5660df90b3b9579bc932e95a9aa01389fe/aluminium_standard/imported.expt
```

### Comparing `dials_data-2.4.85/dials_data/definitions/blend_tutorial.yml` & `dials_data-2.4.9/dials_data/definitions/blend_tutorial.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/centroid_test_data.yml` & `dials_data-2.4.9/dials_data/definitions/centroid_test_data.yml`

 * *Files 8% similar despite different names*

```diff
@@ -20,20 +20,20 @@
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/centroid_0007.cbf
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/centroid_0008.cbf
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/centroid_0009.cbf
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/crystal.json
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/datablock.json
   - url: https://github.com/dials/data-files/raw/12c29cae96057da91a2da5c5ce042846cf9a79fa/centroid_test_data/datablock_with_bad_lookup.json
   - url: https://github.com/dials/data-files/raw/12c29cae96057da91a2da5c5ce042846cf9a79fa/centroid_test_data/datablock_with_lookup.json
-  - url: https://github.com/dials/data-files/raw/3eb66b340b7ade76dd8c41abfbf6f2f83bfb846a/centroid_test_data/experiments.json
+  - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/experiments.json
   - url: https://github.com/dials/data-files/raw/12c29cae96057da91a2da5c5ce042846cf9a79fa/centroid_test_data/experiments_with_bad_lookup.json
   - url: https://github.com/dials/data-files/raw/12c29cae96057da91a2da5c5ce042846cf9a79fa/centroid_test_data/experiments_with_lookup.json
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/fake_long_experiments.json
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/imported_experiments.json
-  - url: https://github.com/dials/data-files/raw/3eb66b340b7ade76dd8c41abfbf6f2f83bfb846a/centroid_test_data/indexed.expt
+  - url: https://github.com/dials/data-files/raw/f18bfc49b4a086db0145097ea2cb67cf23be0835/centroid_test_data/indexed.expt
   - url: https://github.com/dials/data-files/raw/f18bfc49b4a086db0145097ea2cb67cf23be0835/centroid_test_data/indexed.refl
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/integrated.pickle
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/integrated.refl
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/INTEGRATE.HKL
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/lookup_mask.pickle
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/mask.pickle
   - url: https://github.com/dials/data-files/raw/a02df474ff193f102624bd08038cdc2c421dc8ee/centroid_test_data/SPOT.XDS
```

### Comparing `dials_data-2.4.85/dials_data/definitions/cunir_serial.yml` & `dials_data-2.4.9/dials_data/definitions/cunir_serial.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 name: Serial synchrotron crystallography images of CuNiR, taken on I24 beamline at DLS
 author: Robin Owen, Mike Hough (2021)
 license: CC-BY 4.0
 description: >
   5 example SSX images of CuNiR, taken on I24 beamline at Diamond
   Light Source.
-  Also provided is a reference PDB structure for this protein (pdb entry 2BW4),
-  in PDB and cif format, plus the reference intensity data from that deposition.
 
 data:
   - url: https://github.com/dials/data-files/raw/a0e40127492faa165a9f5ef7590ff1591957e6d9/ssx_CuNiR_test_data/merlin0047_17000.cbf
   - url: https://github.com/dials/data-files/raw/a0e40127492faa165a9f5ef7590ff1591957e6d9/ssx_CuNiR_test_data/merlin0047_17001.cbf
   - url: https://github.com/dials/data-files/raw/a0e40127492faa165a9f5ef7590ff1591957e6d9/ssx_CuNiR_test_data/merlin0047_17002.cbf
   - url: https://github.com/dials/data-files/raw/a0e40127492faa165a9f5ef7590ff1591957e6d9/ssx_CuNiR_test_data/merlin0047_17003.cbf
   - url: https://github.com/dials/data-files/raw/a0e40127492faa165a9f5ef7590ff1591957e6d9/ssx_CuNiR_test_data/merlin0047_17004.cbf
-  - url: https://files.rcsb.org/download/2BW4.pdb
-  - url: https://files.rcsb.org/download/2bw4-sf.cif
-  - url: https://files.rcsb.org/download/2bw4.cif
```

### Comparing `dials_data-2.4.85/dials_data/definitions/cunir_serial_processed.yml` & `dials_data-2.4.9/dials_data/definitions/cunir_serial_processed.yml`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 author: James Beilsten-Edmands (2021)
 license: CC-BY 4.0
 description: >
   Example processed SSX data on CuNiR, taken on I24 beamline at Diamond
   Light Source, courtesy of Robin Owen and Mike Hough.
   5 images were processed with DIALS v3.7.3, with and without a reference
   geometry, for testing indexing.
-  Indexed data were integrated with DIALS commit #37ef448 with dev.dials.ssx_integrate
   Images can be found in the 'cunir_serial' data set; file references are
   laid out so that the images can be accessed if that data set is present.
 
 data:
   - url: https://github.com/dials/data-files/raw/13e97f957175c3e31d34e567b7369b748cfa1d55/ssx_CuNiR_test_data/imported_no_ref_5.expt
   - url: https://github.com/dials/data-files/raw/13e97f957175c3e31d34e567b7369b748cfa1d55/ssx_CuNiR_test_data/imported_with_ref_5.expt
   - url: https://github.com/dials/data-files/raw/da38a5de509cb7cb22cc28f439058c66923333d1/ssx_CuNiR_test_data/strong_1.refl
   - url: https://github.com/dials/data-files/raw/da38a5de509cb7cb22cc28f439058c66923333d1/ssx_CuNiR_test_data/strong_5.refl
   - url: https://github.com/dials/data-files/raw/70d2cbb1bb5d0678b133039a7e009a623762f0ff/ssx_CuNiR_test_data/indexed.expt
   - url: https://github.com/dials/data-files/raw/70d2cbb1bb5d0678b133039a7e009a623762f0ff/ssx_CuNiR_test_data/indexed.refl
-  - url: https://github.com/dials/data-files/raw/d42250171384b66828803de1b07d1009db2e5472/ssx_CuNiR_test_data/integrated.expt
-  - url: https://github.com/dials/data-files/raw/d42250171384b66828803de1b07d1009db2e5472/ssx_CuNiR_test_data/integrated.refl
```

### Comparing `dials_data-2.4.85/dials_data/definitions/four_circle_eiger.yml` & `dials_data-2.4.9/dials_data/definitions/four_circle_eiger.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
   03_CuHF2pyz2PF6b_P_O.tar.xz
   Two sequential rotation scans:
     CuHF2pyz2PF6b_P_O_01.nxs — a 1750-image 350° φ scan.
     CuHF2pyz2PF6b_P_O_02.nxs — a 600-image 120° ω scan.
   
 data:
-  - url: https://zenodo.org/record/6347466/files/01_CuHF2pyz2PF6b_Phi.tar.xz
+  - url: https://zenodo.org/record/6093231/files/01_CuHF2pyz2PF6b_Phi.tar.xz
     files:
       - 01_CuHF2pyz2PF6b_Phi/CuHF2pyz2PF6b_Phi_01_000001.h5
       - 01_CuHF2pyz2PF6b_Phi/CuHF2pyz2PF6b_Phi_01_000002.h5
       - 01_CuHF2pyz2PF6b_Phi/CuHF2pyz2PF6b_Phi_01_meta.h5
       - 01_CuHF2pyz2PF6b_Phi/CuHF2pyz2PF6b_Phi_01.nxs
-  - url: https://zenodo.org/record/6347466/files/02_CuHF2pyz2PF6b_2T.tar.xz
+  - url: https://zenodo.org/record/6093231/files/02_CuHF2pyz2PF6b_2T.tar.xz
     files:
       - 02_CuHF2pyz2PF6b_2T/CuHF2pyz2PF6b_2T_01_000001.h5
       - 02_CuHF2pyz2PF6b_2T/CuHF2pyz2PF6b_2T_01_000002.h5
       - 02_CuHF2pyz2PF6b_2T/CuHF2pyz2PF6b_2T_01_meta.h5
       - 02_CuHF2pyz2PF6b_2T/CuHF2pyz2PF6b_2T_01.nxs
-  - url: https://zenodo.org/record/6347466/files/03_CuHF2pyz2PF6b_P_O.tar.xz
+  - url: https://zenodo.org/record/6093231/files/03_CuHF2pyz2PF6b_P_O.tar.xz
     files:
       - 03_CuHF2pyz2PF6b_P_O/CuHF2pyz2PF6b_P_O_01_000001.h5
       - 03_CuHF2pyz2PF6b_P_O/CuHF2pyz2PF6b_P_O_01_000002.h5
       - 03_CuHF2pyz2PF6b_P_O/CuHF2pyz2PF6b_P_O_01_meta.h5
       - 03_CuHF2pyz2PF6b_P_O/CuHF2pyz2PF6b_P_O_01.nxs
       - 03_CuHF2pyz2PF6b_P_O/CuHF2pyz2PF6b_P_O_02_000001.h5
       - 03_CuHF2pyz2PF6b_P_O/CuHF2pyz2PF6b_P_O_02_meta.h5
```

### Comparing `dials_data-2.4.85/dials_data/definitions/fumarase.yml` & `dials_data-2.4.9/dials_data/definitions/fumarase.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/i19_1_pdteet_index.yml` & `dials_data-2.4.9/dials_data/definitions/i19_1_pdteet_index.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/image_examples.yml` & `dials_data-2.4.9/dials_data/definitions/image_examples.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,9 @@
   - url: https://github.com/dials/data-files/raw/1916a8649e9f505199949f90822165d368c93872/image_examples/dlsnxs2cbf_therm_0001.cbf.gz
   - url: https://github.com/dials/data-files/raw/1916a8649e9f505199949f90822165d368c93872/image_examples/simtbx_FormatSMVJHSim_001.img
   - url: https://github.com/dials/data-files/raw/64666892ee8c5fefd2fadef5d5927a2c3c6c6502/image_examples/ThermoFisher_EPU-D_1.5_001.mrc.gz
   - url: https://github.com/dials/data-files/raw/7260492a487e88dde58f8be044b21cef1c7578ef/image_examples/dectris_eiger_data_000001.h5
   - url: https://github.com/dials/data-files/raw/7260492a487e88dde58f8be044b21cef1c7578ef/image_examples/dectris_eiger_master.h5
   - url: https://github.com/dials/data-files/raw/9ecf5a4e6d36a2c77574178d306292dd1c093359/image_examples/Gatan_float32_zero_array_001.dm4.gz
   - url: https://github.com/dials/data-files/raw/f587a81ac82b3c35a757492e92259a0105ee1c2a/image_examples/SACLA-MPCCD-run266702-0-subset-refined_experiments_level1.json
-  - url: https://github.com/dials/data-files/raw/30e7df95d17ef152e1eef6e286a4f8143eac7c73/image_examples/SACLA-MPCCD-run266702-0-subset-known_orientations.expt
   - url: https://github.com/dials/data-files/raw/f587a81ac82b3c35a757492e92259a0105ee1c2a/image_examples/SACLA-MPCCD-run266702-0-subset.h5
   - url: https://github.com/dials/data-files/raw/2fc35b473ea4a9c68279e438d4e39e2662d9dfdb/image_examples/endonat3_001.mar2300
```

### Comparing `dials_data-2.4.85/dials_data/definitions/insulin.yml` & `dials_data-2.4.9/dials_data/definitions/insulin.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/insulin_processed.yml` & `dials_data-2.4.9/dials_data/definitions/insulin_processed.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     $ dials.index imported.expt strong.refl space_group=I23
     $ dials.refine indexed.{expt,refl}
     $ dials.integrate refined.{expt,refl} nproc=8
     $ dials.symmetry integrated.{expt,refl}
     $ dials.scale symmetrized.{expt,refl}
 
 data:
-  - url: https://github.com/dials/data-files/raw/dab5530ec4e1631dda14e91bb59e8d6368b4dcdf/insulin_processed/imported.expt
+  - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/imported.expt
   - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/strong.refl
-  - url: https://github.com/dials/data-files/raw/dab5530ec4e1631dda14e91bb59e8d6368b4dcdf/insulin_processed/indexed.expt
+  - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/indexed.expt
   - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/indexed.refl
-  - url: https://github.com/dials/data-files/raw/dab5530ec4e1631dda14e91bb59e8d6368b4dcdf/insulin_processed/integrated.expt
+  - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/integrated.expt
   - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/integrated.refl
-  - url: https://github.com/dials/data-files/raw/dab5530ec4e1631dda14e91bb59e8d6368b4dcdf/insulin_processed/refined.expt
+  - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/refined.expt
   - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/refined.refl
-  - url: https://github.com/dials/data-files/raw/dab5530ec4e1631dda14e91bb59e8d6368b4dcdf/insulin_processed/scaled.expt
+  - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/scaled.expt
   - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/scaled.refl
-  - url: https://github.com/dials/data-files/raw/dab5530ec4e1631dda14e91bb59e8d6368b4dcdf/insulin_processed/symmetrized.expt
+  - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/symmetrized.expt
   - url: https://github.com/dials/data-files/raw/4ccd4932291c258316530597e40e252d1f5e37c2/insulin_processed/symmetrized.refl
```

### Comparing `dials_data-2.4.85/dials_data/definitions/isis_sxd_example_data.yml` & `dials_data-2.4.9/dials_data/definitions/isis_sxd_example_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml` & `dials_data-2.4.9/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/l_cysteine_dials_output.yml` & `dials_data-2.4.9/dials_data/definitions/l_cysteine_dials_output.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/lcls_rayonix_kapton.yml` & `dials_data-2.4.9/dials_data/definitions/lcls_rayonix_kapton.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/lysozyme_electron_diffraction.yml` & `dials_data-2.4.9/dials_data/definitions/lysozyme_electron_diffraction.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/mpro_x0305_processed.yml` & `dials_data-2.4.9/dials_data/definitions/mpro_x0305_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/mpro_x0692.yml` & `dials_data-2.4.9/dials_data/definitions/mpro_x0692.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/multi_crystal_proteinase_k.yml` & `dials_data-2.4.9/dials_data/definitions/multi_crystal_proteinase_k.yml`

 * *Files 4% similar despite different names*

```diff
@@ -17,8 +17,7 @@
  - url: https://dials.diamond.ac.uk/regression_data/multi_crystal_proteinase_k/reflections_1.pickle
  - url: https://dials.diamond.ac.uk/regression_data/multi_crystal_proteinase_k/reflections_2.pickle
  - url: https://dials.diamond.ac.uk/regression_data/multi_crystal_proteinase_k/reflections_3.pickle
  - url: https://dials.diamond.ac.uk/regression_data/multi_crystal_proteinase_k/reflections_4.pickle
  - url: https://dials.diamond.ac.uk/regression_data/multi_crystal_proteinase_k/reflections_5.pickle
  - url: https://dials.diamond.ac.uk/regression_data/multi_crystal_proteinase_k/reflections_7.pickle
  - url: https://dials.diamond.ac.uk/regression_data/multi_crystal_proteinase_k/reflections_8.pickle
- - url: https://files.rcsb.org/download/2id8.pdb
```

### Comparing `dials_data-2.4.85/dials_data/definitions/pycbf.yml` & `dials_data-2.4.9/dials_data/definitions/pycbf.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/quartz_processed.yml` & `dials_data-2.4.9/dials_data/definitions/quartz_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/relion_tutorial_data.yml` & `dials_data-2.4.9/dials_data/definitions/relion_tutorial_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/small_molecule_example.yml` & `dials_data-2.4.9/dials_data/definitions/small_molecule_example.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/spring8_ccp4_2018.yml` & `dials_data-2.4.9/dials_data/definitions/spring8_ccp4_2018.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/thaumatin_eiger_screen.yml` & `dials_data-2.4.9/dials_data/definitions/thaumatin_eiger_screen.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/thaumatin_grid_scan.yml` & `dials_data-2.4.9/dials_data/definitions/thaumatin_grid_scan.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/thaumatin_i04.yml` & `dials_data-2.4.9/dials_data/definitions/thaumatin_i04.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/trypsin_multi_lattice.yml` & `dials_data-2.4.9/dials_data/definitions/trypsin_multi_lattice.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/vmxi_proteinase_k_sweeps.yml` & `dials_data-2.4.9/dials_data/definitions/vmxi_proteinase_k_sweeps.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/vmxi_thaumatin.yml` & `dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/vmxi_thaumatin_grid_index.yml` & `dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin_grid_index.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/x4wide.yml` & `dials_data-2.4.9/dials_data/definitions/x4wide.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/definitions/x4wide_processed.yml` & `dials_data-2.4.9/dials_data/definitions/x4wide_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/download.py` & `dials_data-2.4.9/dials_data/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import zipfile
 from pathlib import Path
 from typing import Any, Optional, Union
 from urllib.parse import urlparse
 
 import py.path
 import requests
-from requests.adapters import HTTPAdapter
-from urllib3.util.retry import Retry
 
 import dials_data.datasets
 
 if os.name == "posix":
     import fcntl
 
     def _platform_lock(file_handle):
@@ -173,25 +171,14 @@
 
     integrity_info["verify"] = verification_records
     return integrity_info
 
 
 def _fetch_filelist(filelist: list[dict[str, Any]]) -> list[dict[str, Any] | None]:
     with requests.Session() as rs:
-        retry_adapter = HTTPAdapter(
-            max_retries=Retry(
-                total=5,
-                backoff_factor=1,
-                raise_on_status=True,
-                status_forcelist={413, 429, 500, 502, 503, 504},
-            )
-        )
-        rs.mount("http://", retry_adapter)
-        rs.mount("https://", retry_adapter)
-
         pool = concurrent.futures.ThreadPoolExecutor(max_workers=5)
         results = pool.map(functools.partial(_fetch_file, rs), filelist)
         return list(results)
 
 
 def _fetch_file(
     session: requests.Session, source: dict[str, Any]
@@ -246,15 +233,15 @@
                             f"Expected file {f} not present "
                             f"in zip archive {source['file']}"
                         )
             else:
                 with tarfile.open(source["file"]) as tar:
                     for f in source["files"]:
                         try:
-                            tar.extract(f, path=source["file"].parent, set_attrs=False)
+                            tar.extract(f, path=source["file"].parent)
                         except KeyError:
                             print(
                                 f"Expected file {f} not present "
                                 f"in tar archive {source['file']}"
                             )
 
     if valid:
@@ -275,19 +262,18 @@
 
     To disable all downloads:
         df = DataFetcher(read_only=True)
 
     Do not use this class directly in tests! Use the dials_data fixture.
     """
 
-    def __init__(self, read_only: bool = False, verify: bool = True):
+    def __init__(self, read_only=False):
         self._cache: dict[str, Optional[Path]] = {}
         self._target_dir: Path = dials_data.datasets.repository_location()
         self._read_only: bool = read_only and os.access(self._target_dir, os.W_OK)
-        self._verify: bool = verify
 
     def __repr__(self) -> str:
         return "<{}DataFetcher: {}>".format(
             "R/O " if self._read_only else "",
             self._target_dir,
         )
 
@@ -330,21 +316,18 @@
             return self.result_filter(result=False)
         elif not pathlib:
             return self.result_filter(result=py.path.local(self._cache[test_data]))
         return self.result_filter(result=self._cache[test_data])
 
     def _attempt_fetch(self, test_data: str) -> Optional[Path]:
         if self._read_only:
-            hashinfo = fetch_dataset(test_data, pre_scan=True, read_only=True)
+            data_available = fetch_dataset(test_data, pre_scan=True, read_only=True)
         else:
-            hashinfo = fetch_dataset(
+            data_available = fetch_dataset(
                 test_data,
                 pre_scan=True,
                 read_only=False,
-                verify=self._verify,
             )
-            if self._verify and not hashinfo:
-                raise RuntimeError(f"Error downloading dataset {test_data}")
-        if hashinfo:
+        if data_available:
             return self._target_dir / test_data
         else:
             return None
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/blend_tutorial.yml` & `dials_data-2.4.9/dials_data/hashinfo/blend_tutorial.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/centroid_test_data.yml` & `dials_data-2.4.9/dials_data/hashinfo/centroid_test_data.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-definition: 8e66d1b7bb3e11584ab1f6a733ce1731f75327a7444c0bf9af4999fb005bdad5
+definition: 96e4c1bc5b82cbde245d588351eeadf928221b176f2d99e198d349260c3466f6
 formatversion: 1
 verify:
 - hash: 99bcabc5a9e2be4c20768b90e0ca16b23c55006fe66e6edc9be5b90f4103947f
   size: 6230086
 - hash: 1e3aeea0286bbc1096e8f916a652d14c33ca441b80d0e89580251bb58592cdf0
   size: 6230072
 - hash: 7a5031aa91a11314484d3c6ba108fb98552b669a187c00c73867d48352dbef25
@@ -23,26 +23,26 @@
   size: 341
 - hash: 54035a1bdbefa154187517579b0a3677ad636d81eb4ac38f942da3ef837728fe
   size: 4214
 - hash: 2355a54805a0f811de496c7a617d35af3493ce8f7a445e457fbd78c760711aa6
   size: 4385
 - hash: f6eae103f308f66472d5450ba10611f7430422f53fab2b36c2b2f68ff1dc20b2
   size: 4340
-- hash: 1a39d8727a343d8c0d59e996bb5c40f0fac6d87dc32e0878e6432ab6bac15419
-  size: 3089
+- hash: e51a2d338c77d5dfe1af878dfd868c2a1a14ee856c44fee6df78dad822ab036d
+  size: 3090
 - hash: ec92eebf953c1777fd3ef97cbd348d0fabbf825a9f55d0bcb4c95f979ac9bb2b
   size: 3095
 - hash: 448eafa25a87025383c80164f75d5e486462e2d9f8c06cc29292f6da6bb7fdb9
   size: 3050
 - hash: d226c6fae636c90eea8a9848d83d2f164c5f5298b9dd797e363660c14fae1be2
   size: 2663
 - hash: 4d783629f802d8c02711430b8f50384d106209603ae39f3f958d011280853619
   size: 5587
-- hash: 2cdbc2e4c62f1aca7dcc38ce7c86e6584b8725a6f42b2af326abd2ee9e8062dd
-  size: 7003
+- hash: 00febb3e97fb2c0c4fbef1b5a0748a6da9bde8b114111c43f05b4b4568f059dd
+  size: 7004
 - hash: 30e47868e6419f60e2efe9f56b29e28ec897ae30e2a77ca0b57a2a7d3d64acc7
   size: 533261
 - hash: 3e21d06a3b3b44c2171742044a558df348ca3663a41728ed69b266902c07fda0
   size: 876304
 - hash: 6c903c079e105b396c40df6344f0eb9ab092e9d7565c164ddda2373ab15b9b9f
   size: 1014845
 - hash: d221ff6103c7030f64cef3b6643350e61a6b865aafcc96158df4433bffb5a780
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/cunir_serial.yml` & `dials_data-2.4.9/dials_data/hashinfo/cunir_serial.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-definition: f345653a884251cf972677e3ca25d852be762aead4f74659e64e5ae3c1cca317
+definition: 5e499205e846d62b787bc8555ba0774f59b368086534be254a493d895a154a30
 formatversion: 1
 verify:
 - hash: 890da105dc7ef00bf59b1095d1f671f0ca3bf1fea8dd3ff369ecb9c424880473
   size: 6230015
 - hash: e385306e000bf7cbb1dd4fb72e2c32f38610bf912aaae8d6c03041bfc184a3a0
   size: 6229987
 - hash: 199f33b106cd30f1ff678ae8c0b90d9938e574cf3bb7e5750f692e05a0ea5373
   size: 6230219
 - hash: e3b84e719d4ae820913e2ad2866790d09090eee9fa4d766390ec93dc79ac195c
   size: 6229967
 - hash: 92d68ed019bc50f9f480d18acf4fe3345f6bd4343674a20f56e41d2bc1b8e71e
   size: 6229971
-- hash: 6e7e4b5baaaac7e4be1955696d5f44e9aa4291a9552b41fd182194d19ec0d4e7
-  size: 634149
-- hash: b47cf43312f14e6ad567fcc5ddca6025bc2abd3a8cb3e8b3f68e84e7b31da2ce
-  size: 8159030
-- hash: 05f32fb3cf10e25ce23fbe746cfdebc6a3733f69c817149a03bfc146beae579d
-  size: 739295
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/fumarase.yml` & `dials_data-2.4.9/dials_data/hashinfo/fumarase.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/image_examples.yml` & `dials_data-2.4.9/dials_data/hashinfo/image_examples.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-definition: d6189969684d3c9c5fa19e51d2962f24c76f487cf3f223f292c9048323ccb90c
+definition: 663d71414bc6007bd36bc9c249d0b5f16c70c0ccd1c3ac1e8bf593e77d8ce176
 formatversion: 1
 verify:
 - hash: 91a7545b2baff2388a80033d88a948d277b913f923a54b7d0c4100df3122fcc2
   size: 583275
 - hash: e8de6706a41c696006eb3c2b1462c4d759ba533f31f4f5f5e99b0210a6d4a2b7
   size: 1689226
 - hash: 92fd3bb5d8cdbe38846783f0e2c9d661c29f63e382078be9c22987871e2b1581
@@ -21,13 +21,11 @@
   size: 5109557
 - hash: 19ccb5770939cdf141ef45f3e2cf002b6ccf61b04b7b848fb46b637b9cec7aff
   size: 452435
 - hash: 05a381daa1fc84efbad630098769a406fbf191abadc57302e01d3b48b04be1f1
   size: 238496
 - hash: fc26cb2308578ed38f38ed00092b3221d55ac44c1b0e90f80ef92eb490b25f45
   size: 9657
-- hash: b0fa7adcdf731a48d6b9897eaf1992af046a3e8769a4be1b291074656215c873
-  size: 55825
 - hash: e913b3141201347962744a9fa27080711db5d76c9b1e254fcfb28b51b6265006
   size: 7751177
 - hash: ebf8470b43774e9be5d215da3944d952a071728ef34cbe5e645deb0f5461a286
   size: 5750322
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/insulin.yml` & `dials_data-2.4.9/dials_data/hashinfo/insulin.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/insulin_processed.yml` & `dials_data-2.4.9/dials_data/hashinfo/insulin_processed.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-definition: 6f8188c95486befbfeaf65c71b5e2c1604eebad929e2c534e7b84d89b6a3218c
+definition: 5ac9b218995d9a84d216fc977ce5e49bf5d2692a2476edbbd3880ed8a6826b51
 formatversion: 1
 verify:
-- hash: a25389d7d1c006a8b2ee3e45fb459d08666fc6e9bedf63dc26fdaec4238abb7c
-  size: 5083
+- hash: 5054edb58f00f0cd7488995f0aa0ccb56173b83f4c2162bd26c7d3f9571cc516
+  size: 5072
 - hash: 6caf12cdf76c49f69d07b25525e3785f88d3dc8cc6430c2e58a8eec749f88274
   size: 22129777
-- hash: bb511704aff8d9a07b88ce12abcf40d8bc8a0df6cb2eedeb5daebc03662a2105
-  size: 8318
+- hash: 34bd9d49a5d49ab84f7035788ec844170efcc7ccebf2d79e7b703387fc781c3f
+  size: 8307
 - hash: 68b4fa52cd71e322e884fea8bab767c94f42cfc740a721c4b097508e01aee869
   size: 25806186
-- hash: 58b7dc99552d7b61e336b7c22776254543a0c368ca00a9a494b50f94913e659f
-  size: 22981
+- hash: d52a91871724a8186b7cbab546be758f92351990a666816f7802b8874b83a0d6
+  size: 22970
 - hash: 7b1c6a3493f4daffca7a6f7b4a277b5e74ad550a88df3f90e8c3bdc3371fb6b7
   size: 19802366
-- hash: a0e5282b0cb5d14e38a96115c729aa9157ff29c3bcb7e5bcda1f8e24b2e3bffe
-  size: 22818
+- hash: 1a817ac9c096e388ba317357d5950cb45d784d31d2fe85b1d9e4603cfcf920d5
+  size: 22807
 - hash: 2aebab9cba3123cb92463106980a7915da8133d15ba21634841142965f8c6430
   size: 25806186
-- hash: e6e1dce6e99d8aa35583df7bc92ab15575efaa209091ebc4b7a759e9402a92bc
-  size: 22405
+- hash: 57dca301ef4449174b6f5301621866b9bb3b9a74edf1a351802ca345cf96a207
+  size: 22394
 - hash: f761340c3235aac6b4fe01eeee0acf0f67dfddb4e0c2da4f7b47f07003f0015c
   size: 22242390
-- hash: fd99a5eece769e359ea6ee11dfb833c3e349b601f84299f02a878b5068251451
-  size: 20393
+- hash: 3ae17d8824e9fe22a1b8ff4aa7e67e19c26c298a194cf5de298b408afcf7d0a0
+  size: 20382
 - hash: 4c7257fc2a1068653d2a28c0d1bbde6ebad273abeaa9a53a9c9f6baaebc81ae1
   size: 19802366
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/isis_sxd_example_data.yml` & `dials_data-2.4.9/dials_data/hashinfo/isis_sxd_example_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml` & `dials_data-2.4.9/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/l_cysteine_dials_output.yml` & `dials_data-2.4.9/dials_data/hashinfo/l_cysteine_dials_output.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/multi_crystal_proteinase_k.yml` & `dials_data-2.4.9/dials_data/hashinfo/multi_crystal_proteinase_k.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-definition: ebaa70558a6018dc224ba9c265bead1e86f1b01c985de9655e24074e6bc8bf3a
+definition: fe7a47df4ee339cffbfe3c2e344979e7028b59dc699af281219f990ce7ad2aee
 formatversion: 1
 verify:
 - hash: 7f220b2145507a6e2b03d76dabe16297d924f16608d2446b06c5ee6ae9ba29df
   size: 9609
 - hash: 3fb3eb622186f232fb01091b194d6c731681a6ce5d082ac07679f86dfcd530a0
   size: 9615
 - hash: ad671ea12a077a91c7e8db2b2c080e4e8572d899ec80944022727fa20b44ac12
@@ -29,9 +29,7 @@
   size: 7244506
 - hash: 153439b19ba61015feb0ee892e40ef1b938d769acc235509c1ac10bff4db69a7
   size: 7268405
 - hash: 5e3abdc61719383bef7b81ba3a310c2512cf0c91e0fa491d29cd2e5b27f1b4cc
   size: 7279269
 - hash: acd9dd5f1efbdf1af37b8db7382cb1649e9e2435d79da41e1f34b968430d9e69
   size: 7413571
-- hash: 3d40dca41340c50abf5ada10923885c259c53238f7d5951609a9bee3cb00d7b1
-  size: 416259
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/quartz_processed.yml` & `dials_data-2.4.9/dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-definition: 75184e1f17b8ca695487ca696925c7e6c95b72bac7068a677e7049646ff540af
+definition: 9d3f23060868d240fd77a432deee0c2dc8943d0e5e69359f3654dd408ece94fc
 formatversion: 1
 verify:
-- hash: 73c763c82bcc36c77f393431819d33a4eff6936819cd73ce68c5c93b5cf03c09
-  size: 351608
-- hash: 6cf1067ec24a5ca61dfa2fcd3cd0dc9c4529bdcf89011a6e46d9be7ee77d8aa4
-  size: 351608
-- hash: 7b8f9bbfd6019f16e4d08f8dfca9674528bfa06a28cfebe972fa90f24ff6aa58
-  size: 6121
-- hash: f029f64f08a718058e5b5f5aa29c0cf5b28549f8085e46b66435c06f0003b319
-  size: 9330
-- hash: 81b9733c29413208cbbcb0092a7c0316da0eb0708d9158044886b12ac15aa6d7
-  size: 831364
-- hash: b4fd266c23a1bb49eefeaae59084e8f8085dcb0aafabecd3362cda11a16ec434
-  size: 40185
-- hash: d25d7033b2b60622b8f34e2ff08592ab1a7a6264b87afd16f82980e303d03065
-  size: 604462
-- hash: 68eae685fa608e0171505f2738b7cd0f6fcbc112b8b928a5aab7c1057481622a
-  size: 1976
-- hash: f8797d3d2517b97627eb468aff8534405e71848dc752c95ac06346ff2d162d22
-  size: 665
-- hash: 7a8ba47d06a5bb2cca8c2324e4796eb0c49f5a156cbd74a03e49e2a1da62276a
-  size: 40025
-- hash: 45b6d035a9264db54353b045aa2d068f15ddc7e8bcf6293a034d46451977c05f
-  size: 831364
-- hash: f18838ded14632f99bf873c1cdcf744aaccd0671eadf00edfcae34ad911e34df
-  size: 6705
-- hash: 3ba9601c2b5f8cc11bce372c45614073f20afd669690a36996803661a4e28b79
-  size: 44105
-- hash: c3ea883ad2f9e3045693ebd9f6ad2d823728c8ad6a1cbcd073ddf1246d7d0eb6
-  size: 657410
-- hash: cf9d34faaaac5c7e90f248f966ff9739c2a4d1e381e82b7c5daa7fd11c39eb1e
-  size: 749779
+- hash: 6a0c13d70642dceb26424428ad1c1b2fa3d2fe6ff44338594f970bdd19af062c
+  size: 227875
+- hash: 9eda0a55c22ae2e05ba8c73b9d4facdc124955b2925b3dd161c498e714405ece
+  size: 227926
+- hash: 0fad3c34fbf7ad255eaadbea13d3bf12ca9b148ab1bb4e346fe27bd58f7206f9
+  size: 227318
+- hash: 0f0f47b0912245cf53854f60a70d5eefcfcd2462968591b806cd0720751383f5
+  size: 226431
+- hash: 7ffddf757a51b132565b77cff1d6c3345e546cdfc27d4d6e2f5afaad45072a25
+  size: 31102343
+- hash: b82589e92620cf86eccd81204301d1f16d12c9bfedeac2e558051a6536e76d13
+  size: 35168264
+- hash: a2d09035e95ac5539f63a5344f8080e33431cad0572920f327c5d3c2d54b5577
+  size: 32762539
+- hash: 33a773026b8b15dedc0cb0a2d4816683b2ee0b1e961a818fa9242dad25cb1dfe
+  size: 36237171
+- hash: b4df1b1f9e5f9cd350ce477f69bd6f1ce60e04d26d2752a241790c8b47f6c90c
+  size: 224950
+- hash: c8b8a39527b1e118527f1a15d418bcd18bbc537756f7e07fb65c1f737e90fb8e
+  size: 224293
+- hash: f10460f28dc66ad6642049e3bc0629276423a7ab188aa478adf4f8977ebbe771
+  size: 224128
+- hash: 1c2305d83d311885c1f08123e77f79added6fe74ade5eea089f2cb12044cd3b9
+  size: 223737
+- hash: 48a6e778791969c959f47b52b494e7f3482f0c6030889513a8ca97f93ed13c6b
+  size: 31042866
+- hash: 3aa016bd9c8a61d7a3f571090b3fb2a9fa5b0349817e14e3a7d7f03d73043157
+  size: 30145577
+- hash: 19b9c4e445cb4200860dea58b3ea8d64b32a3ab551d7442827cb2d3a18afaaec
+  size: 32141508
+- hash: b909a21931ed21e3e9cd6df4df7e2b6869d58ff8c4b8b452e8c17705e52ecb51
+  size: 32101386
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/refinement_test_data.yml` & `dials_data-2.4.9/dials_data/hashinfo/thaumatin_grid_scan.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-definition: 1f3e32bc2394477bda628d454c0774cab1d69f5fcc6663223745c112c240c111
+definition: 6070581bf5292b49640213be6a558688cfaad8a2f001fccb40493b565b287e55
 formatversion: 1
 verify:
-- hash: fb7a0aadc9a48f42dd5a53484d6855ef3d5447c6ac72f7f7ac15820040b12652
-  size: 79530
-- hash: 268200b6cf1b79ae0288033b2aee81af8998bda6a7592a955c56b310fa99b861
-  size: 112384
-- hash: 8526ffd521c01daa8b287fb2d5f8390086e59c4bf019572818944bd4806e424e
-  size: 576207
-- hash: 59dc6d5d7df49ec49e6b65628cbe6346c9bd9c16ccb17297b164d59a731f8157
-  size: 78067
-- hash: 793acb9083b96a96b3e41518abe8b0679669cb08bf79a36e78596d0f59c99bec
-  size: 69417
-- hash: ea35dd2edbe56722c553fb0f4403aaf9135c45f47afb9f579bac848bd5236467
-  size: 42358074
-- hash: 8e488dd947e6c28beb978ddd46c8620abda8fc67e74bb9287861dcc4a4dfdd8d
-  size: 111954
-- hash: 199247aeb958a088cea06c27b10ebb4ab79579efc3ccf0a909396c20eee4be1f
-  size: 264954
-- hash: 87e7a913a76babbb75743d6a1f2588d439be2c865beda70fc58598a9d6d69a9c
-  size: 79214
-- hash: 123c5d48ad5d380281c6c2d250c367871c9b8976777a6f6a3cc5be4dfae357aa
-  size: 661611
-- hash: 7ee8708b301f7bd4dbd71232a8d7653375ce33026826aff725c30115070242c7
-  size: 24013584
-- hash: c5753dc9217fe53c0ba0214d4761e82a778fb0a1053dea4188abd6ece926e1e0
-  size: 19382
-- hash: 0d8ecbd8ca8f3f5a6d8aa2e65fd6ef22a6b422bcdaa103218291bb8e33b22a3e
-  size: 109597
-- hash: 5ec5b42c027476dc2f0fb39aa3fdb5bfeeddaae86ad68eb813f9aec68181c736
-  size: 3988042
-- hash: ac825426d951983a83615f69ab5a5f27d151d492f1cb3a85d009fdcaf0e99e16
-  size: 24482245
-- hash: 6fbf930a63ea1b057be74af575515b4f22b7c39fadc51609cbfc7c671cb8b5b6
-  size: 21969
-- hash: 2ff2b183633fe103743c952e089574d6287b94bd048851d5f9685f97a6f4c427
-  size: 18907
-- hash: f31ebc7c8a6529eff7ad3c10e7b36a37e266c412af9331cefadf57cfc210c5c9
-  size: 6424911
-- hash: 1c79579d42f50829e709480d2a5c4b0f8604408dea5a63134995e5a96b413ad1
-  size: 238547
-- hash: 4adfe355f85ce2863eb02950c6680b59e925d83aef171eadcfb6735ccef24714
-  size: 26867
+- hash: fe922de9eed599135e203bff809a2dccd884fa595ea0a20235e81ca2d036a18f
+  size: 2425760
+- hash: 41dbc17813adf18936eebb6f51b7b3730c67e211d1aaf27d4bd769cc413f9a0d
+  size: 2493611
+- hash: a368f4d400dd8baea31f72e18272f153e7a83e0aa1676814bebef1f72e3891ea
+  size: 2519468
+- hash: f14f17cfc7408aa4ab7c53ebc9724687d44c43962eb141bcd0c0dbd092b32316
+  size: 2495489
+- hash: 6aafc52ce6a19d894622641078cdd8dd70291d7c01ac2e6b9fb9076a84d425bb
+  size: 2496868
+- hash: 5ea943161d69bc27aad1eb904a8e4d76d8488c84e39ecf88a69c58cde48a9535
+  size: 2468552
+- hash: cf83882b0b44e53e5ffdaef805381666b2c32fbe231937bf125c97af866ed077
+  size: 2463110
+- hash: 6621ca6e84a273ea732205700a433320bae616f6283c65045423ea44c9dcc0d5
+  size: 2452807
+- hash: 81550ac1d0ef0f9b24db80695db3c665b27b3a6988b0e9be2b7268b06e292f4d
+  size: 2432769
+- hash: a12ebeac4c2a3b1e8231ba22f20f6e5a54aa98db061dbf00695ba24a05f0be70
+  size: 2424609
+- hash: 643def1ff39603b22ba0ce03af7d5a64d6389584748d122354f9005f86b1ee5c
+  size: 2390677
+- hash: a9b4700173c8bf149468621484437f816cd497c5e03717c14ebf1c73471ec173
+  size: 2378028
+- hash: 75b073686a45154b1a5b04b2c4ff7ca1aca3c3c3e118c0ef3c09fac2c33afc22
+  size: 2263915
+- hash: b98e3f17c73d39deb279d6a9d73d6a9fcaf431e981adba4416ddcda97a1200f0
+  size: 2129350
+- hash: 5e26df239b6508275a2005ef2d76608eb5c7660e89fd7bbfadf7fb75fc430a97
+  size: 1893854
+- hash: e679907995ad2d408e6269d442084c1ce012d20cf3201ddbae1ecea2401d2ed8
+  size: 1817775
+- hash: 4b6478d651642de3403e180dba56d8d8bf2ae1daac7a3cb2af17bf3486f9a225
+  size: 1811719
+- hash: 0816d1dfa73e0a9d5dfc1b8e0e4a4be2be0f6ab433afc1fc4c6472533603e96a
+  size: 1808794
+- hash: 9a34daf2b2c07145c5fd17ef8e318f084df835a75a65f0325b15e77c2e946ac8
+  size: 1808052
```

### Comparing `dials_data-2.4.85/dials_data/hashinfo/small_molecule_example.yml` & `dials_data-2.4.9/dials_data/hashinfo/small_molecule_example.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/thaumatin_i04.yml` & `dials_data-2.4.9/dials_data/hashinfo/thaumatin_i04.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/trypsin_multi_lattice.yml` & `dials_data-2.4.9/dials_data/hashinfo/trypsin_multi_lattice.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/hashinfo/x4wide.yml` & `dials_data-2.4.9/dials_data/hashinfo/x4wide.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/dials_data/pytest11.py` & `dials_data-2.4.9/dials_data/pytest11.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 pytest plugin functions
 """
 
+
 from __future__ import annotations
 
 import pytest
 
 from .download import DataFetcher
```

### Comparing `dials_data-2.4.85/dials_data.egg-info/PKG-INFO` & `dials_data-2.4.9/dials_data.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
-Name: dials_data
-Version: 2.4.85
+Name: dials-data
+Version: 2.4.9
 Summary: DIALS Regression Data Manager
-Author-email: DIALS development team <dials-support@lists.sourceforge.net>
+Home-page: https://github.com/dials/data
+Author: DIALS development team
+Author-email: dials-support@lists.sourceforge.net
 License: BSD 3-Clause License
-Project-URL: Homepage, https://github.com/dials/data
 Project-URL: Bug Tracker, https://github.com/dials/data/issues
 Project-URL: Documentation, https://dials-data.readthedocs.io/
 Project-URL: Source Code, https://github.com/dials/data
 Keywords: dials,dials_data
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: importlib_resources!=6.2,!=6.3.0,!=6.3.1,>=1.1
-Requires-Dist: pytest
-Requires-Dist: pyyaml
-Requires-Dist: requests
 
 =============================
 DIALS Regression Data Manager
 =============================
 
 .. image:: https://img.shields.io/pypi/v/dials_data.svg
         :target: https://pypi.python.org/pypi/dials_data
@@ -65,34 +63,34 @@
 .. image:: https://img.shields.io/pypi/l/dials_data.svg
         :target: https://pypi.python.org/pypi/dials_data
         :alt: BSD license
 
 A python package providing data files used for regression tests in
 DIALS_, dxtbx_, xia2_ and related packages.
 
-If you want to know more about what ``dials-data`` is you can
+If you want to know more about what ``dials_data`` is you can
 have a read through the `background information <https://dials-data.readthedocs.io/en/latest/why.html>`__.
 
 For everything else `the main documentation <https://dials-data.readthedocs.io/>`__ is probably the best start.
 
 
 Installation
 ^^^^^^^^^^^^
 
 To install this package in a normal Python environment, run::
 
-    pip install dials-data
+    pip install dials_data
 
 and then you can use it with::
 
     dials.data
 
 If you are in a conda environment you can instead run::
 
-    conda install -c conda-forge dials-data
+    conda install -c conda-forge dials_data
 
 For more details please take a look at the
 `installation and usage page <https://dials-data.readthedocs.io/en/latest/installation.html>`__.
 
 
 .. _DIALS: https://dials.github.io
 .. _dxtbx: https://github.com/cctbx/cctbx_project/tree/master/dxtbx
@@ -101,18 +99,14 @@
 =======
 History
 =======
 
 2.5 (????-??-??)
 ^^^^^^^^^^^^^^^^
 
-* Fix permission generation when extracting tar archives. Files extracted will be created with
-  default permissions, instead of what has been packed in with the archive. This solves the issue
-  of shared data stores becoming inaccessible to some users.
-* ``DataFetcher``: new parameter verify=True to verify download hashinfo by default.
 
 2.4 (2022-03-07)
 ^^^^^^^^^^^^^^^^
 
 * dials_data no longer uses ``py.path`` internally.
 * dials_data now includes type checking with mypy.
 * We started using the ``requests`` library for faster downloads.
@@ -188,7 +182,9 @@
 * pytest fixture
 
 
 0.1 (2018-11-02)
 ^^^^^^^^^^^^^^^^
 
 * First automatic deployment and release on PyPI
+
+
```

### Comparing `dials_data-2.4.85/dials_data.egg-info/SOURCES.txt` & `dials_data-2.4.9/dials_data.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,85 @@
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
+setup.cfg
+setup.py
 dials_data/__init__.py
 dials_data/cli.py
 dials_data/datasets.py
 dials_data/download.py
-dials_data/py.typed
 dials_data/pytest11.py
 dials_data.egg-info/PKG-INFO
 dials_data.egg-info/SOURCES.txt
 dials_data.egg-info/dependency_links.txt
 dials_data.egg-info/entry_points.txt
 dials_data.egg-info/not-zip-safe
 dials_data.egg-info/requires.txt
 dials_data.egg-info/top_level.txt
-dials_data/definitions/4fluoro_cxi.yml
 dials_data/definitions/MyD88_processed.yml
 dials_data/definitions/aluminium_standard.yml
 dials_data/definitions/blend_tutorial.yml
 dials_data/definitions/centroid_test_data.yml
-dials_data/definitions/cspad_metrology.yml
 dials_data/definitions/cunir_serial.yml
 dials_data/definitions/cunir_serial_processed.yml
-dials_data/definitions/dtpb_serial_processed.yml
 dials_data/definitions/four_circle_eiger.yml
 dials_data/definitions/fumarase.yml
 dials_data/definitions/i19_1_pdteet_index.yml
 dials_data/definitions/image_examples.yml
-dials_data/definitions/indexing_test_data.yml
 dials_data/definitions/insulin.yml
 dials_data/definitions/insulin_processed.yml
 dials_data/definitions/isis_sxd_example_data.yml
-dials_data/definitions/isis_sxd_nacl_processed.yml
-dials_data/definitions/iterative_cspad_refinement.yml
 dials_data/definitions/l_cysteine_4_sweeps_scaled.yml
 dials_data/definitions/l_cysteine_dials_output.yml
 dials_data/definitions/lcls_rayonix_kapton.yml
-dials_data/definitions/lysozyme_JF16M_4img.yml
-dials_data/definitions/lysozyme_JF16M_4img_spectra.yml
 dials_data/definitions/lysozyme_electron_diffraction.yml
 dials_data/definitions/mpro_x0305_processed.yml
 dials_data/definitions/mpro_x0692.yml
 dials_data/definitions/multi_crystal_proteinase_k.yml
-dials_data/definitions/polyhedra_narrow_wedges.yml
 dials_data/definitions/pycbf.yml
 dials_data/definitions/pychef.yml
 dials_data/definitions/quartz_processed.yml
-dials_data/definitions/refinement_test_data.yml
 dials_data/definitions/relion_tutorial_data.yml
-dials_data/definitions/semisynthetic_multilattice.yml
 dials_data/definitions/small_molecule_example.yml
 dials_data/definitions/spring8_ccp4_2018.yml
 dials_data/definitions/thaumatin_eiger_screen.yml
 dials_data/definitions/thaumatin_grid_scan.yml
 dials_data/definitions/thaumatin_i04.yml
 dials_data/definitions/trypsin_multi_lattice.yml
 dials_data/definitions/vmxi_proteinase_k_sweeps.yml
 dials_data/definitions/vmxi_thaumatin.yml
 dials_data/definitions/vmxi_thaumatin_grid_index.yml
 dials_data/definitions/x4wide.yml
 dials_data/definitions/x4wide_processed.yml
-dials_data/hashinfo/4fluoro_cxi.yml
 dials_data/hashinfo/MyD88_processed.yml
 dials_data/hashinfo/aluminium_standard.yml
 dials_data/hashinfo/blend_tutorial.yml
 dials_data/hashinfo/centroid_test_data.yml
-dials_data/hashinfo/cspad_metrology.yml
 dials_data/hashinfo/cunir_serial.yml
 dials_data/hashinfo/cunir_serial_processed.yml
-dials_data/hashinfo/dtpb_serial_processed.yml
 dials_data/hashinfo/four_circle_eiger.yml
 dials_data/hashinfo/fumarase.yml
 dials_data/hashinfo/i19_1_pdteet_index.yml
 dials_data/hashinfo/image_examples.yml
-dials_data/hashinfo/indexing_test_data.yml
 dials_data/hashinfo/insulin.yml
 dials_data/hashinfo/insulin_processed.yml
 dials_data/hashinfo/isis_sxd_example_data.yml
-dials_data/hashinfo/iterative_cspad_refinement.yml
 dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml
 dials_data/hashinfo/l_cysteine_dials_output.yml
 dials_data/hashinfo/lcls_rayonix_kapton.yml
-dials_data/hashinfo/lysozyme_JF16M_4img.yml
-dials_data/hashinfo/lysozyme_JF16M_4img_spectra.yml
 dials_data/hashinfo/lysozyme_electron_diffraction.yml
 dials_data/hashinfo/mpro_x0305_processed.yml
 dials_data/hashinfo/mpro_x0692.yml
 dials_data/hashinfo/multi_crystal_proteinase_k.yml
-dials_data/hashinfo/polyhedra_narrow_wedges.yml
 dials_data/hashinfo/pycbf.yml
 dials_data/hashinfo/pychef.yml
-dials_data/hashinfo/quartz_processed.yml
-dials_data/hashinfo/refinement_test_data.yml
 dials_data/hashinfo/relion_tutorial_data.yml
-dials_data/hashinfo/semisynthetic_multilattice.yml
 dials_data/hashinfo/small_molecule_example.yml
 dials_data/hashinfo/spring8_ccp4_2018.yml
 dials_data/hashinfo/thaumatin_eiger_screen.yml
 dials_data/hashinfo/thaumatin_grid_scan.yml
 dials_data/hashinfo/thaumatin_i04.yml
 dials_data/hashinfo/trypsin_multi_lattice.yml
 dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml
```

### Comparing `dials_data-2.4.85/docs/conf.py` & `dials_data-2.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/docs/index.rst` & `dials_data-2.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.85/docs/installation.rst` & `dials_data-2.4.9/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 .. highlight:: shell
 
 ======================
 Installation and Usage
 ======================
 
-There are a number of possible ways to install ``dials-data``.
+There are a number of possible ways to install ``dials_data``.
 From the simplest to the most involved these are:
 
 
 As an end user
 ^^^^^^^^^^^^^^
 
-Quite simply: You do not need to install ``dials-data``.
+Quite simply: You do not need to install ``dials_data``.
 It does not add any functionality to end users.
 
 
-As a developer to run tests with ``dials-data``
+As a developer to run tests with ``dials_data``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-You may want to install ``dials-data`` so that you can run regression tests locally.
+You may want to install ``dials_data`` so that you can run regression tests locally.
 Or you might say that continuous integration should take care of this.
 Both are valid opinions.
 
 .. _basic-installation:
 
-However you do not need to install ``dials-data`` from source. You can simply run::
+However you do not need to install ``dials_data`` from source. You can simply run::
 
     pip install -U dials-data
 
 or, in a conda environment::
 
     conda install -c conda-forge dials-data
 
-This will install or update an existing installation of ``dials-data``.
+This will install or update an existing installation of ``dials_data``.
 
 You can then run your tests as usual using::
 
     pytest
 
 although, depending on the configuration of the code under test, you
 probably need to run it as::
 
     pytest --regression
 
-to actually enable those tests depending on files from ``dials-data``.
+to actually enable those tests depending on files from ``dials_data``.
 
 
-As a developer to write tests with ``dials-data``
+As a developer to write tests with ``dials_data``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Install ``dials-data`` as above.
+Install ``dials_data`` as above.
 
 If your test is written in pytest and you use the fixture provided by
-``dials-data`` then you can use regression datasets in your test by
+``dials_data`` then you can use regression datasets in your test by
 adding the ``dials_data`` fixture to your test, ie:
 
 .. code-block:: python
 
     def test_accessing_a_dataset(dials_data):
         location = dials_data("x4wide", pathlib=True)
 
@@ -85,64 +85,64 @@
 
     dials.data list
 
 or by going through the
 `dataset definition files in the repository <https://github.com/dials/data/tree/master/dials_data/definitions>`__.
 
 If you want the tests on your project to be runnable even when
-``dials-data`` is not installed in the environment you could add a
+``dials_data`` is not installed in the environment you could add a
 dummy fixture to your ``conftest.py``, for example:
 
 .. code-block:: python
 
     import pytest
     try:
         import dials_data as _  # noqa: F401
     except ModuleNotFoundError:
         @pytest.fixture(scope="session")
         def dials_data():
             pytest.skip("Test requires python package dials_data")
 
 
-As a developer who wants to add files to ``dials-data``
+As a developer who wants to add files to ``dials_data``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Follow the steps in :doc:`/contributing` to install ``dials-data`` into a
+Follow the steps in :doc:`/contributing` to install ``dials_data`` into a
 virtual environment.
 
-You can install ``dials-data`` using ``pip`` as above *unless* you want to
+You can install ``dials_data`` using ``pip`` as above *unless* you want to
 immediately use your dataset definition in tests without waiting for your
 pull request to be accepted. In this case you can follow the instructions
 in the next step.
 
 
-As a developer who wants to extend ``dials-data``
+As a developer who wants to extend ``dials_data``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Have a look at the :doc:`/contributing` page.
 
-Install your own fork of ``dials-data`` by running::
+Install your own fork of ``dials_data`` by running::
 
     pip install -e path/to/fork
 
 in a cctbx/DIALS environment use ``libtbx.pip`` respectively, followed by
 a round of ``libtbx.configure`` or ``make reconf``.
 
 If you made substantial changes or updated your source copy you may also
 have to run::
 
     python setup.py develop
 
 This will update your python package index and install/update any
-``dials-data`` dependencies if necessary.
+``dials_data`` dependencies if necessary.
 
 To switch back from using your checked out version to the 'official'
-version of ``dials-data`` you can uninstall it with::
+version of ``dials_data`` you can uninstall it with::
 
-    pip uninstall dials-data
+    pip uninstall dials_data
 
 and then reinstall it following the
 `instructions at the top of this page <basic-installation_>`__.
 
 
 Where are the regression datasets stored?
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
@@ -153,8 +153,8 @@
   created then use that location.
 * If the file path ``/dls/science/groups/scisoft/DIALS/dials_data`` exists and is readable then
   use this location. This is a shared directory specific to Diamond Light Source.
 * If the environment variable ``LIBTBX_BUILD`` is set and the directory
   ``dials_data`` exists or can be created underneath that location then
   use that.
 * Use ``~/.cache/dials_data`` if it exists or can be created.
-* Otherwise ``dials-data`` will fail with a RuntimeError.
+* Otherwise ``dials_data`` will fail with a RuntimeError.
```

### Comparing `dials_data-2.4.85/docs/why.rst` & `dials_data-2.4.9/docs/why.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ======================
-What is ``dials-data``
+What is ``dials_data``
 ======================
 
-``dials-data`` is a lightweight, simple python(-only) package.
+``dials_data`` is a lightweight, simple python(-only) package.
 It is used to provide access to data files used in regression tests,
 but does not contain any of those data files itself.
 
 Although we envisage it mostly being used in a cctbx_\ /\ DIALS_
 environment for tests in DIALS_, dxtbx_, xia2_ and related packages,
 it has no dependencies on either cctbx_ or DIALS_, in fact
 all dependencies are explicitly declared in the setup.py_ file and are
 installable via standard setuptools/pip methods.
-This means ``dials-data`` can easily be used in other projects accessing
+This means ``dials_data`` can easily be used in other projects accessing
 the same data, and can be used in temporary environments such as
 Travis containers.
 
 But - why?
 ==========
 
 In the past DIALS_ tests used an internal SVN repository called
@@ -48,17 +48,17 @@
 With dxtbx_, dials_ and xia2_ moving to pytest_ we extended the
 xia2_regression_ concept into the regression_data_ fixture to provide
 a simple way to access the datasets in tests, but the data still
 needed downloading separately and could not easily be used outside
 of the dials_ repository and not at all outside of a dials_
 distribution. Adding data files was still a very involved process.
 
-``dials-data`` is the next iteration of our solution to this problem.
+``dials_data`` is the next iteration of our solution to this problem.
 
-What can ``dials-data`` do
+What can ``dials_data`` do
 ==========================
 
 The entire pipeline, from adding new data files, to the automatic
 download, storage, preparation, verification and provisioning of the
 files to tests happens in a single, independent Python package.
 
 Data files are versioned without being kept in an SVN or git
```

### Comparing `dials_data-2.4.85/tests/test_dials_data.py` & `dials_data-2.4.9/tests/test_dials_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,17 +40,15 @@
     fetcher.return_value = True
 
     df = dials_data.download.DataFetcher(read_only=True)
     with pytest.warns(DeprecationWarning):
         ds = df("dataset")
     assert pathlib.Path(ds).resolve() == pathlib.Path("/tmp/root/dataset").resolve()
     assert isinstance(ds, py.path.local)
-    fetcher.assert_called_once_with(
-        "dataset", pre_scan=True, read_only=False, verify=True
-    )
+    fetcher.assert_called_once_with("dataset", pre_scan=True, read_only=False)
 
     ds = df("dataset", pathlib=False)
     assert pathlib.Path(ds).resolve() == pathlib.Path("/tmp/root/dataset").resolve()
     assert isinstance(ds, py.path.local)
     fetcher.assert_called_once()
 
 
@@ -62,20 +60,16 @@
     fetcher.return_value = True
 
     df = dials_data.download.DataFetcher(read_only=True)
     ds = df("dataset", pathlib=True)
     assert ds == test_path / "dataset"
 
     assert isinstance(ds, pathlib.Path)
-    fetcher.assert_called_once_with(
-        "dataset", pre_scan=True, read_only=False, verify=True
-    )
+    fetcher.assert_called_once_with("dataset", pre_scan=True, read_only=False)
 
     with pytest.warns(DeprecationWarning):
         ds = df("dataset")
     assert pathlib.Path(ds).resolve() == test_path.joinpath("dataset").resolve()
     assert not isinstance(
         ds, pathlib.Path
     )  # default is currently to return py.path.local()
-    fetcher.assert_called_once_with(
-        "dataset", pre_scan=True, read_only=False, verify=True
-    )
+    fetcher.assert_called_once_with("dataset", pre_scan=True, read_only=False)
```

### Comparing `dials_data-2.4.85/tests/test_yaml_files.py` & `dials_data-2.4.9/tests/test_yaml_files.py`

 * *Files identical despite different names*

