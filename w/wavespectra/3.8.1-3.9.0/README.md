# Comparing `tmp/wavespectra-3.8.1.tar.gz` & `tmp/wavespectra-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wavespectra-3.8.1.tar", last modified: Tue Apr  6 02:11:58 2021, max compression
+gzip compressed data, was "dist/wavespectra-3.9.0.tar", last modified: Sat May 29 08:53:57 2021, max compression
```

## Comparing `wavespectra-3.8.1.tar` & `wavespectra-3.9.0.tar`

### file list

```diff
@@ -1,406 +1,325 @@
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.124963 wavespectra-3.8.1/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      248 2020-10-01 10:30:02.000000 wavespectra-3.8.1/AUTHORS.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3548 2020-10-01 10:30:02.000000 wavespectra-3.8.1/CONTRIBUTING.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    11993 2021-04-06 02:09:00.000000 wavespectra-3.8.1/HISTORY.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1065 2020-10-01 10:30:02.000000 wavespectra-3.8.1/LICENSE.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      463 2020-10-01 10:30:02.000000 wavespectra-3.8.1/MANIFEST.in
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     9180 2021-04-06 02:11:58.124963 wavespectra-3.8.1/PKG-INFO
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6647 2021-03-30 08:47:13.000000 wavespectra-3.8.1/README.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.072963 wavespectra-3.8.1/docs/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      610 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/Makefile
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.068963 wavespectra-3.8.1/docs/_build/
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.084963 wavespectra-3.8.1/docs/_build/_images/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    80861 2021-03-30 21:28:22.000000 wavespectra-3.8.1/docs/_build/_images/contour_type_plot.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    79521 2021-03-30 21:28:22.000000 wavespectra-3.8.1/docs/_build/_images/contourf_type_plot.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    77092 2021-03-30 21:28:26.000000 wavespectra-3.8.1/docs/_build/_images/faceted_polar_plot.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   287637 2021-03-30 21:28:20.000000 wavespectra-3.8.1/docs/_build/_images/faceted_polar_plot2.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   119415 2021-03-30 21:28:21.000000 wavespectra-3.8.1/docs/_build/_images/faceted_polar_plot3.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    37557 2021-03-30 21:28:24.000000 wavespectra-3.8.1/docs/_build/_images/freq_split_hs.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    29187 2021-03-30 21:28:26.000000 wavespectra-3.8.1/docs/_build/_images/hovmoller_plot.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    47484 2021-03-30 21:28:22.000000 wavespectra-3.8.1/docs/_build/_images/hs.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    29053 2021-03-30 21:28:26.000000 wavespectra-3.8.1/docs/_build/_images/interp_stations_plot.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    72225 2021-03-30 21:28:23.000000 wavespectra-3.8.1/docs/_build/_images/many_stats.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    68800 2021-03-30 21:28:18.000000 wavespectra-3.8.1/docs/_build/_images/single_polar_plot.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    67817 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/_build/_images/single_polar_plot_ax_extent1.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    68307 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/_build/_images/single_polar_plot_ax_extent2.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69818 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/_build/_images/single_polar_plot_ax_extent3.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    58306 2021-03-30 21:28:18.000000 wavespectra-3.8.1/docs/_build/_images/single_polar_plot_period.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    59952 2021-03-30 21:28:18.000000 wavespectra-3.8.1/docs/_build/_images/single_polar_plot_period_realvalues.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    61374 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/_build/_images/single_polar_plot_xarray_parameters.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   116255 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_clean_axis_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    43605 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_clean_axis_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   286096 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_faceting_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    71988 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_faceting_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    42812 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_hs_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    19887 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_hs_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    68863 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contour_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    45317 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contour_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69633 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contourf_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    61438 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contourf_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    45610 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    43566 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    58770 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_period_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    53289 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_period_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    60411 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_real_values_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    51830 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_real_values_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69597 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    50932 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    27980 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_timeseries_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    20757 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_timeseries_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    62764 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    55675 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    37580 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_split_sea_swell_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    20313 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_split_sea_swell_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    72748 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_001.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    29209 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    72456 2021-03-30 21:28:25.000000 wavespectra-3.8.1/docs/_build/_images/watershed_hs.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21757 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/_build/_images/wavespectra_logo.png
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.084963 wavespectra-3.8.1/docs/_build/_static/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21404 2021-03-10 21:33:20.000000 wavespectra-3.8.1/docs/_build/_static/broken_example.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      286 2021-03-30 18:53:40.000000 wavespectra-3.8.1/docs/_build/_static/file.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       90 2021-03-30 18:53:40.000000 wavespectra-3.8.1/docs/_build/_static/minus.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4315 2021-03-10 21:33:20.000000 wavespectra-3.8.1/docs/_build/_static/no_image.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       90 2021-03-30 18:53:40.000000 wavespectra-3.8.1/docs/_build/_static/plus.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21757 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/_build/_static/wavespectra_logo.png
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.084963 wavespectra-3.8.1/docs/_static/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21757 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/_static/wavespectra_logo.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4494 2021-03-30 08:47:13.000000 wavespectra-3.8.1/docs/api.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      106 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/authors.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.084963 wavespectra-3.8.1/docs/auto_gallery/
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.088963 wavespectra-3.8.1/docs/auto_gallery/images/
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   116255 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_clean_axis_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   286096 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_faceting_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    42812 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_hs_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    68863 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_contour_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    69633 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_contourf_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    45610 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_pcolormesh_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    58770 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_period_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    60411 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_real_values_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    69597 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_slice_radius_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    27980 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_timeseries_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    62764 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_xarray_params_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    37580 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_split_sea_swell_001.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    72748 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_watershed_sea_swell_001.png
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.088963 wavespectra-3.8.1/docs/auto_gallery/images/thumb/
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    43605 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_clean_axis_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    71988 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_faceting_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    19887 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_hs_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    45317 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contour_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    61438 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contourf_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    43566 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_pcolormesh_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    53289 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_period_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    51830 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_real_values_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    50932 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_slice_radius_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    20757 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_timeseries_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    55675 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_xarray_params_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    20313 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_split_sea_swell_thumb.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    29209 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_watershed_sea_swell_thumb.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5854 2021-03-10 21:33:36.000000 wavespectra-3.8.1/docs/auto_gallery/index.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     2691 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/plot_clean_axis.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     2487 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/plot_faceting.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1353 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/plot_hs.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1503 2020-10-01 06:37:01.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_contour.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1515 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_contourf.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1535 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_pcolormesh.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1507 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_period.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1600 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_real_values.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1609 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_slice_radius.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1815 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_timeseries.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1670 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_spectra_xarray_params.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1916 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_split_sea_swell.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     3414 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/plot_watershed_sea_swell.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     3398 2020-10-01 06:37:02.000000 wavespectra-3.8.1/docs/auto_gallery/sg_execution_times.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6300 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/conf.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      111 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/contributing.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2313 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/conventions.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.088963 wavespectra-3.8.1/docs/gallery/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       30 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/gallery/README.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      139 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/gallery.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.100963 wavespectra-3.8.1/docs/generated/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      132 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.celerity.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      114 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.dm.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      114 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.dp.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      117 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.dpm.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      120 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.dspr.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      120 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.hmax.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      114 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.hs.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      120 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.momd.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      120 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.momf.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      120 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.oned.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      135 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.partition.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      122 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.plot.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      918 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      145 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.scale_by_hs.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      123 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.split.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      123 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.stats.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      114 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.sw.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      117 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.swe.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      120 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.tm01.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      120 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.tm02.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      137 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.to_energy.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      114 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.tp.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      129 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecArray.wavelen.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      407 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecDataset.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      123 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecDataset.sel.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      137 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecDataset.to_json.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      143 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecDataset.to_netcdf.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      146 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecDataset.to_octopus.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      137 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecDataset.to_swan.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      134 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.SpecDataset.to_ww3.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      178 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.construct.helpers.arrange_inputs.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      187 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.construct.helpers.check_coordinates.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      172 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.construct.helpers.make_dataset.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      152 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.construct.helpers.spread.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      131 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.construct.jonswap.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      140 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.construct.ochihubble.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      144 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.attributes.attrs.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      189 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.attributes.set_spec_attributes.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      144 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.npstats.dp_gufunc.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      147 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.npstats.dpm_gufunc.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      144 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.npstats.tp_gufunc.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      147 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.npstats.tps_gufunc.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      174 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.select.Coordinates.distance.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      168 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.select.Coordinates.nearer.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      171 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.select.Coordinates.nearest.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      142 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.select.sel_bbox.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      139 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.select.sel_idw.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      151 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.select.sel_nearest.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      425 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.swan.SwanSpecFile.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      142 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.swan._dateparse.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      136 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.swan.read_tab.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      137 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.celerity.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      165 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.dnum_to_datetime.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      151 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.flatten_list.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      148 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.interp_spec.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      153 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.spddir_to_uv.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      148 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.to_datetime.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      148 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.to_nautical.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      151 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.unique_times.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      153 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.uv_to_spddir.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      134 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.wavelen.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      137 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.utils.wavenuma.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      187 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.watershed.frequency_resolution.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      131 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.watershed.hs.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      155 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.watershed.inflection.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      152 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.watershed.partition.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      231 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.xrstats.mean_direction_at_peak_wave_period.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      180 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.xrstats.peak_wave_direction.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      171 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.core.xrstats.peak_wave_period.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      151 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.input.swan.read_hotswan.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      148 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.input.swan.read_swanow.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      145 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.input.swan.read_swans.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      118 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_dataset.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_era5.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_json.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      115 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_ncswan.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_ndbc.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      115 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_netcdf.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      118 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_octopus.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      118 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_spotter.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_swan.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      118 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_triaxys.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      106 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_ww3.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      106 2021-03-30 20:59:17.000000 wavespectra-3.8.1/docs/generated/wavespectra.read_wwm.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      106 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/history.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1615 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/index.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2141 2021-03-30 08:47:13.000000 wavespectra-3.8.1/docs/install.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2641 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/io-input.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1032 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/io-output.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4676 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/library.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      815 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/make.bat
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5381 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/plotting.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     7719 2021-03-30 21:27:55.000000 wavespectra-3.8.1/docs/quickstart.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.104963 wavespectra-3.8.1/docs/savefig/
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    80861 2021-03-30 21:28:22.000000 wavespectra-3.8.1/docs/savefig/contour_type_plot.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    79521 2021-03-30 21:28:22.000000 wavespectra-3.8.1/docs/savefig/contourf_type_plot.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    76948 2020-10-01 06:37:06.000000 wavespectra-3.8.1/docs/savefig/contourf_type_plot9.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    77092 2021-03-30 21:28:26.000000 wavespectra-3.8.1/docs/savefig/faceted_polar_plot.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   287637 2021-03-30 21:28:20.000000 wavespectra-3.8.1/docs/savefig/faceted_polar_plot2.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   119415 2021-03-30 21:28:21.000000 wavespectra-3.8.1/docs/savefig/faceted_polar_plot3.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    37557 2021-03-30 21:28:24.000000 wavespectra-3.8.1/docs/savefig/freq_split_hs.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    29187 2021-03-30 21:28:26.000000 wavespectra-3.8.1/docs/savefig/hovmoller_plot.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    47484 2021-03-30 21:28:22.000000 wavespectra-3.8.1/docs/savefig/hs.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    29053 2021-03-30 21:28:26.000000 wavespectra-3.8.1/docs/savefig/interp_stations_plot.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    72225 2021-03-30 21:28:23.000000 wavespectra-3.8.1/docs/savefig/many_stats.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    43300 2020-10-01 06:37:06.000000 wavespectra-3.8.1/docs/savefig/pcolormesh_type_plot.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    68800 2021-03-30 21:28:18.000000 wavespectra-3.8.1/docs/savefig/single_polar_plot.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    67817 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/savefig/single_polar_plot_ax_extent1.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    68307 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/savefig/single_polar_plot_ax_extent2.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    69818 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/savefig/single_polar_plot_ax_extent3.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    58306 2021-03-30 21:28:18.000000 wavespectra-3.8.1/docs/savefig/single_polar_plot_period.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    59952 2021-03-30 21:28:18.000000 wavespectra-3.8.1/docs/savefig/single_polar_plot_period_realvalues.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    61374 2021-03-30 21:28:19.000000 wavespectra-3.8.1/docs/savefig/single_polar_plot_xarray_parameters.png
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    72456 2021-03-30 21:28:25.000000 wavespectra-3.8.1/docs/savefig/watershed_hs.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2288 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/selecting.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      458 2020-10-01 10:30:02.000000 wavespectra-3.8.1/docs/support.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.108963 wavespectra-3.8.1/requirements/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      125 2021-03-30 08:47:13.000000 wavespectra-3.8.1/requirements/default.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        7 2021-03-30 08:47:13.000000 wavespectra-3.8.1/requirements/extra.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      163 2020-10-01 10:30:02.000000 wavespectra-3.8.1/requirements/requirements_dev.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      240 2021-03-30 21:38:02.000000 wavespectra-3.8.1/requirements/requirements_doc.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       19 2020-10-01 10:30:02.000000 wavespectra-3.8.1/requirements/requirements_tox.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        6 2020-10-01 10:30:02.000000 wavespectra-3.8.1/requirements/test.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      911 2021-04-06 02:11:58.124963 wavespectra-3.8.1/setup.cfg
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3672 2021-04-06 02:07:38.000000 wavespectra-3.8.1/setup.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.108963 wavespectra-3.8.1/tests/
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.108963 wavespectra-3.8.1/tests/core/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5286 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/core/test_construct.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2676 2021-03-30 08:47:13.000000 wavespectra-3.8.1/tests/core/test_core.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1429 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/core/test_dset_wrapper.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2280 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/core/test_plot.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10029 2021-02-17 08:10:06.000000 wavespectra-3.8.1/tests/core/test_sel.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1372 2021-02-17 07:40:40.000000 wavespectra-3.8.1/tests/core/test_watershed.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1665 2021-04-06 02:06:49.000000 wavespectra-3.8.1/tests/core/test_wave_stats.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.108963 wavespectra-3.8.1/tests/io/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1050 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/io/test_chunk_naming.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3853 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/io/test_io.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2020 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/io/test_json.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      848 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/io/test_ncswan.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2675 2021-02-12 03:05:43.000000 wavespectra-3.8.1/tests/io/test_ndbc.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1661 2021-03-30 08:47:13.000000 wavespectra-3.8.1/tests/io/test_octopus.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1140 2021-02-20 00:55:48.000000 wavespectra-3.8.1/tests/io/test_spotter.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1325 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/io/test_swan_ascii.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      840 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/io/test_triaxys.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.112963 wavespectra-3.8.1/tests/sample_files/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    73584 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/era5file.nc
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    43800 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/jsonfile.json
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.112963 wavespectra-3.8.1/tests/sample_files/ndbc/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    99616 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010.data_spec
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10571 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010.spec
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    96852 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010.swdir
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    96789 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010.swdir2
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    94719 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010.swr1
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    94719 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010.swr2
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     7836 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010d2019part.txt.gz
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     8203 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010i2019part.txt.gz
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6427 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010j2019part.txt.gz
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6575 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010k2019part.txt.gz
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4897 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ndbc/41010w2019part.txt.gz
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1120 2021-02-12 03:05:43.000000 wavespectra-3.8.1/tests/sample_files/ndbc/44004w2000.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    41157 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/octopusfile.oct
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    36170 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/spotter_20180214.json
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    38843 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/swanfile.nc
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    23736 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/swanfile.spec
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1368 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/swanfile.tab
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      469 2021-04-06 02:06:49.000000 wavespectra-3.8.1/tests/sample_files/swanfile.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    92145 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/triaxys.DIRSPEC
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1785 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/triaxys.NONDIRSPEC
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69915 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/wavespectra.nc
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    48008 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.nc
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.112963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        2 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/.zgroup
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    14114 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/.zmetadata
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.112963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/cur/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/cur/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      336 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/cur/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      336 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/cur/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.112963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/curdir/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/curdir/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      390 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/curdir/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      611 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/curdir/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.112963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/direction/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      331 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/direction/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      328 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/direction/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      112 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/direction/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.112963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/dpt/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/dpt/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      307 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/dpt/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       77 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/dpt/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/efth/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      389 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/efth/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      522 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/efth/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    15172 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/efth/0.0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      331 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      316 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      116 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency1/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      339 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency1/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      355 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency1/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      125 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency1/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency2/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      339 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency2/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      355 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency2/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      125 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/frequency2/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/latitude/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/latitude/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      324 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/latitude/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       68 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/latitude/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/longitude/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/longitude/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      327 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/longitude/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       67 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/longitude/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/station/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      319 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/station/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      102 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/station/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/station/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/time/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      317 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/time/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      293 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/time/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      156 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/time/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnd/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnd/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      328 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnd/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      551 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnd/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.116963 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnddir/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnddir/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      344 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnddir/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      666 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnddir/0.0
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    52738 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/sample_files/wwmfile.nc
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      987 2020-10-01 10:30:02.000000 wavespectra-3.8.1/tests/test_cookiecutter_template.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.120963 wavespectra-3.8.1/wavespectra/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1493 2021-04-06 02:09:28.000000 wavespectra-3.8.1/wavespectra/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      410 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/cli.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.120963 wavespectra-3.8.1/wavespectra/construct/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      143 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/construct/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2344 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/construct/helpers.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1137 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/construct/jonswap.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1266 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/construct/ochihubble.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.120963 wavespectra-3.8.1/wavespectra/core/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/core/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1390 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/core/attributes.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2413 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/core/attributes.yml
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4071 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/core/npstats.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    12274 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/core/select.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     9041 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/core/swan.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5967 2021-04-06 02:06:49.000000 wavespectra-3.8.1/wavespectra/core/utils.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6036 2021-03-30 21:38:02.000000 wavespectra-3.8.1/wavespectra/core/watershed.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4197 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/core/xrstats.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.124963 wavespectra-3.8.1/wavespectra/input/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2568 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1819 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/dataset.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1710 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/era5.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1061 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/json.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3022 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/input/ncswan.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5698 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/ndbc.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1704 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/netcdf.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      276 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/octopus.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6206 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/spotter.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    19448 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/input/swan.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6967 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/input/triaxys.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1344 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/input/wavespectra.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2675 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/input/ww3.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2749 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/input/wwm.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.124963 wavespectra-3.8.1/wavespectra/output/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      726 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/output/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      775 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/output/json.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1251 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/output/netcdf.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     7571 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/output/octopus.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2777 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/output/swan.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3735 2021-03-30 08:47:13.000000 wavespectra-3.8.1/wavespectra/output/ww3.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3294 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/output/ww3.yml
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    25915 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/plot.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    24788 2021-04-06 02:06:49.000000 wavespectra-3.8.1/wavespectra/specarray.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6097 2021-03-10 22:13:13.000000 wavespectra-3.8.1/wavespectra/specdataset.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.124963 wavespectra-3.8.1/wavespectra/specpart/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    12334 2021-03-30 21:38:02.000000 wavespectra-3.8.1/wavespectra/specpart/specpart.f90
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      841 2021-03-30 21:38:02.000000 wavespectra-3.8.1/wavespectra/specpart/specpart.pyf
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-04-06 02:11:58.120963 wavespectra-3.8.1/wavespectra.egg-info/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     9180 2021-04-06 02:11:57.000000 wavespectra-3.8.1/wavespectra.egg-info/PKG-INFO
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    15590 2021-04-06 02:11:58.000000 wavespectra-3.8.1/wavespectra.egg-info/SOURCES.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        1 2021-04-06 02:11:57.000000 wavespectra-3.8.1/wavespectra.egg-info/dependency_links.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       54 2021-04-06 02:11:57.000000 wavespectra-3.8.1/wavespectra.egg-info/entry_points.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        1 2021-04-06 02:11:57.000000 wavespectra-3.8.1/wavespectra.egg-info/not-zip-safe
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      152 2021-04-06 02:11:57.000000 wavespectra-3.8.1/wavespectra.egg-info/requires.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       12 2021-04-06 02:11:57.000000 wavespectra-3.8.1/wavespectra.egg-info/top_level.txt
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.427734 wavespectra-3.9.0/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      248 2020-10-01 10:30:02.000000 wavespectra-3.9.0/AUTHORS.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3548 2020-10-01 10:30:02.000000 wavespectra-3.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    12349 2021-05-29 08:35:20.000000 wavespectra-3.9.0/HISTORY.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1065 2020-10-01 10:30:02.000000 wavespectra-3.9.0/LICENSE.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      463 2020-10-01 10:30:02.000000 wavespectra-3.9.0/MANIFEST.in
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     9180 2021-05-29 08:53:57.427734 wavespectra-3.9.0/PKG-INFO
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6647 2021-03-30 08:47:13.000000 wavespectra-3.9.0/README.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.259737 wavespectra-3.9.0/docs/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      610 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/Makefile
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.239737 wavespectra-3.9.0/docs/_build/
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.315736 wavespectra-3.9.0/docs/_build/_images/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    80861 2021-03-30 21:28:22.000000 wavespectra-3.9.0/docs/_build/_images/contour_type_plot.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    79521 2021-03-30 21:28:22.000000 wavespectra-3.9.0/docs/_build/_images/contourf_type_plot.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    77092 2021-03-30 21:28:26.000000 wavespectra-3.9.0/docs/_build/_images/faceted_polar_plot.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   287637 2021-03-30 21:28:20.000000 wavespectra-3.9.0/docs/_build/_images/faceted_polar_plot2.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   119415 2021-03-30 21:28:21.000000 wavespectra-3.9.0/docs/_build/_images/faceted_polar_plot3.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    37557 2021-03-30 21:28:24.000000 wavespectra-3.9.0/docs/_build/_images/freq_split_hs.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    29187 2021-03-30 21:28:26.000000 wavespectra-3.9.0/docs/_build/_images/hovmoller_plot.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    47484 2021-03-30 21:28:22.000000 wavespectra-3.9.0/docs/_build/_images/hs.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    29053 2021-03-30 21:28:26.000000 wavespectra-3.9.0/docs/_build/_images/interp_stations_plot.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    72225 2021-03-30 21:28:23.000000 wavespectra-3.9.0/docs/_build/_images/many_stats.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    68800 2021-03-30 21:28:18.000000 wavespectra-3.9.0/docs/_build/_images/single_polar_plot.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    67817 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/_build/_images/single_polar_plot_ax_extent1.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    68307 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/_build/_images/single_polar_plot_ax_extent2.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69818 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/_build/_images/single_polar_plot_ax_extent3.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    58306 2021-03-30 21:28:18.000000 wavespectra-3.9.0/docs/_build/_images/single_polar_plot_period.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    59952 2021-03-30 21:28:18.000000 wavespectra-3.9.0/docs/_build/_images/single_polar_plot_period_realvalues.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    61374 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/_build/_images/single_polar_plot_xarray_parameters.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   116255 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_clean_axis_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    43605 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_clean_axis_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)   286096 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_faceting_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    71988 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_faceting_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    42812 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_hs_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    19887 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_hs_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    68863 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contour_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    45317 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contour_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69633 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contourf_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    61438 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contourf_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    45610 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    43566 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    58770 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_period_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    53289 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_period_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    60411 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_real_values_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    51830 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_real_values_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69597 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    50932 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    27980 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_timeseries_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    20757 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_timeseries_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    62764 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    55675 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    37580 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_split_sea_swell_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    20313 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_split_sea_swell_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    72748 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_001.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    29209 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    72456 2021-03-30 21:28:25.000000 wavespectra-3.9.0/docs/_build/_images/watershed_hs.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21757 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/_build/_images/wavespectra_logo.png
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.319736 wavespectra-3.9.0/docs/_build/_static/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21404 2021-03-10 21:33:20.000000 wavespectra-3.9.0/docs/_build/_static/broken_example.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      286 2021-03-30 18:53:40.000000 wavespectra-3.9.0/docs/_build/_static/file.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       90 2021-03-30 18:53:40.000000 wavespectra-3.9.0/docs/_build/_static/minus.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4315 2021-03-10 21:33:20.000000 wavespectra-3.9.0/docs/_build/_static/no_image.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       90 2021-03-30 18:53:40.000000 wavespectra-3.9.0/docs/_build/_static/plus.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21757 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/_build/_static/wavespectra_logo.png
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.319736 wavespectra-3.9.0/docs/_static/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21757 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/_static/wavespectra_logo.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4494 2021-03-30 08:47:13.000000 wavespectra-3.9.0/docs/api.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      106 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/authors.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.335736 wavespectra-3.9.0/docs/auto_gallery/
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.363735 wavespectra-3.9.0/docs/auto_gallery/images/
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   116255 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_clean_axis_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   286096 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_faceting_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    42812 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_hs_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    68863 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_contour_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    69633 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_contourf_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    45610 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_pcolormesh_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    58770 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_period_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    60411 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_real_values_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    69597 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_slice_radius_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    27980 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_timeseries_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    62764 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_xarray_params_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    37580 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_split_sea_swell_001.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    72748 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_watershed_sea_swell_001.png
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.371735 wavespectra-3.9.0/docs/auto_gallery/images/thumb/
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    43605 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_clean_axis_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    71988 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_faceting_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    19887 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_hs_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    45317 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contour_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    61438 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contourf_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    43566 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_pcolormesh_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    53289 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_period_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    51830 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_real_values_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    50932 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_slice_radius_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    20757 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_timeseries_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    55675 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_xarray_params_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    20313 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_split_sea_swell_thumb.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    29209 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_watershed_sea_swell_thumb.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5854 2021-03-10 21:33:36.000000 wavespectra-3.9.0/docs/auto_gallery/index.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     2691 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/plot_clean_axis.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     2487 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/plot_faceting.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1353 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/plot_hs.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1503 2020-10-01 06:37:01.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_contour.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1515 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_contourf.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1535 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_pcolormesh.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1507 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_period.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1600 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_real_values.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1609 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_slice_radius.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1815 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_timeseries.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1670 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_spectra_xarray_params.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     1916 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_split_sea_swell.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     3414 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/plot_watershed_sea_swell.rst
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     3398 2020-10-01 06:37:02.000000 wavespectra-3.9.0/docs/auto_gallery/sg_execution_times.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6300 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/conf.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      111 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/contributing.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2313 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/conventions.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.371735 wavespectra-3.9.0/docs/gallery/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       30 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/gallery/README.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      139 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/gallery.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      106 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/history.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1615 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/index.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2141 2021-03-30 08:47:13.000000 wavespectra-3.9.0/docs/install.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2641 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/io-input.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1032 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/io-output.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4676 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/library.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      815 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/make.bat
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5381 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/plotting.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     7719 2021-03-30 21:27:55.000000 wavespectra-3.9.0/docs/quickstart.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.383735 wavespectra-3.9.0/docs/savefig/
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    80861 2021-03-30 21:28:22.000000 wavespectra-3.9.0/docs/savefig/contour_type_plot.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    79521 2021-03-30 21:28:22.000000 wavespectra-3.9.0/docs/savefig/contourf_type_plot.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    76948 2020-10-01 06:37:06.000000 wavespectra-3.9.0/docs/savefig/contourf_type_plot9.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    77092 2021-03-30 21:28:26.000000 wavespectra-3.9.0/docs/savefig/faceted_polar_plot.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   287637 2021-03-30 21:28:20.000000 wavespectra-3.9.0/docs/savefig/faceted_polar_plot2.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)   119415 2021-03-30 21:28:21.000000 wavespectra-3.9.0/docs/savefig/faceted_polar_plot3.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    37557 2021-03-30 21:28:24.000000 wavespectra-3.9.0/docs/savefig/freq_split_hs.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    29187 2021-03-30 21:28:26.000000 wavespectra-3.9.0/docs/savefig/hovmoller_plot.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    47484 2021-03-30 21:28:22.000000 wavespectra-3.9.0/docs/savefig/hs.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    29053 2021-03-30 21:28:26.000000 wavespectra-3.9.0/docs/savefig/interp_stations_plot.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    72225 2021-03-30 21:28:23.000000 wavespectra-3.9.0/docs/savefig/many_stats.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    43300 2020-10-01 06:37:06.000000 wavespectra-3.9.0/docs/savefig/pcolormesh_type_plot.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    68800 2021-03-30 21:28:18.000000 wavespectra-3.9.0/docs/savefig/single_polar_plot.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    67817 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/savefig/single_polar_plot_ax_extent1.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    68307 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/savefig/single_polar_plot_ax_extent2.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    69818 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/savefig/single_polar_plot_ax_extent3.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    58306 2021-03-30 21:28:18.000000 wavespectra-3.9.0/docs/savefig/single_polar_plot_period.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    59952 2021-03-30 21:28:18.000000 wavespectra-3.9.0/docs/savefig/single_polar_plot_period_realvalues.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    61374 2021-03-30 21:28:19.000000 wavespectra-3.9.0/docs/savefig/single_polar_plot_xarray_parameters.png
+-rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)    72456 2021-03-30 21:28:25.000000 wavespectra-3.9.0/docs/savefig/watershed_hs.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2288 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/selecting.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      458 2020-10-01 10:30:02.000000 wavespectra-3.9.0/docs/support.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.391734 wavespectra-3.9.0/requirements/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      125 2021-03-30 08:47:13.000000 wavespectra-3.9.0/requirements/default.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        7 2021-03-30 08:47:13.000000 wavespectra-3.9.0/requirements/extra.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      163 2020-10-01 10:30:02.000000 wavespectra-3.9.0/requirements/requirements_dev.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      240 2021-05-29 08:35:35.000000 wavespectra-3.9.0/requirements/requirements_doc.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       19 2020-10-01 10:30:02.000000 wavespectra-3.9.0/requirements/requirements_tox.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        6 2020-10-01 10:30:02.000000 wavespectra-3.9.0/requirements/test.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      911 2021-05-29 08:53:57.427734 wavespectra-3.9.0/setup.cfg
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3672 2021-05-29 08:35:35.000000 wavespectra-3.9.0/setup.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.391734 wavespectra-3.9.0/tests/
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.391734 wavespectra-3.9.0/tests/core/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5286 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/core/test_construct.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2676 2021-03-30 08:47:13.000000 wavespectra-3.9.0/tests/core/test_core.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1429 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/core/test_dset_wrapper.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2280 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/core/test_plot.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10029 2021-02-17 08:10:06.000000 wavespectra-3.9.0/tests/core/test_sel.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1372 2021-02-17 07:40:40.000000 wavespectra-3.9.0/tests/core/test_watershed.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1665 2021-04-09 02:47:42.000000 wavespectra-3.9.0/tests/core/test_wave_stats.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.395734 wavespectra-3.9.0/tests/io/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1050 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/io/test_chunk_naming.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3272 2021-05-29 08:35:20.000000 wavespectra-3.9.0/tests/io/test_funwave.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3909 2021-05-29 08:35:20.000000 wavespectra-3.9.0/tests/io/test_io.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2020 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/io/test_json.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      848 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/io/test_ncswan.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2675 2021-02-12 03:05:43.000000 wavespectra-3.9.0/tests/io/test_ndbc.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1661 2021-03-30 08:47:13.000000 wavespectra-3.9.0/tests/io/test_octopus.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1140 2021-02-20 00:55:48.000000 wavespectra-3.9.0/tests/io/test_spotter.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1325 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/io/test_swan_ascii.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      840 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/io/test_triaxys.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.399734 wavespectra-3.9.0/tests/sample_files/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    73584 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/era5file.nc
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    14905 2021-05-29 08:35:20.000000 wavespectra-3.9.0/tests/sample_files/funwavefile.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    43800 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/jsonfile.json
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.403734 wavespectra-3.9.0/tests/sample_files/ndbc/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    99616 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010.data_spec
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10571 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010.spec
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    96852 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010.swdir
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    96789 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010.swdir2
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    94719 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010.swr1
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    94719 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010.swr2
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     7836 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010d2019part.txt.gz
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     8203 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010i2019part.txt.gz
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6427 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010j2019part.txt.gz
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6575 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010k2019part.txt.gz
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4897 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ndbc/41010w2019part.txt.gz
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1120 2021-02-12 03:05:43.000000 wavespectra-3.9.0/tests/sample_files/ndbc/44004w2000.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    41157 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/octopusfile.oct
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    36170 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/spotter_20180214.json
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    38843 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/swanfile.nc
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    23736 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/swanfile.spec
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1368 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/swanfile.tab
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      469 2021-04-09 02:47:42.000000 wavespectra-3.9.0/tests/sample_files/swanfile.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    92145 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/triaxys.DIRSPEC
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1785 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/triaxys.NONDIRSPEC
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69915 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/wavespectra.nc
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    48008 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.nc
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.403734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        2 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/.zgroup
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    14114 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/.zmetadata
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.407734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/cur/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/cur/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      336 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/cur/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      336 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/cur/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.407734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/curdir/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/curdir/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      390 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/curdir/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      611 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/curdir/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.407734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/direction/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      331 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/direction/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      328 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/direction/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      112 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/direction/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.411734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/dpt/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/dpt/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      307 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/dpt/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       77 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/dpt/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.411734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/efth/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      389 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/efth/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      522 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/efth/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    15172 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/efth/0.0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.411734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      331 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      316 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      116 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.411734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency1/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      339 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency1/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      355 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency1/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      125 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency1/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.415734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency2/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      339 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency2/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      355 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency2/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      125 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/frequency2/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.415734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/latitude/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/latitude/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      324 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/latitude/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       68 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/latitude/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.415734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/longitude/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/longitude/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      327 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/longitude/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       67 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/longitude/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.415734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/station/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      319 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/station/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      102 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/station/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/station/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.415734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/time/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      317 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/time/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      293 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/time/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      156 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/time/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.419734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnd/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnd/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      328 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnd/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      551 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnd/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.419734 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnddir/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      341 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnddir/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      344 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnddir/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      666 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnddir/0.0
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    52738 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/sample_files/wwmfile.nc
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      987 2020-10-01 10:30:02.000000 wavespectra-3.9.0/tests/test_cookiecutter_template.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.423734 wavespectra-3.9.0/wavespectra/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1493 2021-05-29 08:35:20.000000 wavespectra-3.9.0/wavespectra/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      410 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/cli.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.423734 wavespectra-3.9.0/wavespectra/construct/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      143 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/construct/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2344 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/construct/helpers.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1137 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/construct/jonswap.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1266 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/construct/ochihubble.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.423734 wavespectra-3.9.0/wavespectra/core/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/core/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1390 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/core/attributes.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2413 2021-04-09 02:47:42.000000 wavespectra-3.9.0/wavespectra/core/attributes.yml
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4071 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/core/npstats.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    12274 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/core/select.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     9041 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/core/swan.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5967 2021-04-09 02:47:42.000000 wavespectra-3.9.0/wavespectra/core/utils.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6036 2021-05-29 08:35:35.000000 wavespectra-3.9.0/wavespectra/core/watershed.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4197 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/core/xrstats.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.427734 wavespectra-3.9.0/wavespectra/input/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2568 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1819 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/dataset.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1710 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/era5.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1903 2021-05-29 08:35:20.000000 wavespectra-3.9.0/wavespectra/input/funwave.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1061 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/json.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3022 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/input/ncswan.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5698 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/ndbc.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1704 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/netcdf.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      276 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/octopus.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6206 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/spotter.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    19448 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/input/swan.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6967 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/input/triaxys.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1344 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/input/wavespectra.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2675 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/input/ww3.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2749 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/input/wwm.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.427734 wavespectra-3.9.0/wavespectra/output/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      726 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/output/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4485 2021-05-29 08:35:20.000000 wavespectra-3.9.0/wavespectra/output/funwave.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      775 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/output/json.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1251 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/output/netcdf.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     7571 2021-04-09 02:47:42.000000 wavespectra-3.9.0/wavespectra/output/octopus.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2777 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/output/swan.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3735 2021-03-30 08:47:13.000000 wavespectra-3.9.0/wavespectra/output/ww3.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3294 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/output/ww3.yml
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    25915 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/plot.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    24788 2021-04-09 02:47:42.000000 wavespectra-3.9.0/wavespectra/specarray.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6097 2021-03-10 22:13:13.000000 wavespectra-3.9.0/wavespectra/specdataset.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.427734 wavespectra-3.9.0/wavespectra/specpart/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    12334 2021-05-29 08:35:35.000000 wavespectra-3.9.0/wavespectra/specpart/specpart.f90
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      841 2021-05-29 08:35:35.000000 wavespectra-3.9.0/wavespectra/specpart/specpart.pyf
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2021-05-29 08:53:57.423734 wavespectra-3.9.0/wavespectra.egg-info/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     9180 2021-05-29 08:53:57.000000 wavespectra-3.9.0/wavespectra.egg-info/PKG-INFO
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    11408 2021-05-29 08:53:57.000000 wavespectra-3.9.0/wavespectra.egg-info/SOURCES.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        1 2021-05-29 08:53:57.000000 wavespectra-3.9.0/wavespectra.egg-info/dependency_links.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       54 2021-05-29 08:53:57.000000 wavespectra-3.9.0/wavespectra.egg-info/entry_points.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        1 2021-05-29 08:53:57.000000 wavespectra-3.9.0/wavespectra.egg-info/not-zip-safe
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      152 2021-05-29 08:53:57.000000 wavespectra-3.9.0/wavespectra.egg-info/requires.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       12 2021-05-29 08:53:57.000000 wavespectra-3.9.0/wavespectra.egg-info/top_level.txt
```

### Comparing `wavespectra-3.8.1/CONTRIBUTING.rst` & `wavespectra-3.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/HISTORY.rst` & `wavespectra-3.9.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,25 @@
 changelog covers the release history since v3.0 when wavespectra was open-sourced.
 
 
 ********
 Releases
 ********
 
+3.9.0 (2021-05-29)
+__________________
+
+New Features
+------------
+* Funwave spectra reader `read_funwave`_.
+* Funwave spectra writer `to_funwave`_.
+
+.. _`read_funwave`: https://github.com/wavespectra/wavespectra/blob/master/wavespectra/input/funwave.py
+.. _`to_funwave`: https://github.com/wavespectra/wavespectra/blob/master/wavespectra/output/funwave.py
+
 
 3.8.1 (2021-04-06)
 __________________
 
 Bug Fixes
 ---------
 * Add numba to setup.py, not installed properly from requirements/default.txt for some reason.
```

### Comparing `wavespectra-3.8.1/LICENSE.txt` & `wavespectra-3.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/PKG-INFO` & `wavespectra-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavespectra
-Version: 3.8.1
+Version: 3.9.0
 Summary: Library for ocean wave spectra
 Home-page: http://github.com/wavespectra/wavespectra
 Author: Wavespectra Developers
 Author-email: r.guedes@oceanum.science
 License: MIT license
 Project-URL: Source, https://github.com/wavespectra/wavespectra
 Project-URL: Bug Reports, https://github.com/wavespectra/wavespectra/issues
```

### Comparing `wavespectra-3.8.1/README.rst` & `wavespectra-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/Makefile` & `wavespectra-3.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/contour_type_plot.png` & `wavespectra-3.9.0/docs/_build/_images/contour_type_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/contourf_type_plot.png` & `wavespectra-3.9.0/docs/_build/_images/contourf_type_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/faceted_polar_plot.png` & `wavespectra-3.9.0/docs/_build/_images/faceted_polar_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/faceted_polar_plot2.png` & `wavespectra-3.9.0/docs/_build/_images/faceted_polar_plot2.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/faceted_polar_plot3.png` & `wavespectra-3.9.0/docs/_build/_images/faceted_polar_plot3.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/freq_split_hs.png` & `wavespectra-3.9.0/docs/_build/_images/freq_split_hs.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/hovmoller_plot.png` & `wavespectra-3.9.0/docs/_build/_images/hovmoller_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/hs.png` & `wavespectra-3.9.0/docs/_build/_images/hs.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/interp_stations_plot.png` & `wavespectra-3.9.0/docs/_build/_images/interp_stations_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/many_stats.png` & `wavespectra-3.9.0/docs/_build/_images/many_stats.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/single_polar_plot.png` & `wavespectra-3.9.0/docs/_build/_images/single_polar_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/single_polar_plot_ax_extent1.png` & `wavespectra-3.9.0/docs/_build/_images/single_polar_plot_ax_extent1.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/single_polar_plot_ax_extent2.png` & `wavespectra-3.9.0/docs/_build/_images/single_polar_plot_ax_extent2.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/single_polar_plot_ax_extent3.png` & `wavespectra-3.9.0/docs/_build/_images/single_polar_plot_ax_extent3.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/single_polar_plot_period.png` & `wavespectra-3.9.0/docs/_build/_images/single_polar_plot_period.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/single_polar_plot_period_realvalues.png` & `wavespectra-3.9.0/docs/_build/_images/single_polar_plot_period_realvalues.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/single_polar_plot_xarray_parameters.png` & `wavespectra-3.9.0/docs/_build/_images/single_polar_plot_xarray_parameters.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_clean_axis_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_clean_axis_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_clean_axis_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_clean_axis_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_faceting_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_faceting_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_faceting_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_faceting_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_hs_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_hs_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_hs_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_hs_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contour_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contour_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contour_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contour_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contourf_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contourf_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_contourf_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_contourf_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_pcolormesh_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_period_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_period_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_period_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_period_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_real_values_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_real_values_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_real_values_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_real_values_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_slice_radius_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_timeseries_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_timeseries_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_timeseries_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_timeseries_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_spectra_xarray_params_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_split_sea_swell_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_split_sea_swell_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_split_sea_swell_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_split_sea_swell_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_001.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_thumb.png` & `wavespectra-3.9.0/docs/_build/_images/sphx_glr_plot_watershed_sea_swell_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/watershed_hs.png` & `wavespectra-3.9.0/docs/_build/_images/watershed_hs.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_images/wavespectra_logo.png` & `wavespectra-3.9.0/docs/_build/_images/wavespectra_logo.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_static/broken_example.png` & `wavespectra-3.9.0/docs/_build/_static/broken_example.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_static/no_image.png` & `wavespectra-3.9.0/docs/_build/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_build/_static/wavespectra_logo.png` & `wavespectra-3.9.0/docs/_build/_static/wavespectra_logo.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/_static/wavespectra_logo.png` & `wavespectra-3.9.0/docs/_static/wavespectra_logo.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/api.rst` & `wavespectra-3.9.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_clean_axis_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_clean_axis_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_faceting_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_faceting_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_hs_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_hs_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_contour_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_contour_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_contourf_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_contourf_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_pcolormesh_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_pcolormesh_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_period_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_period_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_real_values_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_real_values_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_slice_radius_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_slice_radius_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_timeseries_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_timeseries_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_spectra_xarray_params_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_spectra_xarray_params_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_split_sea_swell_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_split_sea_swell_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/sphx_glr_plot_watershed_sea_swell_001.png` & `wavespectra-3.9.0/docs/auto_gallery/images/sphx_glr_plot_watershed_sea_swell_001.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_clean_axis_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_clean_axis_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_faceting_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_faceting_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_hs_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_hs_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contour_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contour_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contourf_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_contourf_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_pcolormesh_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_pcolormesh_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_period_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_period_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_real_values_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_real_values_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_slice_radius_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_slice_radius_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_timeseries_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_timeseries_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_xarray_params_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_spectra_xarray_params_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_split_sea_swell_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_split_sea_swell_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/images/thumb/sphx_glr_plot_watershed_sea_swell_thumb.png` & `wavespectra-3.9.0/docs/auto_gallery/images/thumb/sphx_glr_plot_watershed_sea_swell_thumb.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/index.rst` & `wavespectra-3.9.0/docs/auto_gallery/index.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_clean_axis.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_clean_axis.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_faceting.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_faceting.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_hs.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_hs.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_contour.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_contour.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_contourf.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_contourf.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_pcolormesh.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_pcolormesh.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_period.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_period.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_real_values.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_real_values.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_slice_radius.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_slice_radius.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_timeseries.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_timeseries.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_spectra_xarray_params.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_spectra_xarray_params.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_split_sea_swell.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_split_sea_swell.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/plot_watershed_sea_swell.rst` & `wavespectra-3.9.0/docs/auto_gallery/plot_watershed_sea_swell.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/auto_gallery/sg_execution_times.rst` & `wavespectra-3.9.0/docs/auto_gallery/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/conf.py` & `wavespectra-3.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/conventions.rst` & `wavespectra-3.9.0/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/index.rst` & `wavespectra-3.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/install.rst` & `wavespectra-3.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/io-input.rst` & `wavespectra-3.9.0/docs/io-input.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/io-output.rst` & `wavespectra-3.9.0/docs/io-output.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/library.rst` & `wavespectra-3.9.0/docs/library.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/make.bat` & `wavespectra-3.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/plotting.rst` & `wavespectra-3.9.0/docs/plotting.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/quickstart.rst` & `wavespectra-3.9.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/contour_type_plot.png` & `wavespectra-3.9.0/docs/savefig/contour_type_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/contourf_type_plot.png` & `wavespectra-3.9.0/docs/savefig/contourf_type_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/contourf_type_plot9.png` & `wavespectra-3.9.0/docs/savefig/contourf_type_plot9.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/faceted_polar_plot.png` & `wavespectra-3.9.0/docs/savefig/faceted_polar_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/faceted_polar_plot2.png` & `wavespectra-3.9.0/docs/savefig/faceted_polar_plot2.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/faceted_polar_plot3.png` & `wavespectra-3.9.0/docs/savefig/faceted_polar_plot3.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/freq_split_hs.png` & `wavespectra-3.9.0/docs/savefig/freq_split_hs.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/hovmoller_plot.png` & `wavespectra-3.9.0/docs/savefig/hovmoller_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/hs.png` & `wavespectra-3.9.0/docs/savefig/hs.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/interp_stations_plot.png` & `wavespectra-3.9.0/docs/savefig/interp_stations_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/many_stats.png` & `wavespectra-3.9.0/docs/savefig/many_stats.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/pcolormesh_type_plot.png` & `wavespectra-3.9.0/docs/savefig/pcolormesh_type_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/single_polar_plot.png` & `wavespectra-3.9.0/docs/savefig/single_polar_plot.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/single_polar_plot_ax_extent1.png` & `wavespectra-3.9.0/docs/savefig/single_polar_plot_ax_extent1.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/single_polar_plot_ax_extent2.png` & `wavespectra-3.9.0/docs/savefig/single_polar_plot_ax_extent2.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/single_polar_plot_ax_extent3.png` & `wavespectra-3.9.0/docs/savefig/single_polar_plot_ax_extent3.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/single_polar_plot_period.png` & `wavespectra-3.9.0/docs/savefig/single_polar_plot_period.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/single_polar_plot_period_realvalues.png` & `wavespectra-3.9.0/docs/savefig/single_polar_plot_period_realvalues.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/single_polar_plot_xarray_parameters.png` & `wavespectra-3.9.0/docs/savefig/single_polar_plot_xarray_parameters.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/savefig/watershed_hs.png` & `wavespectra-3.9.0/docs/savefig/watershed_hs.png`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/docs/selecting.rst` & `wavespectra-3.9.0/docs/selecting.rst`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/setup.cfg` & `wavespectra-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/setup.py` & `wavespectra-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/core/test_construct.py` & `wavespectra-3.9.0/tests/core/test_construct.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/core/test_core.py` & `wavespectra-3.9.0/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/core/test_dset_wrapper.py` & `wavespectra-3.9.0/tests/core/test_dset_wrapper.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/core/test_plot.py` & `wavespectra-3.9.0/tests/core/test_plot.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/core/test_sel.py` & `wavespectra-3.9.0/tests/core/test_sel.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/core/test_watershed.py` & `wavespectra-3.9.0/tests/core/test_watershed.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/core/test_wave_stats.py` & `wavespectra-3.9.0/tests/core/test_wave_stats.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_chunk_naming.py` & `wavespectra-3.9.0/tests/io/test_chunk_naming.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_io.py` & `wavespectra-3.9.0/tests/io/test_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,24 @@
     read_ww3,
     read_octopus,
     read_ncswan,
     read_triaxys,
     read_wwm,
     read_dataset,
     read_era5,
-    read_wavespectra
+    read_wavespectra,
+    read_funwave,
 )
 
 FILES_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../sample_files")
 
 
 class TestIO(object):
     """Test reading and writing of different file formats.
-    
+
     Extend IO tests by adding tuple to parametrize, e.g.:
         ('filename', read_{filetype}, 'to_{filetype}')
     Use None for 'to_{filetype} if there is no output method defined'.
 
     """
 
     @classmethod
@@ -44,31 +45,31 @@
         [
             ("swanfile.spec", read_swan, "to_swan"),
             ("ww3file.nc", read_ww3, "to_ww3"),
             ("swanfile.nc", read_ncswan, None),
             ("triaxys.DIRSPEC", read_triaxys, None),
             ("triaxys.NONDIRSPEC", read_triaxys, None),
             ("wavespectra.nc", read_netcdf, "to_netcdf"),
-            ("era5file.nc", read_era5, None)
+            ("era5file.nc", read_era5, None),
+            ("funwavefile.txt", read_funwave, "to_funwave"),
         ],
     )
     def test_io(self, filename, read_func, write_method_name):
         self.filename = filename
         self.read_func = read_func
         self.write_method_name = write_method_name
         # Execute io tests in order
         self._read()
         if self.write_method_name is not None:
             try:
                 self._write()
                 self._check()
             except NotImplementedError:
-                pytest.skip("Writing function {} not implemented yet".format(
-                    write_method_name
-                    )
+                pytest.skip(
+                    "Writing function {} not implemented yet".format(write_method_name)
                 )
         else:
             print(
                 "No output method defined for {}, "
                 "skipping output tests".format(filename)
             )
```

### Comparing `wavespectra-3.8.1/tests/io/test_json.py` & `wavespectra-3.9.0/tests/io/test_json.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_ncswan.py` & `wavespectra-3.9.0/tests/io/test_ncswan.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_ndbc.py` & `wavespectra-3.9.0/tests/io/test_ndbc.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_octopus.py` & `wavespectra-3.9.0/tests/io/test_octopus.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_spotter.py` & `wavespectra-3.9.0/tests/io/test_spotter.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_swan_ascii.py` & `wavespectra-3.9.0/tests/io/test_swan_ascii.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/io/test_triaxys.py` & `wavespectra-3.9.0/tests/io/test_triaxys.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/era5file.nc` & `wavespectra-3.9.0/tests/sample_files/era5file.nc`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/jsonfile.json` & `wavespectra-3.9.0/tests/sample_files/jsonfile.json`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010.data_spec` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010.data_spec`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010.spec` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010.spec`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010.swdir` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010.swdir`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010.swdir2` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010.swdir2`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010.swr1` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010.swr1`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010.swr2` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010.swr2`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010d2019part.txt.gz` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010d2019part.txt.gz`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010i2019part.txt.gz` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010i2019part.txt.gz`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010j2019part.txt.gz` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010j2019part.txt.gz`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010k2019part.txt.gz` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010k2019part.txt.gz`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/41010w2019part.txt.gz` & `wavespectra-3.9.0/tests/sample_files/ndbc/41010w2019part.txt.gz`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ndbc/44004w2000.txt` & `wavespectra-3.9.0/tests/sample_files/ndbc/44004w2000.txt`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/octopusfile.oct` & `wavespectra-3.9.0/tests/sample_files/octopusfile.oct`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/spotter_20180214.json` & `wavespectra-3.9.0/tests/sample_files/spotter_20180214.json`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/swanfile.nc` & `wavespectra-3.9.0/tests/sample_files/swanfile.nc`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/swanfile.spec` & `wavespectra-3.9.0/tests/sample_files/swanfile.spec`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/swanfile.tab` & `wavespectra-3.9.0/tests/sample_files/swanfile.tab`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/triaxys.DIRSPEC` & `wavespectra-3.9.0/tests/sample_files/triaxys.DIRSPEC`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/triaxys.NONDIRSPEC` & `wavespectra-3.9.0/tests/sample_files/triaxys.NONDIRSPEC`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/wavespectra.nc` & `wavespectra-3.9.0/tests/sample_files/wavespectra.nc`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ww3file.nc` & `wavespectra-3.9.0/tests/sample_files/ww3file.nc`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ww3file.zarr/.zmetadata` & `wavespectra-3.9.0/tests/sample_files/ww3file.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ww3file.zarr/curdir/0.0` & `wavespectra-3.9.0/tests/sample_files/ww3file.zarr/curdir/0.0`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ww3file.zarr/efth/.zattrs` & `wavespectra-3.9.0/tests/sample_files/ww3file.zarr/efth/.zattrs`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ww3file.zarr/efth/0.0.0.0` & `wavespectra-3.9.0/tests/sample_files/ww3file.zarr/efth/0.0.0.0`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnd/0.0` & `wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnd/0.0`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/ww3file.zarr/wnddir/0.0` & `wavespectra-3.9.0/tests/sample_files/ww3file.zarr/wnddir/0.0`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/sample_files/wwmfile.nc` & `wavespectra-3.9.0/tests/sample_files/wwmfile.nc`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/tests/test_cookiecutter_template.py` & `wavespectra-3.9.0/tests/test_cookiecutter_template.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/__init__.py` & `wavespectra-3.9.0/wavespectra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 try:
     from wavespectra.specdataset import SpecDataset
     from wavespectra.specarray import SpecArray
 except ImportError:
     warnings.warn("Cannot import accessors at the main module level")
 
 
-__version__ = "3.8.1"
+__version__ = "3.9.0"
 __author__ = "Wavespectra Developers"
 __contact__ = "r.guedes@oceanum.science"
 __url__ = "http://github.com/wavespectra/wavespectra"
 __description__ = "Library for ocean wave spectra"
 __keywords__ = "wave spectra ocean xarray statistics analysis"
```

### Comparing `wavespectra-3.8.1/wavespectra/construct/helpers.py` & `wavespectra-3.9.0/wavespectra/construct/helpers.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/construct/jonswap.py` & `wavespectra-3.9.0/wavespectra/construct/jonswap.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/construct/ochihubble.py` & `wavespectra-3.9.0/wavespectra/construct/ochihubble.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/attributes.py` & `wavespectra-3.9.0/wavespectra/core/attributes.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/attributes.yml` & `wavespectra-3.9.0/wavespectra/core/attributes.yml`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/npstats.py` & `wavespectra-3.9.0/wavespectra/core/npstats.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/select.py` & `wavespectra-3.9.0/wavespectra/core/select.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/swan.py` & `wavespectra-3.9.0/wavespectra/core/swan.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/utils.py` & `wavespectra-3.9.0/wavespectra/core/utils.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/watershed.py` & `wavespectra-3.9.0/wavespectra/core/watershed.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/core/xrstats.py` & `wavespectra-3.9.0/wavespectra/core/xrstats.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/__init__.py` & `wavespectra-3.9.0/wavespectra/input/__init__.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/dataset.py` & `wavespectra-3.9.0/wavespectra/input/dataset.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/era5.py` & `wavespectra-3.9.0/wavespectra/input/era5.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/json.py` & `wavespectra-3.9.0/wavespectra/input/json.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/ncswan.py` & `wavespectra-3.9.0/wavespectra/input/ncswan.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/ndbc.py` & `wavespectra-3.9.0/wavespectra/input/ndbc.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/netcdf.py` & `wavespectra-3.9.0/wavespectra/input/netcdf.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/spotter.py` & `wavespectra-3.9.0/wavespectra/input/spotter.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/swan.py` & `wavespectra-3.9.0/wavespectra/input/swan.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/triaxys.py` & `wavespectra-3.9.0/wavespectra/input/triaxys.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/wavespectra.py` & `wavespectra-3.9.0/wavespectra/input/wavespectra.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/ww3.py` & `wavespectra-3.9.0/wavespectra/input/ww3.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/input/wwm.py` & `wavespectra-3.9.0/wavespectra/input/wwm.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/output/__init__.py` & `wavespectra-3.9.0/wavespectra/output/__init__.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/output/json.py` & `wavespectra-3.9.0/wavespectra/output/json.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/output/netcdf.py` & `wavespectra-3.9.0/wavespectra/output/netcdf.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/output/octopus.py` & `wavespectra-3.9.0/wavespectra/output/octopus.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/output/swan.py` & `wavespectra-3.9.0/wavespectra/output/swan.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/output/ww3.py` & `wavespectra-3.9.0/wavespectra/output/ww3.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/output/ww3.yml` & `wavespectra-3.9.0/wavespectra/output/ww3.yml`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/plot.py` & `wavespectra-3.9.0/wavespectra/plot.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/specarray.py` & `wavespectra-3.9.0/wavespectra/specarray.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/specdataset.py` & `wavespectra-3.9.0/wavespectra/specdataset.py`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/specpart/specpart.f90` & `wavespectra-3.9.0/wavespectra/specpart/specpart.f90`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra/specpart/specpart.pyf` & `wavespectra-3.9.0/wavespectra/specpart/specpart.pyf`

 * *Files identical despite different names*

### Comparing `wavespectra-3.8.1/wavespectra.egg-info/PKG-INFO` & `wavespectra-3.9.0/wavespectra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavespectra
-Version: 3.8.1
+Version: 3.9.0
 Summary: Library for ocean wave spectra
 Home-page: http://github.com/wavespectra/wavespectra
 Author: Wavespectra Developers
 Author-email: r.guedes@oceanum.science
 License: MIT license
 Project-URL: Source, https://github.com/wavespectra/wavespectra
 Project-URL: Bug Reports, https://github.com/wavespectra/wavespectra/issues
```

