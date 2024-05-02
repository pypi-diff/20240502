# Comparing `tmp/xsuite-0.6.0.tar.gz` & `tmp/xsuite-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsuite-0.6.0.tar", last modified: Mon Jan 22 16:51:12 2024, max compression
+gzip compressed data, was "xsuite-0.7.1.tar", last modified: Thu May  2 13:50:38 2024, max compression
```

## Comparing `xsuite-0.6.0.tar` & `xsuite-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,158 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-01-22 16:51:12.466849 xsuite-0.6.0/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:50.000000 xsuite-0.6.0/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      106 2023-03-23 11:04:50.000000 xsuite-0.6.0/MANIFEST.in
--rw-r--r--   0 giadarol   (503) staff       (20)      526 2024-01-22 16:51:12.466684 xsuite-0.6.0/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      746 2023-11-24 19:44:17.000000 xsuite-0.6.0/README.md
--rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:04:50.000000 xsuite-0.6.0/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2024-01-22 16:51:12.466899 xsuite-0.6.0/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1286 2023-03-23 11:04:50.000000 xsuite-0.6.0/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-01-22 16:51:12.462614 xsuite-0.6.0/xsuite/
--rw-r--r--   0 giadarol   (503) staff       (20)       34 2023-03-23 11:04:50.000000 xsuite-0.6.0/xsuite/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2024-01-22 16:50:52.000000 xsuite-0.6.0/xsuite/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      742 2023-03-23 11:04:50.000000 xsuite-0.6.0/xsuite/cli.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-01-22 16:51:12.466432 xsuite-0.6.0/xsuite.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      526 2024-01-22 16:51:12.000000 xsuite-0.6.0/xsuite.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      287 2024-01-22 16:51:12.000000 xsuite-0.6.0/xsuite.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2024-01-22 16:51:12.000000 xsuite-0.6.0/xsuite.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       52 2024-01-22 16:51:12.000000 xsuite-0.6.0/xsuite.egg-info/entry_points.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       47 2024-01-22 16:51:12.000000 xsuite-0.6.0/xsuite.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        7 2024-01-22 16:51:12.000000 xsuite-0.6.0/xsuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.704612 xsuite-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.668613 xsuite-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.672613 xsuite-0.7.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/scripts/install_branches.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/scripts/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.676612 xsuite-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/cron_test_gh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/cron_test_gh_omp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/cron_test_gpu_cl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/cron_test_gpu_cuda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/cron_test_sh_cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/manual_test_gh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/manual_test_sh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/test_gh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-02 13:50:10.000000 xsuite-0.7.1/.github/workflows/test_sh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-02 13:50:10.000000 xsuite-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-02 13:50:10.000000 xsuite-0.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-02 13:50:10.000000 xsuite-0.7.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-02 13:50:10.000000 xsuite-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 13:50:10.000000 xsuite-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-02 13:50:38.704612 xsuite-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 13:50:10.000000 xsuite-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 13:50:10.000000 xsuite-0.7.1/contributors.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.684613 xsuite-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/acceleration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/apireference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/autogeneration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/beambeam.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/collective.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/collective_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/collimation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/combined_cpu_gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/dev_guide_xtbe_data_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/dev_guide_xtbe_internal_record.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/dev_guide_xtbe_lost_part_codes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/dev_guide_xtbe_tracking_code.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/dev_guide_xtrack_beam_elements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/dynamic_aperture.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/exciter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/fast_lattice_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.692613 xsuite-0.7.1/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   296224 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/acceleration.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38807 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/beambeam_sigmapi.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/beambeamkick.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108018 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/crossing_bump.png
+-rw-r--r--   0 runner    (1001) docker     (127)   395863 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/dynamic_aperture.png
+-rw-r--r--   0 runner    (1001) docker     (127)   201057 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/elena_w_chrom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76009 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/exciter_signals.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64395 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/footprint_HO2D.png
+-rw-r--r--   0 runner    (1001) docker     (127)   140959 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/footprint_bb_no_rescale.png
+-rw-r--r--   0 runner    (1001) docker     (127)   128051 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/footprint_bb_with_rescale.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143371 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/footprint_polar.png
+-rw-r--r--   0 runner    (1001) docker     (127)   179030 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/footprint_unif_action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   179734 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/gaussian.png
+-rw-r--r--   0 runner    (1001) docker     (127)   121485 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/halo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   465172 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/loss_location_refinement.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70669 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/orbit_bump.png
+-rw-r--r--   0 runner    (1001) docker     (127)   203281 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67404 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/phasespacedistortion.png
+-rw-r--r--   0 runner    (1001) docker     (127)   206008 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/radial_steering.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38610 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/stabilitydiagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112097 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/time_dep_knob_pwlin_tracking.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153741 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/time_dep_knob_pwlin_twiss.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109560 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/time_dep_knob_sin_pulse_tracking.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123326 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/time_dep_knob_sin_tracking.png
+-rw-r--r--   0 runner    (1001) docker     (127)   130156 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/time_dep_knob_sin_twiss.png
+-rw-r--r--   0 runner    (1001) docker     (127)   140876 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/twiss.png
+-rw-r--r--   0 runner    (1001) docker     (127)   183220 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/twiss_beam_sizes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88689 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/twiss_periodic.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136677 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/twiss_range.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77880 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/twiss_reverse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67165 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/twiss_vs_delta.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88492 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/figures/xsuite_logo_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/footprint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/freeze_longitudinal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/full_table_of_contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.692613 xsuite-0.7.1/docs/generated_code_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/generated_code_snippets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/intrabeam_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/jupyter_tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/match.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/method_4d.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/numericalreproducibility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/optimize_for_tracking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/particles_monitor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/particlesmanip.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.696612 xsuite-0.7.1/docs/physics_manual/
+-rw-r--r--   0 runner    (1001) docker     (127)    56659 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/bb6d.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/bbconfig.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/bibliography.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.700612 xsuite-0.7.1/docs/physics_manual/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   310545 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/figures/b1ip1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   298299 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/figures/b1ip5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   306208 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/figures/b4ip1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   303009 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/figures/b4ip5.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62776 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/figures/bhabha_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/figures/bs_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   234007 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/figures/xang_xplane.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1450972 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/physics_man.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/physics_man.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    72587 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/xfields.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    97215 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physics_manual/xtrack.tex
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/physicsguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/pyhtinterface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/singlepart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/spacechargeauto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/synchrotron_radiation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/tapering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/time_dependent_knobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/track.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/twiss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/usersguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/v020changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/xmask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/xobjexample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16685 2024-05-02 13:50:10.000000 xsuite-0.7.1/docs/xsuite_data_management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-02 13:50:10.000000 xsuite-0.7.1/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-02 13:50:10.000000 xsuite-0.7.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1418 2024-05-02 13:50:10.000000 xsuite-0.7.1/release.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 13:50:10.000000 xsuite-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-02 13:50:10.000000 xsuite-0.7.1/run_on_gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-02 13:50:10.000000 xsuite-0.7.1/run_release_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:50:38.704612 xsuite-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-02 13:50:10.000000 xsuite-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.700612 xsuite-0.7.1/xsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.704612 xsuite-0.7.1/xsuite/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/__pycache__/kernel_definitions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/__pycache__/prebuild_kernels.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/kernel_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.704612 xsuite-0.7.1/xsuite/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-02 13:50:10.000000 xsuite-0.7.1/xsuite/prebuild_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:38.704612 xsuite-0.7.1/xsuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-02 13:50:38.000000 xsuite-0.7.1/xsuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-02 13:50:38.000000 xsuite-0.7.1/xsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:50:38.000000 xsuite-0.7.1/xsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 13:50:38.000000 xsuite-0.7.1/xsuite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 13:50:38.000000 xsuite-0.7.1/xsuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:50:38.000000 xsuite-0.7.1/xsuite.egg-info/top_level.txt
```

### Comparing `xsuite-0.6.0/LICENSE` & `xsuite-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xsuite-0.6.0/README.md` & `xsuite-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# Xsuite 
-
+# Xsuite
 
 [![Daily test (self-hosted, CUDA)](https://github.com/xsuite/xsuite/actions/workflows/cron_test_gpu_cuda.yaml/badge.svg)](https://github.com/xsuite/xsuite/actions/workflows/cron_test_gpu_cuda.yaml)
 [![Daily test (self-hosted, OpenCL)](https://github.com/xsuite/xsuite/actions/workflows/cron_test_gpu_cl.yaml/badge.svg)](https://github.com/xsuite/xsuite/actions/workflows/cron_test_gpu_cl.yaml)
 [![Daily test (self-hosted, CPU)](https://github.com/xsuite/xsuite/actions/workflows/cron_test_sh_cpu.yaml/badge.svg)](https://github.com/xsuite/xsuite/actions/workflows/cron_test_sh_cpu.yaml)
 
 Suite of python packages for multiparticle simulations for particle accelerators.
 
-Documentation is on: https://xsuite.readthedocs.io/en/latest/.
+Documentation is on: <https://xsuite.readthedocs.io/en/latest/>.
```

