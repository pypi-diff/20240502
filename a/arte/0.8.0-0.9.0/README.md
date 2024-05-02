# Comparing `tmp/arte-0.8.0.tar.gz` & `tmp/arte-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arte-0.8.0.tar", last modified: Thu Sep 21 11:06:06 2023, max compression
+gzip compressed data, was "arte-0.9.0.tar", last modified: Sun Feb 11 23:25:23 2024, max compression
```

## Comparing `arte-0.8.0.tar` & `arte-0.9.0.tar`

### file list

```diff
@@ -1,116 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.053238 arte-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-09-21 11:05:47.000000 arte-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-09-21 11:06:06.053238 arte-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2023-09-21 11:05:47.000000 arte-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.037238 arte-0.8.0/arte/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-21 11:05:47.000000 arte-0.8.0/arte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-21 11:05:47.000000 arte-0.8.0/arte/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.041238 arte-0.8.0/arte/atmo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 11:05:47.000000 arte-0.8.0/arte/atmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18520 2023-09-21 11:05:47.000000 arte-0.8.0/arte/atmo/cn2_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2023-09-21 11:05:47.000000 arte-0.8.0/arte/atmo/phase_screen_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-09-21 11:05:47.000000 arte-0.8.0/arte/atmo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32871 2023-09-21 11:05:47.000000 arte-0.8.0/arte/atmo/von_karman_covariance_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2023-09-21 11:05:47.000000 arte-0.8.0/arte/atmo/von_karman_psd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-09-21 11:05:47.000000 arte-0.8.0/arte/atmo/von_karman_spatial_covariance_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2023-09-21 11:05:47.000000 arte-0.8.0/arte/code_convention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.041238 arte-0.8.0/arte/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/chunk_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/if_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/interpolated_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-09-21 11:05:47.000000 arte-0.8.0/arte/contrib/yes_no.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.041238 arte-0.8.0/arte/control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 11:05:47.000000 arte-0.8.0/arte/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2023-09-21 11:05:47.000000 arte-0.8.0/arte/control/transfer_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.041238 arte-0.8.0/arte/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 11:05:47.000000 arte-0.8.0/arte/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-09-21 11:05:47.000000 arte-0.8.0/arte/math/factors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2023-09-21 11:05:47.000000 arte-0.8.0/arte/math/make_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-09-21 11:05:47.000000 arte-0.8.0/arte/math/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-09-21 11:05:47.000000 arte-0.8.0/arte/math/toccd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.041238 arte-0.8.0/arte/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 11:05:47.000000 arte-0.8.0/arte/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9778 2023-09-21 11:05:47.000000 arte-0.8.0/arte/misc/fourier_adaptive_optics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.045238 arte-0.8.0/arte/photometry/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/eso_sky_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/mag_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45298 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/morfeo_transmissive_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)    10318 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/n_phot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/normalized_star_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/spectral_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/thermal_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/transmissive_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    53838 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/transmissive_elements_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2023-09-21 11:05:47.000000 arte-0.8.0/arte/photometry/transmittance_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2023-09-21 11:05:47.000000 arte-0.8.0/arte/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2023-09-21 11:05:47.000000 arte-0.8.0/arte/sandbox_noise_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.045238 arte-0.8.0/arte/time_series/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-09-21 11:05:47.000000 arte-0.8.0/arte/time_series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-09-21 11:05:47.000000 arte-0.8.0/arte/time_series/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2023-09-21 11:05:47.000000 arte-0.8.0/arte/time_series/multi_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2023-09-21 11:05:47.000000 arte-0.8.0/arte/time_series/time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.045238 arte-0.8.0/arte/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/aperture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/domainxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/fisba_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/guide_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/scalar_bidimensional_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/slopes.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/wavefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-09-21 11:05:47.000000 arte-0.8.0/arte/types/zernike_coefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.049238 arte-0.8.0/arte/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/capture_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/circular_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/circular_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/compareIDL.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/discrete_fourier_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12386 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/footprint_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/generalized_fitting_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/image_moments.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/locate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/marechal.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/modal_decomposer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/multiton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/noise_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/not_available.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/package_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/quadratic_sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/radial_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/rebin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/shape_fitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/shared_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/tabular_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/timekeepers.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/unit_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13085 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/zernike_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2023-09-21 11:05:47.000000 arte-0.8.0/arte/utils/zernike_projection_on_subaperture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.041238 arte-0.8.0/arte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-09-21 11:06:06.000000 arte-0.8.0/arte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2023-09-21 11:06:06.000000 arte-0.8.0/arte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 11:06:06.000000 arte-0.8.0/arte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-09-21 11:06:06.000000 arte-0.8.0/arte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-21 11:06:06.000000 arte-0.8.0/arte.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-21 11:06:06.053238 arte-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2023-09-21 11:05:47.000000 arte-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 11:06:06.049238 arte-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2023-09-21 11:05:47.000000 arte-0.8.0/test/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.579021 arte-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-11 23:25:14.000000 arte-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-02-11 23:25:23.579021 arte-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-11 23:25:14.000000 arte-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.563021 arte-0.9.0/arte/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 23:25:14.000000 arte-0.9.0/arte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-11 23:25:14.000000 arte-0.9.0/arte/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.563021 arte-0.9.0/arte/atmo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:14.000000 arte-0.9.0/arte/atmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-02-11 23:25:14.000000 arte-0.9.0/arte/atmo/cn2_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-02-11 23:25:14.000000 arte-0.9.0/arte/atmo/phase_screen_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-11 23:25:14.000000 arte-0.9.0/arte/atmo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32871 2024-02-11 23:25:14.000000 arte-0.9.0/arte/atmo/von_karman_covariance_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-02-11 23:25:14.000000 arte-0.9.0/arte/atmo/von_karman_psd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-02-11 23:25:14.000000 arte-0.9.0/arte/atmo/von_karman_spatial_covariance_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-11 23:25:14.000000 arte-0.9.0/arte/code_convention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.567021 arte-0.9.0/arte/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/chunk_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/if_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/interpolated_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-11 23:25:14.000000 arte-0.9.0/arte/contrib/yes_no.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.567021 arte-0.9.0/arte/control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:14.000000 arte-0.9.0/arte/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-02-11 23:25:14.000000 arte-0.9.0/arte/control/transfer_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.567021 arte-0.9.0/arte/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:14.000000 arte-0.9.0/arte/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-11 23:25:14.000000 arte-0.9.0/arte/math/factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-02-11 23:25:14.000000 arte-0.9.0/arte/math/make_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-11 23:25:14.000000 arte-0.9.0/arte/math/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-11 23:25:14.000000 arte-0.9.0/arte/math/toccd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.567021 arte-0.9.0/arte/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:14.000000 arte-0.9.0/arte/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-02-11 23:25:14.000000 arte-0.9.0/arte/misc/fourier_adaptive_optics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.567021 arte-0.9.0/arte/photometry/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/eso_sky_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/mag_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/n_phot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/normalized_star_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/spectral_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/transmissive_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15892 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/transmissive_elements_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-11 23:25:14.000000 arte-0.9.0/arte/photometry/transmittance_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-02-11 23:25:14.000000 arte-0.9.0/arte/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-02-11 23:25:14.000000 arte-0.9.0/arte/sandbox_noise_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.571021 arte-0.9.0/arte/time_series/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-11 23:25:14.000000 arte-0.9.0/arte/time_series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-02-11 23:25:14.000000 arte-0.9.0/arte/time_series/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-02-11 23:25:14.000000 arte-0.9.0/arte/time_series/multi_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-02-11 23:25:14.000000 arte-0.9.0/arte/time_series/time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.571021 arte-0.9.0/arte/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/domainxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/fisba_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/guide_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/scalar_bidimensional_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/slopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/wavefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-11 23:25:14.000000 arte-0.9.0/arte/types/zernike_coefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.579021 arte-0.9.0/arte/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/capture_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/circular_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/circular_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/compareIDL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/discrete_fourier_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/footprint_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/generalized_fitting_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/image_moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/locate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/marechal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/modal_decomposer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/multiton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/noise_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/not_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/quadratic_sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/radial_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/rebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/shape_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/shared_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/tabular_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/timekeepers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/unit_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/zernike_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-02-11 23:25:14.000000 arte-0.9.0/arte/utils/zernike_projection_on_subaperture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.579021 arte-0.9.0/arte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-02-11 23:25:23.000000 arte-0.9.0/arte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-02-11 23:25:23.000000 arte-0.9.0/arte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 23:25:23.000000 arte-0.9.0/arte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-11 23:25:23.000000 arte-0.9.0/arte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-11 23:25:23.000000 arte-0.9.0/arte.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 23:25:23.579021 arte-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-11 23:25:14.000000 arte-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 23:25:23.579021 arte-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-02-11 23:25:14.000000 arte-0.9.0/test/test_helper.py
```

### Comparing `arte-0.8.0/LICENSE` & `arte-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/PKG-INFO` & `arte-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arte
-Version: 0.8.0
+Version: 0.9.0
 Summary: Arcetri Random sTuff collEction
 Home-page: https://github.com/ArcetriAdaptiveOptics/arte
 Author: Lorenzo Busoni, Alfio Puglisi, INAF Arcetri Adaptive Optics group
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: Adaptive Optics, Astrophysics, INAF, Arcetri
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Requires-Dist: astropy
 Requires-Dist: synphot
 Requires-Dist: pytest
 Requires-Dist: skycalc-cli
 Requires-Dist: scikit-image>=0.17
 Requires-Dist: scipy
 Requires-Dist: mpmath
+Requires-Dist: requests
 
 # arte: Arcetri Random sTuff collEction
 
 A collection of routines and utilities
 developed by the Arcetri Astrophysical Observatory's AO group.
 
 ## Documentation
```

### Comparing `arte-0.8.0/README.md` & `arte-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/atmo/cn2_profile.py` & `arte-0.9.0/arte/atmo/cn2_profile.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/atmo/phase_screen_generator.py` & `arte-0.9.0/arte/atmo/phase_screen_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from arte.utils.discrete_fourier_transform \
     import BidimensionalFourierTransform as bfft
 
+from astropy.io import fits
 
 class PhaseScreenGenerator(object):
 
     def __init__(self,
                  screenSizeInPixels,
                  screenSizeInMeters,
                  outerScaleInMeters,
@@ -99,7 +100,36 @@
                         modul[ix, jx] * (sh - sh0)
         lowFreqScreen *= np.sqrt(0.0228) * self._screenSzInPx**(5. / 6)
         return lowFreqScreen
 
     def _determineNumberOfSubHarmonics(self):
         maxNoOfSubHarm = 8
         pass
+    
+    def save_normalized_phase_screens(self, fname):
+        hdr = fits.Header()
+        hdr['SZ_IN_PX'] =  self._screenSzInPx
+        hdr['SZ_IN_M'] = self._screenSzInM
+        hdr['OS_IN_M'] = self._outerScaleInM
+        hdr['SEED'] = self._seed
+        
+        fits.writeto(fname, self._phaseScreens, hdr)
+        
+    
+    @staticmethod 
+    def load_normalized_phase_screens(fname):
+        header = fits.getheader(fname)
+        screenSizeInPixels = header['SZ_IN_PX'] 
+        screenSizeInMeters = header['SZ_IN_M'] 
+        outerScaleInMeters = header['OS_IN_M'] 
+        seed = header['SEED'] 
+        
+        psg = PhaseScreenGenerator(
+            screenSizeInPixels,
+            screenSizeInMeters,
+            outerScaleInMeters,
+            seed)
+        
+        hduList = fits.open(fname)
+        psg._phaseScreens = hduList[0].data
+        
+        return psg
```

### Comparing `arte-0.8.0/arte/atmo/von_karman_covariance_calculator.py` & `arte-0.9.0/arte/atmo/von_karman_covariance_calculator.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/atmo/von_karman_psd.py` & `arte-0.9.0/arte/atmo/von_karman_psd.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/atmo/von_karman_spatial_covariance_calculator.py` & `arte-0.9.0/arte/atmo/von_karman_spatial_covariance_calculator.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/code_convention.py` & `arte-0.9.0/arte/code_convention.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/contrib/chunk_iterator.py` & `arte-0.9.0/arte/contrib/chunk_iterator.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/contrib/daemonize.py` & `arte-0.9.0/arte/contrib/daemonize.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/contrib/debug.py` & `arte-0.9.0/arte/contrib/debug.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/contrib/if_.py` & `arte-0.9.0/arte/contrib/if_.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/contrib/interpolated_array.py` & `arte-0.9.0/arte/contrib/interpolated_array.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/contrib/timer.py` & `arte-0.9.0/arte/contrib/timer.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/contrib/yes_no.py` & `arte-0.9.0/arte/contrib/yes_no.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/control/transfer_function.py` & `arte-0.9.0/arte/control/transfer_function.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/math/make_xy.py` & `arte-0.9.0/arte/math/make_xy.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/math/masks.py` & `arte-0.9.0/arte/math/masks.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/math/toccd.py` & `arte-0.9.0/arte/math/toccd.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/misc/fourier_adaptive_optics.py` & `arte-0.9.0/arte/misc/fourier_adaptive_optics.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/photometry/eso_sky_calc.py` & `arte-0.9.0/arte/photometry/eso_sky_calc.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/photometry/filters.py` & `arte-0.9.0/arte/photometry/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import os
 from synphot.spectrum import SpectralElement
 from astropy import units as u
 
 
 class Filters(object):
 
-    BESSEL_J = 'bessel_j'
-    BESSEL_H = 'bessel_h'
-    BESSEL_K = 'bessel_k'
-    COUSIN_R = 'cousin_r'
-    COUSIN_I = 'cousin_i'
+    BESSELL_J = 'bessel_j'
+    BESSELL_H = 'bessel_h'
+    BESSELL_K = 'bessel_k'
+    BESSELL90_R = 'bessell90_r'
+    BESSELL90_I = 'bessell90_i'
+    COUSINS_R = 'cousins_r'
+    COUSINS_I = 'cousins_i'
     JOHNSON_U = 'johnson_u'
     JOHNSON_B = 'johnson_b'
     JOHNSON_V = 'johnson_v'
     JOHNSON_R = 'johnson_r'
     JOHNSON_I = 'johnson_i'
     JOHNSON_J = 'johnson_j'
     JOHNSON_K = 'johnson_k'
@@ -31,21 +33,20 @@
     ESO_ETC_L = 'eso_etc_l'
     ESO_ETC_M = 'eso_etc_m'
     ESO_ETC_N = 'eso_etc_n'
     ESO_ETC_Q = 'eso_etc_q'
     C_RED_ONE = 'c_red_one'
     CCD_220 = 'ccd_220'
 
-
     SYNPHOT = [
-        BESSEL_J,
-        BESSEL_H,
-        BESSEL_K,
-        COUSIN_R,
-        COUSIN_I,
+        BESSELL_J,
+        BESSELL_H,
+        BESSELL_K,
+        COUSINS_R,
+        COUSINS_I,
         JOHNSON_U,
         JOHNSON_B,
         JOHNSON_V,
         JOHNSON_R,
         JOHNSON_I,
         JOHNSON_J,
         JOHNSON_K
@@ -64,15 +65,20 @@
         ESO_ETC_K,
         ESO_ETC_L,
         ESO_ETC_M,
         ESO_ETC_N,
         ESO_ETC_Q
     ]
 
-    ALL = SYNPHOT+ESO_ETC
+    BESSELL90 = [
+        BESSELL90_R,
+        BESSELL90_I
+    ]
+
+    ALL = SYNPHOT + ESO_ETC + BESSELL90
 
     @classmethod
     def names(cls):
         return cls.ALL
 
     @classmethod
     def get(cls, filter_name):
@@ -89,14 +95,20 @@
     @staticmethod
     def _EsoEtcFiltersFolder():
         rootDir = dataRootDir()
         dirname = os.path.join(rootDir, 'photometry', 'filters', 'eso_etc')
         return dirname
 
     @staticmethod
+    def _Bessell90FiltersFolder():
+        rootDir = dataRootDir()
+        dirname = os.path.join(rootDir, 'photometry', 'filters', 'bessell90')
+        return dirname
+
+    @staticmethod
     def _DetectorsFolder():
         rootDir = dataRootDir()
         dirname = os.path.join(rootDir, 'photometry', 'detectors')
         return dirname
 
     @classmethod
     def _eso_etc_u(cls):
@@ -162,15 +174,28 @@
 
     @classmethod
     def _c_red_one(cls):
         return SpectralElement.from_file(
             os.path.join(cls._DetectorsFolder(), 'c_red_one.dat'),
             wave_unit=u.nm)
 
-
     @classmethod
     def _eso_etc(cls, filter_name, wavelength_unit):
         return SpectralElement.from_file(
             os.path.join(cls._EsoEtcFiltersFolder(),
                          'phot_%s.dat' % filter_name),
             wave_unit=wavelength_unit)
 
+    @classmethod
+    def _bessell90(cls, filter_name):
+        return SpectralElement.from_file(
+            os.path.join(cls._Bessell90FiltersFolder(),
+                         'bessell90_%s.dat' % filter_name),
+            wave_unit=u.AA)
+
+    @classmethod
+    def _bessell90_r(cls):
+        return cls._bessell90('r')
+
+    @classmethod
+    def _bessell90_i(cls):
+        return cls._bessell90('i')
```

### Comparing `arte-0.8.0/arte/photometry/mag_estimator.py` & `arte-0.9.0/arte/photometry/mag_estimator.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/photometry/n_phot.py` & `arte-0.9.0/arte/photometry/n_phot.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/photometry/normalized_star_spectrum.py` & `arte-0.9.0/arte/photometry/normalized_star_spectrum.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/photometry/sandbox.py` & `arte-0.9.0/arte/photometry/sandbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -93,16 +93,53 @@
     eso_etc_zp = np.array([
         4.18023e-09, 6.60085e-09, 3.60994e-09,
         2.28665e-09, 1.22603e-09, 7.76068e-10,
         5.973e-10, 3.12e-10, 1.14e-10, 3.94e-11,
         4.83e-12, 2.04e-12, 1.23e-13, 6.8e-15]) * FLAM
 
     star = get_normalized_star_spectrum('vega', 0.0, Filters.ESO_ETC_R)
+    print(f"{'filter':10s} | {'flux':15s} | {'zp err %':8s} | {'cnts':17s} |"
+          f"{'boundaries'}")
     for filt_name, etc_zp in zip(filters, eso_etc_zp):
         filt = Filters.get(filt_name)
         obs = Observation(star, filt)
         zp = obs.effstim('flam', wavelengths=filt.waveset)
         err = (zp - etc_zp) / etc_zp * 100
         cnts = obs.countrate(area=1 * u.m ** 2, wavelengths=filt.waveset)
         print(f"{filt_name:10s} | {zp:10.3e} | {err:+7.3f}% | {cnts:10.3e} |"
               f"{filt.waveset.to(u.nm)[0]:g} {filt.waveset.to(u.nm)[-1]:g}")
 
+
+
+def pippo(filt):
+    f_source = get_normalized_star_spectrum(spectral_type='vega', magnitude=0, filter_name=filt)
+    obs = Observation(spec=f_source, band=Filters.get(filt), binset=f_source.waveset)
+    return obs.countrate(area=1*u.m**2)
+
+
+def compare_integrate_with_observation(filt_name, filt_minmax=None, filt_obs=None, star_spectral_type='A0V'):
+    sp = get_normalized_star_spectrum(star_spectral_type, 0, filt_name)
+    filt = Filters.get(filt_name)
+    if filt_minmax is None:
+        waveset = filt.waveset
+    else:
+        waveset = np.linspace(filt_minmax[0], filt_minmax[1], 1000)
+    counts_int = sp.integrate(waveset) * 1e4 * u.cm**2/u.m**2
+    if filt_obs == 'one':
+        #Observation integrates the spectrum considering 100% transmission within the band
+        filt_obs = SpectralElement(
+            Box1D, amplitude=1., x_0=(waveset.max() + waveset.min())/2, width=(waveset.max() - waveset.min()))
+    elif filt_obs is None:
+        filt_obs = filt
+    obs = Observation(spec=sp, band=filt_obs, binset=waveset, force='taper')
+    counts_obs = obs.countrate(area=1 * u.m**2)
+    print('Flux with integrate function: %s' %counts_int)
+    print('Flux with Observation: %s' %counts_obs)
+    return sp
+
+
+def main_observation_playing_with_parameters():
+    print('Integrate considering a waveset built by us with minmax of our H band and a Box1D filter:')
+    sp = compare_integrate_with_observation(filt_name=Filters.ESO_ETC_H, filt_minmax=(14900, 17800), filt_obs='one', star_spectral_type='vega')
+
+    print('\nIntegrate considering the ESO filter waveset (min is smaller and max is larger) and a Box1D filter:')
+    sp = compare_integrate_with_observation(filt_name=Filters.ESO_ETC_H, filt_obs='one', star_spectral_type='vega')
```

### Comparing `arte-0.8.0/arte/photometry/spectral_types.py` & `arte-0.9.0/arte/photometry/spectral_types.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/photometry/transmissive_elements.py` & `arte-0.9.0/arte/photometry/transmissive_elements.py`

 * *Files 5% similar despite different names*

```diff
@@ -216,14 +216,32 @@
         new_r = self._insert_spectral_element(self.reflectance, reflectance,
                                               wavelengths)
         new_a = self._insert_spectral_element(self.absorptance, absorptance,
                                               wavelengths)
 
         self._initialize(transmittance=new_t, reflectance=new_r,
                          absorptance=new_a)
+        
+    def to_dat(self, filepath, data_type):
+        if data_type == 'transmittance':
+            data = self.transmittance(self.waveset).value
+            title = np.array([['Wavelength [um]', 'Transmittance']])
+        elif data_type == 'reflectance':
+            data = self.reflectance(self.waveset).value
+            title = np.array([['Wavelength [um]', 'Reflectance']])
+        elif data_type == 'absorptance':
+            data = self.absorptance(self.waveset).value
+            title = np.array([['Wavelength [um]', 'Absorptance']])
+        to_write = np.stack((
+            self.waveset.to(u.um).value,
+            data), axis=1)
+        with open(filepath, 'a') as datafile:
+            np.savetxt(datafile,
+                       np.vstack((title, to_write)),
+                       fmt=['%-30s', '%-30s'])
 
     def to_fits(self, filename, **kwargs):
         wv = self.waveset
         hdu1 = fits.PrimaryHDU(wv.to(u.nm).value)
         hdu2 = fits.ImageHDU(self.transmittance(wv).value)
         hdu3 = fits.ImageHDU(self.absorptance(wv).value)
         hdul = fits.HDUList([hdu1, hdu2, hdu3])
```

### Comparing `arte-0.8.0/arte/photometry/transmittance_calculator.py` & `arte-0.9.0/arte/photometry/transmittance_calculator.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/sandbox.py` & `arte-0.9.0/arte/sandbox.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/sandbox_noise_propagation.py` & `arte-0.9.0/arte/sandbox_noise_propagation.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/time_series/indexer.py` & `arte-0.9.0/arte/time_series/indexer.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/time_series/multi_time_series.py` & `arte-0.9.0/arte/time_series/multi_time_series.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/time_series/time_series.py` & `arte-0.9.0/arte/time_series/time_series.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/aperture.py` & `arte-0.9.0/arte/types/aperture.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/domainxy.py` & `arte-0.9.0/arte/types/domainxy.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/fisba_measure.py` & `arte-0.9.0/arte/types/fisba_measure.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/guide_source.py` & `arte-0.9.0/arte/types/guide_source.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/mask.py` & `arte-0.9.0/arte/types/mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,56 @@
 import numpy as np
 from arte.types.region_of_interest import RegionOfInterest
 from arte.utils.image_moments import ImageMoments
 
-# class BaseMask
 
+class BaseMask():
+    '''
+    '''
+
+    def __init__(self, mask_array):
+        self._shape = mask_array.shape
+        self._mask = mask_array
+    
+    def mask(self):
+        '''
+        Boolean mask of the mask
+
+        Returns
+        -------
+        mask: boolean `~numpy.array`
+            mask of the pupil. Array is True outside the pupil,
+            and False inside the pupil
+        '''
+        return self._mask
+    
+    def as_masked_array(self):
+        return np.ma.array(np.ones(self._shape),
+                           mask=self.mask())
+        
+    def shape(self):
+        '''
+        Array shape
+
+        Returns
+        -------
+        shape: list (2,)
+            shape of the mask array
+        '''
+        return self._shape
+    
+    @staticmethod
+    def from_masked_array(numpy_masked_array):
+        return BaseMask(numpy_masked_array)
+    
+    # TODO: funzione per verificare che tutti i punti di questa maschera stanno
+    # dentro una maschera passata
 
-class CircularMask():
+
+class CircularMask(BaseMask):
     '''
     Represent a circular mask
 
     A `~numpy.array` representing a circular pupil. Frame shape, pupil radius
     and center can be specified.
 
     Use `mask` method to access the mask as boolean mask (e.g. to be used
@@ -59,27 +100,15 @@
                                                self._shape[1]])
 
         r = self._maskRadius
         cc = self._maskCenter
         y, x = np.mgrid[0.5: self._shape[0] + 0.5:1,
                         0.5: self._shape[1] + 0.5:1]
         self._mask = np.where(
-            ((x - cc[1])**2 + (y - cc[0])**2) <= r**2, False, True)
-
-    def mask(self):
-        '''
-        Boolean mask of the Circular Mask
-
-        Returns
-        -------
-        mask: boolean `~numpy.array`
-            mask of the circular pupil. Array is True outside the pupil,
-            and False inside the pupil
-        '''
-        return self._mask
+            ((x - cc[1]) ** 2 + (y - cc[0]) ** 2) <= r ** 2, False, True)
 
     def asTransmissionValue(self):
         return np.logical_not(self._mask).astype(int)
 
     def radius(self):
         '''
         Radius of the mask 
@@ -100,25 +129,14 @@
         -------
         center: `~numpy.array` of shape (2,)
             Y, X coordinate of the mask center in the array reference system
 
         '''
         return self._maskCenter
 
-    def shape(self):
-        '''
-        Array shape
-
-        Returns
-        -------
-        shape: list (2,)
-            shape of the mask array
-        '''
-        return self._shape
-
     @staticmethod
     def fromMaskedArray(maskedArray):
         '''
         Creates a `CircularMask` roughly corresponding to the mask of a masked
         array
         
         Returns a `CircularMask` object having radius and center guessed from
@@ -140,17 +158,17 @@
             a circular mask included in the mask of `maskedArray`
 
         '''
         assert isinstance(maskedArray, np.ma.masked_array)
         shape = maskedArray.shape
         again = 0.995
         while again:
-            im = ImageMoments(maskedArray.mask.astype(int)*-1 + 1)
-            centerYX = np.roll(im.centroid(),1)
-            radius = again*np.min(im.semiAxes())
+            im = ImageMoments(maskedArray.mask.astype(int) * -1 + 1)
+            centerYX = np.roll(im.centroid(), 1)
+            radius = again * np.min(im.semiAxes())
             circularMask = CircularMask(shape, radius, centerYX)
             if np.in1d(circularMask.in_mask_indices(),
                        np.argwhere(maskedArray.mask.flatten() == False)).all():
                 again = False
             if radius < 1:
                 raise Exception("Couldn't estimate a CircularMask")
             else:
@@ -161,21 +179,18 @@
     def regionOfInterest(self):
         centerX = int(self.center()[1])
         centerY = int(self.center()[0])
         radius = int(self.radius())
         return RegionOfInterest(centerX - radius, centerX + radius,
                                 centerY - radius, centerY + radius)
 
-    def as_masked_array(self):
-        return np.ma.array(np.ones(self._shape),
-                           mask=self.mask())
-
     def in_mask_indices(self):
         return self.asTransmissionValue().flatten().nonzero()[0]
 
+
 class AnnularMask(CircularMask):
     '''
     Inheritance of CircularMask class to provide an annular mask
 
     Added inRadius parameter, radius of central obstruction.
     Default inRadius values is 0 with AnnularMask converging to CircularMask
     '''
@@ -204,15 +219,15 @@
                                                self._shape[1]])
 
         r = self._maskRadius
         cc = self._maskCenter
         y, x = np.mgrid[0.5: self._shape[0] + 0.5:1,
                         0.5: self._shape[1] + 0.5:1]
 
-        tmp = ((x - cc[1])**2 + (y - cc[0])**2) <= r**2
+        tmp = ((x - cc[1]) ** 2 + (y - cc[0]) ** 2) <= r ** 2
         if self._inRadius == 0:
             self._mask = np.where(tmp, False, True)
         else:
             cc = CircularMask(self._shape, self._inRadius, self._maskCenter)
             tmp[cc.asTransmissionValue() > 0] = False
             self._mask = np.where(tmp, False, True)
```

### Comparing `arte-0.8.0/arte/types/region_of_interest.py` & `arte-0.9.0/arte/types/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/scalar_bidimensional_function.py` & `arte-0.9.0/arte/types/scalar_bidimensional_function.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/slopes.py` & `arte-0.9.0/arte/types/slopes.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/wavefront.py` & `arte-0.9.0/arte/types/wavefront.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/types/zernike_coefficients.py` & `arte-0.9.0/arte/types/zernike_coefficients.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/capture_output.py` & `arte-0.9.0/arte/utils/capture_output.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/circular_buffer.py` & `arte-0.9.0/arte/utils/circular_buffer.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/compareIDL.py` & `arte-0.9.0/arte/utils/compareIDL.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/decorator.py` & `arte-0.9.0/arte/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/discrete_fourier_transform.py` & `arte-0.9.0/arte/utils/discrete_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/executor.py` & `arte-0.9.0/arte/utils/executor.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/footprint_geometry.py` & `arte-0.9.0/arte/utils/footprint_geometry.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/generalized_fitting_error.py` & `arte-0.9.0/arte/utils/generalized_fitting_error.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/gpu.py` & `arte-0.9.0/arte/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/help.py` & `arte-0.9.0/arte/utils/help.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/image_moments.py` & `arte-0.9.0/arte/utils/image_moments.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/iterators.py` & `arte-0.9.0/arte/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/locate.py` & `arte-0.9.0/arte/utils/locate.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/logger.py` & `arte-0.9.0/arte/utils/logger.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/marechal.py` & `arte-0.9.0/arte/utils/marechal.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/math.py` & `arte-0.9.0/arte/utils/math.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/modal_decomposer.py` & `arte-0.9.0/arte/utils/modal_decomposer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from scipy.linalg import pinv
 from arte.utils.decorator import cacheResult, returns
 from arte.utils.zernike_generator import ZernikeGenerator
 from arte.types.zernike_coefficients import ZernikeCoefficients
-from arte.types.mask import CircularMask
+from arte.types.mask import CircularMask, BaseMask
 from arte.types.wavefront import Wavefront
 from arte.types.slopes import Slopes
 
 
 class ModalDecomposer(object):
 
     def __init__(self, n_zernike_modes):
@@ -19,15 +19,15 @@
         dx = zg.getDerivativeXDict(list(range(2, 2 + nModes)))
         dy = zg.getDerivativeYDict(list(range(2, 2 + nModes)))
         im = np.zeros((nModes, 2 * dx[2].compressed().size))
         modesIdx = list(range(2, 2 + nModes))
 
         i = 0
         for idx in modesIdx:
-            im[i, :] = np.hstack((dx[idx].compressed(), dy[idx].compressed()))
+            im[i,:] = np.hstack((dx[idx].compressed(), dy[idx].compressed()))
             i += 1
         return pinv(im)
 
     @returns(ZernikeCoefficients)
     def measureZernikeCoefficientsFromSlopes(self, slopes, mask, nModes=None):
         if nModes is None:
             nModes = self._nZernikeModes
@@ -45,42 +45,53 @@
              np.ma.masked_array(slopes.mapY(), mask.mask()).compressed())
         )
 
         return ZernikeCoefficients.fromNumpyArray(
             np.dot(slopesInMaskVector, reconstructor))
 
     @cacheResult
-    def _synthZernikeRecFromWavefront(self, nModes, mask):
-        zg = ZernikeGenerator(mask)
+    def _synthZernikeRecFromWavefront(self, nModes, circular_mask,
+                                      user_mask):
+        zg = ZernikeGenerator(circular_mask)
         wf = zg.getZernikeDict(list(range(2, 2 + nModes)))
-        im = np.zeros((nModes, wf[2].compressed().size))
+        im = np.zeros((nModes, user_mask.as_masked_array().compressed().size))
         modesIdx = list(range(2, 2 + nModes))
 
         i = 0
         for idx in modesIdx:
-            im[i, :] = wf[idx].compressed()
+            wf_masked = np.ma.masked_array(wf[idx].data, mask=user_mask.mask())
+            im[i,:] = wf_masked.compressed()
             i += 1
         return pinv(im)
 
     @returns(ZernikeCoefficients)
     def measureZernikeCoefficientsFromWavefront(self,
                                                 wavefront,
-                                                mask,
+                                                circular_mask,
+                                                user_mask,
                                                 nModes=None):
         if nModes is None:
             nModes = self._nZernikeModes
         assert isinstance(wavefront, Wavefront), \
             'wavefront argument must be of type Wavefront, instead is %s' % \
             wavefront.__class__.__name__
-        assert isinstance(mask, CircularMask), \
-            'Mask argument must be of type CircularMask, instead is %s' % \
-            mask.__class__.__name__
+        assert isinstance(circular_mask, CircularMask), \
+            'Circular mask argument must be of type CircularMask, instead is %s' % \
+            circular_mask.__class__.__name__
+        assert isinstance(user_mask, BaseMask), \
+            'User mask argument must be of type BaseMask, instead is %s' % \
+            user_mask.__class__.__name__
+        if not np.all(
+            circular_mask.as_masked_array() * user_mask.as_masked_array()
+            == user_mask.as_masked_array()):
+            raise Exception('User mask must be fully contained in circular mask')
 
         reconstructor = self._synthZernikeRecFromWavefront(nModes,
-                                                           mask)
+                                                           circular_mask,
+                                                           user_mask)
         wavefrontInMaskVector = \
             np.ma.masked_array(wavefront.toNumpyArray(),
-                               mask.mask()).compressed()
+                               user_mask.mask()).compressed()
         wavefrontInMaskVectorNoPiston = wavefrontInMaskVector - \
             wavefrontInMaskVector.mean()
         return ZernikeCoefficients.fromNumpyArray(
             np.dot(wavefrontInMaskVectorNoPiston, reconstructor))
```

### Comparing `arte-0.8.0/arte/utils/multiton.py` & `arte-0.9.0/arte/utils/multiton.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/noise_propagation.py` & `arte-0.9.0/arte/utils/noise_propagation.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/not_available.py` & `arte-0.9.0/arte/utils/not_available.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/radial_profile.py` & `arte-0.9.0/arte/utils/radial_profile.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/rebin.py` & `arte-0.9.0/arte/utils/rebin.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/shape_fitter.py` & `arte-0.9.0/arte/utils/shape_fitter.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/shared_array.py` & `arte-0.9.0/arte/utils/shared_array.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/tabular_report.py` & `arte-0.9.0/arte/utils/tabular_report.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/timekeepers.py` & `arte-0.9.0/arte/utils/timekeepers.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/timestamp.py` & `arte-0.9.0/arte/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/unit_checker.py` & `arte-0.9.0/arte/utils/unit_checker.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/zernike_generator.py` & `arte-0.9.0/arte/utils/zernike_generator.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte/utils/zernike_projection_on_subaperture.py` & `arte-0.9.0/arte/utils/zernike_projection_on_subaperture.py`

 * *Files identical despite different names*

### Comparing `arte-0.8.0/arte.egg-info/PKG-INFO` & `arte-0.9.0/arte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arte
-Version: 0.8.0
+Version: 0.9.0
 Summary: Arcetri Random sTuff collEction
 Home-page: https://github.com/ArcetriAdaptiveOptics/arte
 Author: Lorenzo Busoni, Alfio Puglisi, INAF Arcetri Adaptive Optics group
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: Adaptive Optics, Astrophysics, INAF, Arcetri
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Requires-Dist: astropy
 Requires-Dist: synphot
 Requires-Dist: pytest
 Requires-Dist: skycalc-cli
 Requires-Dist: scikit-image>=0.17
 Requires-Dist: scipy
 Requires-Dist: mpmath
+Requires-Dist: requests
 
 # arte: Arcetri Random sTuff collEction
 
 A collection of routines and utilities
 developed by the Arcetri Astrophysical Observatory's AO group.
 
 ## Documentation
```

### Comparing `arte-0.8.0/arte.egg-info/SOURCES.txt` & `arte-0.9.0/arte.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,18 @@
 arte/math/toccd.py
 arte/misc/__init__.py
 arte/misc/fourier_adaptive_optics.py
 arte/photometry/__init__.py
 arte/photometry/eso_sky_calc.py
 arte/photometry/filters.py
 arte/photometry/mag_estimator.py
-arte/photometry/morfeo_transmissive_systems.py
 arte/photometry/n_phot.py
 arte/photometry/normalized_star_spectrum.py
 arte/photometry/sandbox.py
 arte/photometry/spectral_types.py
-arte/photometry/thermal_flux.py
 arte/photometry/transmissive_elements.py
 arte/photometry/transmissive_elements_catalogs.py
 arte/photometry/transmittance_calculator.py
 arte/time_series/__init__.py
 arte/time_series/indexer.py
 arte/time_series/multi_time_series.py
 arte/time_series/time_series.py
```

### Comparing `arte-0.8.0/setup.py` & `arte-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,13 +89,14 @@
                         "matplotlib",
                         "astropy",
                         "synphot",
                         "pytest",
                         "skycalc-cli",
                         "scikit-image>=0.17",
                         "scipy",
-                        "mpmath"
+                        "mpmath",
+                        "requests"
                         ],
       include_package_data=True,
       test_suite='test',
       cmdclass={'upload': UploadCommand, },
       )
```

### Comparing `arte-0.8.0/test/test_helper.py` & `arte-0.9.0/test/test_helper.py`

 * *Files identical despite different names*

