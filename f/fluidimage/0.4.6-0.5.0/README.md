# Comparing `tmp/fluidimage-0.4.6.tar.gz` & `tmp/fluidimage-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidimage-0.4.6.tar", last modified: Sat Apr 20 06:44:33 2024, max compression
+gzip compressed data, was "fluidimage-0.5.0.tar", last modified: Thu May  2 10:24:20 2024, max compression
```

## Comparing `fluidimage-0.4.6.tar` & `fluidimage-0.5.0.tar`

### file list

```diff
@@ -1,262 +1,263 @@
--rw-r--r--   0        0        0       58 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.flake8
--rw-r--r--   0        0        0     1166 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.github/workflows/ci-linux.yml
--rw-r--r--   0        0        0      554 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.github/workflows/ci-pixi.yml
--rw-r--r--   0        0        0     3919 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     3223 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.gitlab-ci.yml
--rw-r--r--   0        0        0     1057 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.hgtags
--rw-r--r--   0        0        0       43 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.mdformat.toml
--rw-r--r--   0        0        0      376 2024-04-20 06:38:01.000000 fluidimage-0.4.6/.readthedocs.yml
--rw-r--r--   0        0        0      210 2024-04-20 06:38:01.000000 fluidimage-0.4.6/AUTHORS.md
--rw-r--r--   0        0        0     7098 2024-04-20 06:38:01.000000 fluidimage-0.4.6/CHANGES.md
--rw-r--r--   0        0        0     1266 2024-04-20 06:38:01.000000 fluidimage-0.4.6/CONTRIBUTING.md
--rw-r--r--   0        0        0    21781 2024-04-20 06:38:01.000000 fluidimage-0.4.6/LICENSE.txt
--rw-r--r--   0        0        0      205 2024-04-20 06:38:01.000000 fluidimage-0.4.6/MANIFEST.in
--rw-r--r--   0        0        0      309 2024-04-20 06:38:01.000000 fluidimage-0.4.6/Makefile
--rw-r--r--   0        0        0     3151 2024-04-20 06:38:01.000000 fluidimage-0.4.6/README.md
--rw-r--r--   0        0        0     1266 2024-04-20 06:44:33.502598 fluidimage-0.4.6/doc/CONTRIBUTING.md
--rw-r--r--   0        0        0     5780 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/Makefile
--rw-r--r--   0        0        0      210 2024-04-20 06:44:33.502598 fluidimage-0.4.6/doc/authors.md
--rw-r--r--   0        0        0      412 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/autosum.rst
--rw-r--r--   0        0        0     8443 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/build-from-source.md
--rw-r--r--   0        0        0     7098 2024-04-20 06:44:33.502598 fluidimage-0.4.6/doc/changes.md
--rw-r--r--   0        0        0     9545 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/conf.py
--rw-r--r--   0        0        0       36 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/Makefile
--rw-r--r--   0        0        0      275 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/bos_parallel.md
--rw-r--r--   0        0        0      708 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/bos_parallel.py
--rw-r--r--   0        0        0      914 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/im2im_parallel.py
--rw-r--r--   0        0        0      442 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/im2im_try_params.py
--rw-r--r--   0        0        0      217 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/my_example_im2im.py
--rw-r--r--   0        0        0      370 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/my_example_im2im_class.py
--rw-r--r--   0        0        0      375 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/optflow_parallel.md
--rw-r--r--   0        0        0      864 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/optflow_parallel.py
--rw-r--r--   0        0        0      645 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/optflow_try_params.md
--rw-r--r--   0        0        0      675 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/optflow_try_params.py
--rw-r--r--   0        0        0     2124 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/README.md
--rw-r--r--   0        0        0        0 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/args.py
--rwxr-xr-x   0        0        0      779 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/job_piv.py
--rwxr-xr-x   0        0        0     1095 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/job_pre.py
--rwxr-xr-x   0        0        0     2087 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/params_piv.py
--rwxr-xr-x   0        0        0     1811 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/params_pre.py
--rwxr-xr-x   0        0        0      672 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/submit_piv.py
--rwxr-xr-x   0        0        0      787 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/submit_pre.py
--rw-r--r--   0        0        0      896 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/test_piv_as_real.py
--rwxr-xr-x   0        0        0      724 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/try_piv.py
--rwxr-xr-x   0        0        0      538 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_as_real/try_pre.py
--rw-r--r--   0        0        0      457 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_cluster.md
--rw-r--r--   0        0        0      918 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_parallel.md
--rw-r--r--   0        0        0      827 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_parallel.py
--rw-r--r--   0        0        0      536 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_parallel_complete.py
--rw-r--r--   0        0        0      953 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_parallel_im2im.py
--rw-r--r--   0        0        0      989 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_parallel_im2im_class.py
--rw-r--r--   0        0        0      863 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_try_params.md
--rw-r--r--   0        0        0      614 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_try_params.py
--rw-r--r--   0        0        0      655 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_try_params_Karman.py
--rw-r--r--   0        0        0      814 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/piv_try_params_with_im2im_preproc.py
--rw-r--r--   0        0        0      380 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/README.md
--rw-r--r--   0        0        0      908 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/bench_piv_2005C.py
--rw-r--r--   0        0        0     1419 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/download.py
--rw-r--r--   0        0        0      744 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/path_images.py
--rw-r--r--   0        0        0      437 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/piv_2001A_topology.py
--rw-r--r--   0        0        0      496 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/piv_2001A_work.py
--rw-r--r--   0        0        0      548 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/piv_2005C_topology.py
--rw-r--r--   0        0        0      682 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/piv_2005C_work.py
--rw-r--r--   0        0        0      117 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/pivchallenge/possible_paths.txt
--rw-r--r--   0        0        0     1413 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/preproc.md
--rw-r--r--   0        0        0     1061 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/preproc_parallel.py
--rw-r--r--   0        0        0      816 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/preproc_sback1_filter.py
--rw-r--r--   0        0        0     1037 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/preproc_sback2_rescale.py
--rw-r--r--   0        0        0      544 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/preproc_try_params.py
--rw-r--r--   0        0        0      364 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/preproc_try_params_opencv.py
--rw-r--r--   0        0        0     1553 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/profile_piv_work.py
--rw-r--r--   0        0        0      448 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/submit_job_legi.py
--rw-r--r--   0        0        0      711 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/surface_tracking.py
--rw-r--r--   0        0        0     1201 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples/test_run_examples.py
--rw-r--r--   0        0        0      357 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/examples.md
--rw-r--r--   0        0        0      238 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/for_dev.md
--rw-r--r--   0        0        0      673 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/index.md
--rw-r--r--   0        0        0     1686 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/install.md
--rw-r--r--   0        0        0      405 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/ipynbslides/README.txt
--rw-r--r--   0        0        0   493343 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/ipynbslides/fluidimage_legi_20170403.ipynb
--rw-r--r--   0        0        0     2094 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/overview.md
--rw-r--r--   0        0        0     1424 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/overview_orga_package.md
--rw-r--r--   0        0        0     1857 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/related_codes.md
--rw-r--r--   0        0        0       77 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/to_do.md
--rw-r--r--   0        0        0      432 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorial.md
--rw-r--r--   0        0        0     3116 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorials/tuto_calibration2dsimple.md
--rw-r--r--   0        0        0     2412 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorials/tuto_direct_calibration.md
--rw-r--r--   0        0        0     7352 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorials/tuto_opencv_calibration.md
--rw-r--r--   0        0        0     4407 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorials/tuto_opencv_tomo_reconstruct.md
--rw-r--r--   0        0        0     8785 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorials/tuto_piv.md
--rw-r--r--   0        0        0     2950 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorials/tuto_stereo_reconstruction.md
--rw-r--r--   0        0        0     1367 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/tutorials/tuto_tsai_calibration.md
--rw-r--r--   0        0        0     8971 2024-04-20 06:38:01.000000 fluidimage-0.4.6/doc/uvmat.md
--rw-r--r--   0        0        0     1252 2024-04-20 06:38:01.000000 fluidimage-0.4.6/docker/Dockerfile
--rw-r--r--   0        0        0     1147 2024-04-20 06:38:01.000000 fluidimage-0.4.6/docker/Makefile
--rw-r--r--   0        0        0      618 2024-04-20 06:38:01.000000 fluidimage-0.4.6/docker/hgrc
--rw-r--r--   0        0        0       77 2024-04-20 06:38:01.000000 fluidimage-0.4.6/docker/pythranrc
--rw-r--r--   0        0        0     1803 2024-04-20 06:38:01.000000 fluidimage-0.4.6/meson.build
--rw-r--r--   0        0        0      655 2024-04-20 06:38:01.000000 fluidimage-0.4.6/meson.options
--rw-r--r--   0        0        0     4888 2024-04-20 06:38:01.000000 fluidimage-0.4.6/noxfile.py
--rw-r--r--   0        0        0   310844 2024-04-20 06:38:01.000000 fluidimage-0.4.6/pdm.lock
--rw-r--r--   0        0        0   594569 2024-04-20 06:38:01.000000 fluidimage-0.4.6/pixi.lock
--rw-r--r--   0        0        0      993 2024-04-20 06:38:01.000000 fluidimage-0.4.6/pixi.toml
--rw-r--r--   0        0        0    21630 2024-04-20 06:38:01.000000 fluidimage-0.4.6/pylintrc
--rw-r--r--   0        0        0     4483 2024-04-20 06:38:01.000000 fluidimage-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     3311 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/__init__.py
--rw-r--r--   0        0        0      534 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/_opencv.py
--rw-r--r--   0        0        0      162 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/_version.py
--rw-r--r--   0        0        0      278 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/bos.py
--rw-r--r--   0        0        0      263 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/__init__.py
--rw-r--r--   0        0        0     2858 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/_evaluate_subpix.py
--rw-r--r--   0        0        0      878 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/correl.cu
--rw-r--r--   0        0        0    21039 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/correl.py
--rw-r--r--   0        0        0    10794 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/correl_pycuda.py
--rw-r--r--   0        0        0      333 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/errors.py
--rw-r--r--   0        0        0     7467 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/fft.py
--rw-r--r--   0        0        0      132 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/interpolate/__init__.py
--rw-r--r--   0        0        0      613 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/interpolate/griddata.py
--rw-r--r--   0        0        0      388 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/interpolate/meson.build
--rw-r--r--   0        0        0      863 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py
--rw-r--r--   0        0        0     8006 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/interpolate/thin_plate_spline.py
--rw-r--r--   0        0        0     7878 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py
--rw-r--r--   0        0        0     4807 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/mean_neighbors.py
--rw-r--r--   0        0        0      489 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/meson.build
--rw-r--r--   0        0        0    39595 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    37615 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    36317 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    35832 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    37828 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    38146 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    36451 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    34562 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0     1188 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/reduction_kernel.cu
--rw-r--r--   0        0        0     6180 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/subpix.py
--rw-r--r--   0        0        0     6544 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/test_correl.py
--rw-r--r--   0        0        0     2519 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calcul/test_fft.py
--rw-r--r--   0        0        0      465 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/__init__.py
--rw-r--r--   0        0        0     3587 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/calib2d_simple.py
--rw-r--r--   0        0        0     9318 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/calib_cv.py
--rw-r--r--   0        0        0    23798 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/calib_direct.py
--rw-r--r--   0        0        0     7528 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/calib_tsai.py
--rw-r--r--   0        0        0      302 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/meson.build
--rw-r--r--   0        0        0     2033 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/test_calib_cv.py
--rw-r--r--   0        0        0     2609 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/test_direct_stereo_reconstruction.py
--rw-r--r--   0        0        0     1302 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/test_tsai_calibration.py
--rw-r--r--   0        0        0     4272 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/calibration/util.py
--rw-r--r--   0        0        0      635 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/config.py
--rw-r--r--   0        0        0     1434 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/conftest.py
--rw-r--r--   0        0        0      274 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/__init__.py
--rw-r--r--   0        0        0    13257 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/display_piv.py
--rw-r--r--   0        0        0     4822 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/display_pre.py
--rw-r--r--   0        0        0      214 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/meson.build
--rw-r--r--   0        0        0    25845 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/piv.py
--rw-r--r--   0        0        0     4457 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/preproc.py
--rw-r--r--   0        0        0      425 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/test_piv.py
--rw-r--r--   0        0        0     9009 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/data_objects/tomo.py
--rw-r--r--   0        0        0     3376 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/__init__.py
--rw-r--r--   0        0        0    17789 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/base.py
--rw-r--r--   0        0        0    10536 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/exec_async.py
--rw-r--r--   0        0        0     4054 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/exec_async_multiproc.py
--rw-r--r--   0        0        0     3892 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/exec_async_seq_for_multi.py
--rw-r--r--   0        0        0     2106 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/exec_async_sequential.py
--rw-r--r--   0        0        0     8058 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/exec_async_servers.py
--rw-r--r--   0        0        0      396 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/exec_async_servers_threading.py
--rw-r--r--   0        0        0     2210 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/exec_sequential.py
--rw-r--r--   0        0        0      393 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/meson.build
--rw-r--r--   0        0        0     7358 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/multi_exec_async.py
--rw-r--r--   0        0        0     3668 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/multi_exec_subproc.py
--rw-r--r--   0        0        0     7661 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/executors/servers.py
--rw-r--r--   0        0        0      338 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/__init__.py
--rw-r--r--   0        0        0      769 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/base_matplotlib.py
--rw-r--r--   0        0        0     8981 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/imviewer.py
--rw-r--r--   0        0        0      228 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/launcher/Makefile
--rw-r--r--   0        0        0      153 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/launcher/__init__.py
--rw-r--r--   0        0        0     2659 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/launcher/main.py
--rw-r--r--   0        0        0     3750 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/launcher/mainwindow.py
--rw-r--r--   0        0        0     1671 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/launcher/mainwindow.ui
--rw-r--r--   0        0        0      170 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/launcher/meson.build
--rw-r--r--   0        0        0      568 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/launcher/test_launcher.py
--rw-r--r--   0        0        0      348 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/meson.build
--rw-r--r--   0        0        0    10974 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/monitor.py
--rw-r--r--   0        0        0       67 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/monitor.tcss
--rw-r--r--   0        0        0     2459 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/pg_main.py
--rw-r--r--   0        0        0     5903 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/pg_wrapper.py
--rw-r--r--   0        0        0     6018 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/piv_viewer.py
--rw-r--r--   0        0        0     1093 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/test_imviewer.py
--rw-r--r--   0        0        0      965 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/test_imviewer_pg.py
--rw-r--r--   0        0        0     2727 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/test_monitor.py
--rw-r--r--   0        0        0     1132 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/gui/test_piv_viewer.py
--rw-r--r--   0        0        0     2612 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/image2image.py
--rw-r--r--   0        0        0      529 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/meson.build
--rw-r--r--   0        0        0      337 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/optical_flow.py
--rw-r--r--   0        0        0      278 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/piv.py
--rw-r--r--   0        0        0      104 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/__init__.py
--rw-r--r--   0        0        0      210 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/meson.build
--rw-r--r--   0        0        0     2412 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/piv.py
--rw-r--r--   0        0        0    14134 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/postproc.py
--rw-r--r--   0        0        0     2927 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/test_piv.py
--rw-r--r--   0        0        0     3771 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/test_util.py
--rw-r--r--   0        0        0     4070 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/util.py
--rw-r--r--   0        0        0    24145 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/postproc/vector_field.py
--rw-r--r--   0        0        0      580 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/preproc.py
--rw-r--r--   0        0        0      351 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/reconstruct/__init__.py
--rw-r--r--   0        0        0      131 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/reconstruct/meson.build
--rw-r--r--   0        0        0      230 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/reconstruct/tomo/__init__.py
--rw-r--r--   0        0        0      151 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/reconstruct/tomo/meson.build
--rw-r--r--   0        0        0     7578 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/reconstruct/tomo/mlos.py
--rw-r--r--   0        0        0     1362 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/reconstruct/tomo/test_mlos.py
--rw-r--r--   0        0        0     8009 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/run_from_xml.py
--rw-r--r--   0        0        0     1516 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/synthetic.py
--rw-r--r--   0        0        0      521 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/test_image2image.py
--rw-r--r--   0        0        0     1407 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/test_run_from_xml.py
--rw-r--r--   0        0        0     2874 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/__init__.py
--rw-r--r--   0        0        0    17551 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/base.py
--rw-r--r--   0        0        0     6355 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/bos.py
--rw-r--r--   0        0        0     5706 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/example.py
--rw-r--r--   0        0        0     3999 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/image2image.py
--rw-r--r--   0        0        0     2497 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/launcher.py
--rw-r--r--   0        0        0    10209 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/log.py
--rw-r--r--   0        0        0      642 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/meson.build
--rw-r--r--   0        0        0     1422 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/nb_cpu_cores.py
--rw-r--r--   0        0        0     1020 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/optical_flow.py
--rw-r--r--   0        0        0     8447 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/piv.py
--rw-r--r--   0        0        0    10337 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/preproc.py
--rw-r--r--   0        0        0     8772 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/splitters.py
--rw-r--r--   0        0        0    10745 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/surface_tracking.py
--rw-r--r--   0        0        0     1347 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_bos.py
--rw-r--r--   0        0        0     1993 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_example.py
--rw-r--r--   0        0        0     1628 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_image2image.py
--rw-r--r--   0        0        0     1220 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_optical_flow.py
--rw-r--r--   0        0        0     2578 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_piv.py
--rw-r--r--   0        0        0     1773 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_preproc.py
--rw-r--r--   0        0        0     1919 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_splitters.py
--rw-r--r--   0        0        0     2251 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/topologies/test_surftracking.py
--rw-r--r--   0        0        0      683 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/util/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/util/log.py
--rw-r--r--   0        0        0      151 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/util/meson.build
--rw-r--r--   0        0        0      398 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/util/test_util.py
--rw-r--r--   0        0        0     2789 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/util/util.py
--rw-r--r--   0        0        0     6699 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/bos.py
--rw-r--r--   0        0        0     2687 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/image2image.py
--rw-r--r--   0        0        0      301 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/meson.build
--rw-r--r--   0        0        0     6651 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/optical_flow.py
--rw-r--r--   0        0        0      198 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/piv/__init__.py
--rw-r--r--   0        0        0     7836 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/piv/fix.py
--rw-r--r--   0        0        0      179 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/piv/meson.build
--rw-r--r--   0        0        0     6361 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/piv/multipass.py
--rw-r--r--   0        0        0    25776 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/piv/singlepass.py
--rw-r--r--   0        0        0     2456 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/piv/test_piv.py
--rw-r--r--   0        0        0     4587 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/preproc/__init__.py
--rw-r--r--   0        0        0     3844 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/preproc/_toolbox_cv.py
--rw-r--r--   0        0        0    14387 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/preproc/_toolbox_py.py
--rw-r--r--   0        0        0     2213 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/preproc/io.py
--rw-r--r--   0        0        0      184 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/preproc/meson.build
--rw-r--r--   0        0        0     3977 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/preproc/toolbox.py
--rw-r--r--   0        0        0    22183 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/surface_tracking.py
--rw-r--r--   0        0        0      776 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/test_bos.py
--rw-r--r--   0        0        0      542 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/test_image2image.py
--rw-r--r--   0        0        0     1815 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/test_preproc.py
--rw-r--r--   0        0        0     1307 2024-04-20 06:38:01.000000 fluidimage-0.4.6/src/fluidimage/works/with_mask.py
--rw-r--r--   0        0        0     4742 2024-04-20 06:44:33.981539 fluidimage-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0       58 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.flake8
+-rw-r--r--   0        0        0     1166 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.github/workflows/ci-linux.yml
+-rw-r--r--   0        0        0      554 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.github/workflows/ci-pixi.yml
+-rw-r--r--   0        0        0     3919 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     3223 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1104 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.hgtags
+-rw-r--r--   0        0        0       43 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.mdformat.toml
+-rw-r--r--   0        0        0      376 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0      210 2024-05-02 10:23:27.000000 fluidimage-0.5.0/AUTHORS.md
+-rw-r--r--   0        0        0     7457 2024-05-02 10:23:27.000000 fluidimage-0.5.0/CHANGES.md
+-rw-r--r--   0        0        0     1266 2024-05-02 10:23:27.000000 fluidimage-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    21781 2024-05-02 10:23:27.000000 fluidimage-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      205 2024-05-02 10:23:27.000000 fluidimage-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0      309 2024-05-02 10:23:27.000000 fluidimage-0.5.0/Makefile
+-rw-r--r--   0        0        0     3151 2024-05-02 10:23:27.000000 fluidimage-0.5.0/README.md
+-rw-r--r--   0        0        0     1266 2024-05-02 10:24:19.935472 fluidimage-0.5.0/doc/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5780 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/Makefile
+-rw-r--r--   0        0        0      210 2024-05-02 10:24:19.935472 fluidimage-0.5.0/doc/authors.md
+-rw-r--r--   0        0        0      748 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/autosum.rst
+-rw-r--r--   0        0        0     8443 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/build-from-source.md
+-rw-r--r--   0        0        0     7457 2024-05-02 10:24:19.935472 fluidimage-0.5.0/doc/changes.md
+-rw-r--r--   0        0        0     9545 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/conf.py
+-rw-r--r--   0        0        0       36 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/Makefile
+-rw-r--r--   0        0        0      275 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/bos_parallel.md
+-rw-r--r--   0        0        0      708 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/bos_parallel.py
+-rw-r--r--   0        0        0      914 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/im2im_parallel.py
+-rw-r--r--   0        0        0      442 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/im2im_try_params.py
+-rw-r--r--   0        0        0      217 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/my_example_im2im.py
+-rw-r--r--   0        0        0      370 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/my_example_im2im_class.py
+-rw-r--r--   0        0        0      375 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_parallel.md
+-rw-r--r--   0        0        0      864 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_parallel.py
+-rw-r--r--   0        0        0      645 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_try_params.md
+-rw-r--r--   0        0        0      675 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_try_params.py
+-rw-r--r--   0        0        0     2124 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/__init__.py
+-rw-r--r--   0        0        0     1386 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/args.py
+-rwxr-xr-x   0        0        0      779 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/job_piv.py
+-rwxr-xr-x   0        0        0     1095 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/job_pre.py
+-rwxr-xr-x   0        0        0     2087 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/params_piv.py
+-rwxr-xr-x   0        0        0     1811 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/params_pre.py
+-rwxr-xr-x   0        0        0      672 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/submit_piv.py
+-rwxr-xr-x   0        0        0      787 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/submit_pre.py
+-rw-r--r--   0        0        0      896 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/test_piv_as_real.py
+-rwxr-xr-x   0        0        0      724 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/try_piv.py
+-rwxr-xr-x   0        0        0      538 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/try_pre.py
+-rw-r--r--   0        0        0      457 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_cluster.md
+-rw-r--r--   0        0        0      918 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel.md
+-rw-r--r--   0        0        0      827 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel.py
+-rw-r--r--   0        0        0      536 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel_complete.py
+-rw-r--r--   0        0        0      953 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel_im2im.py
+-rw-r--r--   0        0        0      989 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel_im2im_class.py
+-rw-r--r--   0        0        0      863 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params.md
+-rw-r--r--   0        0        0      614 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params.py
+-rw-r--r--   0        0        0      747 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params_Karman.py
+-rw-r--r--   0        0        0      814 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params_with_im2im_preproc.py
+-rw-r--r--   0        0        0      380 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/README.md
+-rw-r--r--   0        0        0      908 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/bench_piv_2005C.py
+-rw-r--r--   0        0        0     1419 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/download.py
+-rw-r--r--   0        0        0      744 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/path_images.py
+-rw-r--r--   0        0        0      437 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2001A_topology.py
+-rw-r--r--   0        0        0      496 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2001A_work.py
+-rw-r--r--   0        0        0      622 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_topology.py
+-rw-r--r--   0        0        0      682 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_work.py
+-rw-r--r--   0        0        0      117 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/possible_paths.txt
+-rw-r--r--   0        0        0     1413 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc.md
+-rw-r--r--   0        0        0     1061 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_parallel.py
+-rw-r--r--   0        0        0      816 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_sback1_filter.py
+-rw-r--r--   0        0        0     1037 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_sback2_rescale.py
+-rw-r--r--   0        0        0      544 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_try_params.py
+-rw-r--r--   0        0        0      364 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_try_params_opencv.py
+-rw-r--r--   0        0        0     1553 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/profile_piv_work.py
+-rw-r--r--   0        0        0      448 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/submit_job_legi.py
+-rw-r--r--   0        0        0      711 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/surface_tracking.py
+-rw-r--r--   0        0        0     1201 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/test_run_examples.py
+-rw-r--r--   0        0        0      357 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples.md
+-rw-r--r--   0        0        0      238 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/for_dev.md
+-rw-r--r--   0        0        0      673 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/index.md
+-rw-r--r--   0        0        0     1686 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/install.md
+-rw-r--r--   0        0        0      405 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/ipynbslides/README.txt
+-rw-r--r--   0        0        0   493343 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/ipynbslides/fluidimage_legi_20170403.ipynb
+-rw-r--r--   0        0        0     2094 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/overview.md
+-rw-r--r--   0        0        0     1424 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/overview_orga_package.md
+-rw-r--r--   0        0        0     1857 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/related_codes.md
+-rw-r--r--   0        0        0       77 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/to_do.md
+-rw-r--r--   0        0        0      432 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorial.md
+-rw-r--r--   0        0        0     3116 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_calibration2dsimple.md
+-rw-r--r--   0        0        0     2412 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_direct_calibration.md
+-rw-r--r--   0        0        0     7352 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_opencv_calibration.md
+-rw-r--r--   0        0        0     4407 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_opencv_tomo_reconstruct.md
+-rw-r--r--   0        0        0     8785 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_piv.md
+-rw-r--r--   0        0        0     2950 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_stereo_reconstruction.md
+-rw-r--r--   0        0        0     1367 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_tsai_calibration.md
+-rw-r--r--   0        0        0     8971 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/uvmat.md
+-rw-r--r--   0        0        0     1252 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/Dockerfile
+-rw-r--r--   0        0        0     1147 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/Makefile
+-rw-r--r--   0        0        0      618 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/hgrc
+-rw-r--r--   0        0        0       77 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/pythranrc
+-rw-r--r--   0        0        0     1803 2024-05-02 10:23:27.000000 fluidimage-0.5.0/meson.build
+-rw-r--r--   0        0        0      655 2024-05-02 10:23:27.000000 fluidimage-0.5.0/meson.options
+-rw-r--r--   0        0        0     4888 2024-05-02 10:23:27.000000 fluidimage-0.5.0/noxfile.py
+-rw-r--r--   0        0        0   310844 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pdm.lock
+-rw-r--r--   0        0        0   782153 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pixi.lock
+-rw-r--r--   0        0        0     1009 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pixi.toml
+-rw-r--r--   0        0        0    21630 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pylintrc
+-rw-r--r--   0        0        0     4483 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3311 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/_opencv.py
+-rw-r--r--   0        0        0      162 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/_version.py
+-rw-r--r--   0        0        0      278 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/bos.py
+-rw-r--r--   0        0        0      263 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/__init__.py
+-rw-r--r--   0        0        0     2858 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/_evaluate_subpix.py
+-rw-r--r--   0        0        0      878 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/correl.cu
+-rw-r--r--   0        0        0    21039 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/correl.py
+-rw-r--r--   0        0        0    10794 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/correl_pycuda.py
+-rw-r--r--   0        0        0      333 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/errors.py
+-rw-r--r--   0        0        0     7467 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/fft.py
+-rw-r--r--   0        0        0      132 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/__init__.py
+-rw-r--r--   0        0        0      613 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/griddata.py
+-rw-r--r--   0        0        0      388 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/meson.build
+-rw-r--r--   0        0        0      867 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py
+-rw-r--r--   0        0        0     8006 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/thin_plate_spline.py
+-rw-r--r--   0        0        0    10216 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py
+-rw-r--r--   0        0        0     4807 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/mean_neighbors.py
+-rw-r--r--   0        0        0      489 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/meson.build
+-rw-r--r--   0        0        0    39595 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    37615 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    36317 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    35832 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    37828 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    38146 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    36451 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    34562 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0     1188 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/reduction_kernel.cu
+-rw-r--r--   0        0        0     6180 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/subpix.py
+-rw-r--r--   0        0        0     6544 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/test_correl.py
+-rw-r--r--   0        0        0     2519 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/test_fft.py
+-rw-r--r--   0        0        0      465 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/__init__.py
+-rw-r--r--   0        0        0     3587 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib2d_simple.py
+-rw-r--r--   0        0        0     9318 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib_cv.py
+-rw-r--r--   0        0        0    23798 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib_direct.py
+-rw-r--r--   0        0        0     7528 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib_tsai.py
+-rw-r--r--   0        0        0      302 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/meson.build
+-rw-r--r--   0        0        0     2033 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/test_calib_cv.py
+-rw-r--r--   0        0        0     2609 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/test_direct_stereo_reconstruction.py
+-rw-r--r--   0        0        0     1302 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/test_tsai_calibration.py
+-rw-r--r--   0        0        0     4272 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/util.py
+-rw-r--r--   0        0        0      739 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/config.py
+-rw-r--r--   0        0        0     1434 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/conftest.py
+-rw-r--r--   0        0        0      274 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/__init__.py
+-rw-r--r--   0        0        0    13511 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/display_piv.py
+-rw-r--r--   0        0        0     4822 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/display_pre.py
+-rw-r--r--   0        0        0      214 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/meson.build
+-rw-r--r--   0        0        0    26293 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/piv.py
+-rw-r--r--   0        0        0     4457 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/preproc.py
+-rw-r--r--   0        0        0      425 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/test_piv.py
+-rw-r--r--   0        0        0     9009 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/tomo.py
+-rw-r--r--   0        0        0     3376 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/__init__.py
+-rw-r--r--   0        0        0    17837 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/base.py
+-rw-r--r--   0        0        0    10536 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async.py
+-rw-r--r--   0        0        0     4054 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_multiproc.py
+-rw-r--r--   0        0        0     3892 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_seq_for_multi.py
+-rw-r--r--   0        0        0     2106 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_sequential.py
+-rw-r--r--   0        0        0     8058 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_servers.py
+-rw-r--r--   0        0        0      396 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_servers_threading.py
+-rw-r--r--   0        0        0     2210 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_sequential.py
+-rw-r--r--   0        0        0      393 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/meson.build
+-rw-r--r--   0        0        0     7358 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/multi_exec_async.py
+-rw-r--r--   0        0        0     3668 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/multi_exec_subproc.py
+-rw-r--r--   0        0        0     7661 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/servers.py
+-rw-r--r--   0        0        0      338 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/base_matplotlib.py
+-rw-r--r--   0        0        0     8981 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/imviewer.py
+-rw-r--r--   0        0        0      228 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/Makefile
+-rw-r--r--   0        0        0      153 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/__init__.py
+-rw-r--r--   0        0        0     2659 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/main.py
+-rw-r--r--   0        0        0     3750 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.py
+-rw-r--r--   0        0        0     1671 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.ui
+-rw-r--r--   0        0        0      170 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/meson.build
+-rw-r--r--   0        0        0      568 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/test_launcher.py
+-rw-r--r--   0        0        0      348 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/meson.build
+-rw-r--r--   0        0        0    10703 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/monitor.py
+-rw-r--r--   0        0        0       67 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/monitor.tcss
+-rw-r--r--   0        0        0     2459 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/pg_main.py
+-rw-r--r--   0        0        0     5903 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/pg_wrapper.py
+-rw-r--r--   0        0        0     6018 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/piv_viewer.py
+-rw-r--r--   0        0        0     1093 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_imviewer.py
+-rw-r--r--   0        0        0      965 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_imviewer_pg.py
+-rw-r--r--   0        0        0     2727 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_monitor.py
+-rw-r--r--   0        0        0     1132 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_piv_viewer.py
+-rw-r--r--   0        0        0     2612 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/image2image.py
+-rw-r--r--   0        0        0      543 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/meson.build
+-rw-r--r--   0        0        0      337 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/optical_flow.py
+-rw-r--r--   0        0        0      278 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/piv.py
+-rw-r--r--   0        0        0      104 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/__init__.py
+-rw-r--r--   0        0        0      210 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/meson.build
+-rw-r--r--   0        0        0     2412 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/piv.py
+-rw-r--r--   0        0        0    14134 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/postproc.py
+-rw-r--r--   0        0        0     2927 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/test_piv.py
+-rw-r--r--   0        0        0     3771 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/test_util.py
+-rw-r--r--   0        0        0     4070 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/util.py
+-rw-r--r--   0        0        0    24145 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/vector_field.py
+-rw-r--r--   0        0        0      580 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/preproc.py
+-rw-r--r--   0        0        0      351 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/meson.build
+-rw-r--r--   0        0        0      230 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/meson.build
+-rw-r--r--   0        0        0     7578 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/mlos.py
+-rw-r--r--   0        0        0     1362 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/test_mlos.py
+-rw-r--r--   0        0        0     2730 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/run_from_xml.py
+-rw-r--r--   0        0        0     1605 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/synthetic.py
+-rw-r--r--   0        0        0      521 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/test_image2image.py
+-rw-r--r--   0        0        0     2259 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/test_run_from_xml.py
+-rw-r--r--   0        0        0     2874 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/__init__.py
+-rw-r--r--   0        0        0    17551 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/base.py
+-rw-r--r--   0        0        0     6355 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/bos.py
+-rw-r--r--   0        0        0     5706 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/example.py
+-rw-r--r--   0        0        0     3999 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/image2image.py
+-rw-r--r--   0        0        0     2497 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/launcher.py
+-rw-r--r--   0        0        0    10341 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/log.py
+-rw-r--r--   0        0        0      642 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/meson.build
+-rw-r--r--   0        0        0     1422 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/nb_cpu_cores.py
+-rw-r--r--   0        0        0     1020 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/optical_flow.py
+-rw-r--r--   0        0        0     8851 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/piv.py
+-rw-r--r--   0        0        0    10337 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/preproc.py
+-rw-r--r--   0        0        0     8772 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/splitters.py
+-rw-r--r--   0        0        0    10745 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/surface_tracking.py
+-rw-r--r--   0        0        0     1347 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_bos.py
+-rw-r--r--   0        0        0     1993 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_example.py
+-rw-r--r--   0        0        0     1628 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_image2image.py
+-rw-r--r--   0        0        0     1220 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_optical_flow.py
+-rw-r--r--   0        0        0     2578 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_piv.py
+-rw-r--r--   0        0        0     1773 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_preproc.py
+-rw-r--r--   0        0        0     1919 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_splitters.py
+-rw-r--r--   0        0        0     2251 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_surftracking.py
+-rw-r--r--   0        0        0      741 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/log.py
+-rw-r--r--   0        0        0      151 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/meson.build
+-rw-r--r--   0        0        0      398 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/test_util.py
+-rw-r--r--   0        0        0     3154 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/util.py
+-rw-r--r--   0        0        0     7306 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/uvmat.py
+-rw-r--r--   0        0        0     6699 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/__init__.py
+-rw-r--r--   0        0        0     2662 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/bos.py
+-rw-r--r--   0        0        0     2687 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/image2image.py
+-rw-r--r--   0        0        0      301 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/meson.build
+-rw-r--r--   0        0        0     6651 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/optical_flow.py
+-rw-r--r--   0        0        0      198 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/__init__.py
+-rw-r--r--   0        0        0     7836 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/fix.py
+-rw-r--r--   0        0        0      179 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/meson.build
+-rw-r--r--   0        0        0     6418 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/multipass.py
+-rw-r--r--   0        0        0    26467 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/singlepass.py
+-rw-r--r--   0        0        0     2492 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/test_piv.py
+-rw-r--r--   0        0        0     4587 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_cv.py
+-rw-r--r--   0        0        0    14387 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_py.py
+-rw-r--r--   0        0        0     2213 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/io.py
+-rw-r--r--   0        0        0      184 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/meson.build
+-rw-r--r--   0        0        0     3977 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/toolbox.py
+-rw-r--r--   0        0        0    22183 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/surface_tracking.py
+-rw-r--r--   0        0        0      776 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/test_bos.py
+-rw-r--r--   0        0        0      542 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/test_image2image.py
+-rw-r--r--   0        0        0     1815 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/test_preproc.py
+-rw-r--r--   0        0        0     1307 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/with_mask.py
+-rw-r--r--   0        0        0     4742 2024-05-02 10:24:20.412518 fluidimage-0.5.0/PKG-INFO
```

### Comparing `fluidimage-0.4.6/.github/workflows/ci-linux.yml` & `fluidimage-0.5.0/.github/workflows/ci-linux.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/.github/workflows/ci-pixi.yml` & `fluidimage-0.5.0/.github/workflows/ci-pixi.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/.github/workflows/wheels.yml` & `fluidimage-0.5.0/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/.gitlab-ci.yml` & `fluidimage-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/.hgtags` & `fluidimage-0.5.0/.hgtags`

 * *Files 6% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 2506df1b76802880d2b1acaeb737bd6a875762e5 0.4.0
 4bb44f739762f5fffbd2a8b0e7b759bd63709c03 0.4.1
 bb6f0ccc21452f0e1aa5caa5e058c8a163556c0d 0.4.2
 d1026b6b03c5e9ef8d0f23b60158684ed3d9e936 0.4.3
 f615cec0efdc3377cb9c7dfa96926fc2100d8c02 0.4.3.post0
 e66f70954560bbccdde36c76eac0a12f82ada45d 0.4.4
 80b7c7a51553b4ff08206a336e3e5d4795ffe306 0.4.5
+15eedfa330603df0403c6d8d6fc49ec468536e9b 0.4.6
```

### Comparing `fluidimage-0.4.6/CHANGES.md` & `fluidimage-0.5.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Release notes
 
 See also the
-[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...branch%2Fdefault).
+[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...branch%2Fdefault).
+
+## [0.5.0] (2024-05-02)
+
+- UVmat compatibility (launching in "local" mode).
+- Change defaults and exact meaning for parameters. `params.multipass.smoothing_coef`
+  (=2) and `params.multipass.threshold_tps` (=1.5).
+- PIV saving: use float32 and save "smooth" displacement fields.
 
 ## [0.4.6] (2024-04-20)
 
 - Fix a memory leak related to Pythran in {mod}`fluidimage.calcul.subpix` (see
   [!97](https://foss.heptapod.net/fluiddyn/fluidimage/-/merge_requests/97)).
 - Performance optimizations for PIV.
 - Remove `params.piv0.coef_correl_no_displ` (old useless parameter).
@@ -199,7 +206,8 @@
 [0.4.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.3.0...0.4.0
 [0.4.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.0...0.4.1
 [0.4.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.1...0.4.2
 [0.4.3]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.2...0.4.3
 [0.4.4]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.3...0.4.4
 [0.4.5]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.4...0.4.5
 [0.4.6]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...0.4.6
+[0.5.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.6...0.5.0
```

### Comparing `fluidimage-0.4.6/CONTRIBUTING.md` & `fluidimage-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/LICENSE.txt` & `fluidimage-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/README.md` & `fluidimage-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/CONTRIBUTING.md` & `fluidimage-0.5.0/doc/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/Makefile` & `fluidimage-0.5.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/build-from-source.md` & `fluidimage-0.5.0/doc/build-from-source.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/changes.md` & `fluidimage-0.5.0/doc/changes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Release notes
 
 See also the
-[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...branch%2Fdefault).
+[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...branch%2Fdefault).
+
+## [0.5.0] (2024-05-02)
+
+- UVmat compatibility (launching in "local" mode).
+- Change defaults and exact meaning for parameters. `params.multipass.smoothing_coef`
+  (=2) and `params.multipass.threshold_tps` (=1.5).
+- PIV saving: use float32 and save "smooth" displacement fields.
 
 ## [0.4.6] (2024-04-20)
 
 - Fix a memory leak related to Pythran in {mod}`fluidimage.calcul.subpix` (see
   [!97](https://foss.heptapod.net/fluiddyn/fluidimage/-/merge_requests/97)).
 - Performance optimizations for PIV.
 - Remove `params.piv0.coef_correl_no_displ` (old useless parameter).
@@ -199,7 +206,8 @@
 [0.4.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.3.0...0.4.0
 [0.4.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.0...0.4.1
 [0.4.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.1...0.4.2
 [0.4.3]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.2...0.4.3
 [0.4.4]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.3...0.4.4
 [0.4.5]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.4...0.4.5
 [0.4.6]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...0.4.6
+[0.5.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.6...0.5.0
```

### Comparing `fluidimage-0.4.6/doc/conf.py` & `fluidimage-0.5.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/bos_parallel.py` & `fluidimage-0.5.0/doc/examples/bos_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/im2im_parallel.py` & `fluidimage-0.5.0/doc/examples/im2im_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/optflow_parallel.py` & `fluidimage-0.5.0/doc/examples/optflow_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/optflow_try_params.md` & `fluidimage-0.5.0/doc/examples/optflow_try_params.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/optflow_try_params.py` & `fluidimage-0.5.0/doc/examples/optflow_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/README.md` & `fluidimage-0.5.0/doc/examples/piv_as_real/README.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/args.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/args.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/job_piv.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/job_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/job_pre.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/job_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/params_piv.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/params_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/params_pre.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/params_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/submit_piv.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/submit_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/submit_pre.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/submit_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/test_piv_as_real.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/test_piv_as_real.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/try_piv.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/try_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_as_real/try_pre.py` & `fluidimage-0.5.0/doc/examples/piv_as_real/try_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_parallel.md` & `fluidimage-0.5.0/doc/examples/piv_parallel.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_parallel.py` & `fluidimage-0.5.0/doc/examples/piv_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_parallel_complete.py` & `fluidimage-0.5.0/doc/examples/piv_parallel_complete.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_parallel_im2im.py` & `fluidimage-0.5.0/doc/examples/piv_parallel_im2im.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_parallel_im2im_class.py` & `fluidimage-0.5.0/doc/examples/piv_parallel_im2im_class.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_try_params.md` & `fluidimage-0.5.0/doc/examples/piv_try_params.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_try_params.py` & `fluidimage-0.5.0/doc/examples/piv_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/piv_try_params_Karman.py` & `fluidimage-0.5.0/doc/examples/piv_try_params_Karman.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from fluidimage.piv import Work
 
 params = Work.create_default_params()
 
 params.series.path = "../../image_samples/Karman/Images"
 
-params.mask.strcrop = "50:350, 0:380"
+params.mask.strcrop = "20:380, 0:450"
 
 params.fix.correl_min = 0.4
 params.fix.threshold_diff_neighbour = 2.0
 
 params.piv0.shape_crop_im0 = 32
 params.piv0.displacement_max = 5
 params.piv0.nb_peaks_to_search = 2
 
 params.multipass.number = 2
 params.multipass.use_tps = "last"
+params.multipass.subdom_size = 400
+params.multipass.smoothing_coef = 2.0
 
 work = Work(params=params)
 
 piv = work.process_1_serie()
 
-# piv.display(show_interp=True, scale=0.3, show_error=False)
-piv.display(show_interp=False, scale=1, show_error=True)
+piv.display(show_interp=True, scale=0.3, show_error=False, show_correl=False)
+# piv.display(show_interp=False, scale=1, show_error=True)
 
 # piv.save()
```

### Comparing `fluidimage-0.4.6/doc/examples/piv_try_params_with_im2im_preproc.py` & `fluidimage-0.5.0/doc/examples/piv_try_params_with_im2im_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/pivchallenge/bench_piv_2005C.py` & `fluidimage-0.5.0/doc/examples/pivchallenge/bench_piv_2005C.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/pivchallenge/download.py` & `fluidimage-0.5.0/doc/examples/pivchallenge/download.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/pivchallenge/path_images.py` & `fluidimage-0.5.0/doc/examples/pivchallenge/path_images.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/pivchallenge/piv_2005C_topology.py` & `fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_topology.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 params.series.path = str(get_path("2005C") / "c*.bmp")
 # params.series.ind_stop = 12
 
 params.piv0.shape_crop_im0 = 64
 params.piv0.grid.overlap = 0.5
 
 params.multipass.number = 3
-params.multipass.use_tps = False
+params.multipass.use_tps = "last"
+params.multipass.subdom_size = 200
 
 params.fix.displacement_max = 3
 params.fix.correl_min = 0.1
 params.fix.threshold_diff_neighbour = 3
 
-params.saving.how = "complete"
+params.saving.how = "recompute"
 
 topology = Topology(params)
 
 topology.compute()
+# topology.compute(nb_max_workers=4)
 # topology.compute("multi_exec_subproc")
```

### Comparing `fluidimage-0.4.6/doc/examples/pivchallenge/piv_2005C_work.py` & `fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_work.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/preproc.md` & `fluidimage-0.5.0/doc/examples/preproc.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/preproc_parallel.py` & `fluidimage-0.5.0/doc/examples/preproc_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/preproc_sback1_filter.py` & `fluidimage-0.5.0/doc/examples/preproc_sback1_filter.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/preproc_sback2_rescale.py` & `fluidimage-0.5.0/doc/examples/preproc_sback2_rescale.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/preproc_try_params.py` & `fluidimage-0.5.0/doc/examples/preproc_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/profile_piv_work.py` & `fluidimage-0.5.0/doc/examples/profile_piv_work.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 params.multipass.number = 2
 
 # params.multipass.use_tps = "last"
 params.multipass.use_tps = False
 params.multipass.subdom_size = 200
 params.multipass.smoothing_coef = 10.0
-params.multipass.threshold_tps = 0.5
+params.multipass.threshold_tps = 1.5
 
 params.fix.correl_min = 0.15
 params.fix.threshold_diff_neighbour = 3
 
 work = Work(params=params)
 
 profiler = Profiler()
```

### Comparing `fluidimage-0.4.6/doc/examples/surface_tracking.py` & `fluidimage-0.5.0/doc/examples/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/examples/test_run_examples.py` & `fluidimage-0.5.0/doc/examples/test_run_examples.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/index.md` & `fluidimage-0.5.0/doc/index.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/install.md` & `fluidimage-0.5.0/doc/install.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/ipynbslides/fluidimage_legi_20170403.ipynb` & `fluidimage-0.5.0/doc/ipynbslides/fluidimage_legi_20170403.ipynb`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/overview.md` & `fluidimage-0.5.0/doc/overview.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/overview_orga_package.md` & `fluidimage-0.5.0/doc/overview_orga_package.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/related_codes.md` & `fluidimage-0.5.0/doc/related_codes.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/tutorials/tuto_calibration2dsimple.md` & `fluidimage-0.5.0/doc/tutorials/tuto_calibration2dsimple.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/tutorials/tuto_direct_calibration.md` & `fluidimage-0.5.0/doc/tutorials/tuto_direct_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/tutorials/tuto_opencv_calibration.md` & `fluidimage-0.5.0/doc/tutorials/tuto_opencv_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/tutorials/tuto_opencv_tomo_reconstruct.md` & `fluidimage-0.5.0/doc/tutorials/tuto_opencv_tomo_reconstruct.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/tutorials/tuto_piv.md` & `fluidimage-0.5.0/doc/tutorials/tuto_piv.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/tutorials/tuto_stereo_reconstruction.md` & `fluidimage-0.5.0/doc/tutorials/tuto_stereo_reconstruction.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/tutorials/tuto_tsai_calibration.md` & `fluidimage-0.5.0/doc/tutorials/tuto_tsai_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/doc/uvmat.md` & `fluidimage-0.5.0/doc/uvmat.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/docker/Dockerfile` & `fluidimage-0.5.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/docker/Makefile` & `fluidimage-0.5.0/docker/Makefile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/docker/hgrc` & `fluidimage-0.5.0/docker/hgrc`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/meson.build` & `fluidimage-0.5.0/meson.build`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/meson.options` & `fluidimage-0.5.0/meson.options`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/noxfile.py` & `fluidimage-0.5.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/pdm.lock` & `fluidimage-0.5.0/pdm.lock`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/pixi.lock` & `fluidimage-0.5.0/pixi.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 version: 3
 metadata:
   content_hash:
     linux-64: e90c2ee71ad70fc0a1c8302029533a7d1498f2bffcd0eaa8d2934700e775dc1d
     osx-64: e90c2ee71ad70fc0a1c8302029533a7d1498f2bffcd0eaa8d2934700e775dc1d
+    osx-arm64: e90c2ee71ad70fc0a1c8302029533a7d1498f2bffcd0eaa8d2934700e775dc1d
     win-64: e90c2ee71ad70fc0a1c8302029533a7d1498f2bffcd0eaa8d2934700e775dc1d
   channels:
   - url: https://conda.anaconda.org/conda-forge/
     used_env_vars: []
   platforms:
   - linux-64
   - osx-64
+  - osx-arm64
   - win-64
   sources: []
   time_metadata: null
   git_metadata: null
   inputs_metadata: null
   custom_metadata: null
 package:
@@ -110,14 +112,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   size: 2922373
   timestamp: 1710388791338
+- platform: osx-arm64
+  name: aom
+  version: 3.8.2
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aom-3.8.2-h078ce10_0.conda
+  hash:
+    md5: 3c5057d1d4494caab891ed6f276c3f63
+    sha256: d3a6cb707373a8d2d219259ad017a35c20fc3618e39c87db0d6200af0f984379
+  build: h078ce10_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 2204439
+  timestamp: 1710388305837
 - platform: win-64
   name: aom
   version: 3.7.1
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -177,14 +198,37 @@
   license: Apache-2.0
   license_family: Apache
   noarch: python
   size: 28922
   timestamp: 1698341257884
   purls:
   - pkg:pypi/asttokens
+- platform: osx-arm64
+  name: asttokens
+  version: 2.4.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.5
+  - six >=1.12.0
+  url: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 5f25798dcefd8252ce5f9dc494d5f571
+    sha256: 708168f026df19a0344983754d27d1f7b28bb21afc7b97a82f02c4798a3d2111
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  noarch: python
+  size: 28922
+  timestamp: 1698341257884
+  purls:
+  - pkg:pypi/asttokens
 - platform: win-64
   name: asttokens
   version: 2.4.1
   category: main
   manager: conda
   dependencies:
   - python >=3.5
@@ -263,14 +307,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 54582
   timestamp: 1704011393776
   purls:
   - pkg:pypi/attrs
+- platform: osx-arm64
+  name: attrs
+  version: 23.2.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/attrs-23.2.0-pyh71513ae_0.conda
+  hash:
+    md5: 5e4c0743c70186509d1412e03c2d8dfa
+    sha256: 77c7d03bdb243a048fff398cedc74327b7dc79169ebe3b4c8448b0331ea55fea
+  build: pyh71513ae_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 54582
+  timestamp: 1704011393776
+  purls:
+  - pkg:pypi/attrs
 - platform: win-64
   name: attrs
   version: 23.2.0
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -335,14 +401,39 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 45455
   timestamp: 1710677615519
   purls:
   - pkg:pypi/autopep8
+- platform: osx-arm64
+  name: autopep8
+  version: 2.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - packaging
+  - pycodestyle >=2.11.0
+  - python >=3.6
+  - tomli
+  url: https://conda.anaconda.org/conda-forge/noarch/autopep8-2.1.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 86d1a0a5e07cb9ad7792d2398eccd057
+    sha256: 1316650986ecb81626213034220ac6549e55cacfcbe1fc874328205fc3f26556
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 45455
+  timestamp: 1710677615519
+  purls:
+  - pkg:pypi/autopep8
 - platform: win-64
   name: autopep8
   version: 2.1.0
   category: main
   manager: conda
   dependencies:
   - packaging
@@ -408,14 +499,38 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: Apache-2.0
   license_family: Apache
   size: 91309
   timestamp: 1712670722676
+- platform: osx-arm64
+  name: aws-c-auth
+  version: 0.7.17
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-c-cal >=0.6.11,<0.6.12.0a0
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  - aws-c-http >=0.8.1,<0.8.2.0a0
+  - aws-c-io >=0.14.7,<0.14.8.0a0
+  - aws-c-sdkutils >=0.1.15,<0.1.16.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-auth-0.7.17-h382b9c6_2.conda
+  hash:
+    md5: f38724f2e96212bf6c5c96861dc887f1
+    sha256: 50c87bf0fa68b5a6b9d2fbde5a17b1cf8c5f81ddbf659d78452de779598b1177
+  build: h382b9c6_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: Apache-2.0
+  license_family: Apache
+  size: 89585
+  timestamp: 1712670760388
 - platform: win-64
   name: aws-c-auth
   version: 0.7.11
   category: main
   manager: conda
   dependencies:
   - aws-c-cal >=0.6.9,<0.6.10.0a0
@@ -474,14 +589,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 38803
   timestamp: 1712495186044
+- platform: osx-arm64
+  name: aws-c-cal
+  version: 0.6.11
+  category: main
+  manager: conda
+  dependencies:
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-cal-0.6.11-hd34e5fa_0.conda
+  hash:
+    md5: 92d0e6abc836c1c00facbd08d3b01ce9
+    sha256: 8296f9ad5415f6e640862116c4c3f4c1bc555ea05eab2ec32e112073cd697d79
+  build: hd34e5fa_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 39697
+  timestamp: 1712495118765
 - platform: win-64
   name: aws-c-cal
   version: 0.6.9
   category: main
   manager: conda
   dependencies:
   - aws-c-common >=0.9.12,<0.9.13.0a0
@@ -533,14 +667,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 209383
   timestamp: 1712101871696
+- platform: osx-arm64
+  name: aws-c-common
+  version: 0.9.15
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-common-0.9.15-h93a5062_0.conda
+  hash:
+    md5: 4ca05bd64cc4decc54089fcd0cc69082
+    sha256: ae4a47f032886a7175fe6e7ccbf1233cbe06bdfc747fc707afd83d2bdff43dff
+  build: h93a5062_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 204504
+  timestamp: 1712101989588
 - platform: win-64
   name: aws-c-common
   version: 0.9.12
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -593,14 +745,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: Apache-2.0
   license_family: Apache
   size: 17976
   timestamp: 1712138779036
+- platform: osx-arm64
+  name: aws-c-compression
+  version: 0.2.18
+  category: main
+  manager: conda
+  dependencies:
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-compression-0.2.18-hd34e5fa_3.conda
+  hash:
+    md5: 194b36e2ac364c12c7fa89e84391722d
+    sha256: c501b4f00d1518956aa3fb45378e0dacdec941cca5d78e8d8ba07b46674fa877
+  build: hd34e5fa_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: Apache-2.0
+  license_family: Apache
+  size: 18089
+  timestamp: 1712138821785
 - platform: win-64
   name: aws-c-compression
   version: 0.2.17
   category: main
   manager: conda
   dependencies:
   - aws-c-common >=0.9.12,<0.9.13.0a0
@@ -660,14 +831,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 8
   license: Apache-2.0
   license_family: Apache
   size: 46574
   timestamp: 1712507348124
+- platform: osx-arm64
+  name: aws-c-event-stream
+  version: 0.4.2
+  category: main
+  manager: conda
+  dependencies:
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  - aws-c-io >=0.14.7,<0.14.8.0a0
+  - aws-checksums >=0.1.18,<0.1.19.0a0
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-event-stream-0.4.2-h247c08a_8.conda
+  hash:
+    md5: 47912c9d76ebf3146dc5c5358fe94a97
+    sha256: f4a8ee85ed51793bdfaa5ff863db5fa02eb1935e25857109b8650af2c66f46c5
+  build: h247c08a_8
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 8
+  license: Apache-2.0
+  license_family: Apache
+  size: 46788
+  timestamp: 1712507379999
 - platform: win-64
   name: aws-c-event-stream
   version: 0.4.1
   category: main
   manager: conda
   dependencies:
   - aws-c-common >=0.9.12,<0.9.13.0a0
@@ -730,14 +923,37 @@
   arch: x86_64
   subdir: osx-64
   build_number: 10
   license: Apache-2.0
   license_family: Apache
   size: 162863
   timestamp: 1712654842013
+- platform: osx-arm64
+  name: aws-c-http
+  version: 0.8.1
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-c-cal >=0.6.11,<0.6.12.0a0
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  - aws-c-compression >=0.2.18,<0.2.19.0a0
+  - aws-c-io >=0.14.7,<0.14.8.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-http-0.8.1-hf9e830b_10.conda
+  hash:
+    md5: 532e961f28b3c8fcdcb0ecb1e017961d
+    sha256: 6c06720a8700f65e68ad740b5dd0e559242f62a179067c029792d226b3b065fc
+  build: hf9e830b_10
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 10
+  license: Apache-2.0
+  license_family: Apache
+  size: 151666
+  timestamp: 1712654734379
 - platform: win-64
   name: aws-c-http
   version: 0.8.0
   category: main
   manager: conda
   dependencies:
   - aws-c-cal >=0.6.9,<0.6.10.0a0
@@ -764,48 +980,69 @@
   version: 0.14.7
   category: main
   manager: conda
   dependencies:
   - aws-c-cal >=0.6.11,<0.6.12.0a0
   - aws-c-common >=0.9.15,<0.9.16.0a0
   - libgcc-ng >=12
-  - s2n >=1.4.10,<1.4.11.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/aws-c-io-0.14.7-h62f3060_4.conda
+  - s2n >=1.4.12,<1.4.13.0a0
+  url: https://conda.anaconda.org/conda-forge/linux-64/aws-c-io-0.14.7-hbfbeace_6.conda
   hash:
-    md5: 4f7ff4952228e6f222f592fb9edb9241
-    sha256: f4a82249573addf387b22f8a92942cea98a71aec4b9be1f05797e19954571f22
-  build: h62f3060_4
+    md5: d6382461de9a91a2665e964f92d8da0a
+    sha256: 10c8df9b71be8aba9b1aad48b123fc81896eb7b73c686042bed4a9e77d92e812
+  build: hbfbeace_6
   arch: x86_64
   subdir: linux-64
-  build_number: 4
+  build_number: 6
   license: Apache-2.0
   license_family: Apache
-  size: 158268
-  timestamp: 1713185235625
+  size: 158124
+  timestamp: 1713346977725
 - platform: osx-64
   name: aws-c-io
   version: 0.14.7
   category: main
   manager: conda
   dependencies:
   - __osx >=10.9
   - aws-c-cal >=0.6.11,<0.6.12.0a0
   - aws-c-common >=0.9.15,<0.9.16.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/aws-c-io-0.14.7-h6254544_4.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/aws-c-io-0.14.7-h6254544_6.conda
   hash:
-    md5: b5c9d4896f5a8026562fe730eb562c0a
-    sha256: 48f3fb0bcbea2329fdd6a405707fac4ccc73411641ebc59427e49434b6f222f8
-  build: h6254544_4
+    md5: 9c997fbd219f8db5714dbdc240e355a0
+    sha256: 5d2327f3742cfabd53bf8c935eb2cffd50e3ea8c03c9fee12940b2ffb94ad1cb
+  build: h6254544_6
   arch: x86_64
   subdir: osx-64
-  build_number: 4
+  build_number: 6
   license: Apache-2.0
   license_family: Apache
-  size: 137942
-  timestamp: 1713185462350
+  size: 137495
+  timestamp: 1713347345969
+- platform: osx-arm64
+  name: aws-c-io
+  version: 0.14.7
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-c-cal >=0.6.11,<0.6.12.0a0
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-io-0.14.7-h33d81b3_6.conda
+  hash:
+    md5: def574dc950fa350d49db8438ca5d1af
+    sha256: a93a3e23c0407cbfaa9807784a32c96a00fea32b2d015f0be59c0cb79cc4aaa5
+  build: h33d81b3_6
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 6
+  license: Apache-2.0
+  license_family: Apache
+  size: 137603
+  timestamp: 1713347142779
 - platform: win-64
   name: aws-c-io
   version: 0.14.0
   category: main
   manager: conda
   dependencies:
   - aws-c-cal >=0.6.9,<0.6.10.0a0
@@ -865,14 +1102,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 4
   license: Apache-2.0
   license_family: Apache
   size: 139268
   timestamp: 1712547737430
+- platform: osx-arm64
+  name: aws-c-mqtt
+  version: 0.10.3
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  - aws-c-http >=0.8.1,<0.8.2.0a0
+  - aws-c-io >=0.14.7,<0.14.8.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-mqtt-0.10.3-h5f4abda_4.conda
+  hash:
+    md5: 49dfa5667f57d5a7f9716ff06f80d28f
+    sha256: ee1296c91f1624a67199b4885f79d3123a9bbc5b7def6de056f0d8c1c4525d0d
+  build: h5f4abda_4
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 4
+  license: Apache-2.0
+  license_family: Apache
+  size: 118034
+  timestamp: 1712547383899
 - platform: win-64
   name: aws-c-mqtt
   version: 0.10.1
   category: main
   manager: conda
   dependencies:
   - aws-c-common >=0.9.12,<0.9.13.0a0
@@ -940,14 +1199,39 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: Apache-2.0
   license_family: Apache
   size: 93544
   timestamp: 1712685831186
+- platform: osx-arm64
+  name: aws-c-s3
+  version: 0.5.7
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-c-auth >=0.7.17,<0.7.18.0a0
+  - aws-c-cal >=0.6.11,<0.6.12.0a0
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  - aws-c-http >=0.8.1,<0.8.2.0a0
+  - aws-c-io >=0.14.7,<0.14.8.0a0
+  - aws-checksums >=0.1.18,<0.1.19.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-s3-0.5.7-h606a3d2_1.conda
+  hash:
+    md5: 9bd413b520a8768af02e3a5810e9a42a
+    sha256: 7365e76ad87e39bf58eea10515001007e275bbd270981f3a1641c840f052017a
+  build: h606a3d2_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: Apache-2.0
+  license_family: Apache
+  size: 93368
+  timestamp: 1712686042460
 - platform: win-64
   name: aws-c-s3
   version: 0.4.9
   category: main
   manager: conda
   dependencies:
   - aws-c-auth >=0.7.11,<0.7.12.0a0
@@ -1006,14 +1290,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: Apache-2.0
   license_family: Apache
   size: 49610
   timestamp: 1712146120263
+- platform: osx-arm64
+  name: aws-c-sdkutils
+  version: 0.1.15
+  category: main
+  manager: conda
+  dependencies:
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-c-sdkutils-0.1.15-hd34e5fa_3.conda
+  hash:
+    md5: d4afb2c3ed05bf792183ffdbc723aaeb
+    sha256: e128818c57f6273df6dc64d7c3868eb179011766d790a8a93ad152fa26be4b9d
+  build: hd34e5fa_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: Apache-2.0
+  license_family: Apache
+  size: 49627
+  timestamp: 1712146003862
 - platform: win-64
   name: aws-c-sdkutils
   version: 0.1.13
   category: main
   manager: conda
   dependencies:
   - aws-c-common >=0.9.12,<0.9.13.0a0
@@ -1067,14 +1370,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: Apache-2.0
   license_family: Apache
   size: 48730
   timestamp: 1712146097053
+- platform: osx-arm64
+  name: aws-checksums
+  version: 0.1.18
+  category: main
+  manager: conda
+  dependencies:
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-checksums-0.1.18-hd34e5fa_3.conda
+  hash:
+    md5: 69f9b2281805ff1e0c87962d74de1360
+    sha256: d91ba44e14b31c5fe13fd78a567fc6cf76c62ad8bfaba250e317b354a75c64dd
+  build: hd34e5fa_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: Apache-2.0
+  license_family: Apache
+  size: 48999
+  timestamp: 1712145929885
 - platform: win-64
   name: aws-checksums
   version: 0.1.17
   category: main
   manager: conda
   dependencies:
   - aws-c-common >=0.9.12,<0.9.13.0a0
@@ -1147,14 +1469,43 @@
   arch: x86_64
   subdir: osx-64
   build_number: 4
   license: Apache-2.0
   license_family: Apache
   size: 283365
   timestamp: 1712752909519
+- platform: osx-arm64
+  name: aws-crt-cpp
+  version: 0.26.6
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-c-auth >=0.7.17,<0.7.18.0a0
+  - aws-c-cal >=0.6.11,<0.6.12.0a0
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  - aws-c-event-stream >=0.4.2,<0.4.3.0a0
+  - aws-c-http >=0.8.1,<0.8.2.0a0
+  - aws-c-io >=0.14.7,<0.14.8.0a0
+  - aws-c-mqtt >=0.10.3,<0.10.4.0a0
+  - aws-c-s3 >=0.5.7,<0.5.8.0a0
+  - aws-c-sdkutils >=0.1.15,<0.1.16.0a0
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-crt-cpp-0.26.6-h13f0230_4.conda
+  hash:
+    md5: 4e2b2d2f1ae778ed49d542974403fb60
+    sha256: abf4618412f03fad2f3a1d4dd15200237afce54e1d1eff5eb17f834aa7acd32d
+  build: h13f0230_4
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 4
+  license: Apache-2.0
+  license_family: Apache
+  size: 220730
+  timestamp: 1712752845989
 - platform: win-64
   name: aws-crt-cpp
   version: 0.26.0
   category: main
   manager: conda
   dependencies:
   - aws-c-auth >=0.7.11,<0.7.12.0a0
@@ -1231,14 +1582,41 @@
   arch: x86_64
   subdir: osx-64
   build_number: 6
   license: Apache-2.0
   license_family: Apache
   size: 3394339
   timestamp: 1712754051179
+- platform: osx-arm64
+  name: aws-sdk-cpp
+  version: 1.11.267
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-c-common >=0.9.15,<0.9.16.0a0
+  - aws-c-event-stream >=0.4.2,<0.4.3.0a0
+  - aws-checksums >=0.1.18,<0.1.19.0a0
+  - aws-crt-cpp >=0.26.6,<0.26.7.0a0
+  - libcurl >=8.7.1,<9.0a0
+  - libcxx >=16
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.1,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/aws-sdk-cpp-1.11.267-h134aaec_6.conda
+  hash:
+    md5: 25727bad6dc72a38c856c3e9a578ebc7
+    sha256: 5eff7b834368f9e710cded2e7c0a56f1595b5b617f310547874df10c275cd6a0
+  build: h134aaec_6
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 6
+  license: Apache-2.0
+  license_family: Apache
+  size: 3411167
+  timestamp: 1712754307571
 - platform: win-64
   name: aws-sdk-cpp
   version: 1.11.210
   category: main
   manager: conda
   dependencies:
   - aws-c-common >=0.9.12,<0.9.13.0a0
@@ -1303,14 +1681,37 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 12659
   timestamp: 1627922710217
   purls:
   - pkg:pypi/beniget
+- platform: osx-arm64
+  name: beniget
+  version: 0.4.1
+  category: main
+  manager: conda
+  dependencies:
+  - gast >=0.5.0,<0.6.0
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/beniget-0.4.1-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 66744e23ceca50ebb022b0a6cba866a8
+    sha256: 767cecb8b32d981f5c666eac1cc231d6fbcb29042124efe1b921a9de9201924b
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 12659
+  timestamp: 1627922710217
+  purls:
+  - pkg:pypi/beniget
 - platform: win-64
   name: beniget
   version: 0.4.1
   category: main
   manager: conda
   dependencies:
   - gast >=0.5.0,<0.6.0
@@ -1332,28 +1733,28 @@
   - pkg:pypi/beniget
 - platform: linux-64
   name: binutils_impl_linux-64
   version: '2.40'
   category: main
   manager: conda
   dependencies:
-  - ld_impl_linux-64 2.40 h41732ed_0
+  - ld_impl_linux-64 2.40 h55db66e_0
   - sysroot_linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/binutils_impl_linux-64-2.40-hf600244_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/binutils_impl_linux-64-2.40-ha885e6a_0.conda
   hash:
-    md5: 33084421a8c0af6aef1b439707f7662a
-    sha256: a7e0ea2b71a5b03d82e5a58fb6b612ab1c44d72ce161f9aa441f7ba467cd4c8d
-  build: hf600244_0
+    md5: 800a4c872b5bc06fa83888d112fe6c4f
+    sha256: 180b268f207d1481beb9de5c173751d14c429a7226fa9a85941e4a54cf6be1b4
+  build: ha885e6a_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: GPL-3.0-only
   license_family: GPL
-  size: 5414922
-  timestamp: 1674833958334
+  size: 5797310
+  timestamp: 1713651250214
 - platform: linux-64
   name: binutils_linux-64
   version: '2.40'
   category: main
   manager: conda
   dependencies:
   - binutils_impl_linux-64 2.40.*
@@ -1414,14 +1815,38 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 46932
   timestamp: 1712682252461
+- platform: osx-arm64
+  name: blosc
+  version: 1.21.5
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libzlib >=1.2.13,<1.3.0a0
+  - lz4-c >=1.9.3,<1.10.0a0
+  - snappy >=1.2.0,<1.3.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/blosc-1.21.5-h9c252e8_1.conda
+  hash:
+    md5: e1be80625e4f6bdc2154ee099c641683
+    sha256: 3b38493b95cc3d9f6369bbcbab55a2cdbbe6bbe32c74b923f8d638e874033139
+  build: h9c252e8_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 32983
+  timestamp: 1712682317564
 - platform: win-64
   name: blosc
   version: 1.21.5
   category: main
   manager: conda
   dependencies:
   - libzlib >=1.2.13,<1.3.0a0
@@ -1501,14 +1926,45 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 4689064
   timestamp: 1712901219432
   purls:
   - pkg:pypi/bokeh
+- platform: osx-arm64
+  name: bokeh
+  version: 3.4.1
+  category: main
+  manager: conda
+  dependencies:
+  - contourpy >=1.2
+  - jinja2 >=2.9
+  - numpy >=1.16
+  - packaging >=16.8
+  - pandas >=1.2
+  - pillow >=7.1.0
+  - python >=3.9
+  - pyyaml >=3.10
+  - tornado >=6.2
+  - xyzservices >=2021.09.1
+  url: https://conda.anaconda.org/conda-forge/noarch/bokeh-3.4.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 0f8e0831bbf38d83973438ce9af9af9a
+    sha256: 0289e61d7a30a693cf79d36484abd13f72ad785bd23cadc227c29dca89d95046
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 4689064
+  timestamp: 1712901219432
+  purls:
+  - pkg:pypi/bokeh
 - platform: win-64
   name: bokeh
   version: 3.4.1
   category: main
   manager: conda
   dependencies:
   - contourpy >=1.2
@@ -1575,14 +2031,35 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: MIT
   license_family: MIT
   size: 19530
   timestamp: 1695990310168
+- platform: osx-arm64
+  name: brotli
+  version: 1.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - brotli-bin 1.1.0 hb547adb_1
+  - libbrotlidec 1.1.0 hb547adb_1
+  - libbrotlienc 1.1.0 hb547adb_1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-1.1.0-hb547adb_1.conda
+  hash:
+    md5: a33aa58d448cbc054f887e39dd1dfaea
+    sha256: 62d1587deab752fcee07adc371eb20fcadc09f72c0c85399c22b637ca858020f
+  build: hb547adb_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 19506
+  timestamp: 1695990588610
 - platform: win-64
   name: brotli
   version: 1.1.0
   category: main
   manager: conda
   dependencies:
   - brotli-bin 1.1.0 hcfcfb64_1
@@ -1640,14 +2117,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: MIT
   license_family: MIT
   size: 16660
   timestamp: 1695990286737
+- platform: osx-arm64
+  name: brotli-bin
+  version: 1.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - libbrotlidec 1.1.0 hb547adb_1
+  - libbrotlienc 1.1.0 hb547adb_1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-bin-1.1.0-hb547adb_1.conda
+  hash:
+    md5: 990d04f8c017b1b77103f9a7730a5f12
+    sha256: 8fbfc2834606292016f2faffac67deea4c5cdbc21a61169f0b355e1600105a24
+  build: hb547adb_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 17001
+  timestamp: 1695990551239
 - platform: win-64
   name: brotli-bin
   version: 1.1.0
   category: main
   manager: conda
   dependencies:
   - libbrotlidec 1.1.0 hcfcfb64_1
@@ -1710,14 +2207,38 @@
   build_number: 1
   constrains:
   - libbrotlicommon 1.1.0 h0dc2134_1
   license: MIT
   license_family: MIT
   size: 367037
   timestamp: 1695990378635
+- platform: osx-arm64
+  name: brotli-python
+  version: 1.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=15.0.7
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-python-1.1.0-py310h1253130_1.conda
+  hash:
+    md5: 26fab7f65a80fff9f402ec3b7860b88a
+    sha256: dab21e18c0275bfd93a09b751096998485677ed17c2e2d08298bc5b43c10bee1
+  build: py310h1253130_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  constrains:
+  - libbrotlicommon 1.1.0 hb547adb_1
+  license: MIT
+  license_family: MIT
+  size: 344275
+  timestamp: 1695990848681
 - platform: win-64
   name: brotli-python
   version: 1.1.0
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -1776,14 +2297,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 183140
   timestamp: 1607309287088
+- platform: osx-arm64
+  name: brunsli
+  version: '0.1'
+  category: main
+  manager: conda
+  dependencies:
+  - brotli >=1.0.9,<2.0a0
+  - libcxx >=11.0.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/brunsli-0.1-h9f76cd9_0.tar.bz2
+  hash:
+    md5: 37a072dad6b844df1b5a32428bb08692
+    sha256: 816f929193a614b9a663e76e4267994ad99d04812b8a8e513e957d750deb4b04
+  build: h9f76cd9_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 178300
+  timestamp: 1607309265926
 - platform: linux-64
   name: bzip2
   version: 1.0.8
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -1813,14 +2354,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 5
   license: bzip2-1.0.6
   license_family: BSD
   size: 127885
   timestamp: 1699280178474
+- platform: osx-arm64
+  name: bzip2
+  version: 1.0.8
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
+  hash:
+    md5: 1bbc659ca658bfd49a481b5ef7a0f40f
+    sha256: bfa84296a638bea78a8bb29abc493ee95f2a0218775642474a840411b950fe5f
+  build: h93a5062_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  license: bzip2-1.0.6
+  license_family: BSD
+  size: 122325
+  timestamp: 1699280294368
 - platform: win-64
   name: bzip2
   version: 1.0.8
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -1871,14 +2430,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 152607
   timestamp: 1711819681694
+- platform: osx-arm64
+  name: c-ares
+  version: 1.28.1
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/c-ares-1.28.1-h93a5062_0.conda
+  hash:
+    md5: 04f776a6139f7eafc2f38668570eb7db
+    sha256: 2fc553d7a75e912efbdd6b82cd7916cc9cb2773e6cd873b77e02d631dd7be698
+  build: h93a5062_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 150488
+  timestamp: 1711819630164
 - platform: win-64
   name: c-ares
   version: 1.28.1
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -1937,14 +2514,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 278885
   timestamp: 1712846740754
+- platform: osx-arm64
+  name: c-blosc2
+  version: 2.14.4
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - lz4-c >=1.9.3,<1.10.0a0
+  - zlib-ng >=2.0.7,<2.1.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/c-blosc2-2.14.4-ha57e6be_1.conda
+  hash:
+    md5: e41d85c09af916227139aa0289f09b7f
+    sha256: 49421def0fb3e633b738fe4796f5aa0e99399ac603cc12ad089b40523a4d4e0a
+  build: ha57e6be_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 239927
+  timestamp: 1712841405614
 - platform: win-64
   name: c-blosc2
   version: 2.14.3
   category: main
   manager: conda
   dependencies:
   - lz4-c >=1.9.3,<1.10.0a0
@@ -1995,14 +2594,31 @@
   build: h8857fd0_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: ISC
   size: 155665
   timestamp: 1706843838227
+- platform: osx-arm64
+  name: ca-certificates
+  version: 2024.2.2
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
+  hash:
+    md5: fb416a1795f18dcc5a038bc2dc54edf9
+    sha256: 49bc3439816ac72d0c0e0f144b8cc870fdcc4adec2e861407ec818d8116b2204
+  build: hf0a4a13_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: ISC
+  size: 155725
+  timestamp: 1706844034242
 - platform: win-64
   name: ca-certificates
   version: 2024.2.2
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
@@ -2052,14 +2668,34 @@
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 4134
   timestamp: 1615209571450
+- platform: osx-arm64
+  name: cached-property
+  version: 1.5.2
+  category: main
+  manager: conda
+  dependencies:
+  - cached_property >=1.5.2,<1.5.3.0a0
+  url: https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2
+  hash:
+    md5: 9b347a7ec10940d3f7941ff6c460b551
+    sha256: 561e6660f26c35d137ee150187d89767c988413c978e1b712d53f27ddf70ea17
+  build: hd8ed1ab_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 4134
+  timestamp: 1615209571450
 - platform: win-64
   name: cached-property
   version: 1.5.2
   category: main
   manager: conda
   dependencies:
   - cached_property >=1.5.2,<1.5.3.0a0
@@ -2116,14 +2752,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 11065
   timestamp: 1615209567874
   purls:
   - pkg:pypi/cached-property
+- platform: osx-arm64
+  name: cached_property
+  version: 1.5.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2
+  hash:
+    md5: 576d629e47797577ab0f1b351297ef4a
+    sha256: 6dbf7a5070cc43d90a1e4c2ec0c541c69d8e30a0e25f50ce9f6e4a432e42c5d7
+  build: pyha770c72_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 11065
+  timestamp: 1615209567874
+  purls:
+  - pkg:pypi/cached-property
 - platform: win-64
   name: cached_property
   version: 1.5.2
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -2200,14 +2858,42 @@
   build: h99e66fa_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: LGPL-2.1-only or MPL-1.1
   size: 885311
   timestamp: 1697028802967
+- platform: osx-arm64
+  name: cairo
+  version: 1.18.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=10.9
+  - fontconfig >=2.14.2,<3.0a0
+  - fonts-conda-ecosystem
+  - freetype >=2.12.1,<3.0a0
+  - icu >=73.2,<74.0a0
+  - libcxx >=16.0.6
+  - libglib >=2.78.0,<3.0a0
+  - libpng >=1.6.39,<1.7.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - pixman >=0.42.2,<1.0a0
+  - zlib
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/cairo-1.18.0-hd1e100b_0.conda
+  hash:
+    md5: 3fa6eebabb77f65e82f86b72b95482db
+    sha256: 599f8820553b3a3405706d9cad390ac199e24515a0a82c87153c9b5b5fdba3b8
+  build: hd1e100b_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: LGPL-2.1-only or MPL-1.1
+  size: 897919
+  timestamp: 1697028755150
 - platform: win-64
   name: cairo
   version: 1.18.0
   category: main
   manager: conda
   dependencies:
   - fontconfig >=2.14.2,<3.0a0
@@ -2256,14 +2942,41 @@
   - ld64 711.*
   - cctools 986.*
   - clang 18.1.*
   license: APSL-2.0
   license_family: Other
   size: 1104790
   timestamp: 1710484461097
+- platform: osx-arm64
+  name: cctools_osx-arm64
+  version: '986'
+  category: main
+  manager: conda
+  dependencies:
+  - ld64_osx-arm64 >=711,<712.0a0
+  - libcxx
+  - libllvm18 >=18.1.1,<18.2.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - sigtool
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/cctools_osx-arm64-986-hd11630f_0.conda
+  hash:
+    md5: cce200c91b2d291c85e66098fe0d31c2
+    sha256: 4152323bbb78e2730fea9004333c9c51fb82a9ddd935f005280bf621849ec53d
+  build: hd11630f_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - cctools 986.*
+  - clang 18.1.*
+  - ld64 711.*
+  license: APSL-2.0
+  license_family: Other
+  size: 1123368
+  timestamp: 1710484635601
 - platform: linux-64
   name: certifi
   version: 2024.2.2
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -2294,14 +3007,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: ISC
   noarch: python
   size: 160559
   timestamp: 1707022289175
+- platform: osx-arm64
+  name: certifi
+  version: 2024.2.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: 0876280e409658fc6f9e75d035960333
+    sha256: f1faca020f988696e6b6ee47c82524c7806380b37cfdd1def32f92c326caca54
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: ISC
+  noarch: python
+  size: 160559
+  timestamp: 1707022289175
 - platform: win-64
   name: certifi
   version: 2024.2.2
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -2376,14 +3108,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 138062
   timestamp: 1684263362836
+- platform: osx-arm64
+  name: charls
+  version: 2.4.2
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=15.0.7
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/charls-2.4.2-h13dd4ca_0.conda
+  hash:
+    md5: 6faf3cf8df25572c7f70138a45f37363
+    sha256: b9f79954e6d37ad59016b434abfdd096a75ff08c6de14e5198bcea497a10fae5
+  build: h13dd4ca_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 116255
+  timestamp: 1684263271583
 - platform: win-64
   name: charls
   version: 2.4.2
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -2421,14 +3172,38 @@
   - llvm 18.1.3.*
   - llvm-tools 18.1.3.*
   - llvmdev 18.1.3.*
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 22898
   timestamp: 1712569254288
+- platform: osx-arm64
+  name: clang
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - clang-18 18.1.3 default_he012953_0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/clang-18.1.3-default_h4cf2255_0.conda
+  hash:
+    md5: efbaa3d968b1dcacba9eb980d1ab66f4
+    sha256: 613f4c4773f1dd274d2682a9170d52cb466f437a47ebcad2c2634c3b37aeb73f
+  build: default_h4cf2255_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - clang-tools 18.1.3.*
+  - llvm 18.1.3.*
+  - llvm-tools 18.1.3.*
+  - llvmdev 18.1.3.*
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 22913
+  timestamp: 1712569692457
 - platform: win-64
   name: clang
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - clang-18 18.1.3 default_h3a3e6c3_0
@@ -2473,14 +3248,40 @@
   - llvm-tools 18.1.3
   - clang-tools 18.1.3
   - clangdev 18.1.3
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 760437
   timestamp: 1712569132861
+- platform: osx-arm64
+  name: clang-18
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - libclang-cpp18.1 18.1.3 default_he012953_0
+  - libcxx >=16.0.6
+  - libllvm18 >=18.1.3,<18.2.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/clang-18-18.1.3-default_he012953_0.conda
+  hash:
+    md5: 931dd6124b399ae12172f235f5ace407
+    sha256: edb5c1e2ffc7704b0e0bce0f5315eb1aba8fd9710e61bcbdeb40e340720123c6
+  build: default_he012953_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - clang-tools 18.1.3
+  - clangxx 18.1.3
+  - llvm-tools 18.1.3
+  - clangdev 18.1.3
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 754206
+  timestamp: 1712569562918
 - platform: win-64
   name: clang-18
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - libzlib >=1.2.13,<1.3.0a0
@@ -2524,14 +3325,37 @@
   arch: x86_64
   subdir: osx-64
   build_number: 11
   license: BSD-3-Clause
   license_family: BSD
   size: 17413
   timestamp: 1712621383914
+- platform: osx-arm64
+  name: clang_impl_osx-arm64
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - cctools_osx-arm64
+  - clang 18.1.3.*
+  - compiler-rt 18.1.3.*
+  - ld64_osx-arm64
+  - llvm-tools 18.1.3.*
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/clang_impl_osx-arm64-18.1.3-hda94301_11.conda
+  hash:
+    md5: 90e54a957e833f7cd2412b6d2e1d84fa
+    sha256: f00e3930fa341ad5fa87a90f297b385a949bf2ee100a3a2cc2a135629fde6d7e
+  build: hda94301_11
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 11
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 17571
+  timestamp: 1712621386541
 - platform: osx-64
   name: clang_osx-64
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - clang_impl_osx-64 18.1.3 hdbcc6ac_11
@@ -2543,14 +3367,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 11
   license: BSD-3-Clause
   license_family: BSD
   size: 20494
   timestamp: 1712621391590
+- platform: osx-arm64
+  name: clang_osx-arm64
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - clang_impl_osx-arm64 18.1.3 hda94301_11
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/clang_osx-arm64-18.1.3-h54d7cd3_11.conda
+  hash:
+    md5: 7bdafeb8d61d59551df2417995bc3d46
+    sha256: 595cbec0f835ba16ad551315079193d16fc7f3a4e136aa1045ab9104cac79bf7
+  build: h54d7cd3_11
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 11
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 20490
+  timestamp: 1712621394350
 - platform: osx-64
   name: clangxx
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - clang 18.1.3 default_h7151d67_0
@@ -2562,14 +3405,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 22972
   timestamp: 1712569279378
+- platform: osx-arm64
+  name: clangxx
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - clang 18.1.3 default_h4cf2255_0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/clangxx-18.1.3-default_h4cf2255_0.conda
+  hash:
+    md5: fd98656c5b62774633c84c41f42bdd6d
+    sha256: 1f9c1605d4f74b1d5df7d44676a5a6c53d542fc8c44d94fcc1d4d1977cede661
+  build: default_h4cf2255_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 22939
+  timestamp: 1712569715149
 - platform: win-64
   name: clangxx
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - clang 18.1.3 default_hb53fc94_0
@@ -2605,14 +3467,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 11
   license: BSD-3-Clause
   license_family: BSD
   size: 17496
   timestamp: 1712621429065
+- platform: osx-arm64
+  name: clangxx_impl_osx-arm64
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - clang_osx-arm64 18.1.3 h54d7cd3_11
+  - clangxx 18.1.3.*
+  - libcxx >=16
+  - libllvm18 >=18.1.3,<18.2.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/clangxx_impl_osx-arm64-18.1.3-h1ba0cb9_11.conda
+  hash:
+    md5: 5c29e4473f07af49ced6984531048fa4
+    sha256: 91c6d2a6d9555110d6710d3766eb724dfdeed17b23a7965649523675d2251fce
+  build: h1ba0cb9_11
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 11
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 17636
+  timestamp: 1712621421262
 - platform: osx-64
   name: clangxx_osx-64
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - clang_osx-64 18.1.3 hb91bd55_11
@@ -2625,14 +3509,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 11
   license: BSD-3-Clause
   license_family: BSD
   size: 19255
   timestamp: 1712621436405
+- platform: osx-arm64
+  name: clangxx_osx-arm64
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - clang_osx-arm64 18.1.3 h54d7cd3_11
+  - clangxx_impl_osx-arm64 18.1.3 h1ba0cb9_11
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/clangxx_osx-arm64-18.1.3-h54d7cd3_11.conda
+  hash:
+    md5: 3b5c8fe78441bc034aceadfa80dae7cc
+    sha256: c92c008817c2e25409b1328e580798855d082b504b39d8f42b21791da215c9f6
+  build: h54d7cd3_11
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 11
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 19244
+  timestamp: 1712621431069
 - platform: linux-64
   name: click
   version: 8.1.7
   category: main
   manager: conda
   dependencies:
   - __unix
@@ -2671,14 +3575,37 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 84437
   timestamp: 1692311973840
   purls:
   - pkg:pypi/click
+- platform: osx-arm64
+  name: click
+  version: 8.1.7
+  category: main
+  manager: conda
+  dependencies:
+  - __unix
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
+  hash:
+    md5: f3ad426304898027fc619827ff428eca
+    sha256: f0016cbab6ac4138a429e28dbcb904a90305b34b3fe41a9b89d697c90401caec
+  build: unix_pyh707e725_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 84437
+  timestamp: 1692311973840
+  purls:
+  - pkg:pypi/click
 - platform: win-64
   name: click
   version: 8.1.7
   category: main
   manager: conda
   dependencies:
   - __win
@@ -2739,14 +3666,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 24746
   timestamp: 1697464875382
   purls:
   - pkg:pypi/cloudpickle
+- platform: osx-arm64
+  name: cloudpickle
+  version: 3.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/cloudpickle-3.0.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 753d29fe41bb881e4b9c004f0abf973f
+    sha256: 0dfbc1ffa72e7a0882f486c9b1e4e9cccb68cf5c576fe53a89d076c9f1d43754
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 24746
+  timestamp: 1697464875382
+  purls:
+  - pkg:pypi/cloudpickle
 - platform: win-64
   name: cloudpickle
   version: 3.0.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -2805,14 +3754,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 25170
   timestamp: 1666700778190
   purls:
   - pkg:pypi/colorama
+- platform: osx-arm64
+  name: colorama
+  version: 0.4.6
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 3faab06a954c2a04039983f2c4a50d99
+    sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 25170
+  timestamp: 1666700778190
+  purls:
+  - pkg:pypi/colorama
 - platform: win-64
   name: colorama
   version: 0.4.6
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -2871,14 +3842,37 @@
   build_number: 0
   license: MIT
   license_family: MIT
   size: 19810
   timestamp: 1706286038997
   purls:
   - pkg:pypi/colorlog
+- platform: osx-arm64
+  name: colorlog
+  version: 6.8.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/colorlog-6.8.2-py310hbe9552e_0.conda
+  hash:
+    md5: b452cbe13136d50bcb4c2b9e192cd43d
+    sha256: ff2cbb212014224ebbd686979a642a9fcdef720ab9dba3b9d4ef47ceb0677682
+  build: py310hbe9552e_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 20119
+  timestamp: 1706286200602
+  purls:
+  - pkg:pypi/colorlog
 - platform: win-64
   name: colorlog
   version: 6.8.2
   category: main
   manager: conda
   dependencies:
   - colorama
@@ -2915,14 +3909,35 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0 WITH LLVM-exception
   license_family: APACHE
   size: 96452
   timestamp: 1712580504480
+- platform: osx-arm64
+  name: compiler-rt
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - clang 18.1.3.*
+  - clangxx 18.1.3.*
+  - compiler-rt_osx-arm64 18.1.3.*
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/compiler-rt-18.1.3-h3808999_0.conda
+  hash:
+    md5: 09f614cf0dc4ea2b249c2e522b337730
+    sha256: dfada604649fb2cfa6fb3dbd657fccf81cd01e00a7f6f29da24fc40e36cd51fa
+  build: h3808999_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: APACHE
+  size: 96152
+  timestamp: 1712580507858
 - platform: osx-64
   name: compiler-rt_osx-64
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - clang 18.1.3.*
@@ -2938,14 +3953,37 @@
   constrains:
   - compiler-rt 18.1.3
   license: Apache-2.0 WITH LLVM-exception
   license_family: APACHE
   noarch: generic
   size: 10367732
   timestamp: 1712580438913
+- platform: osx-arm64
+  name: compiler-rt_osx-arm64
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - clang 18.1.3.*
+  - clangxx 18.1.3.*
+  url: https://conda.anaconda.org/conda-forge/noarch/compiler-rt_osx-arm64-18.1.3-h3808999_0.conda
+  hash:
+    md5: 78c11131b59e53aedcf7854956a9347c
+    sha256: 4bbe97d77ae12edd5c0206d014e0473ae8c4fcacbc1e1b21e8e92fd694608301
+  build: h3808999_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - compiler-rt 18.1.3
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: APACHE
+  noarch: generic
+  size: 10165573
+  timestamp: 1712580450851
 - platform: linux-64
   name: contourpy
   version: 1.2.1
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -2987,14 +4025,39 @@
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 233310
   timestamp: 1712430195722
   purls:
   - pkg:pypi/contourpy
+- platform: osx-arm64
+  name: contourpy
+  version: 1.2.1
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - numpy >=1.20
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/contourpy-1.2.1-py310h21239e6_0.conda
+  hash:
+    md5: db10923835b6b8c082b126c7cbbe50ff
+    sha256: 3b97cb954719a53ea66e0c024eb9a5ed28da61036a2c74b9104eaac425ee95fd
+  build: py310h21239e6_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 226024
+  timestamp: 1712430306572
+  purls:
+  - pkg:pypi/contourpy
 - platform: win-64
   name: contourpy
   version: 1.2.1
   category: main
   manager: conda
   dependencies:
   - numpy >=1.20
@@ -3015,83 +4078,109 @@
   license_family: BSD
   size: 189962
   timestamp: 1712430301862
   purls:
   - pkg:pypi/contourpy
 - platform: linux-64
   name: coverage
-  version: 7.4.4
+  version: 7.5.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
   - python >=3.10,<3.11.0a0
   - python_abi 3.10.* *_cp310
   - tomli
-  url: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.4-py310h2372a71_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.0-py310hc51659f_0.conda
   hash:
-    md5: 2d948842110ae68e4f2e7738f92bf7e1
-    sha256: e95f08ca0f555a5e16e7ef800317e04a237ef6622073d1c9dfb8792a06d28336
-  build: py310h2372a71_0
+    md5: 3609fdb03842f67e2ec68a9c137221b8
+    sha256: b7f29f2cef34873a7f345a989c8203507b4f177fe54a864c5f8c82d29bf10373
+  build: py310hc51659f_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
-  size: 289440
-  timestamp: 1710462962144
+  size: 293491
+  timestamp: 1713908143438
   purls:
   - pkg:pypi/coverage
 - platform: osx-64
   name: coverage
-  version: 7.4.4
+  version: 7.5.0
   category: main
   manager: conda
   dependencies:
+  - __osx >=10.9
   - python >=3.10,<3.11.0a0
   - python_abi 3.10.* *_cp310
   - tomli
-  url: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.4.4-py310hb372a2b_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.0-py310h74a5a53_0.conda
   hash:
-    md5: 9036869b7b769be5d2c9efcb89155bf7
-    sha256: a95c1faac282519626990b399803d9c47025e17a03f088fc1004359ec26a954d
-  build: py310hb372a2b_0
+    md5: 95f7866059c6f718effd7939d583d6d0
+    sha256: 21809604ee17e6f4987e4692d461905a645aca1606f0db3d6806d907d842f77e
+  build: py310h74a5a53_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
-  size: 287682
-  timestamp: 1710463314543
+  size: 293861
+  timestamp: 1713908291942
+  purls:
+  - pkg:pypi/coverage
+- platform: osx-arm64
+  name: coverage
+  version: 7.5.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - tomli
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.0-py310h8431ef1_0.conda
+  hash:
+    md5: 786d0b18a15c116c01f3c530d6c7e0d2
+    sha256: d6a28f94a02e25d608cf78f8af154767eb55612b6bfce5d3494003ca8503ec1c
+  build: py310h8431ef1_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  size: 293836
+  timestamp: 1713908497071
   purls:
   - pkg:pypi/coverage
 - platform: win-64
   name: coverage
-  version: 7.4.4
+  version: 7.5.0
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
   - python_abi 3.10.* *_cp310
   - tomli
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
-  url: https://conda.anaconda.org/conda-forge/win-64/coverage-7.4.4-py310h8d17308_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.0-py310ha8f682b_0.conda
   hash:
-    md5: f52d17cf10b0451ec05c24d14f72870b
-    sha256: 1d12680e79b05ef32d04142539307b2744de2e6798870340ac27982e2adb052d
-  build: py310h8d17308_0
+    md5: 02ca9058b92ec2c17bf9f392d2548c35
+    sha256: 67ca0a658cb4714c197dd8acff394eb49d307d368b8a0339ca359197141f1fe5
+  build: py310ha8f682b_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
-  size: 305911
-  timestamp: 1710463439024
+  size: 311424
+  timestamp: 1713908762259
   purls:
   - pkg:pypi/coverage
 - platform: linux-64
   name: cycler
   version: 0.12.1
   category: main
   manager: conda
@@ -3130,14 +4219,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 13458
   timestamp: 1696677888423
   purls:
   - pkg:pypi/cycler
+- platform: osx-arm64
+  name: cycler
+  version: 0.12.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/cycler-0.12.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 5cd86562580f274031ede6aa6aa24441
+    sha256: f221233f21b1d06971792d491445fd548224641af9443739b4b7b6d5d72954a8
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 13458
+  timestamp: 1696677888423
+  purls:
+  - pkg:pypi/cycler
 - platform: win-64
   name: cycler
   version: 0.12.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -3199,14 +4310,38 @@
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 316676
   timestamp: 1706897332355
   purls:
   - pkg:pypi/cytoolz
+- platform: osx-arm64
+  name: cytoolz
+  version: 0.12.3
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - toolz >=0.10.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/cytoolz-0.12.3-py310hd125d64_0.conda
+  hash:
+    md5: a2d459b5f4df33378ff8089e31a9460a
+    sha256: 82841782ce65086bbc90e5736c0b494f6aaa7d4424490517ff7ba483fcd40aab
+  build: py310hd125d64_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 315555
+  timestamp: 1706897593187
+  purls:
+  - pkg:pypi/cytoolz
 - platform: win-64
   name: cytoolz
   version: 0.12.3
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -3227,274 +4362,362 @@
   license_family: BSD
   size: 295577
   timestamp: 1706897660502
   purls:
   - pkg:pypi/cytoolz
 - platform: linux-64
   name: dask
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - bokeh >=2.4.2,!=3.0.*
   - cytoolz >=0.11.0
-  - dask-core >=2024.4.1,<2024.4.2.0a0
+  - dask-core >=2024.4.2,<2024.4.3.0a0
   - dask-expr >=1.0,<1.1
-  - distributed >=2024.4.1,<2024.4.2.0a0
+  - distributed >=2024.4.2,<2024.4.3.0a0
   - jinja2 >=2.10.3
   - lz4 >=4.3.2
   - numpy >=1.21
   - pandas >=1.3
   - pyarrow >=7.0
   - pyarrow-hotfix
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1afbed2c3ca32ee7c7acd9939460ddd3
-    sha256: 5f6151fcb5e5395c3e2601e969645c5b8097db74381a3e41001dce846937ab7b
+    md5: a0e5045f4fae04acbe70f4c821d65302
+    sha256: 7c12de297cef16920dd96ec0796578b071086dfbe6d7befb1a9c6ceaaf4c572a
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   constrains:
   - openssl !=1.1.1e
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 7461
-  timestamp: 1712330526382
+  size: 7540
+  timestamp: 1713583754159
 - platform: osx-64
   name: dask
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - bokeh >=2.4.2,!=3.0.*
   - cytoolz >=0.11.0
-  - dask-core >=2024.4.1,<2024.4.2.0a0
+  - dask-core >=2024.4.2,<2024.4.3.0a0
   - dask-expr >=1.0,<1.1
-  - distributed >=2024.4.1,<2024.4.2.0a0
+  - distributed >=2024.4.2,<2024.4.3.0a0
   - jinja2 >=2.10.3
   - lz4 >=4.3.2
   - numpy >=1.21
   - pandas >=1.3
   - pyarrow >=7.0
   - pyarrow-hotfix
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1afbed2c3ca32ee7c7acd9939460ddd3
-    sha256: 5f6151fcb5e5395c3e2601e969645c5b8097db74381a3e41001dce846937ab7b
+    md5: a0e5045f4fae04acbe70f4c821d65302
+    sha256: 7c12de297cef16920dd96ec0796578b071086dfbe6d7befb1a9c6ceaaf4c572a
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   constrains:
   - openssl !=1.1.1e
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 7461
-  timestamp: 1712330526382
+  size: 7540
+  timestamp: 1713583754159
+- platform: osx-arm64
+  name: dask
+  version: 2024.4.2
+  category: main
+  manager: conda
+  dependencies:
+  - bokeh >=2.4.2,!=3.0.*
+  - cytoolz >=0.11.0
+  - dask-core >=2024.4.2,<2024.4.3.0a0
+  - dask-expr >=1.0,<1.1
+  - distributed >=2024.4.2,<2024.4.3.0a0
+  - jinja2 >=2.10.3
+  - lz4 >=4.3.2
+  - numpy >=1.21
+  - pandas >=1.3
+  - pyarrow >=7.0
+  - pyarrow-hotfix
+  - python >=3.9
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-2024.4.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: a0e5045f4fae04acbe70f4c821d65302
+    sha256: 7c12de297cef16920dd96ec0796578b071086dfbe6d7befb1a9c6ceaaf4c572a
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - openssl !=1.1.1e
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 7540
+  timestamp: 1713583754159
 - platform: win-64
   name: dask
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - bokeh >=2.4.2,!=3.0.*
   - cytoolz >=0.11.0
-  - dask-core >=2024.4.1,<2024.4.2.0a0
+  - dask-core >=2024.4.2,<2024.4.3.0a0
   - dask-expr >=1.0,<1.1
-  - distributed >=2024.4.1,<2024.4.2.0a0
+  - distributed >=2024.4.2,<2024.4.3.0a0
   - jinja2 >=2.10.3
   - lz4 >=4.3.2
   - numpy >=1.21
   - pandas >=1.3
   - pyarrow >=7.0
   - pyarrow-hotfix
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 1afbed2c3ca32ee7c7acd9939460ddd3
-    sha256: 5f6151fcb5e5395c3e2601e969645c5b8097db74381a3e41001dce846937ab7b
+    md5: a0e5045f4fae04acbe70f4c821d65302
+    sha256: 7c12de297cef16920dd96ec0796578b071086dfbe6d7befb1a9c6ceaaf4c572a
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   constrains:
   - openssl !=1.1.1e
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 7461
-  timestamp: 1712330526382
+  size: 7540
+  timestamp: 1713583754159
 - platform: linux-64
   name: dask-core
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - click >=8.1
   - cloudpickle >=1.5.0
   - fsspec >=2021.09.0
   - importlib_metadata >=4.13.0
   - packaging >=20.0
   - partd >=1.2.0
   - python >=3.9
   - pyyaml >=5.3.1
   - toolz >=0.10.0
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 52387f00fee8dcd5cf75f8886025293f
-    sha256: b5df58b0b24da66acb21343a054e0f04edaf74c6aacf936422e2b000cd654457
+    md5: bb4e6c52855aa64a5443ca4eedaa6cfe
+    sha256: 5911f7de216d57941d1eeb77d6bfa224bd3d7370957807381be1c5c437ac07f0
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 880975
-  timestamp: 1712248575509
+  size: 881318
+  timestamp: 1713561560483
   purls:
   - pkg:pypi/dask
 - platform: osx-64
   name: dask-core
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - click >=8.1
   - cloudpickle >=1.5.0
   - fsspec >=2021.09.0
   - importlib_metadata >=4.13.0
   - packaging >=20.0
   - partd >=1.2.0
   - python >=3.9
   - pyyaml >=5.3.1
   - toolz >=0.10.0
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 52387f00fee8dcd5cf75f8886025293f
-    sha256: b5df58b0b24da66acb21343a054e0f04edaf74c6aacf936422e2b000cd654457
+    md5: bb4e6c52855aa64a5443ca4eedaa6cfe
+    sha256: 5911f7de216d57941d1eeb77d6bfa224bd3d7370957807381be1c5c437ac07f0
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 880975
-  timestamp: 1712248575509
+  size: 881318
+  timestamp: 1713561560483
+  purls:
+  - pkg:pypi/dask
+- platform: osx-arm64
+  name: dask-core
+  version: 2024.4.2
+  category: main
+  manager: conda
+  dependencies:
+  - click >=8.1
+  - cloudpickle >=1.5.0
+  - fsspec >=2021.09.0
+  - importlib_metadata >=4.13.0
+  - packaging >=20.0
+  - partd >=1.2.0
+  - python >=3.9
+  - pyyaml >=5.3.1
+  - toolz >=0.10.0
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: bb4e6c52855aa64a5443ca4eedaa6cfe
+    sha256: 5911f7de216d57941d1eeb77d6bfa224bd3d7370957807381be1c5c437ac07f0
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 881318
+  timestamp: 1713561560483
   purls:
   - pkg:pypi/dask
 - platform: win-64
   name: dask-core
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - click >=8.1
   - cloudpickle >=1.5.0
   - fsspec >=2021.09.0
   - importlib_metadata >=4.13.0
   - packaging >=20.0
   - partd >=1.2.0
   - python >=3.9
   - pyyaml >=5.3.1
   - toolz >=0.10.0
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-core-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 52387f00fee8dcd5cf75f8886025293f
-    sha256: b5df58b0b24da66acb21343a054e0f04edaf74c6aacf936422e2b000cd654457
+    md5: bb4e6c52855aa64a5443ca4eedaa6cfe
+    sha256: 5911f7de216d57941d1eeb77d6bfa224bd3d7370957807381be1c5c437ac07f0
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 880975
-  timestamp: 1712248575509
+  size: 881318
+  timestamp: 1713561560483
   purls:
   - pkg:pypi/dask
 - platform: linux-64
   name: dask-expr
-  version: 1.0.11
+  version: 1.0.13
   category: main
   manager: conda
   dependencies:
-  - dask-core 2024.4.1
+  - dask-core 2024.4.2
   - pandas >=2
   - pyarrow
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-expr-1.0.11-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-expr-1.0.13-pyhd8ed1ab_0.conda
   hash:
-    md5: 5c6bc104095ed12db6b1be04181e9afa
-    sha256: 193e176d808268a7eed7ea5c3f8f68ba3ab03cd9ff94cd5b2369d3d03fabe8cd
+    md5: c4343d7c870bbb7839e071a531fc8959
+    sha256: 757bb4d51d90b047a9dcb9c68fdd700a9ff5144a9c63a4259066ce068228d808
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 142972
-  timestamp: 1712693926118
+  size: 151290
+  timestamp: 1714138223942
   purls:
   - pkg:pypi/dask-expr
 - platform: osx-64
   name: dask-expr
-  version: 1.0.11
+  version: 1.0.13
   category: main
   manager: conda
   dependencies:
-  - dask-core 2024.4.1
+  - dask-core 2024.4.2
   - pandas >=2
   - pyarrow
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-expr-1.0.11-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-expr-1.0.13-pyhd8ed1ab_0.conda
   hash:
-    md5: 5c6bc104095ed12db6b1be04181e9afa
-    sha256: 193e176d808268a7eed7ea5c3f8f68ba3ab03cd9ff94cd5b2369d3d03fabe8cd
+    md5: c4343d7c870bbb7839e071a531fc8959
+    sha256: 757bb4d51d90b047a9dcb9c68fdd700a9ff5144a9c63a4259066ce068228d808
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 142972
-  timestamp: 1712693926118
+  size: 151290
+  timestamp: 1714138223942
+  purls:
+  - pkg:pypi/dask-expr
+- platform: osx-arm64
+  name: dask-expr
+  version: 1.0.13
+  category: main
+  manager: conda
+  dependencies:
+  - dask-core 2024.4.2
+  - pandas >=2
+  - pyarrow
+  - python >=3.9
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-expr-1.0.13-pyhd8ed1ab_0.conda
+  hash:
+    md5: c4343d7c870bbb7839e071a531fc8959
+    sha256: 757bb4d51d90b047a9dcb9c68fdd700a9ff5144a9c63a4259066ce068228d808
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 151290
+  timestamp: 1714138223942
   purls:
   - pkg:pypi/dask-expr
 - platform: win-64
   name: dask-expr
-  version: 1.0.11
+  version: 1.0.13
   category: main
   manager: conda
   dependencies:
-  - dask-core 2024.4.1
+  - dask-core 2024.4.2
   - pandas >=2
   - pyarrow
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/dask-expr-1.0.11-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/dask-expr-1.0.13-pyhd8ed1ab_0.conda
   hash:
-    md5: 5c6bc104095ed12db6b1be04181e9afa
-    sha256: 193e176d808268a7eed7ea5c3f8f68ba3ab03cd9ff94cd5b2369d3d03fabe8cd
+    md5: c4343d7c870bbb7839e071a531fc8959
+    sha256: 757bb4d51d90b047a9dcb9c68fdd700a9ff5144a9c63a4259066ce068228d808
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 142972
-  timestamp: 1712693926118
+  size: 151290
+  timestamp: 1714138223942
   purls:
   - pkg:pypi/dask-expr
 - platform: linux-64
   name: dav1d
   version: 1.2.1
   category: main
   manager: conda
@@ -3526,14 +4749,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   size: 668439
   timestamp: 1685696184631
+- platform: osx-arm64
+  name: dav1d
+  version: 1.2.1
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/dav1d-1.2.1-hb547adb_0.conda
+  hash:
+    md5: 5a74cdee497e6b65173e10d94582fae6
+    sha256: 93e077b880a85baec8227e8c72199220c7f87849ad32d02c14fb3807368260b8
+  build: hb547adb_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 316394
+  timestamp: 1685695959391
 - platform: win-64
   name: dav1d
   version: 1.2.1
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -3612,14 +4853,36 @@
   license: BSD-2-Clause
   license_family: BSD
   noarch: python
   size: 12072
   timestamp: 1641555714315
   purls:
   - pkg:pypi/decorator
+- platform: osx-arm64
+  name: decorator
+  version: 5.1.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.5
+  url: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 43afe5ab04e35e17ba28649471dd7364
+    sha256: 328a6a379f9bdfd0230e51de291ce858e6479411ea4b0545fb377c71662ef3e2
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  noarch: python
+  size: 12072
+  timestamp: 1641555714315
+  purls:
+  - pkg:pypi/decorator
 - platform: win-64
   name: decorator
   version: 5.1.1
   category: main
   manager: conda
   dependencies:
   - python >=3.5
@@ -3636,130 +4899,170 @@
   noarch: python
   size: 12072
   timestamp: 1641555714315
   purls:
   - pkg:pypi/decorator
 - platform: linux-64
   name: distributed
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - click >=8.0
   - cloudpickle >=1.5.0
   - cytoolz >=0.10.1
-  - dask-core >=2024.4.1,<2024.4.2.0a0
+  - dask-core >=2024.4.2,<2024.4.3.0a0
   - jinja2 >=2.10.3
   - locket >=1.0.0
   - msgpack-python >=1.0.0
   - packaging >=20.0
   - psutil >=5.7.2
   - python >=3.9
   - pyyaml >=5.3.1
   - sortedcontainers >=2.0.5
   - tblib >=1.6.0
   - toolz >=0.10.0
   - tornado >=6.0.4
   - urllib3 >=1.24.3
   - zict >=3.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/distributed-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/distributed-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 822b8d8216764941bb099fea588127ad
-    sha256: 747ed8b12aff745c16ac415d17e0f76754fab992ea6ae68cf0c27f3fc2417b1f
+    md5: e4e11467ccf467cbe34cbe84dedbca77
+    sha256: 418df5d885310bb111637054baafe013b75e52cdc5116f844fc0d2aed4784bf5
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   constrains:
   - openssl !=1.1.1e
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 794424
-  timestamp: 1712327639715
+  size: 795222
+  timestamp: 1713569203054
   purls:
   - pkg:pypi/distributed
 - platform: osx-64
   name: distributed
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - click >=8.0
   - cloudpickle >=1.5.0
   - cytoolz >=0.10.1
-  - dask-core >=2024.4.1,<2024.4.2.0a0
+  - dask-core >=2024.4.2,<2024.4.3.0a0
   - jinja2 >=2.10.3
   - locket >=1.0.0
   - msgpack-python >=1.0.0
   - packaging >=20.0
   - psutil >=5.7.2
   - python >=3.9
   - pyyaml >=5.3.1
   - sortedcontainers >=2.0.5
   - tblib >=1.6.0
   - toolz >=0.10.0
   - tornado >=6.0.4
   - urllib3 >=1.24.3
   - zict >=3.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/distributed-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/distributed-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 822b8d8216764941bb099fea588127ad
-    sha256: 747ed8b12aff745c16ac415d17e0f76754fab992ea6ae68cf0c27f3fc2417b1f
+    md5: e4e11467ccf467cbe34cbe84dedbca77
+    sha256: 418df5d885310bb111637054baafe013b75e52cdc5116f844fc0d2aed4784bf5
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   constrains:
   - openssl !=1.1.1e
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 794424
-  timestamp: 1712327639715
+  size: 795222
+  timestamp: 1713569203054
+  purls:
+  - pkg:pypi/distributed
+- platform: osx-arm64
+  name: distributed
+  version: 2024.4.2
+  category: main
+  manager: conda
+  dependencies:
+  - click >=8.0
+  - cloudpickle >=1.5.0
+  - cytoolz >=0.10.1
+  - dask-core >=2024.4.2,<2024.4.3.0a0
+  - jinja2 >=2.10.3
+  - locket >=1.0.0
+  - msgpack-python >=1.0.0
+  - packaging >=20.0
+  - psutil >=5.7.2
+  - python >=3.9
+  - pyyaml >=5.3.1
+  - sortedcontainers >=2.0.5
+  - tblib >=1.6.0
+  - toolz >=0.10.0
+  - tornado >=6.0.4
+  - urllib3 >=1.24.3
+  - zict >=3.0.0
+  url: https://conda.anaconda.org/conda-forge/noarch/distributed-2024.4.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: e4e11467ccf467cbe34cbe84dedbca77
+    sha256: 418df5d885310bb111637054baafe013b75e52cdc5116f844fc0d2aed4784bf5
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - openssl !=1.1.1e
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 795222
+  timestamp: 1713569203054
   purls:
   - pkg:pypi/distributed
 - platform: win-64
   name: distributed
-  version: 2024.4.1
+  version: 2024.4.2
   category: main
   manager: conda
   dependencies:
   - click >=8.0
   - cloudpickle >=1.5.0
   - cytoolz >=0.10.1
-  - dask-core >=2024.4.1,<2024.4.2.0a0
+  - dask-core >=2024.4.2,<2024.4.3.0a0
   - jinja2 >=2.10.3
   - locket >=1.0.0
   - msgpack-python >=1.0.0
   - packaging >=20.0
   - psutil >=5.7.2
   - python >=3.9
   - pyyaml >=5.3.1
   - sortedcontainers >=2.0.5
   - tblib >=1.6.0
   - toolz >=0.10.0
   - tornado >=6.0.4
   - urllib3 >=1.24.3
   - zict >=3.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/distributed-2024.4.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/distributed-2024.4.2-pyhd8ed1ab_0.conda
   hash:
-    md5: 822b8d8216764941bb099fea588127ad
-    sha256: 747ed8b12aff745c16ac415d17e0f76754fab992ea6ae68cf0c27f3fc2417b1f
+    md5: e4e11467ccf467cbe34cbe84dedbca77
+    sha256: 418df5d885310bb111637054baafe013b75e52cdc5116f844fc0d2aed4784bf5
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   constrains:
   - openssl !=1.1.1e
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 794424
-  timestamp: 1712327639715
+  size: 795222
+  timestamp: 1713569203054
   purls:
   - pkg:pypi/distributed
 - platform: linux-64
   name: distro
   version: 1.9.0
   category: main
   manager: conda
@@ -3798,14 +5101,36 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 42039
   timestamp: 1704321683916
   purls:
   - pkg:pypi/distro
+- platform: osx-arm64
+  name: distro
+  version: 1.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/distro-1.9.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: bbdb409974cd6cb30071b1d978302726
+    sha256: ae1c13d709c8001331b5b9345e4bcd77e9ae712d25f7958b2ebcbe0b068731b7
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 42039
+  timestamp: 1704321683916
+  purls:
+  - pkg:pypi/distro
 - platform: win-64
   name: distro
   version: 1.9.0
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -3862,14 +5187,35 @@
   build_number: 2
   license: MIT and PSF-2.0
   noarch: python
   size: 20551
   timestamp: 1704921321122
   purls:
   - pkg:pypi/exceptiongroup
+- platform: osx-arm64
+  name: exceptiongroup
+  version: 1.2.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+  hash:
+    md5: 8d652ea2ee8eaee02ed8dc820bc794aa
+    sha256: a6ae416383bda0e3ed14eaa187c653e22bec94ff2aa3b56970cdf0032761e80d
+  build: pyhd8ed1ab_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: MIT and PSF-2.0
+  noarch: python
+  size: 20551
+  timestamp: 1704921321122
+  purls:
+  - pkg:pypi/exceptiongroup
 - platform: win-64
   name: exceptiongroup
   version: 1.2.0
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -3927,14 +5273,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 27689
   timestamp: 1698580072627
   purls:
   - pkg:pypi/executing
+- platform: osx-arm64
+  name: executing
+  version: 2.0.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=2.7
+  url: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: e16be50e378d8a4533b989035b196ab8
+    sha256: c738804ab1e6376f8ea63372229a04c8d658dc90fd5a218c6273a2eaf02f4057
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 27689
+  timestamp: 1698580072627
+  purls:
+  - pkg:pypi/executing
 - platform: win-64
   name: executing
   version: 2.0.1
   category: main
   manager: conda
   dependencies:
   - python >=2.7
@@ -3988,14 +5356,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 126612
   timestamp: 1710362607162
+- platform: osx-arm64
+  name: expat
+  version: 2.6.2
+  category: main
+  manager: conda
+  dependencies:
+  - libexpat 2.6.2 hebf3989_0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/expat-2.6.2-hebf3989_0.conda
+  hash:
+    md5: de0cff0ec74f273c4b6aa281479906c3
+    sha256: 9ac22553a4d595d7e4c9ca9aa09a0b38da65314529a7a7008edc73d3f9e7904a
+  build: hebf3989_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 124594
+  timestamp: 1710362455984
 - platform: win-64
   name: expat
   version: 2.6.2
   category: main
   manager: conda
   dependencies:
   - libexpat 2.6.2 h63175ca_0
@@ -4115,14 +5502,65 @@
   arch: x86_64
   subdir: osx-64
   build_number: 108
   license: GPL-2.0-or-later
   license_family: GPL
   size: 9694369
   timestamp: 1712658377331
+- platform: osx-arm64
+  name: ffmpeg
+  version: 6.1.1
+  category: main
+  manager: conda
+  dependencies:
+  - aom >=3.8.2,<3.9.0a0
+  - bzip2 >=1.0.8,<2.0a0
+  - dav1d >=1.2.1,<1.2.2.0a0
+  - fontconfig >=2.14.2,<3.0a0
+  - fonts-conda-ecosystem
+  - freetype >=2.12.1,<3.0a0
+  - gmp >=6.3.0,<7.0a0
+  - gnutls >=3.7.9,<3.8.0a0
+  - harfbuzz >=8.3.0,<9.0a0
+  - lame >=3.100,<3.101.0a0
+  - libass >=0.17.1,<0.17.2.0a0
+  - libcxx >=16
+  - libiconv >=1.17,<2.0a0
+  - libopenvino >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-arm-cpu-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-auto-batch-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-auto-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-hetero-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-ir-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-onnx-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-paddle-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-pytorch-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-tensorflow-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-tensorflow-lite-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopus >=1.3.1,<2.0a0
+  - libvpx >=1.14.0,<1.15.0a0
+  - libxml2 >=2.12.6,<3.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openh264 >=2.4.1,<2.4.2.0a0
+  - svt-av1 >=2.0.0,<2.0.1.0a0
+  - x264 >=1!164.3095,<1!165
+  - x265 >=3.5,<3.6.0a0
+  - xz >=5.2.6,<6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ffmpeg-6.1.1-gpl_h4f1e072_108.conda
+  hash:
+    md5: 696ed7a1cb702ca44b8deaf2698703ea
+    sha256: c4e171ec03ca367926a64e64d4ffba65ea7f8e68b8c69a6dc91ee490063f7e7f
+  build: gpl_h4f1e072_108
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 108
+  license: GPL-2.0-or-later
+  license_family: GPL
+  size: 8661815
+  timestamp: 1712658165543
 - platform: win-64
   name: ffmpeg
   version: 6.1.0
   category: main
   manager: conda
   dependencies:
   - aom >=3.7.1,<3.8.0a0
@@ -4175,15 +5613,15 @@
   build_number: 108
   license: GPL-2.0-or-later
   license_family: GPL
   size: 1376842
   timestamp: 1686584753580
 - platform: linux-64
   name: fluiddyn
-  version: 0.6.1
+  version: 0.6.3
   category: main
   manager: conda
   dependencies:
   - distro
   - h5netcdf
   - h5py
   - imageio
@@ -4193,29 +5631,29 @@
   - psutil >=5.2.1
   - python >=3.9
   - qtpy
   - scikit-image
   - scipy
   - setuptools
   - simpleeval >=0.9.13
-  url: https://conda.anaconda.org/conda-forge/noarch/fluiddyn-0.6.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/fluiddyn-0.6.3-pyhd8ed1ab_0.conda
   hash:
-    md5: f080c0b0ecc6ef9124c3c40e502a29f0
-    sha256: e058bc5567c28aa3899486910d0d8b3989ad216fc2dd2e8387ef670a99f10655
+    md5: 51b23a02a84d9519bb66b7c5731cd2f7
+    sha256: 130cb23fc24f68f960ab524720a69b28b4b7610bda062345f26f280c5da5ef18
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: CECILL-B
   noarch: python
-  size: 121398
-  timestamp: 1712080339560
+  size: 122281
+  timestamp: 1713807713094
 - platform: osx-64
   name: fluiddyn
-  version: 0.6.1
+  version: 0.6.3
   category: main
   manager: conda
   dependencies:
   - distro
   - h5netcdf
   - h5py
   - imageio
@@ -4225,29 +5663,61 @@
   - psutil >=5.2.1
   - python >=3.9
   - qtpy
   - scikit-image
   - scipy
   - setuptools
   - simpleeval >=0.9.13
-  url: https://conda.anaconda.org/conda-forge/noarch/fluiddyn-0.6.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/fluiddyn-0.6.3-pyhd8ed1ab_0.conda
   hash:
-    md5: f080c0b0ecc6ef9124c3c40e502a29f0
-    sha256: e058bc5567c28aa3899486910d0d8b3989ad216fc2dd2e8387ef670a99f10655
+    md5: 51b23a02a84d9519bb66b7c5731cd2f7
+    sha256: 130cb23fc24f68f960ab524720a69b28b4b7610bda062345f26f280c5da5ef18
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: CECILL-B
   noarch: python
-  size: 121398
-  timestamp: 1712080339560
+  size: 122281
+  timestamp: 1713807713094
+- platform: osx-arm64
+  name: fluiddyn
+  version: 0.6.3
+  category: main
+  manager: conda
+  dependencies:
+  - distro
+  - h5netcdf
+  - h5py
+  - imageio
+  - matplotlib-base
+  - nbstripout
+  - numpy
+  - psutil >=5.2.1
+  - python >=3.9
+  - qtpy
+  - scikit-image
+  - scipy
+  - setuptools
+  - simpleeval >=0.9.13
+  url: https://conda.anaconda.org/conda-forge/noarch/fluiddyn-0.6.3-pyhd8ed1ab_0.conda
+  hash:
+    md5: 51b23a02a84d9519bb66b7c5731cd2f7
+    sha256: 130cb23fc24f68f960ab524720a69b28b4b7610bda062345f26f280c5da5ef18
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: CECILL-B
+  noarch: python
+  size: 122281
+  timestamp: 1713807713094
 - platform: win-64
   name: fluiddyn
-  version: 0.6.1
+  version: 0.6.3
   category: main
   manager: conda
   dependencies:
   - distro
   - h5netcdf
   - h5py
   - imageio
@@ -4257,26 +5727,26 @@
   - psutil >=5.2.1
   - python >=3.9
   - qtpy
   - scikit-image
   - scipy
   - setuptools
   - simpleeval >=0.9.13
-  url: https://conda.anaconda.org/conda-forge/noarch/fluiddyn-0.6.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/fluiddyn-0.6.3-pyhd8ed1ab_0.conda
   hash:
-    md5: f080c0b0ecc6ef9124c3c40e502a29f0
-    sha256: e058bc5567c28aa3899486910d0d8b3989ad216fc2dd2e8387ef670a99f10655
+    md5: 51b23a02a84d9519bb66b7c5731cd2f7
+    sha256: 130cb23fc24f68f960ab524720a69b28b4b7610bda062345f26f280c5da5ef18
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: CECILL-B
   noarch: python
-  size: 121398
-  timestamp: 1712080339560
+  size: 122281
+  timestamp: 1713807713094
 - platform: linux-64
   name: font-ttf-dejavu-sans-mono
   version: '2.37'
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2
@@ -4307,14 +5777,33 @@
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: generic
   size: 397370
   timestamp: 1566932522327
+- platform: osx-arm64
+  name: font-ttf-dejavu-sans-mono
+  version: '2.37'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2
+  hash:
+    md5: 0c96522c6bdaed4b1566d11387caaf45
+    sha256: 58d7f40d2940dd0a8aa28651239adbf5613254df0f75789919c4e6762054403b
+  build: hab24e00_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: generic
+  size: 397370
+  timestamp: 1566932522327
 - platform: win-64
   name: font-ttf-dejavu-sans-mono
   version: '2.37'
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2
@@ -4364,14 +5853,33 @@
   subdir: osx-64
   build_number: 0
   license: OFL-1.1
   license_family: Other
   noarch: generic
   size: 96530
   timestamp: 1620479909603
+- platform: osx-arm64
+  name: font-ttf-inconsolata
+  version: '3.000'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2
+  hash:
+    md5: 34893075a5c9e55cdafac56607368fc6
+    sha256: c52a29fdac682c20d252facc50f01e7c2e7ceac52aa9817aaf0bb83f7559ec5c
+  build: h77eed37_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: OFL-1.1
+  license_family: Other
+  noarch: generic
+  size: 96530
+  timestamp: 1620479909603
 - platform: win-64
   name: font-ttf-inconsolata
   version: '3.000'
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2
@@ -4421,14 +5929,33 @@
   subdir: osx-64
   build_number: 0
   license: OFL-1.1
   license_family: Other
   noarch: generic
   size: 700814
   timestamp: 1620479612257
+- platform: osx-arm64
+  name: font-ttf-source-code-pro
+  version: '2.038'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2
+  hash:
+    md5: 4d59c254e01d9cde7957100457e2d5fb
+    sha256: 00925c8c055a2275614b4d983e1df637245e19058d79fc7dd1a93b8d9fb4b139
+  build: h77eed37_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: OFL-1.1
+  license_family: Other
+  noarch: generic
+  size: 700814
+  timestamp: 1620479612257
 - platform: win-64
   name: font-ttf-source-code-pro
   version: '2.038'
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2
@@ -4478,14 +6005,33 @@
   subdir: osx-64
   build_number: 1
   license: LicenseRef-Ubuntu-Font-Licence-Version-1.0
   license_family: Other
   noarch: generic
   size: 1619820
   timestamp: 1700944216729
+- platform: osx-arm64
+  name: font-ttf-ubuntu
+  version: '0.83'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda
+  hash:
+    md5: 6185f640c43843e5ad6fd1c5372c3f80
+    sha256: 056c85b482d58faab5fd4670b6c1f5df0986314cca3bc831d458b22e4ef2c792
+  build: h77eed37_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: LicenseRef-Ubuntu-Font-Licence-Version-1.0
+  license_family: Other
+  noarch: generic
+  size: 1619820
+  timestamp: 1700944216729
 - platform: win-64
   name: font-ttf-ubuntu
   version: '0.83'
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-h77eed37_1.conda
@@ -4541,14 +6087,35 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 237068
   timestamp: 1674829100063
+- platform: osx-arm64
+  name: fontconfig
+  version: 2.14.2
+  category: main
+  manager: conda
+  dependencies:
+  - expat >=2.5.0,<3.0a0
+  - freetype >=2.12.1,<3.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/fontconfig-2.14.2-h82840c6_0.conda
+  hash:
+    md5: f77d47ddb6d3cc5b39b9bdf65635afbb
+    sha256: 7094917fc6758186e17c61d8ee8fd2bbbe9f303b4addac61d918fa415c497e2b
+  build: h82840c6_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 237668
+  timestamp: 1674829263740
 - platform: win-64
   name: fontconfig
   version: 2.14.2
   category: main
   manager: conda
   dependencies:
   - expat >=2.5.0,<3.0a0
@@ -4606,14 +6173,34 @@
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: generic
   size: 3667
   timestamp: 1566974674465
+- platform: osx-arm64
+  name: fonts-conda-ecosystem
+  version: '1'
+  category: main
+  manager: conda
+  dependencies:
+  - fonts-conda-forge
+  url: https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2
+  hash:
+    md5: fee5683a3f04bd15cbd8318b096a27ab
+    sha256: a997f2f1921bb9c9d76e6fa2f6b408b7fa549edd349a77639c9fe7a23ea93e61
+  build: '0'
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: generic
+  size: 3667
+  timestamp: 1566974674465
 - platform: win-64
   name: fonts-conda-ecosystem
   version: '1'
   category: main
   manager: conda
   dependencies:
   - fonts-conda-forge
@@ -4672,14 +6259,37 @@
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: generic
   size: 4102
   timestamp: 1566932280397
+- platform: osx-arm64
+  name: fonts-conda-forge
+  version: '1'
+  category: main
+  manager: conda
+  dependencies:
+  - font-ttf-dejavu-sans-mono
+  - font-ttf-inconsolata
+  - font-ttf-source-code-pro
+  - font-ttf-ubuntu
+  url: https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2
+  hash:
+    md5: f766549260d6815b0c52253f1fb1bb29
+    sha256: 53f23a3319466053818540bcdf2091f253cbdbab1e0e9ae7b9e509dcaa2a5e38
+  build: '0'
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: generic
+  size: 4102
+  timestamp: 1566932280397
 - platform: win-64
   name: fonts-conda-forge
   version: '1'
   category: main
   manager: conda
   dependencies:
   - font-ttf-dejavu-sans-mono
@@ -4746,14 +6356,40 @@
   build_number: 0
   license: MIT
   license_family: MIT
   size: 2260458
   timestamp: 1712344974536
   purls:
   - pkg:pypi/fonttools
+- platform: osx-arm64
+  name: fonttools
+  version: 4.51.0
+  category: main
+  manager: conda
+  dependencies:
+  - brotli
+  - munkres
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - unicodedata2 >=14.0.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/fonttools-4.51.0-py310hd125d64_0.conda
+  hash:
+    md5: 5d8c5baf693f53ddd0c4324fe6d14268
+    sha256: 143c4297d05b9a6ab449d11606b96e114e3fac4cd9d19eb7c6494516f85763bb
+  build: py310hd125d64_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 2208748
+  timestamp: 1712344970456
+  purls:
+  - pkg:pypi/fonttools
 - platform: win-64
   name: fonttools
   version: 4.51.0
   category: main
   manager: conda
   dependencies:
   - brotli
@@ -4860,14 +6496,33 @@
   build: h60636b9_2
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: GPL-2.0-only OR FTL
   size: 599300
   timestamp: 1694616137838
+- platform: osx-arm64
+  name: freetype
+  version: 2.12.1
+  category: main
+  manager: conda
+  dependencies:
+  - libpng >=1.6.39,<1.7.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/freetype-2.12.1-hadb7bae_2.conda
+  hash:
+    md5: e6085e516a3e304ce41a8ee08b9b89ad
+    sha256: 791673127e037a2dc0eebe122dc4f904cb3f6e635bb888f42cbe1a76b48748d9
+  build: hadb7bae_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: GPL-2.0-only OR FTL
+  size: 596430
+  timestamp: 1694616332835
 - platform: win-64
   name: freetype
   version: 2.12.1
   category: main
   manager: conda
   dependencies:
   - libpng >=1.6.39,<1.7.0a0
@@ -4917,14 +6572,31 @@
   build: hbcb3906_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: LGPL-2.1
   size: 65388
   timestamp: 1604417213
+- platform: osx-arm64
+  name: fribidi
+  version: 1.0.10
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/fribidi-1.0.10-h27ca646_0.tar.bz2
+  hash:
+    md5: c64443234ff91d70cb9c7dc926c58834
+    sha256: 4b37ea851a2cf85edf0a63d2a63266847ec3dcbba4a31156d430cdd6aa811303
+  build: h27ca646_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: LGPL-2.1
+  size: 60255
+  timestamp: 1604417405528
 - platform: linux-64
   name: fsspec
   version: 2024.3.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -4961,14 +6633,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 129227
   timestamp: 1710808383964
   purls:
   - pkg:pypi/fsspec
+- platform: osx-arm64
+  name: fsspec
+  version: 2024.3.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/fsspec-2024.3.1-pyhca7485f_0.conda
+  hash:
+    md5: b7f0662ef2c9d4404f0af9eef5ed2fde
+    sha256: b8621151939bb5ea4ea4aa84f010e6130a47b1453cd9178283f335816b72a895
+  build: pyhca7485f_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 129227
+  timestamp: 1710808383964
+  purls:
+  - pkg:pypi/fsspec
 - platform: win-64
   name: fsspec
   version: 2024.3.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -5031,14 +6725,38 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 23585
   timestamp: 1688368852991
   purls:
   - pkg:pypi/gast
+- platform: osx-arm64
+  name: gast
+  version: 0.5.4
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.4
+  url: https://conda.anaconda.org/conda-forge/noarch/gast-0.5.4-pyhd8ed1ab_0.conda
+  hash:
+    md5: 8189adbad784030b76bbf81c68d7b0d4
+    sha256: e029d50d55f8fe8cf9323045f84416b7af50e25a0dc1b978f8ba6b9ca8d53ca7
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - pythran >=0.12.2
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 23585
+  timestamp: 1688368852991
+  purls:
+  - pkg:pypi/gast
 - platform: win-64
   name: gast
   version: 0.5.4
   category: main
   manager: conda
   dependencies:
   - python >=3.4
@@ -5061,33 +6779,33 @@
   - pkg:pypi/gast
 - platform: linux-64
   name: gcc_impl_linux-64
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
-  - binutils_impl_linux-64 >=2.39
-  - libgcc-devel_linux-64 13.2.0 ha9c7c90_105
+  - binutils_impl_linux-64 >=2.40
+  - libgcc-devel_linux-64 13.2.0 h95c4c6d_106
   - libgcc-ng >=13.2.0
   - libgomp >=13.2.0
-  - libsanitizer 13.2.0 h7e041cc_5
+  - libsanitizer 13.2.0 h95c4c6d_6
   - libstdcxx-ng >=13.2.0
   - sysroot_linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/gcc_impl_linux-64-13.2.0-h338b0a0_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/gcc_impl_linux-64-13.2.0-h1d3d475_6.conda
   hash:
-    md5: a6be13181cb66a78544b1d5f7bac97d0
-    sha256: baab8f8b9af54959735e629cf6d5ec9378166aa4c68ba8dc98dc0a781d548409
-  build: h338b0a0_5
+    md5: fb523fa3954d16178f7df937af68544f
+    sha256: 9c0651484a777f524c32196b826b89e09fc5dc8ca4f8b86839f8f7d7d48850ae
+  build: h1d3d475_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 53318565
-  timestamp: 1706819323755
+  size: 53768088
+  timestamp: 1713755155489
 - platform: linux-64
   name: gcc_linux-64
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
   - binutils_linux-64 2.40 hdade7a5_3
@@ -5151,14 +6869,40 @@
   build: h5ff76d1_2
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: LGPL-2.1-or-later AND GPL-3.0-or-later
   size: 481687
   timestamp: 1712513003915
+- platform: osx-arm64
+  name: gettext
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies:
+  - gettext-tools 0.22.5 h8fbad5d_2
+  - libasprintf 0.22.5 h8fbad5d_2
+  - libasprintf-devel 0.22.5 h8fbad5d_2
+  - libcxx >=16
+  - libgettextpo 0.22.5 h8fbad5d_2
+  - libgettextpo-devel 0.22.5 h8fbad5d_2
+  - libiconv >=1.17,<2.0a0
+  - libintl 0.22.5 h8fbad5d_2
+  - libintl-devel 0.22.5 h8fbad5d_2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/gettext-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: 404e2894e9cb2835246cef47317ff763
+    sha256: 7188b466071698759b125aaed9b4d78940e72e6299b0c6dbad6f35c85cf3d27b
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: LGPL-2.1-or-later AND GPL-3.0-or-later
+  size: 482649
+  timestamp: 1712512963023
 - platform: win-64
   name: gettext
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - gettext-tools 0.22.5 h7d00a51_2
@@ -5215,14 +6959,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: GPL-3.0-or-later
   license_family: GPL
   size: 2501207
   timestamp: 1712512940076
+- platform: osx-arm64
+  name: gettext-tools
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies:
+  - libiconv >=1.17,<2.0a0
+  - libintl 0.22.5 h8fbad5d_2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/gettext-tools-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: 31117a80d73f4fac856ab09fd9f3c6b5
+    sha256: f60d1671e30ac60598396c11fcec4426f7ddb281bf9e37af2262016b4d812cce
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: GPL-3.0-or-later
+  license_family: GPL
+  size: 2482262
+  timestamp: 1712512901194
 - platform: win-64
   name: gettext-tools
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - libiconv >=1.17,<2.0a0
@@ -5277,14 +7041,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1004
   license: BSD-3-Clause
   license_family: BSD
   size: 94612
   timestamp: 1599590973213
+- platform: osx-arm64
+  name: gflags
+  version: 2.2.2
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=11.0.0.rc1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/gflags-2.2.2-hc88da5d_1004.tar.bz2
+  hash:
+    md5: aab9ddfad863e9ef81229a1f8852211b
+    sha256: 25d4a20af2e5ace95fdec88970f6d190e77e20074d2f6d3cef766198b76a4289
+  build: hc88da5d_1004
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1004
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 86690
+  timestamp: 1599590990520
 - platform: linux-64
   name: giflib
   version: 5.2.2
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -5314,14 +7097,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 74516
   timestamp: 1712692686914
+- platform: osx-arm64
+  name: giflib
+  version: 5.2.2
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/giflib-5.2.2-h93a5062_0.conda
+  hash:
+    md5: 95fa1486c77505330c20f7202492b913
+    sha256: 843b3f364ff844137e37d5c0a181f11f6d51adcedd216f019d074e5aa5d7e09c
+  build: h93a5062_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 71613
+  timestamp: 1712692611426
 - platform: win-64
   name: giflib
   version: 5.2.2
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -5341,97 +7142,97 @@
   timestamp: 1712692952874
 - platform: linux-64
   name: glib
   version: 2.80.0
   category: main
   manager: conda
   dependencies:
-  - glib-tools 2.80.0 hde27a5a_5
+  - glib-tools 2.80.0 hde27a5a_6
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
-  - libglib 2.80.0 hf2295e7_5
+  - libglib 2.80.0 hf2295e7_6
   - python *
-  url: https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/glib-2.80.0-hf2295e7_6.conda
   hash:
-    md5: 87562e94dd3948838172eb97175c0e42
-    sha256: 082a1f095f7511ad4339a656714a0ed623758eb0a1caf69494702a59d86f598c
-  build: hf2295e7_5
+    md5: a1e026a82a562b443845db5614ca568a
+    sha256: 186e366c3a48c07830aa94dfc84616155bdfd08e9b73cb8e482c6ca84a550d3e
+  build: hf2295e7_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: LGPL-2.1-or-later
-  size: 599358
-  timestamp: 1713203410775
+  size: 597788
+  timestamp: 1713639483074
 - platform: win-64
   name: glib
   version: 2.80.0
   category: main
   manager: conda
   dependencies:
-  - glib-tools 2.80.0 h0a98069_5
+  - glib-tools 2.80.0 h0a98069_6
   - libffi >=3.4,<4.0a0
-  - libglib 2.80.0 h39d0aa6_5
+  - libglib 2.80.0 h39d0aa6_6
   - libintl >=0.22.5,<1.0a0
   - libintl-devel
   - python *
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
-  url: https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_5.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/glib-2.80.0-h39d0aa6_6.conda
   hash:
-    md5: 987f0532ee1075a4ef5714fa4af4842b
-    sha256: b1a73c6507378f666fce8a7085f36deee04aef72f32850ae5f03725bc363ebbd
-  build: h39d0aa6_5
+    md5: a4036d0bc6f499ebe9fef7b887f3ca0f
+    sha256: 25b3e8930540cfbb87c03feda23cd412eb1b01fd903f46d1bd067f7d39d5941d
+  build: h39d0aa6_6
   arch: x86_64
   subdir: win-64
-  build_number: 5
+  build_number: 6
   license: LGPL-2.1-or-later
-  size: 571049
-  timestamp: 1713203829694
+  size: 572781
+  timestamp: 1713639879324
 - platform: linux-64
   name: glib-tools
   version: 2.80.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
-  - libglib 2.80.0 hf2295e7_5
-  url: https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_5.conda
+  - libglib 2.80.0 hf2295e7_6
+  url: https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.80.0-hde27a5a_6.conda
   hash:
-    md5: 349c38d491861ff6dd7746729912f2f7
-    sha256: 5d8a1e61d054a7147217f7ba9ad675f45f5b642c413a8d3e33ada224f62ba2a5
-  build: hde27a5a_5
+    md5: a9d23c02485c5cf055f9ac90eb9c9c63
+    sha256: fb63c92ba2b08aad574404c6229d45f12dc78309ff7a540f1e8d941a8a075074
+  build: hde27a5a_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: LGPL-2.1-or-later
-  size: 115170
-  timestamp: 1713203374426
+  size: 113049
+  timestamp: 1713639447140
 - platform: win-64
   name: glib-tools
   version: 2.80.0
   category: main
   manager: conda
   dependencies:
-  - libglib 2.80.0 h39d0aa6_5
+  - libglib 2.80.0 h39d0aa6_6
   - libintl >=0.22.5,<1.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
-  url: https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_5.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.80.0-h0a98069_6.conda
   hash:
-    md5: a3fa92819125c3d9e21f7401427af890
-    sha256: f802e16d4f229938e320bf3bfa4334f48fdb6d58e1621778c001218c6d0137de
-  build: h0a98069_5
+    md5: 40d452e4012c00f644b1dd6319fcdbcf
+    sha256: a7533a2e10fe95c8503e990da15933711843061e962450a1c7e753dc050f221b
+  build: h0a98069_6
   arch: x86_64
   subdir: win-64
-  build_number: 5
+  build_number: 6
   license: LGPL-2.1-or-later
-  size: 95213
-  timestamp: 1713203782182
+  size: 94763
+  timestamp: 1713639812512
 - platform: linux-64
   name: glog
   version: 0.7.0
   category: main
   manager: conda
   dependencies:
   - gflags >=2.2.2,<2.3.0a0
@@ -5466,14 +7267,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 115506
   timestamp: 1708261022187
+- platform: osx-arm64
+  name: glog
+  version: 0.7.0
+  category: main
+  manager: conda
+  dependencies:
+  - gflags >=2.2.2,<2.3.0a0
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/glog-0.7.0-hc6770e3_0.conda
+  hash:
+    md5: 359f6720ba65b7a38b46a85d5ae13338
+    sha256: eba67027affe097ef11e4e9ffbb131a5b2ca3494d1b50e5cc1dd337813b1ab5c
+  build: hc6770e3_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 110059
+  timestamp: 1708261049813
 - platform: linux-64
   name: gmp
   version: 6.3.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -5503,14 +7324,32 @@
   build: h73e2aa4_1
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: GPL-2.0-or-later OR LGPL-3.0-or-later
   size: 519804
   timestamp: 1710170159201
+- platform: osx-arm64
+  name: gmp
+  version: 6.3.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/gmp-6.3.0-hebf3989_1.conda
+  hash:
+    md5: 64f45819921ba710398706e1a6404eb5
+    sha256: 0ed5aff70675dc0ed5c2f39bb02b908b864e8eee4ceb56e1c798ba8d7509551f
+  build: hebf3989_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: GPL-2.0-or-later OR LGPL-3.0-or-later
+  size: 448714
+  timestamp: 1710169869298
 - platform: linux-64
   name: gnutls
   version: 3.7.9
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -5552,14 +7391,39 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: LGPL-2.1-or-later
   license_family: LGPL
   size: 1980037
   timestamp: 1701111603786
+- platform: osx-arm64
+  name: gnutls
+  version: 3.7.9
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=10.9
+  - gettext >=0.21.1,<1.0a0
+  - libcxx >=16.0.6
+  - libidn2 >=2,<3.0a0
+  - libtasn1 >=4.19.0,<5.0a0
+  - nettle >=3.9.1,<3.10.0a0
+  - p11-kit >=0.24.1,<0.25.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/gnutls-3.7.9-hd26332c_0.conda
+  hash:
+    md5: 64af58bb3f2a635471dfbe798a1b81f5
+    sha256: 800eceea27032e6d3edbb0186a76d62ed4e4c05963a7d43b35c2ced9ce27ba68
+  build: hd26332c_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: LGPL-2.1-or-later
+  license_family: LGPL
+  size: 1829713
+  timestamp: 1701110534084
 - platform: linux-64
   name: graphite2
   version: 1.3.13
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -5591,14 +7455,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1003
   license: LGPL-2.0-or-later
   license_family: LGPL
   size: 84384
   timestamp: 1711634311095
+- platform: osx-arm64
+  name: graphite2
+  version: 1.3.13
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/graphite2-1.3.13-hebf3989_1003.conda
+  hash:
+    md5: 339991336eeddb70076d8ca826dac625
+    sha256: 2eadafbfc52f5e7df3da3c3b7e5bbe34d970bea1d645ffe60b0b1c3a216657f5
+  build: hebf3989_1003
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1003
+  license: LGPL-2.0-or-later
+  license_family: LGPL
+  size: 79774
+  timestamp: 1711634444608
 - platform: win-64
   name: graphite2
   version: 1.3.13
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -5731,29 +7614,29 @@
   timestamp: 1711318923388
 - platform: linux-64
   name: gxx_impl_linux-64
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
-  - gcc_impl_linux-64 13.2.0 h338b0a0_5
-  - libstdcxx-devel_linux-64 13.2.0 ha9c7c90_105
+  - gcc_impl_linux-64 13.2.0 h1d3d475_6
+  - libstdcxx-devel_linux-64 13.2.0 h95c4c6d_106
   - sysroot_linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/gxx_impl_linux-64-13.2.0-h338b0a0_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/gxx_impl_linux-64-13.2.0-h1d3d475_6.conda
   hash:
-    md5: 88d0ccab114eb0e837725bd48cdddae5
-    sha256: 9049d84fef7526e1dde8311acd2a592bf1d6f16453e68087c17d1bda01eb7867
-  build: h338b0a0_5
+    md5: a7bdc9ce437d0958ebf0d2c7cf09d770
+    sha256: b9336a1ce10c6d7922830811320098742be8e3bea8591adc8fd244a5ea098046
+  build: h1d3d475_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 13582212
-  timestamp: 1706819574801
+  size: 13577661
+  timestamp: 1713755472248
 - platform: linux-64
   name: gxx_linux-64
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
   - binutils_linux-64 2.40 hdade7a5_3
@@ -5816,14 +7699,38 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 42170
   timestamp: 1699412919171
   purls:
   - pkg:pypi/h5netcdf
+- platform: osx-arm64
+  name: h5netcdf
+  version: 1.3.0
+  category: main
+  manager: conda
+  dependencies:
+  - h5py
+  - packaging
+  - python >=3.9
+  url: https://conda.anaconda.org/conda-forge/noarch/h5netcdf-1.3.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 6890388078d9a3a20ef793c5ffb169ed
+    sha256: 0195b109e6b18d7efa06124d268fd5dd426f67e2feaee50a358211ba4a4b219b
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 42170
+  timestamp: 1699412919171
+  purls:
+  - pkg:pypi/h5netcdf
 - platform: win-64
   name: h5netcdf
   version: 1.3.0
   category: main
   manager: conda
   dependencies:
   - h5py
@@ -5887,14 +7794,38 @@
   arch: x86_64
   subdir: osx-64
   build_number: 100
   license: BSD-3-Clause
   license_family: BSD
   size: 1009497
   timestamp: 1712764039080
+- platform: osx-arm64
+  name: h5py
+  version: 3.11.0
+  category: main
+  manager: conda
+  dependencies:
+  - cached-property
+  - hdf5 >=1.14.3,<1.14.4.0a0
+  - numpy >=1.22.4,<2.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/h5py-3.11.0-nompi_py310h49e257e_100.conda
+  hash:
+    md5: 5046d11f4850d80915da4042c8ff4bee
+    sha256: 700aeef07a5e38589fed9935ebf5d11d382a131d94f6d2218a6406921650ac9f
+  build: nompi_py310h49e257e_100
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 100
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 1022241
+  timestamp: 1712766378072
 - platform: win-64
   name: h5py
   version: 3.11.0
   category: main
   manager: conda
   dependencies:
   - cached-property
@@ -5915,88 +7846,109 @@
   build_number: 100
   license: BSD-3-Clause
   license_family: BSD
   size: 885113
   timestamp: 1712764363075
 - platform: linux-64
   name: harfbuzz
-  version: 8.3.0
+  version: 8.4.0
   category: main
   manager: conda
   dependencies:
   - cairo >=1.18.0,<2.0a0
   - freetype >=2.12.1,<3.0a0
   - graphite2
   - icu >=73.2,<74.0a0
   - libgcc-ng >=12
-  - libglib >=2.78.1,<3.0a0
+  - libglib >=2.80.0,<3.0a0
   - libstdcxx-ng >=12
-  url: https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.3.0-h3d44ed6_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-8.4.0-h3d44ed6_0.conda
   hash:
-    md5: 5a6f6c00ef982a9bc83558d9ac8f64a0
-    sha256: 4b55aea03b18a4084b750eee531ad978d4a3690f63019132c26c6ad26bbe3aed
+    md5: 27f46291a6aaa3c2a4f798ebd35a7ddb
+    sha256: d27441d53498f28a36a1612d8f767bae0418076e9c08dcd2cd511c8439d2fb4d
   build: h3d44ed6_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: MIT
   license_family: MIT
-  size: 1547473
-  timestamp: 1699925311766
+  size: 1587652
+  timestamp: 1713957638950
 - platform: osx-64
   name: harfbuzz
-  version: 8.3.0
+  version: 8.4.0
   category: main
   manager: conda
   dependencies:
-  - __osx >=10.9
   - cairo >=1.18.0,<2.0a0
   - freetype >=2.12.1,<3.0a0
   - graphite2
   - icu >=73.2,<74.0a0
-  - libcxx >=16.0.6
-  - libglib >=2.78.1,<3.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.3.0-hf45c392_0.conda
+  - libcxx >=16
+  - libglib >=2.80.0,<3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-8.4.0-h72fa137_0.conda
   hash:
-    md5: 41d890485f909e4ecdc608741718c75e
-    sha256: c6ea14e4f4869bc78b27276c09832af845dfa415585362ed6064e37a1b5fe9c5
-  build: hf45c392_0
+    md5: 7d065a2266ae5eb2a5d91a6dca4fca69
+    sha256: 1618a47f7001c149c95beb84647f5260f17297c6d52a900de4924873397f9fba
+  build: h72fa137_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
-  size: 1342172
-  timestamp: 1699925847743
+  size: 1356068
+  timestamp: 1713957909497
+- platform: osx-arm64
+  name: harfbuzz
+  version: 8.4.0
+  category: main
+  manager: conda
+  dependencies:
+  - cairo >=1.18.0,<2.0a0
+  - freetype >=2.12.1,<3.0a0
+  - graphite2
+  - icu >=73.2,<74.0a0
+  - libcxx >=16
+  - libglib >=2.80.0,<3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/harfbuzz-8.4.0-hbe0f7c0_0.conda
+  hash:
+    md5: 030a2b3b032cd2616b78439e01f79347
+    sha256: 633d8258bbfc59ba85726320003271b40bd7b7addc9d0b8622241ebd57310cf2
+  build: hbe0f7c0_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  size: 1307565
+  timestamp: 1713958317353
 - platform: win-64
   name: harfbuzz
-  version: 8.3.0
+  version: 8.4.0
   category: main
   manager: conda
   dependencies:
   - cairo >=1.18.0,<2.0a0
   - freetype >=2.12.1,<3.0a0
   - graphite2
   - icu >=73.2,<74.0a0
-  - libglib >=2.78.1,<3.0a0
+  - libglib >=2.80.0,<3.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
-  url: https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.3.0-h7ab893a_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/harfbuzz-8.4.0-h7ab893a_0.conda
   hash:
-    md5: b8ef0beb91df83c5e6038c9509b9f730
-    sha256: 5365595303d95810d10662b46f9e857cedc82757cc7b5576bda30e15d66bb3ad
+    md5: bf9b853f9702724a5ec4e68dc637cc29
+    sha256: 725d669f2c72fc1c09ddf3151aacb5a5ef7ebb5f6d3e6217464b9a741a6d5d15
   build: h7ab893a_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: MIT
-  license_family: MIT
-  size: 1070592
-  timestamp: 1699926990335
+  size: 1081529
+  timestamp: 1713958941420
 - platform: linux-64
   name: hdf5
   version: 1.14.3
   category: main
   manager: conda
   dependencies:
   - libaec >=1.1.2,<2.0a0
@@ -6042,14 +7994,41 @@
   arch: x86_64
   subdir: osx-64
   build_number: 100
   license: LicenseRef-HDF5
   license_family: BSD
   size: 3720132
   timestamp: 1701792909005
+- platform: osx-arm64
+  name: hdf5
+  version: 1.14.3
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=10.9
+  - libaec >=1.1.2,<2.0a0
+  - libcurl >=8.4.0,<9.0a0
+  - libcxx >=16.0.6
+  - libgfortran 5.*
+  - libgfortran5 >=12.3.0
+  - libgfortran5 >=13.2.0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.0,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/hdf5-1.14.3-nompi_h5bb55e9_100.conda
+  hash:
+    md5: 120fefd1da806c4d708ecdfe31263f0c
+    sha256: 22331a0ac71a4dd1868f05f8197c36815a41a9f2dcfd01b73ff0d87d9e0ea087
+  build: nompi_h5bb55e9_100
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 100
+  license: LicenseRef-HDF5
+  license_family: BSD
+  size: 3454453
+  timestamp: 1701791479858
 - platform: win-64
   name: hdf5
   version: 1.14.3
   category: main
   manager: conda
   dependencies:
   - libaec >=1.1.2,<2.0a0
@@ -6105,14 +8084,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 11787527
   timestamp: 1692901622519
+- platform: osx-arm64
+  name: icu
+  version: '73.2'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/icu-73.2-hc8870d7_0.conda
+  hash:
+    md5: 8521bd47c0e11c5902535bb1a17c565f
+    sha256: ff9cd0c6cd1349954c801fb443c94192b637e1b414514539f3c49c56a39f51b1
+  build: hc8870d7_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 11997841
+  timestamp: 1692902104771
 - platform: win-64
   name: icu
   version: '73.2'
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -6128,76 +8125,98 @@
   build_number: 0
   license: MIT
   license_family: MIT
   size: 13422193
   timestamp: 1692901469029
 - platform: linux-64
   name: idna
-  version: '3.6'
+  version: '3.7'
   category: main
   manager: conda
   dependencies:
   - python >=3.6
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
   hash:
-    md5: 1a76f09108576397c41c0b0c5bd84134
-    sha256: 6ee4c986d69ce61e60a20b2459b6f2027baeba153f0a64995fd3cb47c2cc7e07
+    md5: c0cc1420498b17414d8617d0b9f506ca
+    sha256: 9687ee909ed46169395d4f99a0ee94b80a52f87bed69cd454bb6d37ffeb0ec7b
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 50124
-  timestamp: 1701027126206
+  size: 52718
+  timestamp: 1713279497047
   purls:
   - pkg:pypi/idna
 - platform: osx-64
   name: idna
-  version: '3.6'
+  version: '3.7'
   category: main
   manager: conda
   dependencies:
   - python >=3.6
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
   hash:
-    md5: 1a76f09108576397c41c0b0c5bd84134
-    sha256: 6ee4c986d69ce61e60a20b2459b6f2027baeba153f0a64995fd3cb47c2cc7e07
+    md5: c0cc1420498b17414d8617d0b9f506ca
+    sha256: 9687ee909ed46169395d4f99a0ee94b80a52f87bed69cd454bb6d37ffeb0ec7b
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 50124
-  timestamp: 1701027126206
+  size: 52718
+  timestamp: 1713279497047
+  purls:
+  - pkg:pypi/idna
+- platform: osx-arm64
+  name: idna
+  version: '3.7'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
+  hash:
+    md5: c0cc1420498b17414d8617d0b9f506ca
+    sha256: 9687ee909ed46169395d4f99a0ee94b80a52f87bed69cd454bb6d37ffeb0ec7b
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 52718
+  timestamp: 1713279497047
   purls:
   - pkg:pypi/idna
 - platform: win-64
   name: idna
-  version: '3.6'
+  version: '3.7'
   category: main
   manager: conda
   dependencies:
   - python >=3.6
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
   hash:
-    md5: 1a76f09108576397c41c0b0c5bd84134
-    sha256: 6ee4c986d69ce61e60a20b2459b6f2027baeba153f0a64995fd3cb47c2cc7e07
+    md5: c0cc1420498b17414d8617d0b9f506ca
+    sha256: 9687ee909ed46169395d4f99a0ee94b80a52f87bed69cd454bb6d37ffeb0ec7b
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 50124
-  timestamp: 1701027126206
+  size: 52718
+  timestamp: 1713279497047
   purls:
   - pkg:pypi/idna
 - platform: linux-64
   name: imagecodecs
   version: 2024.1.1
   category: main
   manager: conda
@@ -6298,14 +8317,68 @@
   build_number: 6
   license: BSD-3-Clause
   license_family: BSD
   size: 1643902
   timestamp: 1712888922232
   purls:
   - pkg:pypi/imagecodecs
+- platform: osx-arm64
+  name: imagecodecs
+  version: 2024.1.1
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - blosc >=1.21.5,<2.0a0
+  - brunsli >=0.1,<1.0a0
+  - bzip2 >=1.0.8,<2.0a0
+  - c-blosc2 >=2.14.4,<2.15.0a0
+  - charls >=2.4.2,<2.5.0a0
+  - giflib >=5.2.2,<5.3.0a0
+  - jxrlib >=1.1,<1.2.0a0
+  - lcms2 >=2.16,<3.0a0
+  - lerc >=4.0.0,<5.0a0
+  - libaec >=1.1.3,<2.0a0
+  - libavif16 >=1.0.1,<2.0a0
+  - libbrotlicommon >=1.1.0,<1.2.0a0
+  - libbrotlidec >=1.1.0,<1.2.0a0
+  - libbrotlienc >=1.1.0,<1.2.0a0
+  - libcxx >=16
+  - libdeflate >=1.20,<1.21.0a0
+  - libjpeg-turbo >=3.0.0,<4.0a0
+  - libjxl >=0.10,<0.11.0a0
+  - libpng >=1.6.43,<1.7.0a0
+  - libtiff >=4.6.0,<4.7.0a0
+  - libwebp-base >=1.3.2,<2.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - libzopfli >=1.0.3,<1.1.0a0
+  - lz4-c >=1.9.3,<1.10.0a0
+  - numpy >=1.22.4,<2.0a0
+  - openjpeg >=2.5.2,<3.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - snappy >=1.2.0,<1.3.0a0
+  - xz >=5.2.6,<6.0a0
+  - zfp >=1.0.1,<2.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/imagecodecs-2024.1.1-py310h8137ee9_6.conda
+  hash:
+    md5: 46ac9cbc32a1181837e5f6f26f332db6
+    sha256: 05063bcfd4db391f0fadf985fe4bdee48db46bc4266244dc462959d774d97821
+  build: py310h8137ee9_6
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 6
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 1738846
+  timestamp: 1712888490483
+  purls:
+  - pkg:pypi/imagecodecs
 - platform: win-64
   name: imagecodecs
   version: 2024.1.1
   category: main
   manager: conda
   dependencies:
   - blosc >=1.21.5,<2.0a0
@@ -6352,82 +8425,106 @@
   license_family: BSD
   size: 1579418
   timestamp: 1711243735862
   purls:
   - pkg:pypi/imagecodecs
 - platform: linux-64
   name: imageio
-  version: 2.34.0
+  version: 2.34.1
   category: main
   manager: conda
   dependencies:
   - numpy
   - pillow >=8.3.2
   - python >=3
-  url: https://conda.anaconda.org/conda-forge/noarch/imageio-2.34.0-pyh4b66e23_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/imageio-2.34.1-pyh4b66e23_0.conda
   hash:
-    md5: b8853659d596f967c661f544dd89ede7
-    sha256: be0eecc8b3ee49ffe3c38dedc4d3c121e18627624926f7d1d998e8027bce4266
+    md5: bcf6a6f4c6889ca083e8d33afbafb8d5
+    sha256: f99e8f3a81d74f4866260badcc4e2f673c0af5564d54325cb6f2df56a6a30a22
   build: pyh4b66e23_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   noarch: python
-  size: 290617
-  timestamp: 1707730229565
+  size: 291095
+  timestamp: 1713760769964
   purls:
   - pkg:pypi/imageio
 - platform: osx-64
   name: imageio
-  version: 2.34.0
+  version: 2.34.1
   category: main
   manager: conda
   dependencies:
   - numpy
   - pillow >=8.3.2
   - python >=3
-  url: https://conda.anaconda.org/conda-forge/noarch/imageio-2.34.0-pyh4b66e23_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/imageio-2.34.1-pyh4b66e23_0.conda
   hash:
-    md5: b8853659d596f967c661f544dd89ede7
-    sha256: be0eecc8b3ee49ffe3c38dedc4d3c121e18627624926f7d1d998e8027bce4266
+    md5: bcf6a6f4c6889ca083e8d33afbafb8d5
+    sha256: f99e8f3a81d74f4866260badcc4e2f673c0af5564d54325cb6f2df56a6a30a22
   build: pyh4b66e23_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   noarch: python
-  size: 290617
-  timestamp: 1707730229565
+  size: 291095
+  timestamp: 1713760769964
+  purls:
+  - pkg:pypi/imageio
+- platform: osx-arm64
+  name: imageio
+  version: 2.34.1
+  category: main
+  manager: conda
+  dependencies:
+  - numpy
+  - pillow >=8.3.2
+  - python >=3
+  url: https://conda.anaconda.org/conda-forge/noarch/imageio-2.34.1-pyh4b66e23_0.conda
+  hash:
+    md5: bcf6a6f4c6889ca083e8d33afbafb8d5
+    sha256: f99e8f3a81d74f4866260badcc4e2f673c0af5564d54325cb6f2df56a6a30a22
+  build: pyh4b66e23_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  noarch: python
+  size: 291095
+  timestamp: 1713760769964
   purls:
   - pkg:pypi/imageio
 - platform: win-64
   name: imageio
-  version: 2.34.0
+  version: 2.34.1
   category: main
   manager: conda
   dependencies:
   - numpy
   - pillow >=8.3.2
   - python >=3
-  url: https://conda.anaconda.org/conda-forge/noarch/imageio-2.34.0-pyh4b66e23_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/imageio-2.34.1-pyh4b66e23_0.conda
   hash:
-    md5: b8853659d596f967c661f544dd89ede7
-    sha256: be0eecc8b3ee49ffe3c38dedc4d3c121e18627624926f7d1d998e8027bce4266
+    md5: bcf6a6f4c6889ca083e8d33afbafb8d5
+    sha256: f99e8f3a81d74f4866260badcc4e2f673c0af5564d54325cb6f2df56a6a30a22
   build: pyh4b66e23_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   noarch: python
-  size: 290617
-  timestamp: 1707730229565
+  size: 291095
+  timestamp: 1713760769964
   purls:
   - pkg:pypi/imageio
 - platform: linux-64
   name: imath
   version: 3.1.11
   category: main
   manager: conda
@@ -6463,14 +8560,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 155338
   timestamp: 1709194419684
+- platform: osx-arm64
+  name: imath
+  version: 3.1.11
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/imath-3.1.11-h1059232_0.conda
+  hash:
+    md5: e95ef5164e69abc370842b41438065fa
+    sha256: cc6d59bcadde846a81d0c141af6a850f28c397a1c8b8546cee1e1c935b6f8dd6
+  build: h1059232_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 154276
+  timestamp: 1709194436403
 - platform: linux-64
   name: importlib-metadata
   version: 7.1.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -6505,14 +8622,35 @@
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 27043
   timestamp: 1710971498183
+- platform: osx-arm64
+  name: importlib-metadata
+  version: 7.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  - zipp >=0.5
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+  hash:
+    md5: 0896606848b2dc5cebdf111b6543aa04
+    sha256: cc2e7d1f7f01cede30feafc1118b7aefa244d0a12224513734e24165ae12ba49
+  build: pyha770c72_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 27043
+  timestamp: 1710971498183
 - platform: win-64
   name: importlib-metadata
   version: 7.1.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -6566,14 +8704,34 @@
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
   noarch: generic
   size: 9444
   timestamp: 1710971502542
+- platform: osx-arm64
+  name: importlib_metadata
+  version: 7.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - importlib-metadata >=7.1.0,<7.1.1.0a0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+  hash:
+    md5: 6ef2b72d291b39e479d7694efa2b2b98
+    sha256: 01dc057a45dedcc742a71599f67c7383ae2bf873be6018ebcbd06ac8d994dedb
+  build: hd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: generic
+  size: 9444
+  timestamp: 1710971502542
 - platform: win-64
   name: importlib_metadata
   version: 7.1.0
   category: main
   manager: conda
   dependencies:
   - importlib-metadata >=7.1.0,<7.1.1.0a0
@@ -6636,14 +8794,39 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 33056
   timestamp: 1711041009039
   purls:
   - pkg:pypi/importlib-resources
+- platform: osx-arm64
+  name: importlib_resources
+  version: 6.4.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  - zipp >=3.1.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: c5d3907ad8bd7bf557521a1833cf7e6d
+    sha256: c6ae80c0beaeabb342c5b041f19669992ae6e937dbec56ced766cb035900f9de
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - importlib-resources >=6.4.0,<6.4.1.0a0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 33056
+  timestamp: 1711041009039
+  purls:
+  - pkg:pypi/importlib-resources
 - platform: win-64
   name: importlib_resources
   version: 6.4.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -6705,14 +8888,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 11101
   timestamp: 1673103208955
   purls:
   - pkg:pypi/iniconfig
+- platform: osx-arm64
+  name: iniconfig
+  version: 2.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: f800d2da156d08e289b14e87e43c1ae5
+    sha256: 38740c939b668b36a50ef455b077e8015b8c9cf89860d421b3fff86048f49666
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 11101
+  timestamp: 1673103208955
+  purls:
+  - pkg:pypi/iniconfig
 - platform: win-64
   name: iniconfig
   version: 2.0.0
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -6813,14 +9018,48 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 593746
   timestamp: 1709559868257
   purls:
   - pkg:pypi/ipython
+- platform: osx-arm64
+  name: ipython
+  version: 8.22.2
+  category: main
+  manager: conda
+  dependencies:
+  - __unix
+  - decorator
+  - exceptiongroup
+  - jedi >=0.16
+  - matplotlib-inline
+  - pexpect >4.3
+  - pickleshare
+  - prompt-toolkit >=3.0.41,<3.1.0
+  - pygments >=2.4.0
+  - python >=3.10
+  - stack_data
+  - traitlets >=5.13.0
+  - typing_extensions
+  url: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
+  hash:
+    md5: f0abe827c8a7c6d91bccdf90cb1fbee3
+    sha256: 7740505317669f094c881537a643ed26977e209510965164d84942799c997d42
+  build: pyh707e725_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 593746
+  timestamp: 1709559868257
+  purls:
+  - pkg:pypi/ipython
 - platform: win-64
   name: ipython
   version: 8.22.2
   category: main
   manager: conda
   dependencies:
   - __win
@@ -6886,14 +9125,32 @@
   build: h6ff19ee_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: JasPer-2.0
   size: 571791
   timestamp: 1711831194534
+- platform: osx-arm64
+  name: jasper
+  version: 4.2.3
+  category: main
+  manager: conda
+  dependencies:
+  - libjpeg-turbo >=3.0.0,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/jasper-4.2.3-h7c0e182_0.conda
+  hash:
+    md5: 74f2870f01bfa190827f0e74257fcda7
+    sha256: 674855f8ac05e4155fbd921469aaae46ed5e4ee7ab50beb7f40ec898f79c8926
+  build: h7c0e182_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: JasPer-2.0
+  size: 584055
+  timestamp: 1711831130577
 - platform: win-64
   name: jasper
   version: 4.2.3
   category: main
   manager: conda
   dependencies:
   - freeglut >=3.2.2,<4.0a0
@@ -6954,14 +9211,37 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 841312
   timestamp: 1696326218364
   purls:
   - pkg:pypi/jedi
+- platform: osx-arm64
+  name: jedi
+  version: 0.19.1
+  category: main
+  manager: conda
+  dependencies:
+  - parso >=0.8.3,<0.9.0
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 81a3be0b2023e1ea8555781f0ad904a2
+    sha256: 362f0936ef37dfd1eaa860190e42a6ebf8faa094eaa3be6aa4d9ace95f40047a
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 841312
+  timestamp: 1696326218364
+  purls:
+  - pkg:pypi/jedi
 - platform: win-64
   name: jedi
   version: 0.19.1
   category: main
   manager: conda
   dependencies:
   - parso >=0.8.3,<0.9.0
@@ -7023,14 +9303,37 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 111589
   timestamp: 1704967140287
   purls:
   - pkg:pypi/jinja2
+- platform: osx-arm64
+  name: jinja2
+  version: 3.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - markupsafe >=2.0
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.3-pyhd8ed1ab_0.conda
+  hash:
+    md5: e7d8df6509ba635247ff9aea31134262
+    sha256: fd517b7dd3a61eca34f8a6f9f92f306397149cae1204fce72ac3d227107dafdc
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 111589
+  timestamp: 1704967140287
+  purls:
+  - pkg:pypi/jinja2
 - platform: win-64
   name: jinja2
   version: 3.1.3
   category: main
   manager: conda
   dependencies:
   - markupsafe >=2.0
@@ -7098,14 +9401,40 @@
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
   size: 72817
   timestamp: 1705707712082
+- platform: osx-arm64
+  name: jsonschema
+  version: 4.21.1
+  category: main
+  manager: conda
+  dependencies:
+  - attrs >=22.2.0
+  - importlib_resources >=1.4.0
+  - jsonschema-specifications >=2023.03.6
+  - pkgutil-resolve-name >=1.3.10
+  - python >=3.8
+  - referencing >=0.28.4
+  - rpds-py >=0.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.21.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 8a3a3d01629da20befa340919e3dd2c4
+    sha256: c5c1b4e08e91fdd697289015be1a176409b4e63942899a43b276f1f250be8129
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 72817
+  timestamp: 1705707712082
 - platform: win-64
   name: jsonschema
   version: 4.21.1
   category: main
   manager: conda
   dependencies:
   - attrs >=22.2.0
@@ -7172,14 +9501,38 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 16431
   timestamp: 1703778502971
   purls:
   - pkg:pypi/jsonschema-specifications
+- platform: osx-arm64
+  name: jsonschema-specifications
+  version: 2023.12.1
+  category: main
+  manager: conda
+  dependencies:
+  - importlib_resources >=1.4.0
+  - python >=3.8
+  - referencing >=0.31.0
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.12.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: a0e4efb5f35786a05af4809a2fb1f855
+    sha256: a9630556ddc3121c0be32f4cbf792dd9102bd380d5cd81d57759d172cf0c2da2
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 16431
+  timestamp: 1703778502971
+  purls:
+  - pkg:pypi/jsonschema-specifications
 - platform: win-64
   name: jsonschema-specifications
   version: 2023.12.1
   category: main
   manager: conda
   dependencies:
   - importlib_resources >=1.4.0
@@ -7240,14 +9593,37 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 80504
   timestamp: 1710257739574
+- platform: osx-arm64
+  name: jupyter_core
+  version: 5.7.2
+  category: main
+  manager: conda
+  dependencies:
+  - platformdirs >=2.5
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - traitlets >=5.3
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py310hbe9552e_0.conda
+  hash:
+    md5: bd7737fbd26eecd0f39cafb52a956f9e
+    sha256: 9e351b25482c50c49fdf0e2203e238c5f04fed0cf192e227915fec955c5d890f
+  build: py310hbe9552e_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 80605
+  timestamp: 1710257888050
 - platform: win-64
   name: jupyter_core
   version: 5.7.2
   category: main
   manager: conda
   dependencies:
   - platformdirs >=2.5
@@ -7300,14 +9676,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: BSD-2-Clause
   license_family: BSD
   size: 220376
   timestamp: 1703334073774
+- platform: osx-arm64
+  name: jxrlib
+  version: '1.1'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/jxrlib-1.1-h93a5062_3.conda
+  hash:
+    md5: 879997fd868f8e9e4c2a12aec8583799
+    sha256: c9e0d3cf9255d4585fa9b3d07ace3bd934fdc6a67ef4532e5507282eff2364ab
+  build: h93a5062_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 197843
+  timestamp: 1703334079437
 - platform: win-64
   name: jxrlib
   version: '1.1'
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -7428,14 +9822,38 @@
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 60432
   timestamp: 1695380318538
   purls:
   - pkg:pypi/kiwisolver
+- platform: osx-arm64
+  name: kiwisolver
+  version: 1.4.5
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=15.0.7
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/kiwisolver-1.4.5-py310h38f39d4_1.conda
+  hash:
+    md5: 84392f391faad11ea910f38226590a88
+    sha256: e84793b3bef7e5d92f96c511a06dc9cbcc49424995777595365c654effe67d6f
+  build: py310h38f39d4_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 62043
+  timestamp: 1695380329047
+  purls:
+  - pkg:pypi/kiwisolver
 - platform: win-64
   name: kiwisolver
   version: 1.4.5
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -7499,14 +9917,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 1183568
   timestamp: 1692098004387
+- platform: osx-arm64
+  name: krb5
+  version: 1.21.2
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=15.0.7
+  - libedit >=3.1.20191231,<3.2.0a0
+  - libedit >=3.1.20191231,<4.0a0
+  - openssl >=3.1.2,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/krb5-1.21.2-h92f50d5_0.conda
+  hash:
+    md5: 92f1cff174a538e0722bf2efb16fc0b2
+    sha256: 70bdb9b4589ec7c7d440e485ae22b5a352335ffeb91a771d4c162996c3070875
+  build: h92f50d5_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 1195575
+  timestamp: 1692098070699
 - platform: win-64
   name: krb5
   version: 1.21.2
   category: main
   manager: conda
   dependencies:
   - openssl >=3.1.2,<4.0a0
@@ -7558,14 +9998,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1003
   license: LGPL-2.0-only
   license_family: LGPL
   size: 542681
   timestamp: 1664996421531
+- platform: osx-arm64
+  name: lame
+  version: '3.100'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/lame-3.100-h1a8c8d9_1003.tar.bz2
+  hash:
+    md5: bff0e851d66725f78dc2fd8b032ddb7e
+    sha256: f40ce7324b2cf5338b766d4cdb8e0453e4156a4f83c2f31bbfff750785de304c
+  build: h1a8c8d9_1003
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1003
+  license: LGPL-2.0-only
+  license_family: LGPL
+  size: 528805
+  timestamp: 1664996399305
 - platform: linux-64
   name: lazy_loader
   version: '0.4'
   category: main
   manager: conda
   dependencies:
   - importlib-metadata
@@ -7606,14 +10064,38 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 16293
   timestamp: 1712343072987
   purls:
   - pkg:pypi/lazy-loader
+- platform: osx-arm64
+  name: lazy_loader
+  version: '0.4'
+  category: main
+  manager: conda
+  dependencies:
+  - importlib-metadata
+  - packaging
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.4-pyhd8ed1ab_0.conda
+  hash:
+    md5: a284ff318fbdb0dd83928275b4b6087c
+    sha256: 0d30db767c56d3f030069ab7c71320c8e34ca8d694c267b6c0d526e55a3bb929
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 16293
+  timestamp: 1712343072987
+  purls:
+  - pkg:pypi/lazy-loader
 - platform: win-64
   name: lazy_loader
   version: '0.4'
   category: main
   manager: conda
   dependencies:
   - importlib-metadata
@@ -7671,14 +10153,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 224432
   timestamp: 1701648089496
+- platform: osx-arm64
+  name: lcms2
+  version: '2.16'
+  category: main
+  manager: conda
+  dependencies:
+  - libjpeg-turbo >=3.0.0,<4.0a0
+  - libtiff >=4.6.0,<4.7.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/lcms2-2.16-ha0e7c42_0.conda
+  hash:
+    md5: 66f6c134e76fe13cce8a9ea5814b5dd5
+    sha256: 151e0c84feb7e0747fabcc85006b8973b22f5abbc3af76a9add0b0ef0320ebe4
+  build: ha0e7c42_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 211959
+  timestamp: 1701647962657
 - platform: win-64
   name: lcms2
   version: '2.16'
   category: main
   manager: conda
   dependencies:
   - libjpeg-turbo >=3.0.0,<4.0a0
@@ -7721,34 +10223,61 @@
   - ld 711.*
   - cctools 986.*
   - clang >=18.1.1,<19.0a0
   license: APSL-2.0
   license_family: Other
   size: 1071472
   timestamp: 1710484364960
+- platform: osx-arm64
+  name: ld64_osx-arm64
+  version: '711'
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx
+  - libllvm18 >=18.1.1,<18.2.0a0
+  - sigtool
+  - tapi >=1100.0.11,<1101.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ld64_osx-arm64-711-h5e7191b_0.conda
+  hash:
+    md5: c751b76ae8112e3d516831063da179cc
+    sha256: 82f964dcff2052b327762ca44651407451ad396a1540c664928841c72b7cf3c0
+  build: h5e7191b_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - ld 711.*
+  - cctools 986.*
+  - cctools_osx-arm64 986.*
+  - clang >=18.1.1,<19.0a0
+  license: APSL-2.0
+  license_family: Other
+  size: 1064448
+  timestamp: 1710484550965
 - platform: linux-64
   name: ld_impl_linux-64
   version: '2.40'
   category: main
   manager: conda
   dependencies: []
-  url: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
   hash:
-    md5: 7aca3059a1729aa76c597603f10b0dd3
-    sha256: f6cc89d887555912d6c61b295d398cff9ec982a3417d38025c45d5dd9b9e79cd
-  build: h41732ed_0
+    md5: 10569984e7db886e4f1abc2b47ad79a1
+    sha256: ef969eee228cfb71e55146eaecc6af065f468cb0bc0a5239bc053b39db0b5f09
+  build: h55db66e_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   constrains:
   - binutils_impl_linux-64 2.40
   license: GPL-3.0-only
   license_family: GPL
-  size: 704696
-  timestamp: 1674833944779
+  size: 713322
+  timestamp: 1713651222435
 - platform: linux-64
   name: lerc
   version: 4.0.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -7780,14 +10309,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 290319
   timestamp: 1657977526749
+- platform: osx-arm64
+  name: lerc
+  version: 4.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=13.0.1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/lerc-4.0.0-h9a09cb3_0.tar.bz2
+  hash:
+    md5: de462d5aacda3b30721b512c5da4e742
+    sha256: 6f068bb53dfb6147d3147d981bb851bb5477e769407ad4e6a68edf482fdcb958
+  build: h9a09cb3_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 215721
+  timestamp: 1657977558796
 - platform: win-64
   name: lerc
   version: 4.0.0
   category: main
   manager: conda
   dependencies:
   - vc >=14.2,<15
@@ -7846,14 +10394,36 @@
   - libabseil-static =20240116.1=cxx17*
   - __osx >=10.13
   - abseil-cpp =20240116.1
   license: Apache-2.0
   license_family: Apache
   size: 1133225
   timestamp: 1709160179404
+- platform: osx-arm64
+  name: libabseil
+  version: '20240116.1'
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libabseil-20240116.1-cxx17_hebf3989_2.conda
+  hash:
+    md5: 0b85aac2fab429166f76940791de071a
+    sha256: 3e87e8da8e40c71f6107386f6e87aeadc8c7b42e2736f6ac894abe50c763d642
+  build: cxx17_hebf3989_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  constrains:
+  - abseil-cpp =20240116.1
+  - libabseil-static =20240116.1=cxx17*
+  license: Apache-2.0
+  license_family: Apache
+  size: 1144666
+  timestamp: 1709160261245
 - platform: win-64
   name: libabseil
   version: '20230802.1'
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -7909,14 +10479,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   size: 28602
   timestamp: 1711021419744
+- platform: osx-arm64
+  name: libaec
+  version: 1.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libaec-1.1.3-hebf3989_0.conda
+  hash:
+    md5: 6f0b8e56d2e7bae12a18fc5b2cd9f310
+    sha256: 896189b7b48a194c46a3556ea04943ef81cbe0498521231f8eb25816a68bc8ed
+  build: hebf3989_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 28451
+  timestamp: 1711021498493
 - platform: win-64
   name: libaec
   version: 1.1.3
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -7939,47 +10528,48 @@
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - aws-crt-cpp >=0.26.6,<0.26.7.0a0
   - aws-sdk-cpp >=1.11.267,<1.11.268.0a0
   - bzip2 >=1.0.8,<2.0a0
+  - gflags >=2.2.2,<2.3.0a0
   - glog >=0.7.0,<0.8.0a0
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
   - libbrotlidec >=1.1.0,<1.2.0a0
   - libbrotlienc >=1.1.0,<1.2.0a0
   - libgcc-ng >=12
-  - libgoogle-cloud >=2.22.0,<2.23.0a0
-  - libgoogle-cloud-storage >=2.22.0,<2.23.0a0
+  - libgoogle-cloud >=2.23.0,<2.24.0a0
+  - libgoogle-cloud-storage >=2.23.0,<2.24.0a0
   - libre2-11 >=2023.9.1,<2024.0a0
   - libstdcxx-ng >=12
   - libutf8proc >=2.8.0,<3.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - lz4-c >=1.9.3,<1.10.0a0
   - orc >=2.0.0,<2.0.1.0a0
   - re2
   - snappy >=1.2.0,<1.3.0a0
   - zstd >=1.5.5,<1.6.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-15.0.2-he70291f_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-15.0.2-h07fc4ce_5_cpu.conda
   hash:
-    md5: d09f7d5d311728e9e4cd386d86a1e55f
-    sha256: 27157f7cc429ea43093983cfbab3d6a031c10e4330d686f062075b9729f6a982
-  build: he70291f_3_cpu
+    md5: 0dd55e619dcc8b0f65b06c2b1f6eb746
+    sha256: 8dd2f5d4612c3a4bb4bba88cb945144b143b984f8a023d5fe538c7ba83ef7f67
+  build: h07fc4ce_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   constrains:
-  - parquet-cpp <0.0a0
   - apache-arrow-proc =*=cpu
   - arrow-cpp <0.0a0
+  - parquet-cpp <0.0a0
   license: Apache-2.0
   license_family: APACHE
-  size: 8170462
-  timestamp: 1712756370701
+  size: 8190486
+  timestamp: 1713845901698
 - platform: osx-64
   name: libarrow
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
@@ -7988,40 +10578,82 @@
   - bzip2 >=1.0.8,<2.0a0
   - glog >=0.7.0,<0.8.0a0
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
   - libbrotlidec >=1.1.0,<1.2.0a0
   - libbrotlienc >=1.1.0,<1.2.0a0
   - libcxx >=16
-  - libgoogle-cloud >=2.22.0,<2.23.0a0
-  - libgoogle-cloud-storage >=2.22.0,<2.23.0a0
+  - libgoogle-cloud >=2.23.0,<2.24.0a0
+  - libgoogle-cloud-storage >=2.23.0,<2.24.0a0
   - libre2-11 >=2023.9.1,<2024.0a0
   - libutf8proc >=2.8.0,<3.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - lz4-c >=1.9.3,<1.10.0a0
   - orc >=2.0.0,<2.0.1.0a0
   - re2
   - snappy >=1.2.0,<1.3.0a0
   - zstd >=1.5.5,<1.6.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-15.0.2-h965e444_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-15.0.2-h1b20127_5_cpu.conda
   hash:
-    md5: db0e69e54efa4f0aa778a77a039f7f53
-    sha256: a6886cff57529f1ab71e3327b37ea5b55b9d31764c4322abfe3391e7401f56a1
-  build: h965e444_3_cpu
+    md5: 7820c727b6eb7533699b29b5dbd078d0
+    sha256: b167cbf01495e62ee4756d5d2852e8cceb4767a23050c2f52a68742191a0a38e
+  build: h1b20127_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
   constrains:
   - arrow-cpp <0.0a0
   - apache-arrow-proc =*=cpu
   - parquet-cpp <0.0a0
   license: Apache-2.0
   license_family: APACHE
-  size: 5717595
-  timestamp: 1712757257079
+  size: 5720352
+  timestamp: 1713847209419
+- platform: osx-arm64
+  name: libarrow
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - aws-crt-cpp >=0.26.6,<0.26.7.0a0
+  - aws-sdk-cpp >=1.11.267,<1.11.268.0a0
+  - bzip2 >=1.0.8,<2.0a0
+  - glog >=0.7.0,<0.8.0a0
+  - libabseil * cxx17*
+  - libabseil >=20240116.1,<20240117.0a0
+  - libbrotlidec >=1.1.0,<1.2.0a0
+  - libbrotlienc >=1.1.0,<1.2.0a0
+  - libcxx >=16
+  - libgoogle-cloud >=2.23.0,<2.24.0a0
+  - libgoogle-cloud-storage >=2.23.0,<2.24.0a0
+  - libre2-11 >=2023.9.1,<2024.0a0
+  - libutf8proc >=2.8.0,<3.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - lz4-c >=1.9.3,<1.10.0a0
+  - orc >=2.0.0,<2.0.1.0a0
+  - re2
+  - snappy >=1.2.0,<1.3.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libarrow-15.0.2-hca667bd_5_cpu.conda
+  hash:
+    md5: aa6921519142ae7212b6d160873a217c
+    sha256: 4d66f610e7668715a99c295d8cc342a3d62f985697dbccfdd4f3eb8cc3cc8900
+  build: hca667bd_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  constrains:
+  - parquet-cpp <0.0a0
+  - arrow-cpp <0.0a0
+  - apache-arrow-proc =*=cpu
+  license: Apache-2.0
+  license_family: APACHE
+  size: 5123458
+  timestamp: 1713847401283
 - platform: win-64
   name: libarrow
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - aws-crt-cpp >=0.26.0,<0.26.1.0a0
@@ -8064,50 +10696,72 @@
   timestamp: 1706643544752
 - platform: linux-64
   name: libarrow-acero
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
-  - libarrow 15.0.2 he70291f_3_cpu
+  - gflags >=2.2.2,<2.3.0a0
+  - libarrow 15.0.2 h07fc4ce_5_cpu
   - libgcc-ng >=12
   - libstdcxx-ng >=12
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-acero-15.0.2-hac33072_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-acero-15.0.2-hbabe93e_5_cpu.conda
   hash:
-    md5: f70ae2fa9f50bed63564a6190f2cff35
-    sha256: ce25b573fd32e6e9c6cec37d82a375f69125912018246a7d78dfa116952c5105
-  build: hac33072_3_cpu
+    md5: 7e6f6e36a824d459e69486fd551afe8d
+    sha256: 5d049d845fda3e6b4d32f65143ab7060e379c8b74aea3bc7cd48b620ebb6d66c
+  build: hbabe93e_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 597913
-  timestamp: 1712756407762
+  size: 600465
+  timestamp: 1713845939235
 - platform: osx-64
   name: libarrow-acero
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - libarrow 15.0.2 h965e444_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
   - libcxx >=16
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-acero-15.0.2-ha0df490_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-acero-15.0.2-ha0df490_5_cpu.conda
   hash:
-    md5: 5faf0bba140d6881d28690c5e9b5ee00
-    sha256: d5606b5dedc28190a029d466f3f0b525482e0ac6420ac9ad7aef9d455e16cba4
-  build: ha0df490_3_cpu
+    md5: a41582d3bbeb339e1d967cad6ba9ea11
+    sha256: 8752c6e2a0fcb7f5589ba278e62f8f33a56bbca755ceb4f3ec4645a65cc2f104
+  build: ha0df490_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
+  license: Apache-2.0
+  license_family: APACHE
+  size: 524965
+  timestamp: 1713847351891
+- platform: osx-arm64
+  name: libarrow-acero
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libarrow-acero-15.0.2-h3f3aa29_5_cpu.conda
+  hash:
+    md5: c1a1541dba6b31c9e44d6374ac78c970
+    sha256: 8c3db92009e281f330e549a3ca3540afc0f9e173be2b3fed76758a885c49a0aa
+  build: h3f3aa29_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 522427
-  timestamp: 1712757408748
+  size: 486439
+  timestamp: 1713847537488
 - platform: win-64
   name: libarrow-acero
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libarrow 15.0.0 he5f67d5_0_cpu
@@ -8128,54 +10782,78 @@
   timestamp: 1706643672248
 - platform: linux-64
   name: libarrow-dataset
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
-  - libarrow 15.0.2 he70291f_3_cpu
-  - libarrow-acero 15.0.2 hac33072_3_cpu
+  - gflags >=2.2.2,<2.3.0a0
+  - libarrow 15.0.2 h07fc4ce_5_cpu
+  - libarrow-acero 15.0.2 hbabe93e_5_cpu
   - libgcc-ng >=12
-  - libparquet 15.0.2 h6a7eafb_3_cpu
+  - libparquet 15.0.2 hacf5a1f_5_cpu
   - libstdcxx-ng >=12
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-dataset-15.0.2-hac33072_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-dataset-15.0.2-hbabe93e_5_cpu.conda
   hash:
-    md5: 59df0b7cf76763437ac3a5865c23af80
-    sha256: 0e380506725c77f9a102be1ad96c27f3881de74d32aef737e369d95e0e0f61dc
-  build: hac33072_3_cpu
+    md5: 13bd44cd7368264b9bbb4fe7290ef592
+    sha256: becbe51d99bc26144b03fb7a41525d784df3ddead33ad01a0f5a3c3eef24ad8e
+  build: hbabe93e_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 585627
-  timestamp: 1712756482313
+  size: 587740
+  timestamp: 1713846015116
 - platform: osx-64
   name: libarrow-dataset
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - libarrow 15.0.2 h965e444_3_cpu
-  - libarrow-acero 15.0.2 ha0df490_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
+  - libarrow-acero 15.0.2 ha0df490_5_cpu
   - libcxx >=16
-  - libparquet 15.0.2 h7cd3cfe_3_cpu
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-dataset-15.0.2-ha0df490_3_cpu.conda
+  - libparquet 15.0.2 h7cd3cfe_5_cpu
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-dataset-15.0.2-ha0df490_5_cpu.conda
   hash:
-    md5: 9f9d733d0a6ca4b0a2c3bc9e1ff54874
-    sha256: deb92309415fac27db5f2c170d0bed2b3a7b7a3d0265257e1234ddc08b69496b
-  build: ha0df490_3_cpu
+    md5: 39ebf7a2da797513a5d86c3fd30c9fba
+    sha256: 9762584fbd4062d774fd5e1bf9f6f50c0866b06f5114bd030fe2b087faebb84e
+  build: ha0df490_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 512417
-  timestamp: 1712758274474
+  size: 513940
+  timestamp: 1713848182379
+- platform: osx-arm64
+  name: libarrow-dataset
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libarrow-acero 15.0.2 h3f3aa29_5_cpu
+  - libcxx >=16
+  - libparquet 15.0.2 h5304c63_5_cpu
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libarrow-dataset-15.0.2-h3f3aa29_5_cpu.conda
+  hash:
+    md5: 6a1bde415ebcdfa93e4c97b79174c762
+    sha256: d39529954480f7be328443e72adcd9f37abd631a671f2f8efda67e2832ce7f2c
+  build: h3f3aa29_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  license: Apache-2.0
+  license_family: APACHE
+  size: 490843
+  timestamp: 1713848808509
 - platform: win-64
   name: libarrow-dataset
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libarrow 15.0.0 he5f67d5_0_cpu
@@ -8198,59 +10876,85 @@
   timestamp: 1706643963629
 - platform: linux-64
   name: libarrow-flight
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
+  - gflags >=2.2.2,<2.3.0a0
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
-  - libarrow 15.0.2 he70291f_3_cpu
+  - libarrow 15.0.2 h07fc4ce_5_cpu
   - libgcc-ng >=12
-  - libgrpc >=1.62.1,<1.63.0a0
+  - libgrpc >=1.62.2,<1.63.0a0
   - libprotobuf >=4.25.3,<4.25.4.0a0
   - libstdcxx-ng >=12
   - ucx >=1.15.0,<1.16.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-flight-15.0.2-hd42f311_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-flight-15.0.2-hc4f8a93_5_cpu.conda
   hash:
-    md5: 2481d3c17be3a1e8876b733001901162
-    sha256: fd38c1cd423684b7d42e02a30af61fec73b407b50cc0d84975e5f6574140aac6
-  build: hd42f311_3_cpu
+    md5: fcc6ea9306d10ba3ee761ba3d6a190a0
+    sha256: 08badfa51fd0507b3792664c3931585d404a7024ceebaff96e7e400daaddc9dc
+  build: hc4f8a93_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 506382
-  timestamp: 1712756425619
+  size: 509533
+  timestamp: 1713845957389
 - platform: osx-64
   name: libarrow-flight
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
-  - libarrow 15.0.2 h965e444_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
   - libcxx >=16
-  - libgrpc >=1.62.1,<1.63.0a0
+  - libgrpc >=1.62.2,<1.63.0a0
   - libprotobuf >=4.25.3,<4.25.4.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-flight-15.0.2-h41520de_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-flight-15.0.2-h41520de_5_cpu.conda
   hash:
-    md5: a329ec45df9b7c4d91419e3f8bbb9e8c
-    sha256: 92ee4bde00d9896dc2a5bdfc2cf5ec6b09a0da4613cc83585439153fc1f479c0
-  build: h41520de_3_cpu
+    md5: 7b8b2f16c735e48f842ea7d20351fd11
+    sha256: 3cf94a25b924263ceaff15f2dac4442bd28a9fbe723a5f0bb7d3754b0e022fb4
+  build: h41520de_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 322118
-  timestamp: 1712757592284
+  size: 325413
+  timestamp: 1713847524254
+- platform: osx-arm64
+  name: libarrow-flight
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libabseil * cxx17*
+  - libabseil >=20240116.1,<20240117.0a0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libcxx >=16
+  - libgrpc >=1.62.2,<1.63.0a0
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libarrow-flight-15.0.2-h224147a_5_cpu.conda
+  hash:
+    md5: 4dec5d97c5bbcb096e7b405b8454167e
+    sha256: 9570ab8df0e92f4be0d009631b9374698fabb922878537850bbb600e0ace70dc
+  build: h224147a_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  license: Apache-2.0
+  license_family: APACHE
+  size: 313840
+  timestamp: 1713847824392
 - platform: win-64
   name: libarrow-flight
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libabseil * cxx17*
@@ -8275,54 +10979,78 @@
   timestamp: 1706643747971
 - platform: linux-64
   name: libarrow-flight-sql
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
-  - libarrow 15.0.2 he70291f_3_cpu
-  - libarrow-flight 15.0.2 hd42f311_3_cpu
+  - gflags >=2.2.2,<2.3.0a0
+  - libarrow 15.0.2 h07fc4ce_5_cpu
+  - libarrow-flight 15.0.2 hc4f8a93_5_cpu
   - libgcc-ng >=12
   - libprotobuf >=4.25.3,<4.25.4.0a0
   - libstdcxx-ng >=12
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-flight-sql-15.0.2-h9241762_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-flight-sql-15.0.2-he4f5ca8_5_cpu.conda
   hash:
-    md5: 1f74636cb22b3f6bc88a13843249e06f
-    sha256: 6c4678e6b0193344dec99053e1bfc25c0c9bc384a29f7f33896dfc1d7cb6ca48
-  build: h9241762_3_cpu
+    md5: 9dac4008d07e789e8817779dd07f7d95
+    sha256: d2256c21a20ee7a1bfa85b5f659da4912b7b866a33625b64cbfd00a079374366
+  build: he4f5ca8_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 194961
-  timestamp: 1712756499434
+  size: 197250
+  timestamp: 1713846032564
 - platform: osx-64
   name: libarrow-flight-sql
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - libarrow 15.0.2 h965e444_3_cpu
-  - libarrow-flight 15.0.2 h41520de_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
+  - libarrow-flight 15.0.2 h41520de_5_cpu
   - libcxx >=16
   - libprotobuf >=4.25.3,<4.25.4.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-flight-sql-15.0.2-hb2e0ddf_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-flight-sql-15.0.2-hb2e0ddf_5_cpu.conda
   hash:
-    md5: 9c1f618f820f2b26cedec587ed543349
-    sha256: 7b935b8b83ff8b9b1ea4250e0c162de1ffa79a0af34add11f39b76c5a0c09fba
-  build: hb2e0ddf_3_cpu
+    md5: 146cdb3f0ac3b0de9b85927f8b326878
+    sha256: 41d835e46d88da3a594cce590528e64f7f951a472cd854d37119f0cd4bfdea65
+  build: hb2e0ddf_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
+  license: Apache-2.0
+  license_family: APACHE
+  size: 156885
+  timestamp: 1713848258332
+- platform: osx-arm64
+  name: libarrow-flight-sql
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libarrow-flight 15.0.2 h224147a_5_cpu
+  - libcxx >=16
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libarrow-flight-sql-15.0.2-hb630850_5_cpu.conda
+  hash:
+    md5: a410a55c2cf35f1e9f2a55cae4a451d7
+    sha256: 6f1df3e7b84cbbd28f23701032cece9fd10e7edbdd785e198552c344a41db3f7
+  build: hb630850_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 153610
-  timestamp: 1712758355472
+  size: 155395
+  timestamp: 1713848905296
 - platform: win-64
   name: libarrow-flight-sql
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libarrow 15.0.0 he5f67d5_0_cpu
@@ -8345,64 +11073,87 @@
   timestamp: 1706644025665
 - platform: linux-64
   name: libarrow-gandiva
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
-  - libabseil * cxx17*
-  - libabseil >=20240116.1,<20240117.0a0
-  - libarrow 15.0.2 he70291f_3_cpu
+  - gflags >=2.2.2,<2.3.0a0
+  - libarrow 15.0.2 h07fc4ce_5_cpu
   - libgcc-ng >=12
   - libllvm16 >=16.0.6,<16.1.0a0
   - libre2-11 >=2023.9.1,<2024.0a0
   - libstdcxx-ng >=12
   - libutf8proc >=2.8.0,<3.0a0
   - openssl >=3.2.1,<4.0a0
   - re2
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-gandiva-15.0.2-hd4ab825_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-gandiva-15.0.2-hc1954e9_5_cpu.conda
   hash:
-    md5: b7f70a642aef9013a2787b0025c53f01
-    sha256: 9eda95ecfcb985726ad947720c711c7941d25be83d6ed47316bc8aa50febef2b
-  build: hd4ab825_3_cpu
+    md5: 41d244c539e8e759b583ecc7f8ad583e
+    sha256: 20f6dd249fa1be3b9d057bc357535d75dd85a4909a65cd8a38eb8fbff281cbdd
+  build: hc1954e9_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 896197
-  timestamp: 1712756445172
+  size: 898130
+  timestamp: 1713845977276
 - platform: osx-64
   name: libarrow-gandiva
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - libabseil * cxx17*
-  - libabseil >=20240116.1,<20240117.0a0
-  - libarrow 15.0.2 h965e444_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
   - libcxx >=16
   - libllvm16 >=16.0.6,<16.1.0a0
   - libre2-11 >=2023.9.1,<2024.0a0
   - libutf8proc >=2.8.0,<3.0a0
   - openssl >=3.2.1,<4.0a0
   - re2
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-gandiva-15.0.2-h6ac0def_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-gandiva-15.0.2-h81ca85a_5_cpu.conda
   hash:
-    md5: 3fb063fbce68efaa7b7ce614dfa7f6ea
-    sha256: 2500da9593a55363ac16c8f92165ea7002023a1f38d57e6d54968d7922530d7b
-  build: h6ac0def_3_cpu
+    md5: 2ff9c249be1fd479f3f0c86b3431630f
+    sha256: c0583ed6ef25514d474f6844cc1fccb9c5bfe82e71634248ccd520cb6a0871e3
+  build: h81ca85a_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
+  license: Apache-2.0
+  license_family: APACHE
+  size: 703499
+  timestamp: 1713847974165
+- platform: osx-arm64
+  name: libarrow-gandiva
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libcxx >=16
+  - libllvm16 >=16.0.6,<16.1.0a0
+  - libre2-11 >=2023.9.1,<2024.0a0
+  - libutf8proc >=2.8.0,<3.0a0
+  - openssl >=3.2.1,<4.0a0
+  - re2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libarrow-gandiva-15.0.2-h3b9069c_5_cpu.conda
+  hash:
+    md5: 9c69da820490e617642200248d52fe16
+    sha256: 81532d13aa38188cc1d723f50a2aaba2da37a12d000cc463dc1f571edecd880f
+  build: h3b9069c_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 699945
-  timestamp: 1712758054471
+  size: 688807
+  timestamp: 1713848592776
 - platform: win-64
   name: libarrow-gandiva
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libarrow 15.0.0 he5f67d5_0_cpu
@@ -8428,56 +11179,81 @@
   timestamp: 1706643818124
 - platform: linux-64
   name: libarrow-substrait
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
-  - libarrow 15.0.2 he70291f_3_cpu
-  - libarrow-acero 15.0.2 hac33072_3_cpu
-  - libarrow-dataset 15.0.2 hac33072_3_cpu
+  - gflags >=2.2.2,<2.3.0a0
+  - libarrow 15.0.2 h07fc4ce_5_cpu
+  - libarrow-acero 15.0.2 hbabe93e_5_cpu
+  - libarrow-dataset 15.0.2 hbabe93e_5_cpu
   - libgcc-ng >=12
   - libprotobuf >=4.25.3,<4.25.4.0a0
   - libstdcxx-ng >=12
-  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-substrait-15.0.2-h9241762_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libarrow-substrait-15.0.2-he4f5ca8_5_cpu.conda
   hash:
-    md5: d3c3294783206de4e7ad3880d1c9cefe
-    sha256: c7db9a7e0b1e2407afee9775fabba2f8894b0a0fb8040653596099d3d59e8980
-  build: h9241762_3_cpu
+    md5: aa87a690d9b3af960ac95092f3c4aad9
+    sha256: 92a649b44505e30c2fb37b1aeb3e1f17784b8f4bc97d2ca461547fbb3f265756
+  build: he4f5ca8_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 519375
-  timestamp: 1712756517131
+  size: 522457
+  timestamp: 1713846050543
 - platform: osx-64
   name: libarrow-substrait
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - libarrow 15.0.2 h965e444_3_cpu
-  - libarrow-acero 15.0.2 ha0df490_3_cpu
-  - libarrow-dataset 15.0.2 ha0df490_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
+  - libarrow-acero 15.0.2 ha0df490_5_cpu
+  - libarrow-dataset 15.0.2 ha0df490_5_cpu
   - libcxx >=16
   - libprotobuf >=4.25.3,<4.25.4.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-substrait-15.0.2-hb2e0ddf_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libarrow-substrait-15.0.2-hb2e0ddf_5_cpu.conda
   hash:
-    md5: 245d375ea095116d40b8b48d4f2d981a
-    sha256: 4db58054d748b821ac870ac1c51216e10eacdadff894aaa77c25cfdc2ddc2867
-  build: hb2e0ddf_3_cpu
+    md5: c9581f7b5eef437fd224bcec2059f136
+    sha256: 37f0ab5bc550b706aa7f56e216515cb5a63d5ea42ccd42540902904a5e5fe738
+  build: hb2e0ddf_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
+  license: Apache-2.0
+  license_family: APACHE
+  size: 452013
+  timestamp: 1713848379093
+- platform: osx-arm64
+  name: libarrow-substrait
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libarrow-acero 15.0.2 h3f3aa29_5_cpu
+  - libarrow-dataset 15.0.2 h3f3aa29_5_cpu
+  - libcxx >=16
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libarrow-substrait-15.0.2-hd92e347_5_cpu.conda
+  hash:
+    md5: f3d4ff2bee9317f2af48062d2b1bbc1a
+    sha256: 052096e143f58154caf5a80695593c8d24372b6efa400976020f652eec994e06
+  build: hd92e347_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 449659
-  timestamp: 1712758489827
+  size: 442317
+  timestamp: 1713849037021
 - platform: win-64
   name: libarrow-substrait
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libabseil * cxx17*
@@ -8533,14 +11309,31 @@
   build: h5ff76d1_2
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: LGPL-2.1-or-later
   size: 40438
   timestamp: 1712512749697
+- platform: osx-arm64
+  name: libasprintf
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libasprintf-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: 1b27402397a76115679c4855ab2ece41
+    sha256: 04bbe4374719906cd08b639a3f34828030f405c33b47c757b47fd55aa7310179
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: LGPL-2.1-or-later
+  size: 40630
+  timestamp: 1712512727388
 - platform: win-64
   name: libasprintf
   version: 0.22.5
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/win-64/libasprintf-0.22.5-h5728263_2.conda
@@ -8587,14 +11380,32 @@
   build: h5ff76d1_2
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: LGPL-2.1-or-later
   size: 34702
   timestamp: 1712512806211
+- platform: osx-arm64
+  name: libasprintf-devel
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies:
+  - libasprintf 0.22.5 h8fbad5d_2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libasprintf-devel-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: 480c106e87d4c4791e6b55a6d1678866
+    sha256: f5331486854a5fe80bb837891efb28a28623f762327372cb4cbc264c9c4bf9e2
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: LGPL-2.1-or-later
+  size: 34625
+  timestamp: 1712512769736
 - platform: win-64
   name: libasprintf-devel
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - libasprintf 0.22.5 h5728263_2
@@ -8656,14 +11467,39 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: ISC
   license_family: OTHER
   size: 125235
   timestamp: 1693027259439
+- platform: osx-arm64
+  name: libass
+  version: 0.17.1
+  category: main
+  manager: conda
+  dependencies:
+  - fontconfig >=2.14.2,<3.0a0
+  - fonts-conda-ecosystem
+  - freetype >=2.12.1,<3.0a0
+  - fribidi >=1.0.10,<2.0a0
+  - harfbuzz >=8.1.1,<9.0a0
+  - libexpat >=2.5.0,<3.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libass-0.17.1-hf7da4fe_1.conda
+  hash:
+    md5: 53fff6fc379154382f5121325c5fe2f5
+    sha256: 31b17bebadd114c6c3e4a647245888fd83ec93533b6ee8f6bfca0bbbc3a95c35
+  build: hf7da4fe_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: ISC
+  license_family: OTHER
+  size: 110763
+  timestamp: 1693027364342
 - platform: win-64
   name: libavif
   version: 1.0.1
   category: main
   manager: conda
   dependencies:
   - aom >=3.7.0,<3.8.0a0
@@ -8726,14 +11562,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: BSD-2-Clause
   license_family: BSD
   size: 90282
   timestamp: 1710444348838
+- platform: osx-arm64
+  name: libavif16
+  version: 1.0.4
+  category: main
+  manager: conda
+  dependencies:
+  - aom >=3.8.2,<3.9.0a0
+  - dav1d >=1.2.1,<1.2.2.0a0
+  - rav1e >=0.6.6,<1.0a0
+  - svt-av1 >=2.0.0,<2.0.1.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libavif16-1.0.4-hff135a0_2.conda
+  hash:
+    md5: 23201bca75be54d6e7c8d5afcc376c16
+    sha256: e62741d7105a7c5f9cb66d3abc94e319d12599047d905cfdde1b2ba12e0b6546
+  build: hff135a0_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 82067
+  timestamp: 1710443848209
 - platform: linux-64
   name: libblas
   version: 3.9.0
   category: main
   manager: conda
   dependencies:
   - libopenblas >=0.3.27,<0.3.28.0a0
@@ -8776,14 +11634,39 @@
   - blas * openblas
   - libcblas 3.9.0 22_osx64_openblas
   - liblapack 3.9.0 22_osx64_openblas
   license: BSD-3-Clause
   license_family: BSD
   size: 14749
   timestamp: 1712542279018
+- platform: osx-arm64
+  name: libblas
+  version: 3.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - libopenblas >=0.3.27,<0.3.28.0a0
+  - libopenblas >=0.3.27,<1.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libblas-3.9.0-22_osxarm64_openblas.conda
+  hash:
+    md5: aeaf35355ef0f37c7c1ba35b7b7db55f
+    sha256: 8620e13366076011cfcc6b2565c7a2d362c5d3f0423f54b9ef9bfc17b1a012a4
+  build: 22_osxarm64_openblas
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 22
+  constrains:
+  - blas * openblas
+  - liblapack 3.9.0 22_osxarm64_openblas
+  - liblapacke 3.9.0 22_osxarm64_openblas
+  - libcblas 3.9.0 22_osxarm64_openblas
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 14824
+  timestamp: 1712542396471
 - platform: win-64
   name: libblas
   version: 3.9.0
   category: main
   manager: conda
   dependencies:
   - mkl 2024.1.0 h66d3029_692
@@ -8837,14 +11720,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: MIT
   license_family: MIT
   size: 67476
   timestamp: 1695990207321
+- platform: osx-arm64
+  name: libbrotlicommon
+  version: 1.1.0
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libbrotlicommon-1.1.0-hb547adb_1.conda
+  hash:
+    md5: cd68f024df0304be41d29a9088162b02
+    sha256: 556f0fddf4bd4d35febab404d98cb6862ce3b7ca843e393da0451bfc4654cf07
+  build: hb547adb_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 68579
+  timestamp: 1695990426128
 - platform: win-64
   name: libbrotlicommon
   version: 1.1.0
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -8897,14 +11798,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: MIT
   license_family: MIT
   size: 30327
   timestamp: 1695990232422
+- platform: osx-arm64
+  name: libbrotlidec
+  version: 1.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - libbrotlicommon 1.1.0 hb547adb_1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libbrotlidec-1.1.0-hb547adb_1.conda
+  hash:
+    md5: ee1a519335cc10d0ec7e097602058c0a
+    sha256: c1c85937828ad3bc434ac60b7bcbde376f4d2ea4ee42d15d369bf2a591775b4a
+  build: hb547adb_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 28928
+  timestamp: 1695990463780
 - platform: win-64
   name: libbrotlidec
   version: 1.1.0
   category: main
   manager: conda
   dependencies:
   - libbrotlicommon 1.1.0 hcfcfb64_1
@@ -8958,14 +11878,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: MIT
   license_family: MIT
   size: 299092
   timestamp: 1695990259225
+- platform: osx-arm64
+  name: libbrotlienc
+  version: 1.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - libbrotlicommon 1.1.0 hb547adb_1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libbrotlienc-1.1.0-hb547adb_1.conda
+  hash:
+    md5: d7e077f326a98b2cc60087eaff7c730b
+    sha256: 690dfc98e891ee1871c54166d30f6e22edfc2d7d6b29e7988dde5f1ce271c81a
+  build: hb547adb_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 280943
+  timestamp: 1695990509392
 - platform: win-64
   name: libbrotlienc
   version: 1.1.0
   category: main
   manager: conda
   dependencies:
   - libbrotlicommon 1.1.0 hcfcfb64_1
@@ -9046,14 +11985,37 @@
   - liblapacke 3.9.0 22_osx64_openblas
   - blas * openblas
   - liblapack 3.9.0 22_osx64_openblas
   license: BSD-3-Clause
   license_family: BSD
   size: 14636
   timestamp: 1712542311437
+- platform: osx-arm64
+  name: libcblas
+  version: 3.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - libblas 3.9.0 22_osxarm64_openblas
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libcblas-3.9.0-22_osxarm64_openblas.conda
+  hash:
+    md5: 37b3682240a69874a22658dedbca37d9
+    sha256: 2c7902985dc77db1d7252b4e838d92a34b1729799ae402988d62d077868f6cca
+  build: 22_osxarm64_openblas
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 22
+  constrains:
+  - blas * openblas
+  - liblapack 3.9.0 22_osxarm64_openblas
+  - liblapacke 3.9.0 22_osxarm64_openblas
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 14741
+  timestamp: 1712542420590
 - platform: win-64
   name: libcblas
   version: 3.9.0
   category: main
   manager: conda
   dependencies:
   - libblas 3.9.0 22_win64_mkl
@@ -9110,14 +12072,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 13694951
   timestamp: 1712568723512
+- platform: osx-arm64
+  name: libclang-cpp18.1
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16.0.6
+  - libllvm18 >=18.1.3,<18.2.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libclang-cpp18.1-18.1.3-default_he012953_0.conda
+  hash:
+    md5: d8e0decc03dadc234e0885bb2a857c68
+    sha256: a528f933aa430c86591ed94e7eb5e4c16947232f149920250ba78e104d91e0b3
+  build: default_he012953_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 12809223
+  timestamp: 1712569190982
 - platform: linux-64
   name: libclang13
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -9193,14 +12175,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 20128
   timestamp: 1633683906221
+- platform: osx-arm64
+  name: libcrc32c
+  version: 1.1.2
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=11.1.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libcrc32c-1.1.2-hbdafb3b_0.tar.bz2
+  hash:
+    md5: 32bd82a6a625ea6ce090a81c3d34edeb
+    sha256: 58477b67cc719060b5b069ba57161e20ba69b8695d154a719cb4b60caf577929
+  build: hbdafb3b_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 18765
+  timestamp: 1633683992603
 - platform: win-64
   name: libcrc32c
   version: 1.1.2
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15.0a0
@@ -9284,14 +12285,38 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: curl
   license_family: MIT
   size: 378176
   timestamp: 1711548390530
+- platform: osx-arm64
+  name: libcurl
+  version: 8.7.1
+  category: main
+  manager: conda
+  dependencies:
+  - krb5 >=1.21.2,<1.22.0a0
+  - libnghttp2 >=1.58.0,<2.0a0
+  - libssh2 >=1.11.0,<2.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.1,<4.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libcurl-8.7.1-h2d989ff_0.conda
+  hash:
+    md5: 34b9171710f0d9bf093d55bdc36ff355
+    sha256: 973ac9368efca712a8fd19fe68524d7d9a3087fd88ad6b7fcdf60c3d2e19a498
+  build: h2d989ff_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: curl
+  license_family: MIT
+  size: 358080
+  timestamp: 1711548548174
 - platform: win-64
   name: libcurl
   version: 8.7.1
   category: main
   manager: conda
   dependencies:
   - krb5 >=1.21.2,<1.22.0a0
@@ -9326,14 +12351,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 1142172
   timestamp: 1686896907750
+- platform: osx-arm64
+  name: libcxx
+  version: 16.0.6
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
+  hash:
+    md5: 9d7d724faf0413bf1dbc5a85935700c8
+    sha256: 11d3fb51c14832d9e4f6d84080a375dec21ea8a3a381a1910e67ff9cedc20355
+  build: h4653b0c_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 1160232
+  timestamp: 1686896993785
 - platform: linux-64
   name: libdeflate
   version: '1.20'
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -9363,14 +12406,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 70364
   timestamp: 1711196727346
+- platform: osx-arm64
+  name: libdeflate
+  version: '1.20'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libdeflate-1.20-h93a5062_0.conda
+  hash:
+    md5: 97efeaeba2a9a82bdf46fc6d025e3a57
+    sha256: 6d16cccb141b6bb05c38107b335089046664ea1d6611601d3f6e7e4227a99925
+  build: h93a5062_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 54481
+  timestamp: 1711196723486
 - platform: win-64
   name: libdeflate
   version: '1.20'
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -9443,14 +12504,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: BSD-2-Clause
   license_family: BSD
   size: 105382
   timestamp: 1597616576726
+- platform: osx-arm64
+  name: libedit
+  version: 3.1.20191231
+  category: main
+  manager: conda
+  dependencies:
+  - ncurses >=6.2,<7.0.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libedit-3.1.20191231-hc8eb9b7_2.tar.bz2
+  hash:
+    md5: 30e4362988a2623e9eb34337b83e01f9
+    sha256: 3912636197933ecfe4692634119e8644904b41a58f30cad9d1fc02f6ba4d9fca
+  build: hc8eb9b7_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 96607
+  timestamp: 1597616630749
 - platform: linux-64
   name: libev
   version: '4.33'
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -9480,14 +12560,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: BSD-2-Clause
   license_family: BSD
   size: 106663
   timestamp: 1702146352558
+- platform: osx-arm64
+  name: libev
+  version: '4.33'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libev-4.33-h93a5062_2.conda
+  hash:
+    md5: 36d33e440c31857372a72137f78bacf5
+    sha256: 95cecb3902fbe0399c3a7e67a5bed1db813e5ab0e22f4023a5e0f722f2cc214f
+  build: h93a5062_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 107458
+  timestamp: 1702146414478
 - platform: linux-64
   name: libevent
   version: 2.1.12
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -9519,14 +12617,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 372661
   timestamp: 1685726378869
+- platform: osx-arm64
+  name: libevent
+  version: 2.1.12
+  category: main
+  manager: conda
+  dependencies:
+  - openssl >=3.1.1,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libevent-2.1.12-h2757513_1.conda
+  hash:
+    md5: 1a109764bff3bdc7bdd84088347d71dc
+    sha256: 8c136d7586259bb5c0d2b913aaadc5b9737787ae4f40e3ad1beaf96c80b919b7
+  build: h2757513_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 368167
+  timestamp: 1685726248899
 - platform: win-64
   name: libevent
   version: 2.1.12
   category: main
   manager: conda
   dependencies:
   - openssl >=3.1.1,<4.0a0
@@ -9582,14 +12699,34 @@
   build_number: 0
   constrains:
   - expat 2.6.2.*
   license: MIT
   license_family: MIT
   size: 69246
   timestamp: 1710362566073
+- platform: osx-arm64
+  name: libexpat
+  version: 2.6.2
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
+  hash:
+    md5: e3cde7cfa87f82f7cb13d482d5e0ad09
+    sha256: ba7173ac30064ea901a4c9fb5a51846dcc25512ceb565759be7d18cbf3e5415e
+  build: hebf3989_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - expat 2.6.2.*
+  license: MIT
+  license_family: MIT
+  size: 63655
+  timestamp: 1710362424980
 - platform: win-64
   name: libexpat
   version: 2.6.2
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
@@ -9639,14 +12776,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 5
   license: MIT
   license_family: MIT
   size: 51348
   timestamp: 1636488394370
+- platform: osx-arm64
+  name: libffi
+  version: 3.4.2
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
+  hash:
+    md5: 086914b672be056eb70fd4285b6783b6
+    sha256: 41b3d13efb775e340e4dba549ab5c029611ea6918703096b2eaa9c015c0750ca
+  build: h3422bc3_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  license: MIT
+  license_family: MIT
+  size: 39020
+  timestamp: 1636488587153
 - platform: win-64
   name: libffi
   version: 3.4.2
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15.0a0
@@ -9688,49 +12843,49 @@
   timestamp: 1687765514062
 - platform: linux-64
   name: libgcc-devel_linux-64
   version: 13.2.0
   category: main
   manager: conda
   dependencies: []
-  url: https://conda.anaconda.org/conda-forge/noarch/libgcc-devel_linux-64-13.2.0-ha9c7c90_105.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/libgcc-devel_linux-64-13.2.0-h95c4c6d_106.conda
   hash:
-    md5: 3bc29a967fee57e193ce51f51c598bca
-    sha256: 858029ad4d66869c533bb5a22e95e7c044ca66c61d6f403f10d9ae074a0e360e
-  build: ha9c7c90_105
+    md5: 960fa4aaa5c6a4733ac71954d835ce99
+    sha256: b0bf49439d146275a0ad5cb5e6bf15da0f1257cdc7299589da820fd55d19588a
+  build: h95c4c6d_106
   arch: x86_64
   subdir: linux-64
-  build_number: 105
+  build_number: 106
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
   noarch: generic
-  size: 2578210
-  timestamp: 1706819085946
+  size: 2581282
+  timestamp: 1713754805427
 - platform: linux-64
   name: libgcc-ng
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
   - _libgcc_mutex 0.1 conda_forge
   - _openmp_mutex >=4.5
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda
   hash:
-    md5: d4ff227c46917d3b4565302a2bbb276b
-    sha256: d32f78bfaac282cfe5205f46d558704ad737b8dbf71f9227788a5ca80facaba4
-  build: h807b86a_5
+    md5: df88796bd09a0d2ed292e59101478ad8
+    sha256: 836a0057525f1414de43642d357d0ab21ac7f85e24800b010dbc17d132e6efec
+  build: hc881cc4_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   constrains:
-  - libgomp 13.2.0 h807b86a_5
+  - libgomp 13.2.0 hc881cc4_6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 770506
-  timestamp: 1706819192021
+  size: 777315
+  timestamp: 1713755001744
 - platform: linux-64
   name: libgcrypt
   version: 1.10.3
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -9782,14 +12937,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: GPL-3.0-or-later
   license_family: GPL
   size: 172506
   timestamp: 1712512827340
+- platform: osx-arm64
+  name: libgettextpo
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies:
+  - libiconv >=1.17,<2.0a0
+  - libintl 0.22.5 h8fbad5d_2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libgettextpo-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: a66fad933e22d22599a6dd149d359d25
+    sha256: c3f5580e172c3fc03d33e8994024f08b709a239bd599792e51435fa7a06beb64
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: GPL-3.0-or-later
+  license_family: GPL
+  size: 159856
+  timestamp: 1712512788407
 - platform: win-64
   name: libgettextpo
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - libiconv >=1.17,<2.0a0
@@ -9843,14 +13018,35 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: GPL-3.0-or-later
   license_family: GPL
   size: 37189
   timestamp: 1712512859854
+- platform: osx-arm64
+  name: libgettextpo-devel
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies:
+  - libgettextpo 0.22.5 h8fbad5d_2
+  - libiconv >=1.17,<2.0a0
+  - libintl 0.22.5 h8fbad5d_2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libgettextpo-devel-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: 1113aa220b042b7ce8d077ea8f696f98
+    sha256: b1be0bb8a726e2c47a025ff348e6ba8b51ef668f6ace06694657025d84ae66e2
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: GPL-3.0-or-later
+  license_family: GPL
+  size: 37221
+  timestamp: 1712512820461
 - platform: win-64
   name: libgettextpo-devel
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - libgettextpo 0.22.5 h5728263_2
@@ -9883,54 +13079,73 @@
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
   size: 110106
   timestamp: 1707328956438
+- platform: osx-arm64
+  name: libgfortran
+  version: 5.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - libgfortran5 13.2.0 hf226fd6_3
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libgfortran-5.0.0-13_2_0_hd922786_3.conda
+  hash:
+    md5: 4a55d9e169114b2b90d3ec4604cd7bbf
+    sha256: 44e541b4821c96b28b27fef5630883a60ce4fee91fd9c79f25a199f8f73f337b
+  build: 13_2_0_hd922786_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
+  size: 110233
+  timestamp: 1707330749033
 - platform: linux-64
   name: libgfortran-ng
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
-  - libgfortran5 13.2.0 ha4646dd_5
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_5.conda
+  - libgfortran5 13.2.0 h43f5ff8_6
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.2.0-h69a702a_6.conda
   hash:
-    md5: e73e9cfd1191783392131e6238bdb3e9
-    sha256: 238c16c84124d58307376715839aa152bd4a1bf5a043052938ad6c3137d30245
-  build: h69a702a_5
+    md5: 3666a850342f8f3be88f9a93d948d027
+    sha256: 5e436753c55d81005e9383d7a8ec14298ebd35029d148db7e03c4834ffca54ee
+  build: h69a702a_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 23829
-  timestamp: 1706819413770
+  size: 24183
+  timestamp: 1713755271389
 - platform: linux-64
   name: libgfortran5
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=13.2.0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-ha4646dd_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.2.0-h43f5ff8_6.conda
   hash:
-    md5: 7a6bd7a12a4bd359e2afe6c0fa1acace
-    sha256: ba8d94e8493222ce155bb264d9de4200e41498a458e866fedf444de809bde8b6
-  build: ha4646dd_5
+    md5: e54a5ddc67e673f9105cf2a2e9c070b0
+    sha256: 5da2abd9e2c09ec8566fbacb237926b532f6629871ff2733c90a0be77b77679e
+  build: h43f5ff8_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   constrains:
   - libgfortran-ng 13.2.0
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 1442769
-  timestamp: 1706819209473
+  size: 1442624
+  timestamp: 1713755021286
 - platform: osx-64
   name: libgfortran5
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
   - llvm-openmp >=8.0.0
@@ -9944,89 +13159,134 @@
   build_number: 3
   constrains:
   - libgfortran 5.0.0 13_2_0_*_3
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
   size: 1571379
   timestamp: 1707328880361
+- platform: osx-arm64
+  name: libgfortran5
+  version: 13.2.0
+  category: main
+  manager: conda
+  dependencies:
+  - llvm-openmp >=8.0.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libgfortran5-13.2.0-hf226fd6_3.conda
+  hash:
+    md5: 66ac81d54e95c534ae488726c1f698ea
+    sha256: bafc679eedb468a86aa4636061c55966186399ee0a04b605920d208d97ac579a
+  build: hf226fd6_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  constrains:
+  - libgfortran 5.0.0 13_2_0_*_3
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
+  size: 997381
+  timestamp: 1707330687590
 - platform: linux-64
   name: libglib
   version: 2.80.0
   category: main
   manager: conda
   dependencies:
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - pcre2 >=10.43,<10.44.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_6.conda
   hash:
-    md5: 4423ae9726113b68e9527b27baae191f
-    sha256: 18233d83e0385afc50148520e5b9c6ee65886c41ecdc69e335f60a279fb7a1f5
-  build: hf2295e7_5
+    md5: 9342e7c44c38bea649490f72d92c382d
+    sha256: d2867a1515676f3b64265420598badb2e4ad2369d85237fb276173a99959eb37
+  build: hf2295e7_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   constrains:
-  - glib 2.80.0 *_5
+  - glib 2.80.0 *_6
   license: LGPL-2.1-or-later
-  size: 3892640
-  timestamp: 1713203313894
+  size: 3942450
+  timestamp: 1713639388280
 - platform: osx-64
   name: libglib
   version: 2.80.0
   category: main
   manager: conda
   dependencies:
   - libffi >=3.4,<4.0a0
   - libiconv >=1.17,<2.0a0
   - libintl >=0.22.5,<1.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - pcre2 >=10.43,<10.44.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_5.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libglib-2.80.0-h81c1438_6.conda
   hash:
-    md5: 9105a1c35c37d2908a543bdf7f08f80a
-    sha256: a6778ec265222eb9277ec9f2e7519a80dadea0455c7d5386eab624d699346868
-  build: h81c1438_5
+    md5: 54dd1ed37dd65c5d13600bcc5ebbd0a1
+    sha256: 1cbca3cfdc470c528a36c93d9d478103d2a7a6036814ab23fa0486cde29e9607
+  build: h81c1438_6
   arch: x86_64
   subdir: osx-64
-  build_number: 5
+  build_number: 6
+  constrains:
+  - glib 2.80.0 *_6
+  license: LGPL-2.1-or-later
+  size: 3687274
+  timestamp: 1713641327993
+- platform: osx-arm64
+  name: libglib
+  version: 2.80.0
+  category: main
+  manager: conda
+  dependencies:
+  - libffi >=3.4,<4.0a0
+  - libiconv >=1.17,<2.0a0
+  - libintl >=0.22.5,<1.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - pcre2 >=10.43,<10.44.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libglib-2.80.0-hfc324ee_6.conda
+  hash:
+    md5: 762a78b7637203d7ada1403e547470ec
+    sha256: 912913b1d6f3ec1e7dcb3a59426f2d9f70a996891cca718f32195687eb271e06
+  build: hfc324ee_6
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 6
   constrains:
-  - glib 2.80.0 *_5
+  - glib 2.80.0 *_6
   license: LGPL-2.1-or-later
-  size: 3645199
-  timestamp: 1713203913332
+  size: 3615908
+  timestamp: 1713639914767
 - platform: win-64
   name: libglib
   version: 2.80.0
   category: main
   manager: conda
   dependencies:
   - libffi >=3.4,<4.0a0
   - libiconv >=1.17,<2.0a0
   - libintl >=0.22.5,<1.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - pcre2 >=10.43,<10.44.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
-  url: https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_5.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/libglib-2.80.0-h39d0aa6_6.conda
   hash:
-    md5: c2e707c449ac60fa0ad8fbdd8f79327c
-    sha256: 73ed5772acce96d0dc88c13000ee7678d12dda88b07ad721d4d20c807a98b6c2
-  build: h39d0aa6_5
+    md5: cd5c6efbe213c089f78575c98ab9a0ed
+    sha256: 87772cdcfb292a64ddd9e737c5deaaf671c7cd82b22ad70c8a8a9f1f34074fb5
+  build: h39d0aa6_6
   arch: x86_64
   subdir: win-64
-  build_number: 5
+  build_number: 6
   constrains:
-  - glib 2.80.0 *_5
+  - glib 2.80.0 *_6
   license: LGPL-2.1-or-later
-  size: 3699734
-  timestamp: 1713203698247
+  size: 3740691
+  timestamp: 1713639713931
 - platform: linux-64
   name: libglu
   version: 9.0.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -10049,82 +13309,109 @@
 - platform: linux-64
   name: libgomp
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
   - _libgcc_mutex 0.1 conda_forge
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda
   hash:
-    md5: d211c42b9ce49aee3734fdc828731689
-    sha256: 0d3d4b1b0134283ea02d58e8eb5accf3655464cf7159abf098cc694002f8d34e
-  build: h807b86a_5
+    md5: aae89d3736661c36a5591788aebd0817
+    sha256: e722b19b23b31a14b1592d5eceabb38dc52452ff5e4d346e330526971c22e52a
+  build: hc881cc4_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 419751
-  timestamp: 1706819107383
+  size: 422363
+  timestamp: 1713754915251
 - platform: linux-64
   name: libgoogle-cloud
-  version: 2.22.0
+  version: 2.23.0
   category: main
   manager: conda
   dependencies:
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
-  - libcurl >=8.5.0,<9.0a0
+  - libcurl >=8.7.1,<9.0a0
   - libgcc-ng >=12
-  - libgrpc >=1.62.0,<1.63.0a0
+  - libgrpc >=1.62.2,<1.63.0a0
   - libprotobuf >=4.25.3,<4.25.4.0a0
   - libstdcxx-ng >=12
   - openssl >=3.2.1,<4.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgoogle-cloud-2.22.0-h9be4e54_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgoogle-cloud-2.23.0-h9be4e54_1.conda
   hash:
-    md5: 4b4e36a91e7dabf7345b82d85767a7c3
-    sha256: b9980209438b22113f4352df2b260bf43b2eb63a7b6325192ec5ae3a562872ed
+    md5: 1042d8401bb268553f98e60120cdeb40
+    sha256: 680f5a9bc45aa905d9da086b16551438553649e05dd6b94b02b379b050602d5e
   build: h9be4e54_1
   arch: x86_64
   subdir: linux-64
   build_number: 1
   constrains:
-  - libgoogle-cloud 2.22.0 *_1
+  - libgoogle-cloud 2.23.0 *_1
   license: Apache-2.0
   license_family: Apache
-  size: 1209816
-  timestamp: 1709737846418
+  size: 1214608
+  timestamp: 1713798219648
 - platform: osx-64
   name: libgoogle-cloud
-  version: 2.22.0
+  version: 2.23.0
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
-  - libcurl >=8.5.0,<9.0a0
+  - libcurl >=8.7.1,<9.0a0
   - libcxx >=16
-  - libgrpc >=1.62.0,<1.63.0a0
+  - libgrpc >=1.62.2,<1.63.0a0
   - libprotobuf >=4.25.3,<4.25.4.0a0
   - openssl >=3.2.1,<4.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libgoogle-cloud-2.22.0-h651e89d_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libgoogle-cloud-2.23.0-h651e89d_1.conda
   hash:
-    md5: 3f2faf53ecb3b51b92b3eee155b50233
-    sha256: 39f2f50202e50e41ee8581c99a0b3023c2c21cab80ba597f8c5be7c8c8c6a059
+    md5: e39d78408ff66de247fb5fbf60e9255c
+    sha256: 669cab160b07f1083fa641564549f38d143380ad36b05e16aeb59625e6fbd08a
   build: h651e89d_1
   arch: x86_64
   subdir: osx-64
   build_number: 1
   constrains:
-  - libgoogle-cloud 2.22.0 *_1
+  - libgoogle-cloud 2.23.0 *_1
   license: Apache-2.0
   license_family: Apache
-  size: 849198
-  timestamp: 1709738549021
+  size: 852907
+  timestamp: 1713800994635
+- platform: osx-arm64
+  name: libgoogle-cloud
+  version: 2.23.0
+  category: main
+  manager: conda
+  dependencies:
+  - libabseil * cxx17*
+  - libabseil >=20240116.1,<20240117.0a0
+  - libcurl >=8.7.1,<9.0a0
+  - libcxx >=16
+  - libgrpc >=1.62.2,<1.63.0a0
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  - openssl >=3.2.1,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libgoogle-cloud-2.23.0-hbebe991_1.conda
+  hash:
+    md5: fdbdbd1dc8e8ba458057be0a00db8ab1
+    sha256: db7c0dcebafc001ff9fe0ba618ed611721217b4ceefeef189ab79ef111056c02
+  build: hbebe991_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  constrains:
+  - libgoogle-cloud 2.23.0 *_1
+  license: Apache-2.0
+  license_family: Apache
+  size: 840819
+  timestamp: 1713799797441
 - platform: win-64
   name: libgoogle-cloud
   version: 2.12.0
   category: main
   manager: conda
   dependencies:
   - libabseil * cxx17*
@@ -10149,144 +13436,200 @@
   - google-cloud-cpp 2.12.0 *_4
   license: Apache-2.0
   license_family: Apache
   size: 13270
   timestamp: 1698887885269
 - platform: linux-64
   name: libgoogle-cloud-storage
-  version: 2.22.0
+  version: 2.23.0
   category: main
   manager: conda
   dependencies:
   - libabseil
   - libcrc32c >=1.1.2,<1.2.0a0
   - libcurl
   - libgcc-ng >=12
-  - libgoogle-cloud 2.22.0 h9be4e54_1
+  - libgoogle-cloud 2.23.0 h9be4e54_1
   - libstdcxx-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   - openssl
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgoogle-cloud-storage-2.22.0-hc7a4891_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgoogle-cloud-storage-2.23.0-hc7a4891_1.conda
   hash:
-    md5: 7811f043944e010e54640918ea82cecd
-    sha256: 0e00e1ca2a981db1c96071edf266bc29fd6f13ac484225de1736fc4dac5c64a8
+    md5: ee99fb9107ffb579b58ee92a5fb14b06
+    sha256: b85ce8b78e9262670a145a1639e253708e2a9eb9100d60ccec16f8e41d87a4bb
   build: hc7a4891_1
   arch: x86_64
   subdir: linux-64
   build_number: 1
   license: Apache-2.0
   license_family: Apache
-  size: 748818
-  timestamp: 1709738181078
+  size: 752661
+  timestamp: 1713798390317
 - platform: osx-64
   name: libgoogle-cloud-storage
-  version: 2.22.0
+  version: 2.23.0
   category: main
   manager: conda
   dependencies:
   - libabseil
   - libcrc32c >=1.1.2,<1.2.0a0
   - libcurl
   - libcxx >=16
-  - libgoogle-cloud 2.22.0 h651e89d_1
+  - libgoogle-cloud 2.23.0 h651e89d_1
   - libzlib >=1.2.13,<1.3.0a0
   - openssl
-  url: https://conda.anaconda.org/conda-forge/osx-64/libgoogle-cloud-storage-2.22.0-ha67e85c_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libgoogle-cloud-storage-2.23.0-ha67e85c_1.conda
   hash:
-    md5: 0c25180c34b1a58d309b28386698fb6e
-    sha256: e4f351e55fe7c0656cb608eba8690063e3b407d25a855c9d1fd832486d4a1244
+    md5: 62798f6e7af787f3cc550ccf70ddb1e3
+    sha256: 35a6e7824ab06fd21042260fb4b11788c088b570ba32bd3f873f91ae12810326
   build: ha67e85c_1
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: Apache-2.0
   license_family: Apache
-  size: 523045
-  timestamp: 1709739227970
+  size: 524880
+  timestamp: 1713802437812
+- platform: osx-arm64
+  name: libgoogle-cloud-storage
+  version: 2.23.0
+  category: main
+  manager: conda
+  dependencies:
+  - libabseil
+  - libcrc32c >=1.1.2,<1.2.0a0
+  - libcurl
+  - libcxx >=16
+  - libgoogle-cloud 2.23.0 hbebe991_1
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libgoogle-cloud-storage-2.23.0-h8a76758_1.conda
+  hash:
+    md5: 356c74978867e07e12a939a092dcf30d
+    sha256: 3173b65b7e36e9fa0e6ddec69f39e4dd0e7ada38dbf2c1be006fddc2e7257b0c
+  build: h8a76758_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: Apache-2.0
+  license_family: Apache
+  size: 509643
+  timestamp: 1713801031940
 - platform: linux-64
   name: libgpg-error
-  version: '1.48'
+  version: '1.49'
   category: main
   manager: conda
   dependencies:
-  - gettext >=0.21.1,<1.0a0
+  - gettext
+  - libasprintf >=0.22.5,<1.0a0
   - libgcc-ng >=12
+  - libgettextpo >=0.22.5,<1.0a0
   - libstdcxx-ng >=12
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.48-h71f35ed_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.49-h4f305b6_0.conda
   hash:
-    md5: 4d18d86916705d352d5f4adfb7f0edd3
-    sha256: c448c6d86d27e10b9e844172000540e9cbfe9c28f968db87f949ba05add9bd50
-  build: h71f35ed_0
+    md5: dfcfd72c7a430d3616763ecfbefe4ca9
+    sha256: b2664c2c11211a63856f23278efb49d3e65d902297989a0c12dcd228b5d97110
+  build: h4f305b6_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: GPL-2.0-only
   license_family: GPL
-  size: 266447
-  timestamp: 1708702470365
+  size: 263319
+  timestamp: 1714121531915
 - platform: linux-64
   name: libgrpc
-  version: 1.62.1
+  version: 1.62.2
   category: main
   manager: conda
   dependencies:
-  - c-ares >=1.27.0,<2.0a0
+  - c-ares >=1.28.1,<2.0a0
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
   - libgcc-ng >=12
   - libprotobuf >=4.25.3,<4.25.4.0a0
   - libre2-11 >=2023.9.1,<2024.0a0
   - libstdcxx-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   - openssl >=3.2.1,<4.0a0
   - re2
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.62.1-h15f2491_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.62.2-h15f2491_0.conda
   hash:
-    md5: 564517a8cbd095cff75eb996d33d2b7e
-    sha256: 1d4ece94dfef73d904dcba0fd9d56098796f5fdc62ea5f9edff60c71be7a3d63
+    md5: 8dabe607748cb3d7002ad73cd06f1325
+    sha256: 28241ed89335871db33cb6010e9ccb2d9e9b6bb444ddf6884f02f0857363c06a
   build: h15f2491_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   constrains:
-  - grpc-cpp =1.62.1
+  - grpc-cpp =1.62.2
   license: Apache-2.0
   license_family: APACHE
-  size: 7667664
-  timestamp: 1709938059287
+  size: 7316832
+  timestamp: 1713390645548
 - platform: osx-64
   name: libgrpc
-  version: 1.62.1
+  version: 1.62.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - c-ares >=1.27.0,<2.0a0
+  - c-ares >=1.28.1,<2.0a0
   - libabseil * cxx17*
   - libabseil >=20240116.1,<20240117.0a0
   - libcxx >=16
   - libprotobuf >=4.25.3,<4.25.4.0a0
   - libre2-11 >=2023.9.1,<2024.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openssl >=3.2.1,<4.0a0
   - re2
-  url: https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.62.1-h384b2fc_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.62.2-h384b2fc_0.conda
   hash:
-    md5: 2ac05daca7276a4d6ca4465707670380
-    sha256: 8c9898d259e2343df52259b599ec342c386679e1c420df603cba6f06078fcdd6
+    md5: 9421f67cf8b4bc976fe5d0c3ab42de18
+    sha256: 7c228040e7dac4e5e7e6935a4decf6bc2155cc05fcfb0811d25ccb242d0036ba
   build: h384b2fc_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   constrains:
-  - grpc-cpp =1.62.1
+  - grpc-cpp =1.62.2
   license: Apache-2.0
   license_family: APACHE
-  size: 4432823
-  timestamp: 1709938959215
+  size: 5189573
+  timestamp: 1713392887258
+- platform: osx-arm64
+  name: libgrpc
+  version: 1.62.2
+  category: main
+  manager: conda
+  dependencies:
+  - c-ares >=1.28.1,<2.0a0
+  - libabseil * cxx17*
+  - libabseil >=20240116.1,<20240117.0a0
+  - libcxx >=16
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  - libre2-11 >=2023.9.1,<2024.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.1,<4.0a0
+  - re2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libgrpc-1.62.2-h9c18a4f_0.conda
+  hash:
+    md5: e624fc11026dbb84c549435eccd08623
+    sha256: d2c5b5a828f6f1242c11e8c91968f48f64446f7dd5cbfa1197545e465eb7d47a
+  build: h9c18a4f_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - grpc-cpp =1.62.2
+  license: Apache-2.0
+  license_family: APACHE
+  size: 5016525
+  timestamp: 1713392846329
 - platform: win-64
   name: libgrpc
   version: 1.59.3
   category: main
   manager: conda
   dependencies:
   - c-ares >=1.21.0,<2.0a0
@@ -10351,14 +13694,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1000
   license: BSD-3-Clause
   license_family: BSD
   size: 2346864
   timestamp: 1711490587770
+- platform: osx-arm64
+  name: libhwloc
+  version: 2.10.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - libxml2 >=2.12.6,<3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libhwloc-2.10.0-default_h52d8fe8_1000.conda
+  hash:
+    md5: 530b33b17e97f7da76e2c432909daa5b
+    sha256: 4e8a88e1ed996c42b464b1432aa3a70962f27881c0ada9b9f50d0ffd717d059a
+  build: default_h52d8fe8_1000
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1000
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 2321075
+  timestamp: 1711490652210
 - platform: win-64
   name: libhwloc
   version: 2.10.0
   category: main
   manager: conda
   dependencies:
   - libxml2 >=2.12.6,<3.0a0
@@ -10413,14 +13776,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 778925
   timestamp: 1708225689339
+- platform: osx-arm64
+  name: libhwy
+  version: 1.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libhwy-1.1.0-h2ffa867_0.conda
+  hash:
+    md5: 6b0da720436e6410f6624f17aece6af2
+    sha256: 2bab9c7cf1a84bc6add78fe7c4285fd20dfb8461f36e24802fcffb77bc6a10b9
+  build: h2ffa867_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 453634
+  timestamp: 1708225377360
 - platform: linux-64
   name: libiconv
   version: '1.17'
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -10448,14 +13830,31 @@
   build: hd75f5a5_2
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: LGPL-2.1-only
   size: 666538
   timestamp: 1702682713201
+- platform: osx-arm64
+  name: libiconv
+  version: '1.17'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libiconv-1.17-h0d3ecfb_2.conda
+  hash:
+    md5: 69bda57310071cf6d2b86caf11573d2d
+    sha256: bc7de5097b97bcafcf7deaaed505f7ce02f648aac8eccc0d5a47cc599a1d0304
+  build: h0d3ecfb_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: LGPL-2.1-only
+  size: 676469
+  timestamp: 1702682458114
 - platform: win-64
   name: libiconv
   version: '1.17'
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -10507,14 +13906,33 @@
   build: h10d778d_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: LGPLv2
   size: 133237
   timestamp: 1706368325339
+- platform: osx-arm64
+  name: libidn2
+  version: 2.3.7
+  category: main
+  manager: conda
+  dependencies:
+  - gettext >=0.21.1,<1.0a0
+  - libunistring >=0,<1.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libidn2-2.3.7-h93a5062_0.conda
+  hash:
+    md5: 6e4a21ef7a8e4c0cc65381854848e232
+    sha256: ae6be1c42fa18cb76fb1d17093f5b467b7a9bcf402da91081a9126c8843c004d
+  build: h93a5062_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: LGPLv2
+  size: 134491
+  timestamp: 1706368362998
 - platform: osx-64
   name: libintl
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - libiconv >=1.17,<2.0a0
@@ -10525,14 +13943,32 @@
   build: h5ff76d1_2
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: LGPL-2.1-or-later
   size: 74307
   timestamp: 1712512790983
+- platform: osx-arm64
+  name: libintl
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies:
+  - libiconv >=1.17,<2.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libintl-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: 3d216d0add050129007de3342be7b8c5
+    sha256: 21bc79bdf34ffd20cb84d2a8bd82d7d0e2a1b94b9e72773f0fb207e5b4f1ff63
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: LGPL-2.1-or-later
+  size: 81206
+  timestamp: 1712512755390
 - platform: win-64
   name: libintl
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - libiconv >=1.17,<2.0a0
@@ -10562,14 +13998,33 @@
   build: h5ff76d1_2
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: LGPL-2.1-or-later
   size: 38422
   timestamp: 1712512843420
+- platform: osx-arm64
+  name: libintl-devel
+  version: 0.22.5
+  category: main
+  manager: conda
+  dependencies:
+  - libiconv >=1.17,<2.0a0
+  - libintl 0.22.5 h8fbad5d_2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libintl-devel-0.22.5-h8fbad5d_2.conda
+  hash:
+    md5: 962b3348c68efd25da253e94590ea9a2
+    sha256: e52b2d0c5711f64b523756ccd9b800ee6f10a6317432b20a417dc3792e0a794a
+  build: h8fbad5d_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: LGPL-2.1-or-later
+  size: 38616
+  timestamp: 1712512805567
 - platform: win-64
   name: libintl-devel
   version: 0.22.5
   category: main
   manager: conda
   dependencies:
   - libiconv >=1.17,<2.0a0
@@ -10620,14 +14075,33 @@
   subdir: osx-64
   build_number: 1
   constrains:
   - jpeg <0.0.0a
   license: IJG AND BSD-3-Clause AND Zlib
   size: 579748
   timestamp: 1694475265912
+- platform: osx-arm64
+  name: libjpeg-turbo
+  version: 3.0.0
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libjpeg-turbo-3.0.0-hb547adb_1.conda
+  hash:
+    md5: 3ff1e053dc3a2b8e36b9bfa4256a58d1
+    sha256: a42054eaa38e84fc1e5ab443facac4bbc9d1b6b6f23f54b7bf4f1eb687e1d993
+  build: hb547adb_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  constrains:
+  - jpeg <0.0.0a
+  license: IJG AND BSD-3-Clause AND Zlib
+  size: 547541
+  timestamp: 1694475104253
 - platform: win-64
   name: libjpeg-turbo
   version: 3.0.0
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -10644,57 +14118,79 @@
   constrains:
   - jpeg <0.0.0a
   license: IJG AND BSD-3-Clause AND Zlib
   size: 822966
   timestamp: 1694475223854
 - platform: linux-64
   name: libjxl
-  version: 0.10.1
+  version: 0.10.2
   category: main
   manager: conda
   dependencies:
   - libbrotlidec >=1.1.0,<1.2.0a0
   - libbrotlienc >=1.1.0,<1.2.0a0
   - libgcc-ng >=12
   - libhwy >=1.1.0,<1.2.0a0
   - libstdcxx-ng >=12
-  url: https://conda.anaconda.org/conda-forge/linux-64/libjxl-0.10.1-hcae5a98_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libjxl-0.10.2-hcae5a98_0.conda
   hash:
-    md5: ca9532696d031f78d1dc245c413823d4
-    sha256: da25dc6ac688fbd90ba36dbf44c8b02be582fdaaf0cd66f9ea64bb7dce5c40d8
-  build: hcae5a98_1
+    md5: 901db891e1e21afd8524cd636a8c8e3b
+    sha256: 3d3f9907e5c5100b9cb7199b65d5e813f3e6aff30891007b90b7fbf27b68077a
+  build: hcae5a98_0
   arch: x86_64
   subdir: linux-64
-  build_number: 1
+  build_number: 0
   license: BSD-3-Clause
   license_family: BSD
-  size: 1588495
-  timestamp: 1711785278878
+  size: 1586204
+  timestamp: 1713744356802
 - platform: osx-64
   name: libjxl
-  version: 0.10.1
+  version: 0.10.2
   category: main
   manager: conda
   dependencies:
   - libbrotlidec >=1.1.0,<1.2.0a0
   - libbrotlienc >=1.1.0,<1.2.0a0
   - libcxx >=16
   - libhwy >=1.1.0,<1.2.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libjxl-0.10.1-hb3b1962_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libjxl-0.10.2-hb3b1962_0.conda
   hash:
-    md5: 8a03e49804c823f790fe3b12c8fd6d04
-    sha256: 8b23c51aba5821dc153e817f0fb013cdbf44eded2f14f8ec252a9a217f91d659
-  build: hb3b1962_1
+    md5: 8f31b16308b91e62af29a3f856e950c9
+    sha256: a190f6b56e3fe9b9d713f59c98bb18acc8d075ec60dc924d42dc15b567ff5b4b
+  build: hb3b1962_0
   arch: x86_64
   subdir: osx-64
-  build_number: 1
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 1395075
+  timestamp: 1713744830943
+- platform: osx-arm64
+  name: libjxl
+  version: 0.10.2
+  category: main
+  manager: conda
+  dependencies:
+  - libbrotlidec >=1.1.0,<1.2.0a0
+  - libbrotlienc >=1.1.0,<1.2.0a0
+  - libcxx >=16
+  - libhwy >=1.1.0,<1.2.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libjxl-0.10.2-h07599a0_0.conda
+  hash:
+    md5: da2c6acbab771340d3e07f50e9170a8b
+    sha256: 69e627c9e6b33458fa8fa0faeaeda340c32da50801b7dada8cdd41843a38fdd8
+  build: h07599a0_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
   license: BSD-3-Clause
   license_family: BSD
-  size: 1396356
-  timestamp: 1711785853213
+  size: 918813
+  timestamp: 1713745061534
 - platform: linux-64
   name: liblapack
   version: 3.9.0
   category: main
   manager: conda
   dependencies:
   - libblas 3.9.0 22_linux64_openblas
@@ -10733,14 +14229,37 @@
   - liblapacke 3.9.0 22_osx64_openblas
   - blas * openblas
   - libcblas 3.9.0 22_osx64_openblas
   license: BSD-3-Clause
   license_family: BSD
   size: 14657
   timestamp: 1712542322711
+- platform: osx-arm64
+  name: liblapack
+  version: 3.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - libblas 3.9.0 22_osxarm64_openblas
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/liblapack-3.9.0-22_osxarm64_openblas.conda
+  hash:
+    md5: f2794950bc005e123b2c21f7fa3d7a6e
+    sha256: 2b1b24c98d15a6a3ad54cf7c8fef1ddccf84b7c557cde08235aaeffd1ff50ee8
+  build: 22_osxarm64_openblas
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 22
+  constrains:
+  - blas * openblas
+  - liblapacke 3.9.0 22_osxarm64_openblas
+  - libcblas 3.9.0 22_osxarm64_openblas
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 14730
+  timestamp: 1712542435551
 - platform: win-64
   name: liblapack
   version: 3.9.0
   category: main
   manager: conda
   dependencies:
   - libblas 3.9.0 22_win64_mkl
@@ -10802,14 +14321,37 @@
   build_number: 22
   constrains:
   - blas * openblas
   license: BSD-3-Clause
   license_family: BSD
   size: 14654
   timestamp: 1712542334599
+- platform: osx-arm64
+  name: liblapacke
+  version: 3.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - libblas 3.9.0 22_osxarm64_openblas
+  - libcblas 3.9.0 22_osxarm64_openblas
+  - liblapack 3.9.0 22_osxarm64_openblas
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/liblapacke-3.9.0-22_osxarm64_openblas.conda
+  hash:
+    md5: cb2da058b4e05a619f0cf261086e1d82
+    sha256: 88868c5864fe9ca636335ab449a3c8b3a7273836722d2dcae778d2e47705a857
+  build: 22_osxarm64_openblas
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 22
+  constrains:
+  - blas * openblas
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 14743
+  timestamp: 1712542448005
 - platform: win-64
   name: liblapacke
   version: 3.9.0
   category: main
   manager: conda
   dependencies:
   - libblas 3.9.0 22_win64_mkl
@@ -10893,14 +14435,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 25196932
   timestamp: 1701379796962
+- platform: osx-arm64
+  name: libllvm16
+  version: 16.0.6
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - libxml2 >=2.12.1,<3.0.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libllvm16-16.0.6-haab561b_3.conda
+  hash:
+    md5: 9900d62ede9ce25b569beeeab1da094e
+    sha256: f240f3776b02c39a32ce7397d6f2de072510321c835f4def452fc62e5c3babc0
+  build: haab561b_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 23347663
+  timestamp: 1701374993634
 - platform: linux-64
   name: libllvm18
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -10938,14 +14502,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 27580830
   timestamp: 1712517566570
+- platform: osx-arm64
+  name: libllvm18
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - libxml2 >=2.12.6,<3.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libllvm18-18.1.3-h30cc82d_0.conda
+  hash:
+    md5: fad73e8421bcd0de381d172c2224d3a5
+    sha256: 5a8781ab13b163fd028916d050bb209718b14de85493bb7a4b93ea798998b9fe
+  build: h30cc82d_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 25782519
+  timestamp: 1712517407600
 - platform: linux-64
   name: libnghttp2
   version: 1.58.0
   category: main
   manager: conda
   dependencies:
   - c-ares >=1.23.0,<2.0a0
@@ -10988,14 +14574,39 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: MIT
   license_family: MIT
   size: 599736
   timestamp: 1702130398536
+- platform: osx-arm64
+  name: libnghttp2
+  version: 1.58.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=10.9
+  - c-ares >=1.23.0,<2.0a0
+  - libcxx >=16.0.6
+  - libev >=4.33,<4.34.0a0
+  - libev >=4.33,<5.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.0,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libnghttp2-1.58.0-ha4dd798_1.conda
+  hash:
+    md5: 1813e066bfcef82de579a0be8a766df4
+    sha256: fc97aaaf0c6d0f508be313d86c2705b490998d382560df24be918b8e977802cd
+  build: ha4dd798_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 565451
+  timestamp: 1702130473930
 - platform: linux-64
   name: libnl
   version: 3.9.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -11111,14 +14722,37 @@
   build_number: 0
   constrains:
   - openblas >=0.3.27,<0.3.28.0a0
   license: BSD-3-Clause
   license_family: BSD
   size: 6047531
   timestamp: 1712366254156
+- platform: osx-arm64
+  name: libopenblas
+  version: 0.3.27
+  category: main
+  manager: conda
+  dependencies:
+  - libgfortran 5.*
+  - libgfortran5 >=12.3.0
+  - llvm-openmp >=16.0.6
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenblas-0.3.27-openmp_h6c19121_0.conda
+  hash:
+    md5: 82eba59f4eca26a9fc904d584f8761c0
+    sha256: feb2662444fc98a4842fe54cc70b1f109b2146108e7bac2b3bbad1f219cede90
+  build: openmp_h6c19121_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - openblas >=0.3.27,<0.3.28.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 2925015
+  timestamp: 1712364212874
 - platform: linux-64
   name: libopencv
   version: 4.9.0
   category: main
   manager: conda
   dependencies:
   - __glibc >=2.17,<3.0.a0
@@ -11215,14 +14849,64 @@
   arch: x86_64
   subdir: osx-64
   build_number: 12
   license: Apache-2.0
   license_family: Apache
   size: 27223934
   timestamp: 1711060050133
+- platform: osx-arm64
+  name: libopencv
+  version: 4.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - ffmpeg >=6.1.1,<7.0a0
+  - freetype >=2.12.1,<3.0a0
+  - gettext >=0.21.1,<1.0a0
+  - harfbuzz >=8.3.0,<9.0a0
+  - hdf5 >=1.14.3,<1.14.4.0a0
+  - jasper >=4.2.2,<5.0a0
+  - libcblas >=3.9.0,<4.0a0
+  - libcxx >=16
+  - libglib >=2.80.0,<3.0a0
+  - libiconv >=1.17,<2.0a0
+  - libjpeg-turbo >=3.0.0,<4.0a0
+  - liblapack >=3.9.0,<4.0a0
+  - liblapacke >=3.9.0,<4.0a0
+  - libopenvino >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-arm-cpu-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-auto-batch-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-auto-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-hetero-plugin >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-ir-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-onnx-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-paddle-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-pytorch-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-tensorflow-frontend >=2024.0.0,<2024.0.1.0a0
+  - libopenvino-tensorflow-lite-frontend >=2024.0.0,<2024.0.1.0a0
+  - libpng >=1.6.43,<1.7.0a0
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  - libtiff >=4.6.0,<4.7.0a0
+  - libwebp-base >=1.3.2,<2.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - numpy >=1.22.4,<2.0a0
+  - openexr >=3.2.2,<3.3.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopencv-4.9.0-headless_py310hed2a8a7_12.conda
+  hash:
+    md5: a27c35c97b5f373e70d34e7fe60ba182
+    sha256: 7cd9456f82ea59a3f42e81627e1a263553211c9b1edb10154d260edb0fd53fc0
+  build: headless_py310hed2a8a7_12
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 12
+  license: Apache-2.0
+  license_family: Apache
+  size: 16801283
+  timestamp: 1711059956757
 - platform: win-64
   name: libopencv
   version: 4.8.1
   category: main
   manager: conda
   dependencies:
   - ffmpeg >=6.0.0,<7.0a0
@@ -11304,14 +14988,34 @@
     sha256: 41f6bee366ed444d96414a8c2b2f973907c3d174aa221495a212e24808cbf477
   build: hcdf21a5_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 3968556
   timestamp: 1712673697018
+- platform: osx-arm64
+  name: libopenvino
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - pugixml >=1.14,<1.15.0a0
+  - tbb >=2021.11.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-2024.0.0-h200475e_5.conda
+  hash:
+    md5: ddc93f2550998187cd23f00386c6a220
+    sha256: 76d61013cfcc4f2d36c9e28d4465c3721b005fcbc2a5bc6404755bfe71573694
+  build: h200475e_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 3667136
+  timestamp: 1712671410901
 - platform: win-64
   name: libopenvino
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - pugixml >=1.14,<1.15.0a0
@@ -11325,14 +15029,35 @@
     sha256: 8bf31207b1102f0601074e31758220f64c0433caca822f3a7618c7ed99b6c476
   build: h63175ca_2
   arch: x86_64
   subdir: win-64
   build_number: 2
   size: 4115329
   timestamp: 1699599686055
+- platform: osx-arm64
+  name: libopenvino-arm-cpu-plugin
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - pugixml >=1.14,<1.15.0a0
+  - tbb >=2021.11.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-arm-cpu-plugin-2024.0.0-h200475e_5.conda
+  hash:
+    md5: 8ea9b802fdac0a53a4dab2cde18dd45a
+    sha256: a1e2575c386bfc04e8febaf90d031e19db22eabd9ee37a8a1c26086daff2faae
+  build: h200475e_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 5914197
+  timestamp: 1712671469472
 - platform: linux-64
   name: libopenvino-auto-batch-plugin
   version: 2024.0.0
   category: main
   manager: conda
   dependencies:
   - __glibc >=2.17,<3.0.a0
@@ -11366,14 +15091,34 @@
     sha256: 7eefd4faf2e8fbc300a716e6a4199774c5aa8a58c6be2c5d1ee05978371160d5
   build: hb622c4e_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 103908
   timestamp: 1712673767712
+- platform: osx-arm64
+  name: libopenvino-auto-batch-plugin
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - tbb >=2021.11.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-auto-batch-plugin-2024.0.0-hfaea8b3_5.conda
+  hash:
+    md5: cced16c374da830c30de83586dc56f83
+    sha256: 1331f46bbb021c17dedc2a22037549356a7a6f0e32d5b2b0fd907ab474acd5f3
+  build: hfaea8b3_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 102182
+  timestamp: 1712671541106
 - platform: win-64
   name: libopenvino-auto-batch-plugin
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11427,14 +15172,34 @@
     sha256: 231203fb517fe8b08e43f711a4ff2414ba12b15d6f3f43c166c62f78ef4af7a3
   build: hb622c4e_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 205572
   timestamp: 1712673810329
+- platform: osx-arm64
+  name: libopenvino-auto-plugin
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - tbb >=2021.11.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-auto-plugin-2024.0.0-hfaea8b3_5.conda
+  hash:
+    md5: 1affc4342a238127b4e52f5366c161c8
+    sha256: 31ed2b61a68254d607288280ba5fff4fe39e40106f0d500ce503c22191be5f62
+  build: hfaea8b3_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 199377
+  timestamp: 1712671578810
 - platform: win-64
   name: libopenvino-auto-plugin
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11489,14 +15254,34 @@
     sha256: 61ded9a801ba7af6e084e6d86a239cb4ce1dcd8e46698c02cd5938e8953dde02
   build: h321ab60_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 167879
   timestamp: 1712673850284
+- platform: osx-arm64
+  name: libopenvino-hetero-plugin
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - pugixml >=1.14,<1.15.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-hetero-plugin-2024.0.0-hc7e6747_5.conda
+  hash:
+    md5: 91b55825deed0aed37849e4804e591b6
+    sha256: fb593663da52d2f0b8b52b2dd0bfd02c910c7ec55847810c4e86430d1250e5fd
+  build: hc7e6747_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 160337
+  timestamp: 1712671618285
 - platform: win-64
   name: libopenvino-hetero-plugin
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11662,14 +15447,34 @@
     sha256: e06946ba10160c5cf9c1a0e8ed1e5a2c72ba769aa208bb8c2d65139c0d7a3c0b
   build: h321ab60_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 178557
   timestamp: 1712673995491
+- platform: osx-arm64
+  name: libopenvino-ir-frontend
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - pugixml >=1.14,<1.15.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-ir-frontend-2024.0.0-hc7e6747_5.conda
+  hash:
+    md5: ee068fe8f4447046729d5f55e3523eb7
+    sha256: 17ce0aa165acda50d8b5081ba798c7b80973d370793d72a5ef85800c85328b2d
+  build: hc7e6747_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 170420
+  timestamp: 1712671655665
 - platform: win-64
   name: libopenvino-ir-frontend
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11724,14 +15529,34 @@
     sha256: 84b69cc1335cb4024039d9fe8883e166f3a74fa083ae582ae7921e4ab9442e3e
   build: hb2e0ddf_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 1266299
   timestamp: 1712674054702
+- platform: osx-arm64
+  name: libopenvino-onnx-frontend
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-onnx-frontend-2024.0.0-h25b35cd_5.conda
+  hash:
+    md5: 98933b62ed1ff14584fa373843922226
+    sha256: 54df073224fafd53aab49d4a4966f19d0b9759e5cc07f2c8a505f0b4825eecde
+  build: h25b35cd_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 1198819
+  timestamp: 1712671712616
 - platform: win-64
   name: libopenvino-onnx-frontend
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11785,14 +15610,34 @@
     sha256: 9078239135b0bd7f9f91f19dbbd50442497affb32e492013c9c0b72a9120ed49
   build: hb2e0ddf_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 427333
   timestamp: 1712674101191
+- platform: osx-arm64
+  name: libopenvino-paddle-frontend
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-paddle-frontend-2024.0.0-h25b35cd_5.conda
+  hash:
+    md5: d23ceb8301d70ec7e88bd0a98d00551d
+    sha256: c602a48a3048aa1ebf39b971a3b781a568b65ebabef2795855bcda13eab22ab9
+  build: h25b35cd_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 414860
+  timestamp: 1712671756869
 - platform: win-64
   name: libopenvino-paddle-frontend
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11844,14 +15689,33 @@
     sha256: 52da43e15dc40a6431acc8866d41630da14b05a91b5994f74490eff9db61366d
   build: ha0df490_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 761234
   timestamp: 1712674144034
+- platform: osx-arm64
+  name: libopenvino-pytorch-frontend
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-pytorch-frontend-2024.0.0-h3f3aa29_5.conda
+  hash:
+    md5: 47ad5a2082f96eb6c2907cf2cb2fec1a
+    sha256: 350fbd4e97ff8fbd05621f407ec63379db9af1f684041c780ab0efb6ff620533
+  build: h3f3aa29_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 731152
+  timestamp: 1712671796738
 - platform: win-64
   name: libopenvino-pytorch-frontend
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11911,14 +15775,37 @@
     sha256: a0558bb6f9af48de03ef0284f40a599571781a56880bbf42a0b2372b030d088d
   build: h70945bb_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 935580
   timestamp: 1712674220872
+- platform: osx-arm64
+  name: libopenvino-tensorflow-frontend
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libabseil * cxx17*
+  - libabseil >=20240116.1,<20240117.0a0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  - snappy >=1.2.0,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-tensorflow-frontend-2024.0.0-hbc2fe69_5.conda
+  hash:
+    md5: 1094e5981c128afd3fe8f71cfd7fc2ab
+    sha256: 0b9c42f084c2905e596f4ffcb2c1a4e295e30bd06d945625c68711889000ac14
+  build: hbc2fe69_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 881993
+  timestamp: 1712671871242
 - platform: win-64
   name: libopenvino-tensorflow-frontend
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -11971,14 +15858,33 @@
     sha256: 864be4bbf2ce40df31dca6f09fea7715896724f0bfebb255c4ad2dd957c2cb7a
   build: ha0df490_5
   arch: x86_64
   subdir: osx-64
   build_number: 5
   size: 376916
   timestamp: 1712674261940
+- platform: osx-arm64
+  name: libopenvino-tensorflow-lite-frontend
+  version: 2024.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libopenvino 2024.0.0 h200475e_5
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopenvino-tensorflow-lite-frontend-2024.0.0-h3f3aa29_5.conda
+  hash:
+    md5: ecb01a392bb579fed43a6c50a9e12b3b
+    sha256: dbbc7f6c3c29a8f9b28b7358dba24041744d64bf56bf7d1642e7bfb286152f5e
+  build: h3f3aa29_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  size: 374882
+  timestamp: 1712671910235
 - platform: win-64
   name: libopenvino-tensorflow-lite-frontend
   version: 2023.1.0
   category: main
   manager: conda
   dependencies:
   - libopenvino 2023.1.0 h63175ca_2
@@ -12028,14 +15934,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 279983
   timestamp: 1606823633642
+- platform: osx-arm64
+  name: libopus
+  version: 1.3.1
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libopus-1.3.1-h27ca646_1.tar.bz2
+  hash:
+    md5: 3d0dbee0ccd2f6d6781d270313627b62
+    sha256: e9912101a58cbc609a1917c5289f3bd1f600c82ed3a1c90a6dd4ca02df77958a
+  build: h27ca646_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 252854
+  timestamp: 1606823635137
 - platform: win-64
   name: libopus
   version: 1.3.1
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15.0a0
@@ -12054,54 +15978,78 @@
   timestamp: 1606824019288
 - platform: linux-64
   name: libparquet
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
-  - libarrow 15.0.2 he70291f_3_cpu
+  - gflags >=2.2.2,<2.3.0a0
+  - libarrow 15.0.2 h07fc4ce_5_cpu
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - libthrift >=0.19.0,<0.19.1.0a0
   - openssl >=3.2.1,<4.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libparquet-15.0.2-h6a7eafb_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libparquet-15.0.2-hacf5a1f_5_cpu.conda
   hash:
-    md5: d2827e2cf2df4f74f9c76417f559ca46
-    sha256: a37a1416f3ae147a821e8144bda8b0ae31def625b0fdb848952e4f491366f375
-  build: h6a7eafb_3_cpu
+    md5: cbce89f741a51701b99d9017031a38b1
+    sha256: a82142bd9e9dad278a669968ff945d8cb0a080cd52d7f24bd649e565f9f0a491
+  build: hacf5a1f_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 1179560
-  timestamp: 1712756464081
+  size: 1182912
+  timestamp: 1713845996554
 - platform: osx-64
   name: libparquet
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - libarrow 15.0.2 h965e444_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
   - libcxx >=16
   - libthrift >=0.19.0,<0.19.1.0a0
   - openssl >=3.2.1,<4.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libparquet-15.0.2-h7cd3cfe_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libparquet-15.0.2-h7cd3cfe_5_cpu.conda
   hash:
-    md5: 72f92d2ee538cb24f5d8c1870d96cf66
-    sha256: 9b9144697ef4637a0f164c9acb1be5297bedc4d86ad9ae97b97eaec872447104
-  build: h7cd3cfe_3_cpu
+    md5: 4fcb980d97729c23a6d2c23974c9166c
+    sha256: 4c9a64016e7480f7fe030a8d5f6c3c8c736369dbfe95e7710dd7f4a9b3b3f918
+  build: h7cd3cfe_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
   license: Apache-2.0
   license_family: APACHE
-  size: 921797
-  timestamp: 1712758165813
+  size: 923934
+  timestamp: 1713848079818
+- platform: osx-arm64
+  name: libparquet
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libcxx >=16
+  - libthrift >=0.19.0,<0.19.1.0a0
+  - openssl >=3.2.1,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libparquet-15.0.2-h5304c63_5_cpu.conda
+  hash:
+    md5: 47ccaf16a7471288c1fe837690bf6880
+    sha256: 2d3afce7c6e0258e5c7c7f70ff5db20b9e886fb8695a75401dd481e431bee8af
+  build: h5304c63_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  license: Apache-2.0
+  license_family: APACHE
+  size: 864792
+  timestamp: 1713848721427
 - platform: win-64
   name: libparquet
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libarrow 15.0.0 he5f67d5_0_cpu
@@ -12174,14 +16122,32 @@
   build: h92b6c6a_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: zlib-acknowledgement
   size: 268524
   timestamp: 1708780496420
+- platform: osx-arm64
+  name: libpng
+  version: 1.6.43
+  category: main
+  manager: conda
+  dependencies:
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libpng-1.6.43-h091b4b1_0.conda
+  hash:
+    md5: 77e684ca58d82cae9deebafb95b1a2b8
+    sha256: 66c4713b07408398f2221229a1c1d5df57d65dc0902258113f2d9ecac4772495
+  build: h091b4b1_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: zlib-acknowledgement
+  size: 264177
+  timestamp: 1708780447187
 - platform: win-64
   name: libpng
   version: 1.6.43
   category: main
   manager: conda
   dependencies:
   - libzlib >=1.2.13,<1.3.0a0
@@ -12261,14 +16227,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 2216001
   timestamp: 1709514908146
+- platform: osx-arm64
+  name: libprotobuf
+  version: 4.25.3
+  category: main
+  manager: conda
+  dependencies:
+  - libabseil * cxx17*
+  - libabseil >=20240116.1,<20240117.0a0
+  - libcxx >=16
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libprotobuf-4.25.3-hbfab5d5_0.conda
+  hash:
+    md5: 5f70b2b945a9741cba7e6dfe735a02a7
+    sha256: d754519abc3ddbdedab2a38d0639170f5347c1573eef80c707f3a8dc5dff706a
+  build: hbfab5d5_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 2154402
+  timestamp: 1709514097574
 - platform: win-64
   name: libprotobuf
   version: 4.24.4
   category: main
   manager: conda
   dependencies:
   - libabseil * cxx17*
@@ -12333,14 +16321,37 @@
   build_number: 2
   constrains:
   - re2 2023.09.01.*
   license: BSD-3-Clause
   license_family: BSD
   size: 184017
   timestamp: 1708947106275
+- platform: osx-arm64
+  name: libre2-11
+  version: 2023.09.01
+  category: main
+  manager: conda
+  dependencies:
+  - libabseil * cxx17*
+  - libabseil >=20240116.1,<20240117.0a0
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libre2-11-2023.09.01-h7b2c953_2.conda
+  hash:
+    md5: 0b7b2ced046d6b5fe6e9d46b1ee0324c
+    sha256: c8a0a6e7a627dc9c66ffb8858f8f6d499f67fd269b6636b25dc5169760610f05
+  build: h7b2c953_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  constrains:
+  - re2 2023.09.01.*
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 171443
+  timestamp: 1708947163461
 - platform: win-64
   name: libre2-11
   version: 2023.09.01
   category: main
   manager: conda
   dependencies:
   - libabseil * cxx17*
@@ -12365,26 +16376,26 @@
 - platform: linux-64
   name: libsanitizer
   version: 13.2.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=13.2.0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libsanitizer-13.2.0-h7e041cc_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libsanitizer-13.2.0-h95c4c6d_6.conda
   hash:
-    md5: 3f686300a92604d1bdff9a29dd4a6639
-    sha256: 97ecdab7e4e96400d712c2d6ba2b7c30a97278e9f4470ea0ff36bf4f1447b3b9
-  build: h7e041cc_5
+    md5: be66a394ae0eb4bbeba5bba54e83ce53
+    sha256: 7dfe018f816e424692a322aef993096061e28e13ad7e1c19b35c9e16f69c6bb0
+  build: h95c4c6d_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 4114208
-  timestamp: 1706819228913
+  size: 4139988
+  timestamp: 1713755043582
 - platform: linux-64
   name: libsndfile
   version: 1.2.2
   category: main
   manager: conda
   dependencies:
   - lame >=3.100,<3.101.0a0
@@ -12405,69 +16416,87 @@
   build_number: 1
   license: LGPL-2.1-or-later
   license_family: LGPL
   size: 354372
   timestamp: 1695747735668
 - platform: linux-64
   name: libsqlite
-  version: 3.45.2
+  version: 3.45.3
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
   hash:
-    md5: 866983a220e27a80cb75e85cb30466a1
-    sha256: 8cdbeb7902729e319510a82d7c642402981818702b58812af265ef55d1315473
+    md5: b3316cbe90249da4f8e84cd66e1cc55b
+    sha256: e2273d6860eadcf714a759ffb6dc24a69cfd01f2a0ea9d6c20f86049b9334e0c
   build: h2797004_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: Unlicense
-  size: 857489
-  timestamp: 1710254744982
+  size: 859858
+  timestamp: 1713367435849
 - platform: osx-64
   name: libsqlite
-  version: 3.45.2
+  version: 3.45.3
   category: main
   manager: conda
   dependencies:
   - libzlib >=1.2.13,<1.3.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
   hash:
-    md5: 086f56e13a96a6cfb1bf640505ae6b70
-    sha256: 320ec73a4e3dd377757a2595770b8137ec4583df4d7782472d76377cdbdc4543
+    md5: 68e462226209f35182ef66eda0f794ff
+    sha256: 4d44b68fb29dcbc2216a8cae0b274b02ef9b4ae05d1d0f785362ed30b91c9b52
   build: h92b6c6a_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Unlicense
-  size: 902355
-  timestamp: 1710254991672
+  size: 902546
+  timestamp: 1713367776445
+- platform: osx-arm64
+  name: libsqlite
+  version: 3.45.3
+  category: main
+  manager: conda
+  dependencies:
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
+  hash:
+    md5: c8c1186c7f3351f6ffddb97b1f54fc58
+    sha256: 4337f466eb55bbdc74e168b52ec8c38f598e3664244ec7a2536009036e2066cc
+  build: h091b4b1_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Unlicense
+  size: 824794
+  timestamp: 1713367748819
 - platform: win-64
   name: libsqlite
-  version: 3.45.2
+  version: 3.45.3
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
-  url: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
   hash:
-    md5: f95359f8dc5abf7da7776ece9ef10bc5
-    sha256: 4bb24b986550275a6d02835150d943c4c675808d05c0efc5c2a22154d007a69f
+    md5: 73f5dc8e2d55d9a1e14b11f49c3b4a28
+    sha256: 06ec75faa51d7ec6d5db98889e869b579a9df19d7d3d9baff8359627da4a3b7e
   build: hcfcfb64_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: Unlicense
-  size: 869606
-  timestamp: 1710255095740
+  size: 870518
+  timestamp: 1713367888406
 - platform: linux-64
   name: libssh2
   version: 1.11.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -12501,14 +16530,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 259556
   timestamp: 1685837820566
+- platform: osx-arm64
+  name: libssh2
+  version: 1.11.0
+  category: main
+  manager: conda
+  dependencies:
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.1.1,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libssh2-1.11.0-h7a5bd25_0.conda
+  hash:
+    md5: 029f7dc931a3b626b94823bc77830b01
+    sha256: bb57d0c53289721fff1eeb3103a1c6a988178e88d8a8f4345b0b91a35f0e0015
+  build: h7a5bd25_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 255610
+  timestamp: 1685837894256
 - platform: win-64
   name: libssh2
   version: 1.11.0
   category: main
   manager: conda
   dependencies:
   - libzlib >=1.2.13,<1.3.0a0
@@ -12530,45 +16579,45 @@
   timestamp: 1685838242099
 - platform: linux-64
   name: libstdcxx-devel_linux-64
   version: 13.2.0
   category: main
   manager: conda
   dependencies: []
-  url: https://conda.anaconda.org/conda-forge/noarch/libstdcxx-devel_linux-64-13.2.0-ha9c7c90_105.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/libstdcxx-devel_linux-64-13.2.0-h95c4c6d_106.conda
   hash:
-    md5: 66383205c2e1bdf013df52fa9e3e6763
-    sha256: 67e999ee56481844ca4ce2e61132c5c16f3f00a05daa1d0ea4b2c684eea5de5a
-  build: ha9c7c90_105
+    md5: aa932bbdb9cfea51e675f4b5a242ed6f
+    sha256: bb44a66fe3fd5ef35f44d8155edd3d5e18ed8b5154e30d2340aa79a3c77e86e3
+  build: h95c4c6d_106
   arch: x86_64
   subdir: linux-64
-  build_number: 105
+  build_number: 106
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
   noarch: generic
-  size: 13020920
-  timestamp: 1706819128553
+  size: 13096506
+  timestamp: 1713754936901
 - platform: linux-64
   name: libstdcxx-ng
   version: 13.2.0
   category: main
   manager: conda
   dependencies: []
-  url: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda
   hash:
-    md5: f6f6600d18a4047b54f803cf708b868a
-    sha256: a56c5b11f1e73a86e120e6141a42d9e935a99a2098491ac9e15347a1476ce777
-  build: h7e041cc_5
+    md5: 3cfab3e709f77e9f1b3d380eb622494a
+    sha256: 2616dbf9d28431eea20b6e307145c6a92ea0328a047c725ff34b0316de2617da
+  build: h95c4c6d_6
   arch: x86_64
   subdir: linux-64
-  build_number: 5
+  build_number: 6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  size: 3834139
-  timestamp: 1706819252496
+  size: 3842900
+  timestamp: 1713755068572
 - platform: linux-64
   name: libsystemd0
   version: '255'
   category: main
   manager: conda
   dependencies:
   - __glibc >=2.17,<3.0.a0
@@ -12622,14 +16671,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: GPL-3.0-or-later
   license_family: GPL
   size: 118785
   timestamp: 1661325967954
+- platform: osx-arm64
+  name: libtasn1
+  version: 4.19.0
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libtasn1-4.19.0-h1a8c8d9_0.tar.bz2
+  hash:
+    md5: c35bc17c31579789c76739486fc6d27a
+    sha256: 912e96644ea22b49921c71c9c94bcdd2b6463e9313da895c2fcee298a8c0e44c
+  build: h1a8c8d9_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: GPL-3.0-or-later
+  license_family: GPL
+  size: 116745
+  timestamp: 1661325945767
 - platform: linux-64
   name: libthrift
   version: 0.19.0
   category: main
   manager: conda
   dependencies:
   - libevent >=2.1.12,<2.1.13.0a0
@@ -12667,14 +16734,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: Apache-2.0
   license_family: APACHE
   size: 325415
   timestamp: 1695958330036
+- platform: osx-arm64
+  name: libthrift
+  version: 0.19.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=15.0.7
+  - libevent >=2.1.12,<2.1.13.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.1.3,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libthrift-0.19.0-h026a170_1.conda
+  hash:
+    md5: 4b8b21eb00d9019e9fa351141da2a6ac
+    sha256: b2c1b30d36f0412c0c0313db76a0236d736f3a9b887b8ed16182f531e4b7cb80
+  build: h026a170_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: Apache-2.0
+  license_family: APACHE
+  size: 331154
+  timestamp: 1695958512679
 - platform: win-64
   name: libthrift
   version: 0.19.0
   category: main
   manager: conda
   dependencies:
   - libevent >=2.1.12,<2.1.13.0a0
@@ -12742,14 +16831,39 @@
   build: h129831d_3
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: HPND
   size: 257489
   timestamp: 1711218113053
+- platform: osx-arm64
+  name: libtiff
+  version: 4.6.0
+  category: main
+  manager: conda
+  dependencies:
+  - lerc >=4.0.0,<5.0a0
+  - libcxx >=16
+  - libdeflate >=1.20,<1.21.0a0
+  - libjpeg-turbo >=3.0.0,<4.0a0
+  - libwebp-base >=1.3.2,<2.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - xz >=5.2.6,<6.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libtiff-4.6.0-h07db509_3.conda
+  hash:
+    md5: 28c9f8c6dd75666dfb296aea06c49cb8
+    sha256: 6df3e129682f6dc43826e5028e1807624b2a7634c4becbb50e56be9f77167f25
+  build: h07db509_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: HPND
+  size: 238349
+  timestamp: 1711218119201
 - platform: win-64
   name: libtiff
   version: 4.6.0
   category: main
   manager: conda
   dependencies:
   - lerc >=4.0.0,<5.0a0
@@ -12803,14 +16917,31 @@
   build: h0d85af4_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: GPL-3.0-only OR LGPL-3.0-only
   size: 1392865
   timestamp: 1626955817826
+- platform: osx-arm64
+  name: libunistring
+  version: 0.9.10
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libunistring-0.9.10-h3422bc3_0.tar.bz2
+  hash:
+    md5: d88e77a4861e20bd96bde6628ee7a5ae
+    sha256: a1afe12ab199f82f339eae83405d293d197f2485d45346a709703bc7e8299949
+  build: h3422bc3_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: GPL-3.0-only OR LGPL-3.0-only
+  size: 1577561
+  timestamp: 1626955172521
 - platform: linux-64
   name: libutf8proc
   version: 2.8.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -12840,14 +16971,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 98942
   timestamp: 1667316472080
+- platform: osx-arm64
+  name: libutf8proc
+  version: 2.8.0
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libutf8proc-2.8.0-h1a8c8d9_0.tar.bz2
+  hash:
+    md5: f8c9c41a122ab3abdf8943b13f4957ee
+    sha256: a3faddac08efd930fa3a1cc254b5053b4ed9428c49a888d437bf084d403c931a
+  build: h1a8c8d9_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 103492
+  timestamp: 1667316405233
 - platform: win-64
   name: libutf8proc
   version: 2.8.0
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -12983,14 +17132,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 1294811
   timestamp: 1707175761017
+- platform: osx-arm64
+  name: libvpx
+  version: 1.14.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libvpx-1.14.0-h078ce10_0.conda
+  hash:
+    md5: 8a515c7875e4d61734f4ac964851f4a5
+    sha256: e202f23fca763d88ad8170f90fa380510c65f29b86cfe6fb29706843462cee4f
+  build: h078ce10_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 1174097
+  timestamp: 1707175717608
 - platform: linux-64
   name: libwebp-base
   version: 1.4.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -13024,14 +17192,34 @@
   build_number: 0
   constrains:
   - libwebp 1.4.0
   license: BSD-3-Clause
   license_family: BSD
   size: 355099
   timestamp: 1713200298965
+- platform: osx-arm64
+  name: libwebp-base
+  version: 1.4.0
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libwebp-base-1.4.0-h93a5062_0.conda
+  hash:
+    md5: c0af0edfebe780b19940e94871f1a765
+    sha256: 0d4bad713a512d79bfeb4d61821f447afab8b0792aca823f505ce6b195e9fde5
+  build: h93a5062_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - libwebp 1.4.0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 287750
+  timestamp: 1713200194013
 - platform: win-64
   name: libwebp-base
   version: 1.4.0
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -13090,14 +17278,35 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 313793
   timestamp: 1682083036825
+- platform: osx-arm64
+  name: libxcb
+  version: '1.15'
+  category: main
+  manager: conda
+  dependencies:
+  - pthread-stubs
+  - xorg-libxau
+  - xorg-libxdmcp
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libxcb-1.15-hf346824_0.conda
+  hash:
+    md5: 988d5f86ab60fa6de91b3ee3a88a3af9
+    sha256: 6eaa87760ff3e91bb5524189700139db46f8946ff6331f4e571e4a9356edbb0d
+  build: hf346824_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 334770
+  timestamp: 1682082734262
 - platform: win-64
   name: libxcb
   version: '1.15'
   category: main
   manager: conda
   dependencies:
   - m2w64-gcc-libs
@@ -13166,71 +17375,93 @@
   manager: conda
   dependencies:
   - icu >=73.2,<74.0a0
   - libgcc-ng >=12
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - xz >=5.2.6,<6.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.12.6-h232c23b_2.conda
   hash:
-    md5: 6853448e9ca1cfd5f15382afd2a6d123
-    sha256: c0bd693bb1a7e5aba388a0c79be16ff92e2411e03aaa920f94b4b33bf099e254
-  build: h232c23b_1
+    md5: 9a3a42df8a95f65334dfc7b80da1195d
+    sha256: 0fd41df7211aae04f492c8550ce10238e8cfa8b1abebc2215a983c5e66d284ea
+  build: h232c23b_2
   arch: x86_64
   subdir: linux-64
-  build_number: 1
+  build_number: 2
   license: MIT
   license_family: MIT
-  size: 705994
-  timestamp: 1711318087106
+  size: 704938
+  timestamp: 1713314718258
 - platform: osx-64
   name: libxml2
   version: 2.12.6
   category: main
   manager: conda
   dependencies:
   - icu >=73.2,<74.0a0
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - xz >=5.2.6,<6.0a0
-  url: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda
   hash:
-    md5: bd85e0ca9e1ffaadc3b56079fd956035
-    sha256: 07a5dc7316d4c1ff3d924df6a76e6a13380d702fa5b3b1889e56d0672e5b8201
-  build: hc0ae0f7_1
+    md5: 50b997370584f2c83ca0c38e9028eab9
+    sha256: 2598a525b1769338f96c3d4badad7d8b95c9ddcea86db3f9479a274803190e5c
+  build: hc0ae0f7_2
   arch: x86_64
   subdir: osx-64
-  build_number: 1
+  build_number: 2
   license: MIT
   license_family: MIT
-  size: 620164
-  timestamp: 1711318305209
+  size: 619622
+  timestamp: 1713314870641
+- platform: osx-arm64
+  name: libxml2
+  version: 2.12.6
+  category: main
+  manager: conda
+  dependencies:
+  - icu >=73.2,<74.0a0
+  - libiconv >=1.17,<2.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - xz >=5.2.6,<6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libxml2-2.12.6-h0d0cfa8_2.conda
+  hash:
+    md5: 27577d561de7659487b062c363d8a527
+    sha256: a5c10af641d6accf3effb3c3a3c594d931bb374f9e3e796719f3ecf769cfb0fc
+  build: h0d0cfa8_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: MIT
+  license_family: MIT
+  size: 588638
+  timestamp: 1713314780561
 - platform: win-64
   name: libxml2
   version: 2.12.6
   category: main
   manager: conda
   dependencies:
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
-  url: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_1.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-hc3477c8_2.conda
   hash:
-    md5: eb9f59dd51f50f5aa369813fa63ba569
-    sha256: 1846c1318a5987e7315ca3648b55b38e5cfd9853370803a0f5159bc0071609c1
-  build: hc3477c8_1
+    md5: ac7af7a949db01dae61ddc48f4a93d79
+    sha256: 9a717cad6da52c84cfc490f7d52203c4cbc9e0e0389941fc6523273be5ccd17a
+  build: hc3477c8_2
   arch: x86_64
   subdir: win-64
-  build_number: 1
+  build_number: 2
   license: MIT
   license_family: MIT
-  size: 1640801
-  timestamp: 1711318467301
+  size: 1589904
+  timestamp: 1713315104803
 - platform: linux-64
   name: libzlib
   version: 1.2.13
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -13264,14 +17495,34 @@
   build_number: 5
   constrains:
   - zlib 1.2.13 *_5
   license: Zlib
   license_family: Other
   size: 59404
   timestamp: 1686575566695
+- platform: osx-arm64
+  name: libzlib
+  version: 1.2.13
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+  hash:
+    md5: 1a47f5236db2e06a320ffa0392f81bd8
+    sha256: ab1c8aefa2d54322a63aaeeefe9cf877411851738616c4068e0dccc66b9c758a
+  build: h53f4e23_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  constrains:
+  - zlib 1.2.13 *_5
+  license: Zlib
+  license_family: Other
+  size: 48102
+  timestamp: 1686575426584
 - platform: win-64
   name: libzlib
   version: 1.2.13
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -13326,14 +17577,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 162262
   timestamp: 1607309210977
+- platform: osx-arm64
+  name: libzopfli
+  version: 1.0.3
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=11.0.0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libzopfli-1.0.3-h9f76cd9_0.tar.bz2
+  hash:
+    md5: a0758d74f57741aa0d9ede13fd592e56
+    sha256: e3003b8efe551902dc60b21c81d7164b291b26b7862704421368d26ba5c10fa0
+  build: h9f76cd9_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 147901
+  timestamp: 1607309166373
 - platform: win-64
   name: libzopfli
   version: 1.0.3
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15.0a0
@@ -13392,14 +17662,37 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 24035
   timestamp: 1707129321841
   purls:
   - pkg:pypi/linkify-it-py
+- platform: osx-arm64
+  name: linkify-it-py
+  version: 2.0.3
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  - uc-micro-py
+  url: https://conda.anaconda.org/conda-forge/noarch/linkify-it-py-2.0.3-pyhd8ed1ab_0.conda
+  hash:
+    md5: f1b64ca4faf563605cf6f6ca93f9ff3f
+    sha256: aa99d44e8c83865026575a8af253141c53e0b3ab05f053befaa7757c8525064f
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 24035
+  timestamp: 1707129321841
+  purls:
+  - pkg:pypi/linkify-it-py
 - platform: win-64
   name: linkify-it-py
   version: 2.0.3
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -13435,14 +17728,34 @@
   build_number: 0
   constrains:
   - openmp 18.1.3|18.1.3.*
   license: Apache-2.0 WITH LLVM-exception
   license_family: APACHE
   size: 300597
   timestamp: 1712603382363
+- platform: osx-arm64
+  name: llvm-openmp
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/llvm-openmp-18.1.3-hcd81f8e_0.conda
+  hash:
+    md5: 24cbf1fb1b83056f8ba1beaac0619bf8
+    sha256: 4cb4eadd633669496ed70c580c965f5f2ed29336890636c61a53e9c1c1541073
+  build: hcd81f8e_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - openmp 18.1.3|18.1.3.*
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: APACHE
+  size: 276320
+  timestamp: 1712603367897
 - platform: osx-64
   name: llvm-tools
   version: 18.1.3
   category: main
   manager: conda
   dependencies:
   - libllvm18 18.1.3 hbcf5fad_0
@@ -13462,14 +17775,41 @@
   - llvmdev     18.1.3
   - llvm        18.1.3
   - clang       18.1.3
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 24449337
   timestamp: 1712518244229
+- platform: osx-arm64
+  name: llvm-tools
+  version: 18.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - libllvm18 18.1.3 h30cc82d_0
+  - libxml2 >=2.12.6,<3.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/llvm-tools-18.1.3-h30cc82d_0.conda
+  hash:
+    md5: 505aef673d805f9efe0c61954a6a99d0
+    sha256: 48eb7b17ca6de1b43dfddc3b4a629a8a9764c9da3f3012980e1b917c71f06a4f
+  build: h30cc82d_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - llvm        18.1.3
+  - clang-tools 18.1.3
+  - clang       18.1.3
+  - llvmdev     18.1.3
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
+  size: 23023681
+  timestamp: 1712517958538
 - platform: linux-64
   name: locket
   version: 1.0.0
   category: main
   manager: conda
   dependencies:
   - python >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
@@ -13506,14 +17846,36 @@
   license: BSD-2-Clause
   license_family: BSD
   noarch: python
   size: 8250
   timestamp: 1650660473123
   purls:
   - pkg:pypi/locket
+- platform: osx-arm64
+  name: locket
+  version: 1.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+  url: https://conda.anaconda.org/conda-forge/noarch/locket-1.0.0-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 91e27ef3d05cc772ce627e51cff111c4
+    sha256: 9afe0b5cfa418e8bdb30d8917c5a6cec10372b037924916f1f85b9f4899a67a6
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  noarch: python
+  size: 8250
+  timestamp: 1650660473123
+  purls:
+  - pkg:pypi/locket
 - platform: win-64
   name: locket
   version: 1.0.0
   category: main
   manager: conda
   dependencies:
   - python >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
@@ -13575,14 +17937,38 @@
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 34354
   timestamp: 1704831577874
   purls:
   - pkg:pypi/lz4
+- platform: osx-arm64
+  name: lz4
+  version: 4.3.3
+  category: main
+  manager: conda
+  dependencies:
+  - lz4-c >=1.9.3,<1.10.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/lz4-4.3.3-py310haecba8d_0.conda
+  hash:
+    md5: 388a85465bdbaed3bca49f9002634da5
+    sha256: 7acb15a2fc8db187c93fba3a90ec026261e03b6a9f58eaff54d2f63700ecbfb8
+  build: py310haecba8d_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 108122
+  timestamp: 1704831595715
+  purls:
+  - pkg:pypi/lz4
 - platform: win-64
   name: lz4
   version: 4.3.3
   category: main
   manager: conda
   dependencies:
   - lz4-c >=1.9.3,<1.10.0a0
@@ -13640,14 +18026,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   size: 156415
   timestamp: 1674727335352
+- platform: osx-arm64
+  name: lz4-c
+  version: 1.9.4
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=14.0.6
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/lz4-c-1.9.4-hb7217d7_0.conda
+  hash:
+    md5: 45505bec548634f7d05e02fb25262cb9
+    sha256: fc343b8c82efe40819b986e29ba748366514e5ab94a1e1138df195af5f45fa24
+  build: hb7217d7_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 141188
+  timestamp: 1674727268278
 - platform: win-64
   name: lz4-c
   version: 1.9.4
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -13804,14 +18209,37 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 64356
   timestamp: 1686175179621
   purls:
   - pkg:pypi/markdown-it-py
+- platform: osx-arm64
+  name: markdown-it-py
+  version: 3.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - mdurl >=0.1,<1
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 93a8e71256479c62074356ef6ebf501b
+    sha256: c041b0eaf7a6af3344d5dd452815cdc148d6284fec25a4fa3f4263b3a021e962
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 64356
+  timestamp: 1686175179621
+  purls:
+  - pkg:pypi/markdown-it-py
 - platform: win-64
   name: markdown-it-py
   version: 3.0.0
   category: main
   manager: conda
   dependencies:
   - mdurl >=0.1,<1
@@ -13876,14 +18304,39 @@
   - jinja2 >=3.0.0
   license: BSD-3-Clause
   license_family: BSD
   size: 23106
   timestamp: 1706900206202
   purls:
   - pkg:pypi/markupsafe
+- platform: osx-arm64
+  name: markupsafe
+  version: 2.1.5
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/markupsafe-2.1.5-py310hd125d64_0.conda
+  hash:
+    md5: 29a6f644679ed1e2b94fc20c7e3dcc2d
+    sha256: 75a43d7901fadee332b2175c71ba8df0e57ac0d0b2a7c52a10ad0d681cf1dc5a
+  build: py310hd125d64_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - jinja2 >=3.0.0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 23919
+  timestamp: 1706900392293
+  purls:
+  - pkg:pypi/markupsafe
 - platform: win-64
   name: markupsafe
   version: 2.1.5
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -13948,14 +18401,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: PSF-2.0
   license_family: PSF
   size: 8497
   timestamp: 1712606482706
+- platform: osx-arm64
+  name: matplotlib
+  version: 3.8.4
+  category: main
+  manager: conda
+  dependencies:
+  - matplotlib-base >=3.8.4,<3.8.5.0a0
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - tornado >=5
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/matplotlib-3.8.4-py310hb6292c7_0.conda
+  hash:
+    md5: 21409508f096611c3a721c198032cc94
+    sha256: 467ca287a421553d2885b238859084d579410fca8f5a9804ae8a2fb9fd2188df
+  build: py310hb6292c7_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: PSF-2.0
+  license_family: PSF
+  size: 8594
+  timestamp: 1712606667465
 - platform: win-64
   name: matplotlib
   version: 3.8.4
   category: main
   manager: conda
   dependencies:
   - matplotlib-base >=3.8.4,<3.8.5.0a0
@@ -14044,14 +18519,50 @@
   build_number: 0
   license: PSF-2.0
   license_family: PSF
   size: 6908417
   timestamp: 1712606424046
   purls:
   - pkg:pypi/matplotlib
+- platform: osx-arm64
+  name: matplotlib-base
+  version: 3.8.4
+  category: main
+  manager: conda
+  dependencies:
+  - certifi >=2020.06.20
+  - contourpy >=1.0.1
+  - cycler >=0.10
+  - fonttools >=4.22.0
+  - freetype >=2.12.1,<3.0a0
+  - kiwisolver >=1.3.1
+  - libcxx >=16
+  - numpy >=1.21,<2
+  - numpy >=1.22.4,<2.0a0
+  - packaging >=20.0
+  - pillow >=8
+  - pyparsing >=2.3.1
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python-dateutil >=2.7
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/matplotlib-base-3.8.4-py310h2439c42_0.conda
+  hash:
+    md5: 85dbcc76ac05cb6159762d703f344150
+    sha256: 0e8599048873a81f7b4fd56f784403293f264a9980e22cf9b9e8d958949b310a
+  build: py310h2439c42_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: PSF-2.0
+  license_family: PSF
+  size: 6844627
+  timestamp: 1712606596400
+  purls:
+  - pkg:pypi/matplotlib
 - platform: win-64
   name: matplotlib-base
   version: 3.8.4
   category: main
   manager: conda
   dependencies:
   - certifi >=2020.06.20
@@ -14127,14 +18638,37 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 14599
   timestamp: 1713250613726
   purls:
   - pkg:pypi/matplotlib-inline
+- platform: osx-arm64
+  name: matplotlib-inline
+  version: 0.1.7
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  - traitlets
+  url: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+  hash:
+    md5: 779345c95648be40d22aaa89de7d4254
+    sha256: 7ea68676ea35fbb095420bbcc1c82c4767b8be7bb56abb6989b7f89d957a3bab
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 14599
+  timestamp: 1713250613726
+  purls:
+  - pkg:pypi/matplotlib-inline
 - platform: win-64
   name: matplotlib-inline
   version: 0.1.7
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -14194,14 +18728,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 14680
   timestamp: 1704317789138
   purls:
   - pkg:pypi/mdurl
+- platform: osx-arm64
+  name: mdurl
+  version: 0.1.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: 776a8dd9e824f77abac30e6ef43a8f7a
+    sha256: 64073dfb6bb429d52fff30891877b48c7ec0f89625b1bf844905b66a81cce6e1
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 14680
+  timestamp: 1704317789138
+  purls:
+  - pkg:pypi/mdurl
 - platform: win-64
   name: mdurl
   version: 0.1.2
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -14260,14 +18816,36 @@
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 633746
   timestamp: 1710294330259
+- platform: osx-arm64
+  name: meson
+  version: 1.4.0
+  category: main
+  manager: conda
+  dependencies:
+  - ninja >=1.8.2
+  - python >=3.7
+  - setuptools
+  url: https://conda.anaconda.org/conda-forge/noarch/meson-1.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 52a0660cfa40b45bf254ecc3374cb2e0
+    sha256: e4668e6cbc589b82a1481dde6b776ac90ee9ee7aac5d45af347cc943583213b8
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 633746
+  timestamp: 1710294330259
 - platform: win-64
   name: meson
   version: 1.4.0
   category: main
   manager: conda
   dependencies:
   - ninja >=1.8.2
@@ -14284,87 +18862,112 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 633746
   timestamp: 1710294330259
 - platform: linux-64
   name: meson-python
-  version: 0.15.0
+  version: 0.16.0
   category: main
   manager: conda
   dependencies:
-  - colorama
   - meson >=0.63.3
   - ninja
+  - packaging >=19.0
   - pyproject-metadata >=0.7.1
   - python >=3.7
   - tomli >=1.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/meson-python-0.15.0-pyh0c530f3_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/meson-python-0.16.0-pyh0c530f3_0.conda
   hash:
-    md5: 3bc64565ca78ce3bb80248d09926d8f9
-    sha256: 27c4f5132d3697e5bede4179c00d32d07560585d3578d7b8dde4a1e4c5d1a67c
+    md5: e16f0dbf502da873be9f9adb0dc52547
+    sha256: 71377ccefd72c547fe537157d5aeec36b8cc6ed16b15ffea90c59d904b987e24
   build: pyh0c530f3_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 69709
-  timestamp: 1698322017651
+  size: 71369
+  timestamp: 1713362631178
 - platform: osx-64
   name: meson-python
-  version: 0.15.0
+  version: 0.16.0
   category: main
   manager: conda
   dependencies:
-  - colorama
   - meson >=0.63.3
   - ninja
+  - packaging >=19.0
   - pyproject-metadata >=0.7.1
   - python >=3.7
   - tomli >=1.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/meson-python-0.15.0-pyh0c530f3_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/meson-python-0.16.0-pyh0c530f3_0.conda
   hash:
-    md5: 3bc64565ca78ce3bb80248d09926d8f9
-    sha256: 27c4f5132d3697e5bede4179c00d32d07560585d3578d7b8dde4a1e4c5d1a67c
+    md5: e16f0dbf502da873be9f9adb0dc52547
+    sha256: 71377ccefd72c547fe537157d5aeec36b8cc6ed16b15ffea90c59d904b987e24
   build: pyh0c530f3_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 69709
-  timestamp: 1698322017651
+  size: 71369
+  timestamp: 1713362631178
+- platform: osx-arm64
+  name: meson-python
+  version: 0.16.0
+  category: main
+  manager: conda
+  dependencies:
+  - meson >=0.63.3
+  - ninja
+  - packaging >=19.0
+  - pyproject-metadata >=0.7.1
+  - python >=3.7
+  - tomli >=1.0.0
+  url: https://conda.anaconda.org/conda-forge/noarch/meson-python-0.16.0-pyh0c530f3_0.conda
+  hash:
+    md5: e16f0dbf502da873be9f9adb0dc52547
+    sha256: 71377ccefd72c547fe537157d5aeec36b8cc6ed16b15ffea90c59d904b987e24
+  build: pyh0c530f3_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 71369
+  timestamp: 1713362631178
 - platform: win-64
   name: meson-python
-  version: 0.15.0
+  version: 0.16.0
   category: main
   manager: conda
   dependencies:
-  - colorama
   - meson >=0.63.3
   - ninja
+  - packaging >=19.0
   - pyproject-metadata >=0.7.1
   - python >=3.7
   - tomli >=1.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/meson-python-0.15.0-pyh0c530f3_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/meson-python-0.16.0-pyh0c530f3_0.conda
   hash:
-    md5: 3bc64565ca78ce3bb80248d09926d8f9
-    sha256: 27c4f5132d3697e5bede4179c00d32d07560585d3578d7b8dde4a1e4c5d1a67c
+    md5: e16f0dbf502da873be9f9adb0dc52547
+    sha256: 71377ccefd72c547fe537157d5aeec36b8cc6ed16b15ffea90c59d904b987e24
   build: pyh0c530f3_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 69709
-  timestamp: 1698322017651
+  size: 71369
+  timestamp: 1713362631178
 - platform: win-64
   name: mkl
   version: 2024.1.0
   category: main
   manager: conda
   dependencies:
   - intel-openmp 2024.*
@@ -14445,14 +19048,39 @@
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 186894
   timestamp: 1700926844509
   purls:
   - pkg:pypi/msgpack
+- platform: osx-arm64
+  name: msgpack-python
+  version: 1.0.7
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=10.9
+  - libcxx >=16.0.6
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/msgpack-python-1.0.7-py310hd137fd4_0.conda
+  hash:
+    md5: 41c4e1ac2202c508b2d9b8de7e5aebeb
+    sha256: 8d5432cea3db8ad3f2c3bd31dbb037ff986e62a9664f763093d407786d8df269
+  build: py310hd137fd4_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 186753
+  timestamp: 1700926918
+  purls:
+  - pkg:pypi/msgpack
 - platform: win-64
   name: msgpack-python
   version: 1.0.7
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -14526,14 +19154,34 @@
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   noarch: python
   size: 12452
   timestamp: 1600387789153
+- platform: osx-arm64
+  name: munkres
+  version: 1.1.4
+  category: main
+  manager: conda
+  dependencies:
+  - python
+  url: https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2
+  hash:
+    md5: 2ba8498c1018c1e9c61eb99b973dfe19
+    sha256: f86fb22b58e93d04b6f25e0d811b56797689d598788b59dcb47f59045b568306
+  build: pyh9f0ad1d_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  noarch: python
+  size: 12452
+  timestamp: 1600387789153
 - platform: win-64
   name: munkres
   version: 1.1.4
   category: main
   manager: conda
   dependencies:
   - python
@@ -14643,14 +19291,40 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 101232
   timestamp: 1712239122969
   purls:
   - pkg:pypi/nbformat
+- platform: osx-arm64
+  name: nbformat
+  version: 5.10.4
+  category: main
+  manager: conda
+  dependencies:
+  - jsonschema >=2.6
+  - jupyter_core >=4.12,!=5.0.*
+  - python >=3.8
+  - python-fastjsonschema >=2.15
+  - traitlets >=5.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.10.4-pyhd8ed1ab_0.conda
+  hash:
+    md5: 0b57b5368ab7fc7cdc9e3511fa867214
+    sha256: 36fe73da4d37bc7ac2d1540526ecd294fbd09acda04e096181ab8f1ccd2b464c
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 101232
+  timestamp: 1712239122969
+  purls:
+  - pkg:pypi/nbformat
 - platform: win-64
   name: nbformat
   version: 5.10.4
   category: main
   manager: conda
   dependencies:
   - jsonschema >=2.6
@@ -14715,14 +19389,37 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 20630
   timestamp: 1707082710782
   purls:
   - pkg:pypi/nbstripout
+- platform: osx-arm64
+  name: nbstripout
+  version: 0.7.1
+  category: main
+  manager: conda
+  dependencies:
+  - nbformat
+  - python >=3.5
+  url: https://conda.anaconda.org/conda-forge/noarch/nbstripout-0.7.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 768adb906bdf1828ef38abde924996fd
+    sha256: abd1fedd7a268010ee472ab1c8bd8e44ad564dcb2bc2e67e1b18ace28e64cb56
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 20630
+  timestamp: 1707082710782
+  purls:
+  - pkg:pypi/nbstripout
 - platform: win-64
   name: nbstripout
   version: 0.7.1
   category: main
   manager: conda
   dependencies:
   - nbformat
@@ -14773,14 +19470,31 @@
   build: h73e2aa4_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: X11 AND BSD-3-Clause
   size: 823010
   timestamp: 1710866856626
+- platform: osx-arm64
+  name: ncurses
+  version: 6.4.20240210
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
+  hash:
+    md5: 616ae8691e6608527d0071e6766dcb81
+    sha256: 06f0905791575e2cd3aa961493c56e490b3d82ad9eb49f1c332bd338b0216911
+  build: h078ce10_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: X11 AND BSD-3-Clause
+  size: 820249
+  timestamp: 1710866874348
 - platform: linux-64
   name: nettle
   version: 3.9.1
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -14810,14 +19524,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: GPL 2 and LGPL3
   license_family: GPL
   size: 509519
   timestamp: 1686310097670
+- platform: osx-arm64
+  name: nettle
+  version: 3.9.1
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/nettle-3.9.1-h40ed0f5_0.conda
+  hash:
+    md5: b157977e1ec1dde3ba7ebc6e0dde363f
+    sha256: 5de149b6e35adac11e22ae02516a7466412348690da52049f80ea07fe544896d
+  build: h40ed0f5_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: GPL 2 and LGPL3
+  license_family: GPL
+  size: 510164
+  timestamp: 1686310071126
 - platform: linux-64
   name: networkx
   version: '3.3'
   category: main
   manager: conda
   dependencies:
   - python >=3.10
@@ -14864,14 +19596,41 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 1185670
   timestamp: 1712540499262
   purls:
   - pkg:pypi/networkx
+- platform: osx-arm64
+  name: networkx
+  version: '3.3'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10
+  url: https://conda.anaconda.org/conda-forge/noarch/networkx-3.3-pyhd8ed1ab_1.conda
+  hash:
+    md5: d335fd5704b46f4efb89a6774e81aef0
+    sha256: cbd8a6de87ad842e7665df38dcec719873fe74698bc761de5431047b8fada41a
+  build: pyhd8ed1ab_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  constrains:
+  - pandas >=1.4
+  - numpy >=1.22
+  - matplotlib >=3.5
+  - scipy >=1.9,!=1.11.0,!=1.11.1
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 1185670
+  timestamp: 1712540499262
+  purls:
+  - pkg:pypi/networkx
 - platform: win-64
   name: networkx
   version: '3.3'
   category: main
   manager: conda
   dependencies:
   - python >=3.10
@@ -14930,14 +19689,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 124810
   timestamp: 1713204841161
+- platform: osx-arm64
+  name: ninja
+  version: 1.12.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ninja-1.12.0-h2ffa867_0.conda
+  hash:
+    md5: 24e1b17a513393ee4e81e51fdab1fa93
+    sha256: 634ff2cda6a77b9cd8935e748a1d5698f51f87f1a226638ddc95eb22f6a172ea
+  build: h2ffa867_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 111688
+  timestamp: 1713205253264
 - platform: win-64
   name: ninja
   version: 1.12.0
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -15052,14 +19830,43 @@
   - numpy-base <0a0
   license: BSD-3-Clause
   license_family: BSD
   size: 6491938
   timestamp: 1707226191321
   purls:
   - pkg:pypi/numpy
+- platform: osx-arm64
+  name: numpy
+  version: 1.26.4
+  category: main
+  manager: conda
+  dependencies:
+  - libblas >=3.9.0,<4.0a0
+  - libcblas >=3.9.0,<4.0a0
+  - libcxx >=16
+  - liblapack >=3.9.0,<4.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/numpy-1.26.4-py310hd45542a_0.conda
+  hash:
+    md5: 267ee89a3a0b8c8fa838a2353f9ea0c0
+    sha256: e3078108a4973e73c813b89228f4bd8095ec58f96ca29f55d2e45a6223a9a1db
+  build: py310hd45542a_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - numpy-base <0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 5475744
+  timestamp: 1707226187124
+  purls:
+  - pkg:pypi/numpy
 - platform: win-64
   name: numpy
   version: 1.26.4
   category: main
   manager: conda
   dependencies:
   - libblas >=3.9.0,<4.0a0
@@ -15150,14 +19957,38 @@
   build_number: 12
   license: Apache-2.0
   license_family: Apache
   size: 56300
   timestamp: 1711060187886
   purls:
   - pkg:pypi/opencv-python-headless
+- platform: osx-arm64
+  name: opencv
+  version: 4.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - libopencv 4.9.0 headless_py310hed2a8a7_12
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  - py-opencv 4.9.0 headless_py310h1882dd7_12
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/opencv-4.9.0-headless_py310hf593829_12.conda
+  hash:
+    md5: ce839118406025a70e03c49a8c77e0a8
+    sha256: 7aa69bd9f83d576ad2450c0697fb190101b41b831cb620f054fd9849df781faf
+  build: headless_py310hf593829_12
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 12
+  license: Apache-2.0
+  license_family: Apache
+  size: 56233
+  timestamp: 1711060088021
+  purls:
+  - pkg:pypi/opencv-python-headless
 - platform: win-64
   name: opencv
   version: 4.8.1
   category: main
   manager: conda
   dependencies:
   - libopencv 4.8.1 py310h83ca8e6_5
@@ -15217,14 +20048,35 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 1329934
   timestamp: 1709261129338
+- platform: osx-arm64
+  name: openexr
+  version: 3.2.2
+  category: main
+  manager: conda
+  dependencies:
+  - imath >=3.1.11,<3.1.12.0a0
+  - libcxx >=16
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/openexr-3.2.2-h2c51e1d_1.conda
+  hash:
+    md5: 4ccfab8e79256a8480165969dd1d350c
+    sha256: 243b221c708bbe7f5c0fd72bdbd944a08f4ea9bc1e52b4f12f7fdb5f59633e13
+  build: h2c51e1d_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 1361156
+  timestamp: 1709261019544
 - platform: linux-64
   name: openh264
   version: 2.4.1
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -15256,14 +20108,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   size: 660428
   timestamp: 1706874091051
+- platform: osx-arm64
+  name: openh264
+  version: 2.4.1
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/openh264-2.4.1-hebf3989_0.conda
+  hash:
+    md5: 25a7835e284a4d947fe9a70efa97e019
+    sha256: ecadea5985082105b102f86ff8289128fb247c183b36355d867eb6fc6996df29
+  build: hebf3989_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 598764
+  timestamp: 1706874342701
 - platform: win-64
   name: openh264
   version: 2.4.0
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -15322,14 +20193,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   size: 331273
   timestamp: 1709159538792
+- platform: osx-arm64
+  name: openjpeg
+  version: 2.5.2
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - libpng >=1.6.43,<1.7.0a0
+  - libtiff >=4.6.0,<4.7.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/openjpeg-2.5.2-h9f1df11_0.conda
+  hash:
+    md5: 5029846003f0bc14414b9128a1f7c84b
+    sha256: 472d6eaffc1996e6af35ec8e91c967f472a536a470079bfa56383cc0dbf4d463
+  build: h9f1df11_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 316603
+  timestamp: 1709159627299
 - platform: win-64
   name: openjpeg
   version: 2.5.2
   category: main
   manager: conda
   dependencies:
   - libpng >=1.6.43,<1.7.0a0
@@ -15389,14 +20282,35 @@
   build_number: 1
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
   size: 2506344
   timestamp: 1710793930515
+- platform: osx-arm64
+  name: openssl
+  version: 3.2.1
+  category: main
+  manager: conda
+  dependencies:
+  - ca-certificates
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
+  hash:
+    md5: eb580fb888d93d5d550c557323ac5cee
+    sha256: 519dc941d7ab0ebf31a2878d85c2f444450e7c5f6f41c4d07252c6bb3417b78b
+  build: h0d3ecfb_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
+  size: 2855250
+  timestamp: 1710793435903
 - platform: win-64
   name: openssl
   version: 3.2.1
   category: main
   manager: conda
   dependencies:
   - ca-certificates
@@ -15463,14 +20377,39 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: Apache-2.0
   license_family: Apache
   size: 433233
   timestamp: 1712616573866
+- platform: osx-arm64
+  name: orc
+  version: 2.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libcxx >=16
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - lz4-c >=1.9.3,<1.10.0a0
+  - snappy >=1.2.0,<1.3.0a0
+  - zstd >=1.5.5,<1.6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/orc-2.0.0-h4aad248_1.conda
+  hash:
+    md5: b89ff040a46c45fba6687243e09b8509
+    sha256: 1706ed2e71929f5a2bba0e1041c7ecb064031e7b4ab5862777682c8bdc970bd6
+  build: h4aad248_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: Apache-2.0
+  license_family: Apache
+  size: 414513
+  timestamp: 1712616646377
 - platform: win-64
   name: orc
   version: 1.9.2
   category: main
   manager: conda
   dependencies:
   - libprotobuf >=4.24.4,<4.24.5.0a0
@@ -15535,14 +20474,37 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 15544
   timestamp: 1698324206436
   purls:
   - pkg:pypi/outcome
+- platform: osx-arm64
+  name: outcome
+  version: 1.3.0.post0
+  category: main
+  manager: conda
+  dependencies:
+  - attrs >=19.2.0
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/outcome-1.3.0.post0-pyhd8ed1ab_0.conda
+  hash:
+    md5: c2954fba1935b5775755e3f14d951af0
+    sha256: f3d05ad6bf14e33efa0a526289e816f06a0fae8124f783b2231ee9b934de652a
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 15544
+  timestamp: 1698324206436
+  purls:
+  - pkg:pypi/outcome
 - platform: win-64
   name: outcome
   version: 1.3.0.post0
   category: main
   manager: conda
   dependencies:
   - attrs >=19.2.0
@@ -15599,14 +20561,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 834487
   timestamp: 1654869241699
+- platform: osx-arm64
+  name: p11-kit
+  version: 0.24.1
+  category: main
+  manager: conda
+  dependencies:
+  - libffi >=3.4.2,<3.5.0a0
+  - libtasn1 >=4.18.0,<5.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/p11-kit-0.24.1-h29577a5_0.tar.bz2
+  hash:
+    md5: 8f111d56c8c7c1895bde91a942c43d93
+    sha256: 3e124859307956f9f390f39c74b9700be4843eaaf56891c4b09da75b1bd5b57f
+  build: h29577a5_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 890711
+  timestamp: 1654869118646
 - platform: linux-64
   name: packaging
   version: '24.0'
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -15643,14 +20625,36 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 49832
   timestamp: 1710076089469
   purls:
   - pkg:pypi/packaging
+- platform: osx-arm64
+  name: packaging
+  version: '24.0'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 248f521b64ce055e7feae3105e7abeb8
+    sha256: a390182d74c31dfd713c16db888c92c277feeb6d1fe96ff9d9c105f9564be48a
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 49832
+  timestamp: 1710076089469
+  purls:
+  - pkg:pypi/packaging
 - platform: win-64
   name: packaging
   version: '24.0'
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -15716,14 +20720,40 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 12152782
   timestamp: 1712783095703
+- platform: osx-arm64
+  name: pandas
+  version: 2.2.2
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - numpy >=1.22.4,<2.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python-dateutil >=2.8.1
+  - python-tzdata >=2022a
+  - python_abi 3.10.* *_cp310
+  - pytz >=2020.1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pandas-2.2.2-py310h401b61c_0.conda
+  hash:
+    md5: f877f61cffe0418737b88a363942c6d1
+    sha256: 257f49be55b07bc8f6d8c00a5c6bfa23fa382195c9809ef56c5208eb9f6197a3
+  build: py310h401b61c_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 12118921
+  timestamp: 1712783355910
 - platform: win-64
   name: pandas
   version: 2.2.2
   category: main
   manager: conda
   dependencies:
   - numpy >=1.22.4,<2.0a0
@@ -15787,14 +20817,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 75191
   timestamp: 1712320447201
   purls:
   - pkg:pypi/parso
+- platform: osx-arm64
+  name: parso
+  version: 0.8.4
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+  hash:
+    md5: 81534b420deb77da8833f2289b8d47ac
+    sha256: bfe404eebb930cc41782d34f8fc04c0388ea692eeebe2c5fc28df8ec8d4d61ae
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 75191
+  timestamp: 1712320447201
+  purls:
+  - pkg:pypi/parso
 - platform: win-64
   name: parso
   version: 0.8.4
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -15857,14 +20909,38 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 20743
   timestamp: 1695667673391
   purls:
   - pkg:pypi/partd
+- platform: osx-arm64
+  name: partd
+  version: 1.4.1
+  category: main
+  manager: conda
+  dependencies:
+  - locket
+  - python >=3.7
+  - toolz
+  url: https://conda.anaconda.org/conda-forge/noarch/partd-1.4.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: acf4b7c0bcd5fa3b0e05801c4d2accd6
+    sha256: b248238da2bb9dfe98e680af911dc7013af86095e3ec8baf08905555632d34c7
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 20743
+  timestamp: 1695667673391
+  purls:
+  - pkg:pypi/partd
 - platform: win-64
   name: partd
   version: 1.4.1
   category: main
   manager: conda
   dependencies:
   - locket
@@ -15922,14 +20998,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 836581
   timestamp: 1708118455741
+- platform: osx-arm64
+  name: pcre2
+  version: '10.43'
+  category: main
+  manager: conda
+  dependencies:
+  - bzip2 >=1.0.8,<2.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pcre2-10.43-h26f9a81_0.conda
+  hash:
+    md5: 1ddc87f00014612830f3235b5ad6d821
+    sha256: 4bf7b5fa091f5e7ab0b78778458be1e81c1ffa182b63795734861934945a63a7
+  build: h26f9a81_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 615219
+  timestamp: 1708118184900
 - platform: win-64
   name: pcre2
   version: '10.43'
   category: main
   manager: conda
   dependencies:
   - bzip2 >=1.0.8,<2.0a0
@@ -15989,14 +21085,36 @@
   build_number: 0
   license: ISC
   noarch: python
   size: 53600
   timestamp: 1706113273252
   purls:
   - pkg:pypi/pexpect
+- platform: osx-arm64
+  name: pexpect
+  version: 4.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - ptyprocess >=0.5
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 629f3203c99b32e0988910c93e77f3b6
+    sha256: 90a09d134a4a43911b716d4d6eb9d169238aff2349056f7323d9db613812667e
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: ISC
+  noarch: python
+  size: 53600
+  timestamp: 1706113273252
+  purls:
+  - pkg:pypi/pexpect
 - platform: linux-64
   name: pickleshare
   version: 0.7.5
   category: main
   manager: conda
   dependencies:
   - python >=3
@@ -16033,14 +21151,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 9332
   timestamp: 1602536313357
   purls:
   - pkg:pypi/pickleshare
+- platform: osx-arm64
+  name: pickleshare
+  version: 0.7.5
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3
+  url: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+  hash:
+    md5: 415f0ebb6198cc2801c73438a9fb5761
+    sha256: a1ed1a094dd0d1b94a09ed85c283a0eb28943f2e6f22161fb45e128d35229738
+  build: py_1003
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1003
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 9332
+  timestamp: 1602536313357
+  purls:
+  - pkg:pypi/pickleshare
 - platform: win-64
   name: pickleshare
   version: 0.7.5
   category: main
   manager: conda
   dependencies:
   - python >=3
@@ -16112,14 +21252,43 @@
   build: py310h99295b8_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: HPND
   size: 41184672
   timestamp: 1712154890126
+- platform: osx-arm64
+  name: pillow
+  version: 10.3.0
+  category: main
+  manager: conda
+  dependencies:
+  - freetype >=2.12.1,<3.0a0
+  - lcms2 >=2.16,<3.0a0
+  - libjpeg-turbo >=3.0.0,<4.0a0
+  - libtiff >=4.6.0,<4.7.0a0
+  - libwebp-base >=1.3.2,<2.0a0
+  - libxcb >=1.15,<1.16.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openjpeg >=2.5.2,<3.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - tk >=8.6.13,<8.7.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pillow-10.3.0-py310h81a8c2e_0.conda
+  hash:
+    md5: b43bee0bd86ae53a15ebc2858b737e5d
+    sha256: ee1f5c787edb3aaa68003be7d8329b1472141dcb4483398f84137b2205eeb934
+  build: py310h81a8c2e_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: HPND
+  size: 42031745
+  timestamp: 1712155173373
 - platform: win-64
   name: pillow
   version: 10.3.0
   category: main
   manager: conda
   dependencies:
   - freetype >=2.12.1,<3.0a0
@@ -16191,14 +21360,38 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 1398245
   timestamp: 1706960660581
   purls:
   - pkg:pypi/pip
+- platform: osx-arm64
+  name: pip
+  version: '24.0'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  - setuptools
+  - wheel
+  url: https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: f586ac1e56c8638b64f9c8122a7b8a67
+    sha256: b7c1c5d8f13e8cb491c4bd1d0d1896a4cf80fc47de01059ad77509112b664a4a
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 1398245
+  timestamp: 1706960660581
+  purls:
+  - pkg:pypi/pip
 - platform: win-64
   name: pip
   version: '24.0'
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -16254,14 +21447,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 323904
   timestamp: 1709239931160
+- platform: osx-arm64
+  name: pixman
+  version: 0.43.4
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pixman-0.43.4-hebf3989_0.conda
+  hash:
+    md5: 0308c68e711cd295aaa026a4f8c4b1e5
+    sha256: df0ba2710ccdea5c909b63635529797f6eb3635b6fb77ae9cb2f183d08818409
+  build: hebf3989_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 198755
+  timestamp: 1709239846651
 - platform: win-64
   name: pixman
   version: 0.43.4
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -16313,14 +21525,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1008
   license: GPL-2.0-or-later
   license_family: GPL
   size: 269087
   timestamp: 1650238856925
+- platform: osx-arm64
+  name: pkg-config
+  version: 0.29.2
+  category: main
+  manager: conda
+  dependencies:
+  - libglib >=2.70.2,<3.0a0
+  - libiconv >=1.16,<2.0.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pkg-config-0.29.2-hab62308_1008.tar.bz2
+  hash:
+    md5: 8d173d52214679033079d1b0582075aa
+    sha256: e59e69111709d097f9938e72ba19811ec1ef36aababdbed77bd7c767f15639e0
+  build: hab62308_1008
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1008
+  license: GPL-2.0-or-later
+  license_family: GPL
+  size: 46049
+  timestamp: 1650239029040
 - platform: win-64
   name: pkg-config
   version: 0.29.2
   category: main
   manager: conda
   dependencies:
   - libglib >=2.64.6,<3.0a0
@@ -16376,14 +21608,35 @@
   build_number: 1
   license: MIT AND PSF-2.0
   noarch: python
   size: 10778
   timestamp: 1694617398467
   purls:
   - pkg:pypi/pkgutil-resolve-name
+- platform: osx-arm64
+  name: pkgutil-resolve-name
+  version: 1.3.10
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_1.conda
+  hash:
+    md5: 405678b942f2481cecdb3e010f4925d9
+    sha256: fecf95377134b0e8944762d92ecf7b0149c07d8186fb5db583125a2705c7ea0a
+  build: pyhd8ed1ab_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT AND PSF-2.0
+  noarch: python
+  size: 10778
+  timestamp: 1694617398467
+  purls:
+  - pkg:pypi/pkgutil-resolve-name
 - platform: win-64
   name: pkgutil-resolve-name
   version: 1.3.10
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -16399,142 +21652,186 @@
   noarch: python
   size: 10778
   timestamp: 1694617398467
   purls:
   - pkg:pypi/pkgutil-resolve-name
 - platform: linux-64
   name: platformdirs
-  version: 4.2.0
+  version: 4.2.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
   hash:
-    md5: a0bc3eec34b0fab84be6b2da94e98e20
-    sha256: 2ebfb971236ab825dd79dd6086ea742a9901008ffb9c6222c1f2b5172a8039d3
+    md5: d478a8a3044cdff1aa6e62f9269cefe0
+    sha256: 5718fef2954f016834058ae1d359e407ff8e2e847b35ab43d5d91bcf22d5578d
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 20210
-  timestamp: 1706713564353
+  size: 20248
+  timestamp: 1713912912262
   purls:
   - pkg:pypi/platformdirs
 - platform: osx-64
   name: platformdirs
-  version: 4.2.0
+  version: 4.2.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
   hash:
-    md5: a0bc3eec34b0fab84be6b2da94e98e20
-    sha256: 2ebfb971236ab825dd79dd6086ea742a9901008ffb9c6222c1f2b5172a8039d3
+    md5: d478a8a3044cdff1aa6e62f9269cefe0
+    sha256: 5718fef2954f016834058ae1d359e407ff8e2e847b35ab43d5d91bcf22d5578d
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 20210
-  timestamp: 1706713564353
+  size: 20248
+  timestamp: 1713912912262
+  purls:
+  - pkg:pypi/platformdirs
+- platform: osx-arm64
+  name: platformdirs
+  version: 4.2.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: d478a8a3044cdff1aa6e62f9269cefe0
+    sha256: 5718fef2954f016834058ae1d359e407ff8e2e847b35ab43d5d91bcf22d5578d
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 20248
+  timestamp: 1713912912262
   purls:
   - pkg:pypi/platformdirs
 - platform: win-64
   name: platformdirs
-  version: 4.2.0
+  version: 4.2.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
   hash:
-    md5: a0bc3eec34b0fab84be6b2da94e98e20
-    sha256: 2ebfb971236ab825dd79dd6086ea742a9901008ffb9c6222c1f2b5172a8039d3
+    md5: d478a8a3044cdff1aa6e62f9269cefe0
+    sha256: 5718fef2954f016834058ae1d359e407ff8e2e847b35ab43d5d91bcf22d5578d
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 20210
-  timestamp: 1706713564353
+  size: 20248
+  timestamp: 1713912912262
   purls:
   - pkg:pypi/platformdirs
 - platform: linux-64
   name: pluggy
-  version: 1.4.0
+  version: 1.5.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 139e9feb65187e916162917bb2484976
-    sha256: 6edfd2c41938ea772096c674809bfcf2ebb9bef7e82de6c7ea0b966b86bfb4d0
+    md5: d3483c8fc2dc2cc3f5cf43e26d60cabf
+    sha256: 33eaa3359948a260ebccf9cdc2fd862cea5a6029783289e13602d8e634cd9a26
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 23384
-  timestamp: 1706116931972
+  size: 23815
+  timestamp: 1713667175451
   purls:
   - pkg:pypi/pluggy
 - platform: osx-64
   name: pluggy
-  version: 1.4.0
+  version: 1.5.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 139e9feb65187e916162917bb2484976
-    sha256: 6edfd2c41938ea772096c674809bfcf2ebb9bef7e82de6c7ea0b966b86bfb4d0
+    md5: d3483c8fc2dc2cc3f5cf43e26d60cabf
+    sha256: 33eaa3359948a260ebccf9cdc2fd862cea5a6029783289e13602d8e634cd9a26
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 23384
-  timestamp: 1706116931972
+  size: 23815
+  timestamp: 1713667175451
+  purls:
+  - pkg:pypi/pluggy
+- platform: osx-arm64
+  name: pluggy
+  version: 1.5.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: d3483c8fc2dc2cc3f5cf43e26d60cabf
+    sha256: 33eaa3359948a260ebccf9cdc2fd862cea5a6029783289e13602d8e634cd9a26
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 23815
+  timestamp: 1713667175451
   purls:
   - pkg:pypi/pluggy
 - platform: win-64
   name: pluggy
-  version: 1.4.0
+  version: 1.5.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 139e9feb65187e916162917bb2484976
-    sha256: 6edfd2c41938ea772096c674809bfcf2ebb9bef7e82de6c7ea0b966b86bfb4d0
+    md5: d3483c8fc2dc2cc3f5cf43e26d60cabf
+    sha256: 33eaa3359948a260ebccf9cdc2fd862cea5a6029783289e13602d8e634cd9a26
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 23384
-  timestamp: 1706116931972
+  size: 23815
+  timestamp: 1713667175451
   purls:
   - pkg:pypi/pluggy
 - platform: linux-64
   name: ply
   version: '3.11'
   category: main
   manager: conda
@@ -16573,14 +21870,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 49196
   timestamp: 1712243121626
   purls:
   - pkg:pypi/ply
+- platform: osx-arm64
+  name: ply
+  version: '3.11'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=2.6
+  url: https://conda.anaconda.org/conda-forge/noarch/ply-3.11-pyhd8ed1ab_2.conda
+  hash:
+    md5: 18c6deb6f9602e32446398203c8f0e91
+    sha256: d8faaf4dcc13caed560fa32956523b35928a70499a2d08c51320947d637e3a41
+  build: pyhd8ed1ab_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 49196
+  timestamp: 1712243121626
+  purls:
+  - pkg:pypi/ply
 - platform: win-64
   name: ply
   version: '3.11'
   category: main
   manager: conda
   dependencies:
   - python >=2.6
@@ -16641,14 +21960,37 @@
   constrains:
   - prompt_toolkit 3.0.42
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 270398
   timestamp: 1702399557137
+- platform: osx-arm64
+  name: prompt-toolkit
+  version: 3.0.42
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  - wcwidth
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+  hash:
+    md5: 0bf64bf10eee21f46ac83c161917fa86
+    sha256: 58525b2a9305fb154b2b0d43a48b9a6495441b80e4fbea44f2a34a597d2cef16
+  build: pyha770c72_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - prompt_toolkit 3.0.42
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 270398
+  timestamp: 1702399557137
 - platform: win-64
   name: prompt-toolkit
   version: 3.0.42
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -16709,14 +22051,37 @@
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 375259
   timestamp: 1705722685866
   purls:
   - pkg:pypi/psutil
+- platform: osx-arm64
+  name: psutil
+  version: 5.9.8
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py310hd125d64_0.conda
+  hash:
+    md5: 0fb7c0c32b4212cc783aa315ea4fc173
+    sha256: 8d303673271d8a32a79956a5cf7b941a5fa4f9ef7f093a29efc871a6c8e69aa4
+  build: py310hd125d64_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 376671
+  timestamp: 1705722806535
+  purls:
+  - pkg:pypi/psutil
 - platform: win-64
   name: psutil
   version: 5.9.8
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -16771,14 +22136,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1001
   license: MIT
   license_family: MIT
   size: 5653
   timestamp: 1606147699844
+- platform: osx-arm64
+  name: pthread-stubs
+  version: '0.4'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pthread-stubs-0.4-h27ca646_1001.tar.bz2
+  hash:
+    md5: d3f26c6494d4105d4ecb85203d687102
+    sha256: 9da9e6f5d51dff6ad2e4ee0874791437ba952e0a6249942273f0fedfd07ea826
+  build: h27ca646_1001
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1001
+  license: MIT
+  license_family: MIT
+  size: 5696
+  timestamp: 1606147608402
 - platform: win-64
   name: pthread-stubs
   version: '0.4'
   category: main
   manager: conda
   dependencies:
   - m2w64-gcc-libs
@@ -16850,14 +22233,35 @@
   build_number: 0
   license: ISC
   noarch: python
   size: 16546
   timestamp: 1609419417991
   purls:
   - pkg:pypi/ptyprocess
+- platform: osx-arm64
+  name: ptyprocess
+  version: 0.7.0
+  category: main
+  manager: conda
+  dependencies:
+  - python
+  url: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+  hash:
+    md5: 359eeb6536da0e687af562ed265ec263
+    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
+  build: pyhd3deb0d_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: ISC
+  noarch: python
+  size: 16546
+  timestamp: 1609419417991
+  purls:
+  - pkg:pypi/ptyprocess
 - platform: linux-64
   name: pugixml
   version: '1.14'
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -16889,14 +22293,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 94175
   timestamp: 1696182807580
+- platform: osx-arm64
+  name: pugixml
+  version: '1.14'
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=15.0.7
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pugixml-1.14-h13dd4ca_0.conda
+  hash:
+    md5: 4de774bb04e03af9704ec1a2618c636c
+    sha256: 0bfeac4f1a374da9ff0a322344cdab577d397d6a0a0e5591f08cb7b491926825
+  build: h13dd4ca_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 92472
+  timestamp: 1696182843052
 - platform: win-64
   name: pugixml
   version: '1.14'
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -16979,14 +22402,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 14551
   timestamp: 1642876055775
   purls:
   - pkg:pypi/pure-eval
+- platform: osx-arm64
+  name: pure_eval
+  version: 0.2.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.5
+  url: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 6784285c7e55cb7212efabc79e4c2883
+    sha256: 72792f9fc2b1820e37cc57f84a27bc819c71088c3002ca6db05a2e56404f9d44
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 14551
+  timestamp: 1642876055775
+  purls:
+  - pkg:pypi/pure-eval
 - platform: win-64
   name: pure_eval
   version: 0.2.2
   category: main
   manager: conda
   dependencies:
   - python >=3.5
@@ -17048,14 +22493,37 @@
   arch: x86_64
   subdir: osx-64
   build_number: 12
   license: Apache-2.0
   license_family: Apache
   size: 1183017
   timestamp: 1711060144286
+- platform: osx-arm64
+  name: py-opencv
+  version: 4.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - libopencv 4.9.0 headless_py310hed2a8a7_12
+  - libprotobuf >=4.25.3,<4.25.4.0a0
+  - numpy >=1.22.4,<2.0a0
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/py-opencv-4.9.0-headless_py310h1882dd7_12.conda
+  hash:
+    md5: 9b65917ee49e198237a3ad9bed804459
+    sha256: 0742d514614645be7a72897844e201d98c10c6d3f64aa383176dae4059c8e7a0
+  build: headless_py310h1882dd7_12
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 12
+  license: Apache-2.0
+  license_family: Apache
+  size: 1183028
+  timestamp: 1711060040968
 - platform: win-64
   name: py-opencv
   version: 4.8.1
   category: main
   manager: conda
   dependencies:
   - libopencv 4.8.1 py310h83ca8e6_5
@@ -17077,74 +22545,111 @@
   timestamp: 1698895087681
 - platform: linux-64
   name: pyarrow
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
-  - libarrow 15.0.2 he70291f_3_cpu
-  - libarrow-acero 15.0.2 hac33072_3_cpu
-  - libarrow-dataset 15.0.2 hac33072_3_cpu
-  - libarrow-flight 15.0.2 hd42f311_3_cpu
-  - libarrow-flight-sql 15.0.2 h9241762_3_cpu
-  - libarrow-gandiva 15.0.2 hd4ab825_3_cpu
-  - libarrow-substrait 15.0.2 h9241762_3_cpu
+  - libarrow 15.0.2 h07fc4ce_5_cpu
+  - libarrow-acero 15.0.2 hbabe93e_5_cpu
+  - libarrow-dataset 15.0.2 hbabe93e_5_cpu
+  - libarrow-flight 15.0.2 hc4f8a93_5_cpu
+  - libarrow-flight-sql 15.0.2 he4f5ca8_5_cpu
+  - libarrow-gandiva 15.0.2 hc1954e9_5_cpu
+  - libarrow-substrait 15.0.2 he4f5ca8_5_cpu
   - libgcc-ng >=12
-  - libparquet 15.0.2 h6a7eafb_3_cpu
+  - libparquet 15.0.2 hacf5a1f_5_cpu
   - libstdcxx-ng >=12
+  - libzlib >=1.2.13,<1.3.0a0
   - numpy >=1.22.4,<2.0a0
   - python >=3.10,<3.11.0a0
   - python_abi 3.10.* *_cp310
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyarrow-15.0.2-py310hc7d9cee_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyarrow-15.0.2-py310hd207890_5_cpu.conda
   hash:
-    md5: bec1dabcb80054dfa51fdd72f292b442
-    sha256: e0ecdbbc369b90b56c3ecf57149d7aad24fb8515cf1d123decb2aa17cec1e89b
-  build: py310hc7d9cee_3_cpu
+    md5: c0959b216998d8ccd509b9ec79e27a3e
+    sha256: 7fde73140e6461189c7633732d1a51783bc2eac82905b3cc7a8e674984340ce2
+  build: py310hd207890_5_cpu
   arch: x86_64
   subdir: linux-64
-  build_number: 3
+  build_number: 5
   constrains:
   - apache-arrow-proc =*=cpu
   license: Apache-2.0
   license_family: APACHE
-  size: 4502986
-  timestamp: 1712758379342
+  size: 4484295
+  timestamp: 1713847331890
 - platform: osx-64
   name: pyarrow
   version: 15.0.2
   category: main
   manager: conda
   dependencies:
   - __osx >=10.13
-  - libarrow 15.0.2 h965e444_3_cpu
-  - libarrow-acero 15.0.2 ha0df490_3_cpu
-  - libarrow-dataset 15.0.2 ha0df490_3_cpu
-  - libarrow-flight 15.0.2 h41520de_3_cpu
-  - libarrow-flight-sql 15.0.2 hb2e0ddf_3_cpu
-  - libarrow-gandiva 15.0.2 h6ac0def_3_cpu
-  - libarrow-substrait 15.0.2 hb2e0ddf_3_cpu
+  - libarrow 15.0.2 h1b20127_5_cpu
+  - libarrow-acero 15.0.2 ha0df490_5_cpu
+  - libarrow-dataset 15.0.2 ha0df490_5_cpu
+  - libarrow-flight 15.0.2 h41520de_5_cpu
+  - libarrow-flight-sql 15.0.2 hb2e0ddf_5_cpu
+  - libarrow-gandiva 15.0.2 h81ca85a_5_cpu
+  - libarrow-substrait 15.0.2 hb2e0ddf_5_cpu
   - libcxx >=16
-  - libparquet 15.0.2 h7cd3cfe_3_cpu
+  - libparquet 15.0.2 h7cd3cfe_5_cpu
+  - libzlib >=1.2.13,<1.3.0a0
   - numpy >=1.22.4,<2.0a0
   - python >=3.10,<3.11.0a0
   - python_abi 3.10.* *_cp310
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyarrow-15.0.2-py310h60bf71a_3_cpu.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyarrow-15.0.2-py310hfcac963_5_cpu.conda
   hash:
-    md5: 04abe2b5c2b98f9da42f09760aeff2f4
-    sha256: 9b295ead6ae410600b6ad049ec1bca4f0f4e161fedc58152ed86f403fae826c2
-  build: py310h60bf71a_3_cpu
+    md5: 94772fbe71cab9a15174d18a8755137a
+    sha256: 6f8a8649fdf6f2c861a27a28816ba9779385b7e393013bf876972b39e6c8e205
+  build: py310hfcac963_5_cpu
   arch: x86_64
   subdir: osx-64
-  build_number: 3
+  build_number: 5
   constrains:
   - apache-arrow-proc =*=cpu
   license: Apache-2.0
   license_family: APACHE
-  size: 3971511
-  timestamp: 1712759671581
+  size: 3968599
+  timestamp: 1713848954850
+- platform: osx-arm64
+  name: pyarrow
+  version: 15.0.2
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=11.0
+  - libarrow 15.0.2 hca667bd_5_cpu
+  - libarrow-acero 15.0.2 h3f3aa29_5_cpu
+  - libarrow-dataset 15.0.2 h3f3aa29_5_cpu
+  - libarrow-flight 15.0.2 h224147a_5_cpu
+  - libarrow-flight-sql 15.0.2 hb630850_5_cpu
+  - libarrow-gandiva 15.0.2 h3b9069c_5_cpu
+  - libarrow-substrait 15.0.2 hd92e347_5_cpu
+  - libcxx >=16
+  - libparquet 15.0.2 h5304c63_5_cpu
+  - libzlib >=1.2.13,<1.3.0a0
+  - numpy >=1.22.4,<2.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyarrow-15.0.2-py310h01a46da_5_cpu.conda
+  hash:
+    md5: 6cf3497f55c59c8d8693c4440896815f
+    sha256: 0780634913cc528d52d9bb5d69b74d5bfaeef036202e69701f631d35fe402bd4
+  build: py310h01a46da_5_cpu
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  constrains:
+  - apache-arrow-proc =*=cpu
+  license: Apache-2.0
+  license_family: APACHE
+  size: 3919588
+  timestamp: 1713850321360
 - platform: win-64
   name: pyarrow
   version: 15.0.0
   category: main
   manager: conda
   dependencies:
   - libarrow 15.0.0 he5f67d5_0_cpu
@@ -17217,14 +22722,37 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 13567
   timestamp: 1700596511761
   purls:
   - pkg:pypi/pyarrow-hotfix
+- platform: osx-arm64
+  name: pyarrow-hotfix
+  version: '0.6'
+  category: main
+  manager: conda
+  dependencies:
+  - pyarrow >=0.14
+  - python >=3.5
+  url: https://conda.anaconda.org/conda-forge/noarch/pyarrow-hotfix-0.6-pyhd8ed1ab_0.conda
+  hash:
+    md5: ccc06e6ef2064ae129fab3286299abda
+    sha256: 9b767969d059c106aac6596438a7e7ebd3aa1e2ff6553d4b7e05126dfebf4bd6
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 13567
+  timestamp: 1700596511761
+  purls:
+  - pkg:pypi/pyarrow-hotfix
 - platform: win-64
   name: pyarrow-hotfix
   version: '0.6'
   category: main
   manager: conda
   dependencies:
   - pyarrow >=0.14
@@ -17284,14 +22812,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 34318
   timestamp: 1697203012487
   purls:
   - pkg:pypi/pycodestyle
+- platform: osx-arm64
+  name: pycodestyle
+  version: 2.11.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.11.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 29ff12b36df16bb66fdccd4206aaebfb
+    sha256: 1bd1199c16514cfbc92c0fdc143a00fc55a3deaf800a62a09ac79294606e567e
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 34318
+  timestamp: 1697203012487
+  purls:
+  - pkg:pypi/pycodestyle
 - platform: win-64
   name: pycodestyle
   version: 2.11.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -17369,14 +22919,35 @@
   build: py310h936d966_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD or GPL 2
   size: 1792035
   timestamp: 1673618525200
+- platform: osx-arm64
+  name: pyfftw
+  version: 0.13.1
+  category: main
+  manager: conda
+  dependencies:
+  - numpy >=1.21.6,<2.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyfftw-0.13.1-py310hf1a086a_0.conda
+  hash:
+    md5: d8bd8816839a8d46a27f08eb6f7f30b7
+    sha256: 72a603993eb4e5f2fad3d990b3947a6507f03f466a90a39004db098bd39542ff
+  build: py310hf1a086a_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD or GPL 2
+  size: 1078930
+  timestamp: 1673618810589
 - platform: win-64
   name: pyfftw
   version: 0.13.1
   category: main
   manager: conda
   dependencies:
   - fftw >=3.3.10,<4.0a0
@@ -17437,14 +23008,36 @@
   license: BSD-2-Clause
   license_family: BSD
   noarch: python
   size: 860425
   timestamp: 1700608076927
   purls:
   - pkg:pypi/pygments
+- platform: osx-arm64
+  name: pygments
+  version: 2.17.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: 140a7f159396547e9799aa98f9f0742e
+    sha256: af5f8867450dc292f98ea387d4d8945fc574284677c8f60eaa9846ede7387257
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  noarch: python
+  size: 860425
+  timestamp: 1700608076927
+  purls:
+  - pkg:pypi/pygments
 - platform: win-64
   name: pygments
   version: 2.17.2
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -17503,14 +23096,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 89455
   timestamp: 1709721146886
   purls:
   - pkg:pypi/pyparsing
+- platform: osx-arm64
+  name: pyparsing
+  version: 3.1.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: b9a4dacf97241704529131a0dfc0494f
+    sha256: 06c77cb03e5dde2d939b216c99dd2db52ea93a4c7c599f3882f136005c359c7b
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 89455
+  timestamp: 1709721146886
+  purls:
+  - pkg:pypi/pyparsing
 - platform: win-64
   name: pyparsing
   version: 3.1.2
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -17527,79 +23142,102 @@
   noarch: python
   size: 89455
   timestamp: 1709721146886
   purls:
   - pkg:pypi/pyparsing
 - platform: linux-64
   name: pyproject-metadata
-  version: 0.7.1
+  version: 0.8.0
   category: main
   manager: conda
   dependencies:
   - packaging >=19.0
   - python >=3.7
-  url: https://conda.anaconda.org/conda-forge/noarch/pyproject-metadata-0.7.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pyproject-metadata-0.8.0-pyhd8ed1ab_0.conda
   hash:
-    md5: dcb27826ffc94d5f04e241322239983b
-    sha256: 9ec35cffa163f587aeb52d1603df8374659e3be30dbc6db0e980ecb797f21fee
+    md5: 573fe09d7bd0cd4bcc210d8369b5ca47
+    sha256: 99f4971944c74150b1daa15c87fcbf3609b2cd3fef0cf2516840a3748250b75b
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 12538
-  timestamp: 1675133341609
+  size: 13211
+  timestamp: 1713446924896
   purls:
   - pkg:pypi/pyproject-metadata
 - platform: osx-64
   name: pyproject-metadata
-  version: 0.7.1
+  version: 0.8.0
   category: main
   manager: conda
   dependencies:
   - packaging >=19.0
   - python >=3.7
-  url: https://conda.anaconda.org/conda-forge/noarch/pyproject-metadata-0.7.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pyproject-metadata-0.8.0-pyhd8ed1ab_0.conda
   hash:
-    md5: dcb27826ffc94d5f04e241322239983b
-    sha256: 9ec35cffa163f587aeb52d1603df8374659e3be30dbc6db0e980ecb797f21fee
+    md5: 573fe09d7bd0cd4bcc210d8369b5ca47
+    sha256: 99f4971944c74150b1daa15c87fcbf3609b2cd3fef0cf2516840a3748250b75b
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 12538
-  timestamp: 1675133341609
+  size: 13211
+  timestamp: 1713446924896
+  purls:
+  - pkg:pypi/pyproject-metadata
+- platform: osx-arm64
+  name: pyproject-metadata
+  version: 0.8.0
+  category: main
+  manager: conda
+  dependencies:
+  - packaging >=19.0
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/pyproject-metadata-0.8.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 573fe09d7bd0cd4bcc210d8369b5ca47
+    sha256: 99f4971944c74150b1daa15c87fcbf3609b2cd3fef0cf2516840a3748250b75b
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 13211
+  timestamp: 1713446924896
   purls:
   - pkg:pypi/pyproject-metadata
 - platform: win-64
   name: pyproject-metadata
-  version: 0.7.1
+  version: 0.8.0
   category: main
   manager: conda
   dependencies:
   - packaging >=19.0
   - python >=3.7
-  url: https://conda.anaconda.org/conda-forge/noarch/pyproject-metadata-0.7.1-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/pyproject-metadata-0.8.0-pyhd8ed1ab_0.conda
   hash:
-    md5: dcb27826ffc94d5f04e241322239983b
-    sha256: 9ec35cffa163f587aeb52d1603df8374659e3be30dbc6db0e980ecb797f21fee
+    md5: 573fe09d7bd0cd4bcc210d8369b5ca47
+    sha256: 99f4971944c74150b1daa15c87fcbf3609b2cd3fef0cf2516840a3748250b75b
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
-  size: 12538
-  timestamp: 1675133341609
+  size: 13211
+  timestamp: 1713446924896
   purls:
   - pkg:pypi/pyproject-metadata
 - platform: linux-64
   name: pyqt
   version: 5.15.9
   category: main
   manager: conda
@@ -17746,14 +23384,37 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 18981
   timestamp: 1661604969727
   purls:
   - pkg:pypi/pysocks
+- platform: osx-arm64
+  name: pysocks
+  version: 1.7.1
+  category: main
+  manager: conda
+  dependencies:
+  - __unix
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
+  hash:
+    md5: 2a7de29fb590ca14b5243c4c812c8025
+    sha256: a42f826e958a8d22e65b3394f437af7332610e43ee313393d1cf143f0a2d274b
+  build: pyha2e5f31_6
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 6
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 18981
+  timestamp: 1661604969727
+  purls:
+  - pkg:pypi/pysocks
 - platform: win-64
   name: pysocks
   version: 1.7.1
   category: main
   manager: conda
   dependencies:
   - __win
@@ -17830,14 +23491,44 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 255523
   timestamp: 1709992719691
   purls:
   - pkg:pypi/pytest
+- platform: osx-arm64
+  name: pytest
+  version: 8.1.1
+  category: main
+  manager: conda
+  dependencies:
+  - colorama
+  - exceptiongroup >=1.0.0rc8
+  - iniconfig
+  - packaging
+  - pluggy <2.0,>=1.4
+  - python >=3.8
+  - tomli >=1
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 94ff09cdedcb7b17e9cd5097ee2cfcff
+    sha256: 3c481d6b54af1a33c32a3f3eaa3e0971955431e7023db55808740cd062271c73
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - pytest-faulthandler >=2
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 255523
+  timestamp: 1709992719691
+  purls:
+  - pkg:pypi/pytest
 - platform: win-64
   name: pytest
   version: 8.1.1
   category: main
   manager: conda
   dependencies:
   - colorama
@@ -17902,14 +23593,35 @@
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 33372
   timestamp: 1710849429651
+- platform: osx-arm64
+  name: pytest-asyncio
+  version: 0.23.6
+  category: main
+  manager: conda
+  dependencies:
+  - pytest >=7.0.0,<9
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-asyncio-0.23.6-pyhd8ed1ab_0.conda
+  hash:
+    md5: 811340befcada7641384d4f115ddbd6e
+    sha256: 4867959aacaf4402a3e12bb283b8e09a0f8cdc1f6bd7aab84e0d4d2f33b5b994
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 33372
+  timestamp: 1710849429651
 - platform: win-64
   name: pytest-asyncio
   version: 0.23.6
   category: main
   manager: conda
   dependencies:
   - pytest >=7.0.0,<9
@@ -17969,14 +23681,37 @@
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
   size: 25507
   timestamp: 1711411153367
+- platform: osx-arm64
+  name: pytest-cov
+  version: 5.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - coverage >=5.2.1
+  - pytest >=4.6
+  - python >=3.8
+  - toml
+  url: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: c54c0107057d67ddf077751339ec2c63
+    sha256: 218306243faf3c36347131c2b36bb189daa948ac2e92c7ab52bb26cc8c157b3c
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 25507
+  timestamp: 1711411153367
 - platform: win-64
   name: pytest-cov
   version: 5.0.0
   category: main
   manager: conda
   dependencies:
   - coverage >=5.2.1
@@ -18055,14 +23790,43 @@
   subdir: osx-64
   build_number: 0
   constrains:
   - python_abi 3.10.* *_cp310
   license: Python-2.0
   size: 11890228
   timestamp: 1710940046031
+- platform: osx-arm64
+  name: python
+  version: 3.10.14
+  category: main
+  manager: conda
+  dependencies:
+  - bzip2 >=1.0.8,<2.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.10.14-h2469fbe_0_cpython.conda
+  hash:
+    md5: 4ae999c8227c6d8c7623d32d51d25ea9
+    sha256: 454d609fe25daedce9e886efcbfcadad103ed0362e7cb6d2bcddec90b1ecd3ee
+  build: h2469fbe_0_cpython
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - python_abi 3.10.* *_cp310
+  license: Python-2.0
+  size: 12336005
+  timestamp: 1710939659384
 - platform: win-64
   name: python
   version: 3.10.14
   category: main
   manager: conda
   dependencies:
   - bzip2 >=1.0.8,<2.0a0
@@ -18130,14 +23894,37 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 222742
   timestamp: 1709299922152
   purls:
   - pkg:pypi/python-dateutil
+- platform: osx-arm64
+  name: python-dateutil
+  version: 2.9.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  - six >=1.5
+  url: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 2cf4264fffb9e6eff6031c5b6884d61c
+    sha256: f3ceef02ac164a8d3a080d0d32f8e2ebe10dd29e3a685d240e38b3599e146320
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 222742
+  timestamp: 1709299922152
+  purls:
+  - pkg:pypi/python-dateutil
 - platform: win-64
   name: python-dateutil
   version: 2.9.0
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -18197,14 +23984,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 225250
   timestamp: 1703781171097
   purls:
   - pkg:pypi/fastjsonschema
+- platform: osx-arm64
+  name: python-fastjsonschema
+  version: 2.19.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.3
+  url: https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.19.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 4d3ceee3af4b0f9a1f48f57176bf8625
+    sha256: 38b2db169d65cc5595e3ce63294c4fdb6a242ecf71f70b3ad8cad3bd4230d82f
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 225250
+  timestamp: 1703781171097
+  purls:
+  - pkg:pypi/fastjsonschema
 - platform: win-64
   name: python-fastjsonschema
   version: 2.19.1
   category: main
   manager: conda
   dependencies:
   - python >=3.3
@@ -18263,14 +24072,36 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 144024
   timestamp: 1707747742930
   purls:
   - pkg:pypi/tzdata
+- platform: osx-arm64
+  name: python-tzdata
+  version: '2024.1'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2024.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 98206ea9954216ee7540f0c773f2104d
+    sha256: 9da9a849d53705dee450b83507df1ca8ffea5f83bd21a215202221f1c492f8ad
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 144024
+  timestamp: 1707747742930
+  purls:
+  - pkg:pypi/tzdata
 - platform: win-64
   name: python-tzdata
   version: '2024.1'
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -18325,14 +24156,34 @@
   build_number: 4
   constrains:
   - python 3.10.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
   size: 6484
   timestamp: 1695147705581
+- platform: osx-arm64
+  name: python_abi
+  version: '3.10'
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.10-4_cp310.conda
+  hash:
+    md5: 1a3d9c6bb5f0b1b22d9e9296c127e8c7
+    sha256: f69bac2f28082a275ef67313968b2c366d8236c3a6869b9cdf5cdb97a5821812
+  build: 4_cp310
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 4
+  constrains:
+  - python 3.10.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6490
+  timestamp: 1695147522999
 - platform: win-64
   name: python_abi
   version: '3.10'
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.10-4_cp310.conda
@@ -18402,14 +24253,43 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 2219683
   timestamp: 1704695373632
+- platform: osx-arm64
+  name: pythran
+  version: 0.15.0
+  category: main
+  manager: conda
+  dependencies:
+  - beniget 0.4.*
+  - clangxx_osx-arm64
+  - colorlog
+  - decorator
+  - gast 0.5.*
+  - libcxx >=15
+  - numpy >=1.22.4,<2.0a0
+  - ply >=3.4
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pythran-0.15.0-py310h1359cc7_1.conda
+  hash:
+    md5: d07e86e377a24de8cb03d84beb018ada
+    sha256: 1649991f66013bcb20de39555465b0de5ac2180951b80c0a1c2e33debb6f6ba1
+  build: py310h1359cc7_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 2235482
+  timestamp: 1704695488436
 - platform: win-64
   name: pythran
   version: 0.15.0
   category: main
   manager: conda
   dependencies:
   - beniget 0.4.*
@@ -18474,14 +24354,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 188538
   timestamp: 1706886944988
   purls:
   - pkg:pypi/pytz
+- platform: osx-arm64
+  name: pytz
+  version: '2024.1'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3eeeeb9e4827ace8c0c1419c85d590ad
+    sha256: 1a7d6b233f7e6e3bbcbad054c8fd51e690a67b129a899a056a5e45dd9f00cb41
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 188538
+  timestamp: 1706886944988
+  purls:
+  - pkg:pypi/pytz
 - platform: win-64
   name: pytz
   version: '2024.1'
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -18543,14 +24445,38 @@
   build_number: 1
   license: MIT
   license_family: MIT
   size: 3608914
   timestamp: 1695569899715
   purls:
   - pkg:pypi/pywavelets
+- platform: osx-arm64
+  name: pywavelets
+  version: 1.4.1
+  category: main
+  manager: conda
+  dependencies:
+  - numpy >=1.22.4,<2.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pywavelets-1.4.1-py310h280b8fa_1.conda
+  hash:
+    md5: f2824f60b018e93f6883c83a0bdd190c
+    sha256: f7031b0eb0e77dd20c0219e3ee907da9cdef6dd1de603d09685a64abc1e48e59
+  build: py310h280b8fa_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 3616831
+  timestamp: 1695568343231
+  purls:
+  - pkg:pypi/pywavelets
 - platform: win-64
   name: pywavelets
   version: 1.4.1
   category: main
   manager: conda
   dependencies:
   - numpy >=1.22.4,<2.0a0
@@ -18635,14 +24561,36 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: MIT
   license_family: MIT
   size: 160097
   timestamp: 1695373947773
+- platform: osx-arm64
+  name: pyyaml
+  version: 6.0.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - yaml >=0.2.5,<0.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py310h2aa6e3c_1.conda
+  hash:
+    md5: 0e7ccdd121ce7b486f1de7917178387c
+    sha256: 7b8668cd86d2421c62ec241f840d84a600b854afc91383a509bbb60ba907aeec
+  build: py310h2aa6e3c_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  size: 158641
+  timestamp: 1695373859696
 - platform: win-64
   name: pyyaml
   version: 6.0.1
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -18804,14 +24752,37 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 61808
   timestamp: 1698112171285
   purls:
   - pkg:pypi/qtpy
+- platform: osx-arm64
+  name: qtpy
+  version: 2.4.1
+  category: main
+  manager: conda
+  dependencies:
+  - packaging
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/qtpy-2.4.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 7f391bd70d2abfb70f304ba5aa4e1261
+    sha256: 925bf48e747af6ceff1b073c10b12fc94ef79c88a34729059d253e43466a33f1
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 61808
+  timestamp: 1698112171285
+  purls:
+  - pkg:pypi/qtpy
 - platform: win-64
   name: qtpy
   version: 2.4.1
   category: main
   manager: conda
   dependencies:
   - packaging
@@ -18864,14 +24835,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: BSD-2-Clause
   license_family: BSD
   size: 1767853
   timestamp: 1694329738983
+- platform: osx-arm64
+  name: rav1e
+  version: 0.6.6
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/rav1e-0.6.6-h69fbcac_2.conda
+  hash:
+    md5: e309ae86569b1cd55a0285fa4e939844
+    sha256: be6174970193cb4d0ffa7d731a93a4c9542881dbc7ab24e74b460ef312161169
+  build: h69fbcac_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 1526706
+  timestamp: 1694329743011
 - platform: win-64
   name: rav1e
   version: 0.6.6
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -18945,14 +24934,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: BSD-3-Clause
   license_family: BSD
   size: 26814
   timestamp: 1708947195067
+- platform: osx-arm64
+  name: re2
+  version: 2023.09.01
+  category: main
+  manager: conda
+  dependencies:
+  - libre2-11 2023.09.01 h7b2c953_2
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/re2-2023.09.01-h4cba328_2.conda
+  hash:
+    md5: 0342882197116478a42fa4ea35af79c1
+    sha256: 0e0d44414381c39a7e6f3da442cb41c637df0dcb383a07425f19c19ccffa0118
+  build: h4cba328_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 26770
+  timestamp: 1708947220914
 - platform: win-64
   name: re2
   version: 2023.09.01
   category: main
   manager: conda
   dependencies:
   - libre2-11 2023.09.01 h8c5ae5e_1
@@ -19003,84 +25011,123 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: GPL-3.0-only
   license_family: GPL
   size: 255870
   timestamp: 1679532707590
+- platform: osx-arm64
+  name: readline
+  version: '8.2'
+  category: main
+  manager: conda
+  dependencies:
+  - ncurses >=6.3,<7.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
+  hash:
+    md5: 8cbb776a2f641b943d413b3e19df71f4
+    sha256: a1dfa679ac3f6007362386576a704ad2d0d7a02e98f5d0b115f207a2da63e884
+  build: h92ec313_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: GPL-3.0-only
+  license_family: GPL
+  size: 250351
+  timestamp: 1679532511311
 - platform: linux-64
   name: referencing
-  version: 0.34.0
+  version: 0.35.0
   category: main
   manager: conda
   dependencies:
   - attrs >=22.2.0
   - python >=3.8
   - rpds-py >=0.7.0
-  url: https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda
   hash:
-    md5: e4492c22e314be5c75db3469e3bbf3d9
-    sha256: 2e631e9e1d49280770573f7acc7441b70181b2dc21948bb1be15eaae80550672
+    md5: 52ddb316ef9136ba610f7fac57da9062
+    sha256: 1fecb3adca444c68b351e24d8f1eaaee32b79649d1ee4852f10960fc0d11ed48
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: MIT
-  license_family: MIT
   noarch: python
-  size: 42071
-  timestamp: 1710763821612
+  size: 42146
+  timestamp: 1714072614223
   purls:
   - pkg:pypi/referencing
 - platform: osx-64
   name: referencing
-  version: 0.34.0
+  version: 0.35.0
   category: main
   manager: conda
   dependencies:
   - attrs >=22.2.0
   - python >=3.8
   - rpds-py >=0.7.0
-  url: https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda
   hash:
-    md5: e4492c22e314be5c75db3469e3bbf3d9
-    sha256: 2e631e9e1d49280770573f7acc7441b70181b2dc21948bb1be15eaae80550672
+    md5: 52ddb316ef9136ba610f7fac57da9062
+    sha256: 1fecb3adca444c68b351e24d8f1eaaee32b79649d1ee4852f10960fc0d11ed48
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
-  license_family: MIT
   noarch: python
-  size: 42071
-  timestamp: 1710763821612
+  size: 42146
+  timestamp: 1714072614223
+  purls:
+  - pkg:pypi/referencing
+- platform: osx-arm64
+  name: referencing
+  version: 0.35.0
+  category: main
+  manager: conda
+  dependencies:
+  - attrs >=22.2.0
+  - python >=3.8
+  - rpds-py >=0.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 52ddb316ef9136ba610f7fac57da9062
+    sha256: 1fecb3adca444c68b351e24d8f1eaaee32b79649d1ee4852f10960fc0d11ed48
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  noarch: python
+  size: 42146
+  timestamp: 1714072614223
   purls:
   - pkg:pypi/referencing
 - platform: win-64
   name: referencing
-  version: 0.34.0
+  version: 0.35.0
   category: main
   manager: conda
   dependencies:
   - attrs >=22.2.0
   - python >=3.8
   - rpds-py >=0.7.0
-  url: https://conda.anaconda.org/conda-forge/noarch/referencing-0.34.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/referencing-0.35.0-pyhd8ed1ab_0.conda
   hash:
-    md5: e4492c22e314be5c75db3469e3bbf3d9
-    sha256: 2e631e9e1d49280770573f7acc7441b70181b2dc21948bb1be15eaae80550672
+    md5: 52ddb316ef9136ba610f7fac57da9062
+    sha256: 1fecb3adca444c68b351e24d8f1eaaee32b79649d1ee4852f10960fc0d11ed48
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: MIT
-  license_family: MIT
   noarch: python
-  size: 42071
-  timestamp: 1710763821612
+  size: 42146
+  timestamp: 1714072614223
   purls:
   - pkg:pypi/referencing
 - platform: linux-64
   name: rich
   version: 13.7.1
   category: main
   manager: conda
@@ -19121,14 +25168,37 @@
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   noarch: python
   size: 184347
   timestamp: 1709150578093
+- platform: osx-arm64
+  name: rich
+  version: 13.7.1
+  category: main
+  manager: conda
+  dependencies:
+  - markdown-it-py >=2.2.0
+  - pygments >=2.13.0,<3.0.0
+  - python >=3.7.0
+  - typing_extensions >=4.0.0,<5.0.0
+  url: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: ba445bf767ae6f0d959ff2b40c20912b
+    sha256: 2b26d58aa59e46f933c3126367348651b0dab6e0bf88014e857415bb184a4667
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 184347
+  timestamp: 1709150578093
 - platform: win-64
   name: rich
   version: 13.7.1
   category: main
   manager: conda
   dependencies:
   - markdown-it-py >=2.2.0
@@ -19191,14 +25261,39 @@
   - __osx >=10.12
   license: MIT
   license_family: MIT
   size: 299696
   timestamp: 1707923332485
   purls:
   - pkg:pypi/rpds-py
+- platform: osx-arm64
+  name: rpds-py
+  version: 0.18.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/rpds-py-0.18.0-py310hf632f72_0.conda
+  hash:
+    md5: cd1b172bce3f30ef2d3b2d01a8cc296a
+    sha256: ba2404149c4ec942f6f81493f7154ab9d267335c73ae65bfc795808e5bb4917d
+  build: py310hf632f72_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - __osx >=11.0
+  license: MIT
+  license_family: MIT
+  size: 292751
+  timestamp: 1707925657411
+  purls:
+  - pkg:pypi/rpds-py
 - platform: win-64
   name: rpds-py
   version: 0.18.0
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -19218,32 +25313,32 @@
   license_family: MIT
   size: 202632
   timestamp: 1707923848209
   purls:
   - pkg:pypi/rpds-py
 - platform: linux-64
   name: s2n
-  version: 1.4.10
+  version: 1.4.12
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
   - openssl >=3.2.1,<4.0a0
-  url: https://conda.anaconda.org/conda-forge/linux-64/s2n-1.4.10-h06160fa_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/s2n-1.4.12-h06160fa_0.conda
   hash:
-    md5: 74c7020bffae20d9579c47b4684b8ad8
-    sha256: 1121352650d3e88227bf5e9a9008f269e1f3b82c90b4e4ce4a8123a6656cad45
+    md5: bf1899cfd6dea061a220fa7e96a1f4bd
+    sha256: fc5759c4d8136bb9048ed5cd2e8fd1a375104c3a7ec60fee1be0b06e7487d610
   build: h06160fa_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: Apache-2.0
   license_family: Apache
-  size: 344987
-  timestamp: 1712792530529
+  size: 346689
+  timestamp: 1713325107791
 - platform: linux-64
   name: scikit-image
   version: 0.22.0
   category: main
   manager: conda
   dependencies:
   - imageio >=2.27
@@ -19320,14 +25415,57 @@
   - matplotlib-base >=3.5
   license: BSD-3-Clause
   license_family: BSD
   size: 10380683
   timestamp: 1697029630464
   purls:
   - pkg:pypi/scikit-image
+- platform: osx-arm64
+  name: scikit-image
+  version: 0.22.0
+  category: main
+  manager: conda
+  dependencies:
+  - __osx >=10.9
+  - imageio >=2.27
+  - lazy_loader >=0.2
+  - libcxx >=16.0.6
+  - networkx >=2.8
+  - numpy >=1.22.4,<2.0a0
+  - packaging >=21
+  - pillow >=9.0.1
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - pywavelets >=1.1.1
+  - scipy >=1.8
+  - tifffile >=2022.8.12
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/scikit-image-0.22.0-py310h6e3cc31_2.conda
+  hash:
+    md5: ee50df5a86eadd2ebdaaf119eb00150f
+    sha256: 38293a17b509f035ab2ba0ae3cf93f5cb9d8e7389573dcb5dfb3aaafea6aacff
+  build: py310h6e3cc31_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  constrains:
+  - astropy >=5.0
+  - cytoolz >=0.11.0
+  - scikit-learn >=1.0
+  - cloudpickle >=0.2.1
+  - matplotlib-base >=3.5
+  - dask-core >=2021.1.0
+  - toolz >=0.10.0
+  - pooch >=1.6.0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 10478801
+  timestamp: 1697029541475
+  purls:
+  - pkg:pypi/scikit-image
 - platform: win-64
   name: scikit-image
   version: 0.22.0
   category: main
   manager: conda
   dependencies:
   - imageio >=2.27
@@ -19421,14 +25559,44 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 15744737
   timestamp: 1712257554126
+- platform: osx-arm64
+  name: scipy
+  version: 1.13.0
+  category: main
+  manager: conda
+  dependencies:
+  - libblas >=3.9.0,<4.0a0
+  - libcblas >=3.9.0,<4.0a0
+  - libcxx >=16
+  - libgfortran 5.*
+  - libgfortran5 >=12.3.0
+  - libgfortran5 >=13.2.0
+  - liblapack >=3.9.0,<4.0a0
+  - numpy >=1.22.4,<1.28
+  - numpy >=1.22.4,<2.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/scipy-1.13.0-py310hf4b343e_0.conda
+  hash:
+    md5: 9c7f3fdecc0c9af9a573bbc369f681d9
+    sha256: 5c1081f021da306f621d3a3b2f9e0501c8894e68e6e487fdbcc64890afab9dbb
+  build: py310hf4b343e_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 14695788
+  timestamp: 1712253605046
 - platform: win-64
   name: scipy
   version: 1.13.0
   category: main
   manager: conda
   dependencies:
   - libblas >=3.9.0,<4.0a0
@@ -19493,14 +25661,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 501790
   timestamp: 1713094963112
   purls:
   - pkg:pypi/setuptools
+- platform: osx-arm64
+  name: setuptools
+  version: 69.5.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 7462280d81f639363e6e63c81276bd9e
+    sha256: 72d143408507043628b32bed089730b6d5f5445eccc44b59911ec9f262e365e7
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 501790
+  timestamp: 1713094963112
+  purls:
+  - pkg:pypi/setuptools
 - platform: win-64
   name: setuptools
   version: 69.5.1
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -19534,14 +25724,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 213817
   timestamp: 1643442169866
+- platform: osx-arm64
+  name: sigtool
+  version: 0.1.3
+  category: main
+  manager: conda
+  dependencies:
+  - openssl >=3.0.0,<4.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/sigtool-0.1.3-h44b9a77_0.tar.bz2
+  hash:
+    md5: 4a2cac04f86a4540b8c9b8d8f597848f
+    sha256: 70791ae00a3756830cb50451db55f63e2a42a2fa2a8f1bab1ebd36bbb7d55bff
+  build: h44b9a77_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 210264
+  timestamp: 1643442231687
 - platform: linux-64
   name: simpleeval
   version: 0.9.13
   category: main
   manager: conda
   dependencies:
   - python >=2.5,!=3.0.*,!=3.1.*,!=3.2.*
@@ -19578,14 +25787,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 20532
   timestamp: 1698070679462
   purls:
   - pkg:pypi/simpleeval
+- platform: osx-arm64
+  name: simpleeval
+  version: 0.9.13
+  category: main
+  manager: conda
+  dependencies:
+  - python >=2.5,!=3.0.*,!=3.1.*,!=3.2.*
+  url: https://conda.anaconda.org/conda-forge/noarch/simpleeval-0.9.13-pyhd8ed1ab_1.conda
+  hash:
+    md5: b3282d9b9e4a7c42d6c570492316dcaa
+    sha256: 5c9c537011327fc281c3c108020f1ad2a40284df0e1625a87825c0699d98f67f
+  build: pyhd8ed1ab_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 20532
+  timestamp: 1698070679462
+  purls:
+  - pkg:pypi/simpleeval
 - platform: win-64
   name: simpleeval
   version: 0.9.13
   category: main
   manager: conda
   dependencies:
   - python >=2.5,!=3.0.*,!=3.1.*,!=3.2.*
@@ -19699,14 +25930,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 14259
   timestamp: 1620240338595
   purls:
   - pkg:pypi/six
+- platform: osx-arm64
+  name: six
+  version: 1.16.0
+  category: main
+  manager: conda
+  dependencies:
+  - python
+  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+  hash:
+    md5: e5f25f8dbc060e9a8d912e432202afc2
+    sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
+  build: pyh6c4a22f_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 14259
+  timestamp: 1620240338595
+  purls:
+  - pkg:pypi/six
 - platform: win-64
   name: six
   version: 1.16.0
   category: main
   manager: conda
   dependencies:
   - python
@@ -19760,14 +26013,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: BSD-3-Clause
   license_family: BSD
   size: 36881
   timestamp: 1712591355487
+- platform: osx-arm64
+  name: snappy
+  version: 1.2.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/snappy-1.2.0-hd04f947_1.conda
+  hash:
+    md5: 32cf833d440ee18d3c4c04ec38cf2b01
+    sha256: 88afe00f550e1e2d66326516e5372aa1834c51fb6b53afa7a3636c65cd75ce42
+  build: hd04f947_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 35655
+  timestamp: 1712591484831
 - platform: win-64
   name: snappy
   version: 1.1.10
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -19825,14 +26097,36 @@
   license: Apache-2.0
   license_family: Apache
   noarch: python
   size: 15064
   timestamp: 1708953086199
   purls:
   - pkg:pypi/sniffio
+- platform: osx-arm64
+  name: sniffio
+  version: 1.3.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 490730480d76cf9c8f8f2849719c6e2b
+    sha256: bc12100b2d8836b93c55068b463190505b8064d0fc7d025e89f20ebf22fe6c2b
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  noarch: python
+  size: 15064
+  timestamp: 1708953086199
+  purls:
+  - pkg:pypi/sniffio
 - platform: win-64
   name: sniffio
   version: 1.3.1
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -19891,14 +26185,36 @@
   license: Apache-2.0
   license_family: APACHE
   noarch: python
   size: 26314
   timestamp: 1621217159824
   purls:
   - pkg:pypi/sortedcontainers
+- platform: osx-arm64
+  name: sortedcontainers
+  version: 2.4.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=2.7
+  url: https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 6d6552722448103793743dabfbda532d
+    sha256: 0cea408397d50c2afb2d25e987ebac4546ae11e549d65b1403d80dc368dfaaa6
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  noarch: python
+  size: 26314
+  timestamp: 1621217159824
+  purls:
+  - pkg:pypi/sortedcontainers
 - platform: win-64
   name: sortedcontainers
   version: 2.4.0
   category: main
   manager: conda
   dependencies:
   - python >=2.7
@@ -19963,14 +26279,39 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 26205
   timestamp: 1669632203115
   purls:
   - pkg:pypi/stack-data
+- platform: osx-arm64
+  name: stack_data
+  version: 0.6.2
+  category: main
+  manager: conda
+  dependencies:
+  - asttokens
+  - executing
+  - pure_eval
+  - python >=3.5
+  url: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+  hash:
+    md5: e7df0fdd404616638df5ece6e69ba7af
+    sha256: a58433e75229bec39f3be50c02efbe9b7083e53a1f31d8ee247564f370191eec
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 26205
+  timestamp: 1669632203115
+  purls:
+  - pkg:pypi/stack-data
 - platform: win-64
   name: stack_data
   version: 0.6.2
   category: main
   manager: conda
   dependencies:
   - asttokens
@@ -20027,14 +26368,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-2-Clause
   license_family: BSD
   size: 2362393
   timestamp: 1710374582341
+- platform: osx-arm64
+  name: svt-av1
+  version: 2.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/svt-av1-2.0.0-h078ce10_0.conda
+  hash:
+    md5: 9da0cd60486e8037b546f48dfdf00b71
+    sha256: 9d5cb5e3ee41849d60de4997a83efaad2aaaa4d92782f5a8f293931bb3fc4b37
+  build: h078ce10_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  size: 1415570
+  timestamp: 1710374533383
 - platform: win-64
   name: svt-av1
   version: 1.7.0
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -20087,14 +26447,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: NCSA
   license_family: MIT
   size: 201044
   timestamp: 1602664232074
+- platform: osx-arm64
+  name: tapi
+  version: 1100.0.11
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=11.0.0.a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/tapi-1100.0.11-he4954df_0.tar.bz2
+  hash:
+    md5: d83362e7d0513f35f454bc50b0ca591d
+    sha256: 1709265fbee693a9e8b4126b0a3e68a6c4718b05821c659279c1af051f2d40f3
+  build: he4954df_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: NCSA
+  license_family: MIT
+  size: 191416
+  timestamp: 1602687595316
 - platform: linux-64
   name: tbb
   version: 2021.12.0
   category: main
   manager: conda
   dependencies:
   - libgcc-ng >=12
@@ -20128,14 +26507,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Apache-2.0
   license_family: APACHE
   size: 172745
   timestamp: 1712960020101
+- platform: osx-arm64
+  name: tbb
+  version: 2021.12.0
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=16
+  - libhwloc >=2.10.0,<2.10.1.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/tbb-2021.12.0-h2ffa867_0.conda
+  hash:
+    md5: cf605a0a1d025e72c56dcdbe6f23d9f0
+    sha256: c2905ed5cc567e1714e1a3276a1bdd5e119d335798ebdea1937cceee7718cf78
+  build: h2ffa867_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: APACHE
+  size: 128359
+  timestamp: 1712960100130
 - platform: win-64
   name: tbb
   version: 2021.12.0
   category: main
   manager: conda
   dependencies:
   - libhwloc >=2.10.0,<2.10.1.0a0
@@ -20194,14 +26593,36 @@
   license: BSD-2-Clause
   license_family: BSD
   noarch: python
   size: 17386
   timestamp: 1702066480361
   purls:
   - pkg:pypi/tblib
+- platform: osx-arm64
+  name: tblib
+  version: 3.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/tblib-3.0.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 04eedddeb68ad39871c8127dd1c21f4f
+    sha256: 2e2c255b6f24a6d75b9938cb184520e27db697db2c24f04e18342443ae847c0a
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-2-Clause
+  license_family: BSD
+  noarch: python
+  size: 17386
+  timestamp: 1702066480361
+  purls:
+  - pkg:pypi/tblib
 - platform: win-64
   name: tblib
   version: 3.0.0
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -20218,172 +26639,222 @@
   noarch: python
   size: 17386
   timestamp: 1702066480361
   purls:
   - pkg:pypi/tblib
 - platform: linux-64
   name: textual
-  version: 0.56.4
+  version: 0.58.0
   category: main
   manager: conda
   dependencies:
   - markdown-it-py >=2.1.0
   - python >=3.8.0,<4.0.0
   - rich >=13.3.3
   - typing-extensions >=4.4.0,<5.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/textual-0.56.4-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/textual-0.58.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 94c0c6bff0adc8893c8912fda20831d6
-    sha256: df5ee1666df74859458a03771ae9154e4a3041508155567a8b254f41f2db7b56
+    md5: 4c6810190300d756252291faf1c03c17
+    sha256: 21badddc2099f950aabd3fc557d62b8ad5b2b559437d709bffb260b5707ea790
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   constrains:
   - tree-sitter >=0.20.1,<0.21.0
   - tree_sitter_languages >=1.7.0
   license: MIT
-  license_family: MIT
   noarch: python
-  size: 381024
-  timestamp: 1712679288725
+  size: 382124
+  timestamp: 1714053075575
   purls:
   - pkg:pypi/textual
 - platform: osx-64
   name: textual
-  version: 0.56.4
+  version: 0.58.0
   category: main
   manager: conda
   dependencies:
   - markdown-it-py >=2.1.0
   - python >=3.8.0,<4.0.0
   - rich >=13.3.3
   - typing-extensions >=4.4.0,<5.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/textual-0.56.4-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/textual-0.58.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 94c0c6bff0adc8893c8912fda20831d6
-    sha256: df5ee1666df74859458a03771ae9154e4a3041508155567a8b254f41f2db7b56
+    md5: 4c6810190300d756252291faf1c03c17
+    sha256: 21badddc2099f950aabd3fc557d62b8ad5b2b559437d709bffb260b5707ea790
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   constrains:
   - tree-sitter >=0.20.1,<0.21.0
   - tree_sitter_languages >=1.7.0
   license: MIT
-  license_family: MIT
   noarch: python
-  size: 381024
-  timestamp: 1712679288725
+  size: 382124
+  timestamp: 1714053075575
+  purls:
+  - pkg:pypi/textual
+- platform: osx-arm64
+  name: textual
+  version: 0.58.0
+  category: main
+  manager: conda
+  dependencies:
+  - markdown-it-py >=2.1.0
+  - python >=3.8.0,<4.0.0
+  - rich >=13.3.3
+  - typing-extensions >=4.4.0,<5.0.0
+  url: https://conda.anaconda.org/conda-forge/noarch/textual-0.58.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 4c6810190300d756252291faf1c03c17
+    sha256: 21badddc2099f950aabd3fc557d62b8ad5b2b559437d709bffb260b5707ea790
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - tree-sitter >=0.20.1,<0.21.0
+  - tree_sitter_languages >=1.7.0
+  license: MIT
+  noarch: python
+  size: 382124
+  timestamp: 1714053075575
   purls:
   - pkg:pypi/textual
 - platform: win-64
   name: textual
-  version: 0.56.4
+  version: 0.58.0
   category: main
   manager: conda
   dependencies:
   - markdown-it-py >=2.1.0
   - python >=3.8.0,<4.0.0
   - rich >=13.3.3
   - typing-extensions >=4.4.0,<5.0.0
-  url: https://conda.anaconda.org/conda-forge/noarch/textual-0.56.4-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/textual-0.58.0-pyhd8ed1ab_0.conda
   hash:
-    md5: 94c0c6bff0adc8893c8912fda20831d6
-    sha256: df5ee1666df74859458a03771ae9154e4a3041508155567a8b254f41f2db7b56
+    md5: 4c6810190300d756252291faf1c03c17
+    sha256: 21badddc2099f950aabd3fc557d62b8ad5b2b559437d709bffb260b5707ea790
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   constrains:
   - tree-sitter >=0.20.1,<0.21.0
   - tree_sitter_languages >=1.7.0
   license: MIT
-  license_family: MIT
   noarch: python
-  size: 381024
-  timestamp: 1712679288725
+  size: 382124
+  timestamp: 1714053075575
   purls:
   - pkg:pypi/textual
 - platform: linux-64
   name: tifffile
-  version: 2024.2.12
+  version: 2024.4.18
   category: main
   manager: conda
   dependencies:
   - imagecodecs >=2023.8.12
   - numpy >=1.19.2
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/tifffile-2024.2.12-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/tifffile-2024.4.18-pyhd8ed1ab_0.conda
   hash:
-    md5: d5c8bef52be4e70c48b1400eec3eecc8
-    sha256: 5b629ab2eae0508ad554cc831fed72950d74909d6bcf2aebdfd01e0c0afca60b
+    md5: 9640ec921dce12e87e589ac634c7bd8a
+    sha256: f82fecb3daceb55a4dd856edd9c40c0d68a08b4b8ebb94dac24bf16b13f67e16
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   constrains:
   - matplotlib-base >=3.3
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 178320
-  timestamp: 1707824993716
+  size: 178341
+  timestamp: 1713426258609
   purls:
   - pkg:pypi/tifffile
 - platform: osx-64
   name: tifffile
-  version: 2024.2.12
+  version: 2024.4.18
   category: main
   manager: conda
   dependencies:
   - imagecodecs >=2023.8.12
   - numpy >=1.19.2
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/tifffile-2024.2.12-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/tifffile-2024.4.18-pyhd8ed1ab_0.conda
   hash:
-    md5: d5c8bef52be4e70c48b1400eec3eecc8
-    sha256: 5b629ab2eae0508ad554cc831fed72950d74909d6bcf2aebdfd01e0c0afca60b
+    md5: 9640ec921dce12e87e589ac634c7bd8a
+    sha256: f82fecb3daceb55a4dd856edd9c40c0d68a08b4b8ebb94dac24bf16b13f67e16
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   constrains:
   - matplotlib-base >=3.3
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 178320
-  timestamp: 1707824993716
+  size: 178341
+  timestamp: 1713426258609
+  purls:
+  - pkg:pypi/tifffile
+- platform: osx-arm64
+  name: tifffile
+  version: 2024.4.18
+  category: main
+  manager: conda
+  dependencies:
+  - imagecodecs >=2023.8.12
+  - numpy >=1.19.2
+  - python >=3.9
+  url: https://conda.anaconda.org/conda-forge/noarch/tifffile-2024.4.18-pyhd8ed1ab_0.conda
+  hash:
+    md5: 9640ec921dce12e87e589ac634c7bd8a
+    sha256: f82fecb3daceb55a4dd856edd9c40c0d68a08b4b8ebb94dac24bf16b13f67e16
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  constrains:
+  - matplotlib-base >=3.3
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 178341
+  timestamp: 1713426258609
   purls:
   - pkg:pypi/tifffile
 - platform: win-64
   name: tifffile
-  version: 2024.2.12
+  version: 2024.4.18
   category: main
   manager: conda
   dependencies:
   - imagecodecs >=2023.8.12
   - numpy >=1.19.2
   - python >=3.9
-  url: https://conda.anaconda.org/conda-forge/noarch/tifffile-2024.2.12-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/tifffile-2024.4.18-pyhd8ed1ab_0.conda
   hash:
-    md5: d5c8bef52be4e70c48b1400eec3eecc8
-    sha256: 5b629ab2eae0508ad554cc831fed72950d74909d6bcf2aebdfd01e0c0afca60b
+    md5: 9640ec921dce12e87e589ac634c7bd8a
+    sha256: f82fecb3daceb55a4dd856edd9c40c0d68a08b4b8ebb94dac24bf16b13f67e16
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   constrains:
   - matplotlib-base >=3.3
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 178320
-  timestamp: 1707824993716
+  size: 178341
+  timestamp: 1713426258609
   purls:
   - pkg:pypi/tifffile
 - platform: linux-64
   name: tk
   version: 8.6.13
   category: main
   manager: conda
@@ -20417,14 +26888,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 1
   license: TCL
   license_family: BSD
   size: 3270220
   timestamp: 1699202389792
+- platform: osx-arm64
+  name: tk
+  version: 8.6.13
+  category: main
+  manager: conda
+  dependencies:
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
+  hash:
+    md5: b50a57ba89c32b62428b71a875291c9b
+    sha256: 72457ad031b4c048e5891f3f6cb27a53cb479db68a52d965f796910e71a403a8
+  build: h5083fa2_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: TCL
+  license_family: BSD
+  size: 3145523
+  timestamp: 1699202432999
 - platform: win-64
   name: tk
   version: 8.6.13
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -20482,14 +26972,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 18433
   timestamp: 1604308660817
   purls:
   - pkg:pypi/toml
+- platform: osx-arm64
+  name: toml
+  version: 0.10.2
+  category: main
+  manager: conda
+  dependencies:
+  - python >=2.7
+  url: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: f832c45a477c78bebd107098db465095
+    sha256: f0f3d697349d6580e4c2f35ba9ce05c65dc34f9f049e85e45da03800b46139c1
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 18433
+  timestamp: 1604308660817
+  purls:
+  - pkg:pypi/toml
 - platform: win-64
   name: toml
   version: 0.10.2
   category: main
   manager: conda
   dependencies:
   - python >=2.7
@@ -20548,14 +27060,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 15940
   timestamp: 1644342331069
   purls:
   - pkg:pypi/tomli
+- platform: osx-arm64
+  name: tomli
+  version: 2.0.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+  hash:
+    md5: 5844808ffab9ebdb694585b50ba02a96
+    sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 15940
+  timestamp: 1644342331069
+  purls:
+  - pkg:pypi/tomli
 - platform: win-64
   name: tomli
   version: 2.0.1
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -20610,14 +27144,34 @@
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 52358
   timestamp: 1706112720607
+- platform: osx-arm64
+  name: toolz
+  version: 0.12.1
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 2fcb582444635e2c402e8569bb94e039
+    sha256: 22b0a9790317526e08609d5dfdd828210ae89e6d444a9e954855fc29012e90c6
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 52358
+  timestamp: 1706112720607
 - platform: win-64
   name: toolz
   version: 0.12.1
   category: main
   manager: conda
   dependencies:
   - python >=3.7
@@ -20675,14 +27229,37 @@
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 651434
   timestamp: 1708363551700
   purls:
   - pkg:pypi/tornado
+- platform: osx-arm64
+  name: tornado
+  version: '6.4'
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py310hd125d64_0.conda
+  hash:
+    md5: 918e4a0c909366d09cf9530bdf3dc398
+    sha256: 8ee446ec68401a54540e3d848ffe7e4eb5633b7462c2a990efe0fb2621ebb50a
+  build: py310hd125d64_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 652190
+  timestamp: 1708363567796
+  purls:
+  - pkg:pypi/tornado
 - platform: win-64
   name: tornado
   version: '6.4'
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -20702,76 +27279,98 @@
   license_family: Apache
   size: 652769
   timestamp: 1708363845639
   purls:
   - pkg:pypi/tornado
 - platform: linux-64
   name: traitlets
-  version: 5.14.2
+  version: 5.14.3
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
   hash:
-    md5: af5fa2d2186003472e766a23c46cae04
-    sha256: 9ea6073091c130470a51b51703c8d2d959434992e29c4aa4abeba07cd56533a3
+    md5: 3df84416a021220d8b5700c613af2dc5
+    sha256: 8a64fa0f19022828513667c2c7176cfd125001f3f4b9bc00d33732e627dd2592
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: linux-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 110288
-  timestamp: 1710254564088
+  size: 110187
+  timestamp: 1713535244513
   purls:
   - pkg:pypi/traitlets
 - platform: osx-64
   name: traitlets
-  version: 5.14.2
+  version: 5.14.3
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
   hash:
-    md5: af5fa2d2186003472e766a23c46cae04
-    sha256: 9ea6073091c130470a51b51703c8d2d959434992e29c4aa4abeba07cd56533a3
+    md5: 3df84416a021220d8b5700c613af2dc5
+    sha256: 8a64fa0f19022828513667c2c7176cfd125001f3f4b9bc00d33732e627dd2592
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 110288
-  timestamp: 1710254564088
+  size: 110187
+  timestamp: 1713535244513
+  purls:
+  - pkg:pypi/traitlets
+- platform: osx-arm64
+  name: traitlets
+  version: 5.14.3
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3df84416a021220d8b5700c613af2dc5
+    sha256: 8a64fa0f19022828513667c2c7176cfd125001f3f4b9bc00d33732e627dd2592
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 110187
+  timestamp: 1713535244513
   purls:
   - pkg:pypi/traitlets
 - platform: win-64
   name: traitlets
-  version: 5.14.2
+  version: 5.14.3
   category: main
   manager: conda
   dependencies:
   - python >=3.8
-  url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
   hash:
-    md5: af5fa2d2186003472e766a23c46cae04
-    sha256: 9ea6073091c130470a51b51703c8d2d959434992e29c4aa4abeba07cd56533a3
+    md5: 3df84416a021220d8b5700c613af2dc5
+    sha256: 8a64fa0f19022828513667c2c7176cfd125001f3f4b9bc00d33732e627dd2592
   build: pyhd8ed1ab_0
   arch: x86_64
   subdir: win-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
-  size: 110288
-  timestamp: 1710254564088
+  size: 110187
+  timestamp: 1713535244513
   purls:
   - pkg:pypi/traitlets
 - platform: linux-64
   name: transonic
   version: 0.6.4
   category: main
   manager: conda
@@ -20814,14 +27413,38 @@
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: OTHER
   noarch: python
   size: 62458
   timestamp: 1711764672001
+- platform: osx-arm64
+  name: transonic
+  version: 0.6.4
+  category: main
+  manager: conda
+  dependencies:
+  - autopep8
+  - beniget ~=0.4.0
+  - gast ~=0.5.0
+  - numpy
+  - python >=3.9
+  url: https://conda.anaconda.org/conda-forge/noarch/transonic-0.6.4-pyhd8ed1ab_0.conda
+  hash:
+    md5: 9c9081ba670ae4e9bb5097bf2697febf
+    sha256: 781351d83b8deb4cd0eb21c056bd891324cbc0203703a2360f703cb1b5c1f500
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: OTHER
+  noarch: python
+  size: 62458
+  timestamp: 1711764672001
 - platform: win-64
   name: transonic
   version: 0.6.4
   category: main
   manager: conda
   dependencies:
   - autopep8
@@ -20894,14 +27517,43 @@
   build_number: 0
   license: MIT
   license_family: MIT
   size: 655550
   timestamp: 1710661917363
   purls:
   - pkg:pypi/trio
+- platform: osx-arm64
+  name: trio
+  version: 0.25.0
+  category: main
+  manager: conda
+  dependencies:
+  - attrs >=23.2.0
+  - exceptiongroup
+  - idna
+  - outcome
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - sniffio >=1.3.0
+  - sortedcontainers
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/trio-0.25.0-py310hbe9552e_0.conda
+  hash:
+    md5: f36fedf2788468f759f84bb92ddcb2ff
+    sha256: 2782644781c20196df53dc3fb78795213905bf78a3a73096632126c9b05253a8
+  build: py310hbe9552e_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 655718
+  timestamp: 1710661995434
+  purls:
+  - pkg:pypi/trio
 - platform: win-64
   name: trio
   version: 0.25.0
   category: main
   manager: conda
   dependencies:
   - attrs >=23.2.0
@@ -20963,14 +27615,34 @@
   subdir: osx-64
   build_number: 0
   license: PSF-2.0
   license_family: PSF
   noarch: python
   size: 10093
   timestamp: 1712330094282
+- platform: osx-arm64
+  name: typing-extensions
+  version: 4.11.0
+  category: main
+  manager: conda
+  dependencies:
+  - typing_extensions 4.11.0 pyha770c72_0
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
+  hash:
+    md5: 471e3988f8ca5e9eb3ce6be7eac3bcee
+    sha256: aecbd9c601ba5a6c128da8975276fd817b968a9edc969b7ae97aee76e80a14a6
+  build: hd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: PSF-2.0
+  license_family: PSF
+  noarch: python
+  size: 10093
+  timestamp: 1712330094282
 - platform: win-64
   name: typing-extensions
   version: 4.11.0
   category: main
   manager: conda
   dependencies:
   - typing_extensions 4.11.0 pyha770c72_0
@@ -21027,14 +27699,36 @@
   license: PSF-2.0
   license_family: PSF
   noarch: python
   size: 37583
   timestamp: 1712330089194
   purls:
   - pkg:pypi/typing-extensions
+- platform: osx-arm64
+  name: typing_extensions
+  version: 4.11.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+  hash:
+    md5: 6ef2fc37559256cf682d8b3375e89b80
+    sha256: a7e8714d14f854058e971a6ed44f18cc37cc685f98ddefb2e6b7899a0cc4d1a2
+  build: pyha770c72_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: PSF-2.0
+  license_family: PSF
+  noarch: python
+  size: 37583
+  timestamp: 1712330089194
+  purls:
+  - pkg:pypi/typing-extensions
 - platform: win-64
   name: typing_extensions
   version: 4.11.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -21085,14 +27779,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: LicenseRef-Public-Domain
   noarch: generic
   size: 119815
   timestamp: 1706886945727
+- platform: osx-arm64
+  name: tzdata
+  version: 2024a
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+  hash:
+    md5: 161081fc7cec0bfda0d86d7cb595f8d8
+    sha256: 7b2b69c54ec62a243eb6fba2391b5e443421608c3ae5dbff938ad33ca8db5122
+  build: h0c530f3_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: LicenseRef-Public-Domain
+  noarch: generic
+  size: 119815
+  timestamp: 1706886945727
 - platform: win-64
   name: tzdata
   version: 2024a
   category: main
   manager: conda
   dependencies: []
   url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
@@ -21147,14 +27859,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 11162
   timestamp: 1707507514699
   purls:
   - pkg:pypi/uc-micro-py
+- platform: osx-arm64
+  name: uc-micro-py
+  version: 1.0.3
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.6
+  url: https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.3-pyhd8ed1ab_0.conda
+  hash:
+    md5: 3b7fc78d7be7b450952aaa916fb78877
+    sha256: 54293cd94da3a6b978b353eb7897555055d925ad0008bc73e85cca19e2587ed0
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 11162
+  timestamp: 1707507514699
+  purls:
+  - pkg:pypi/uc-micro-py
 - platform: win-64
   name: uc-micro-py
   version: 1.0.3
   category: main
   manager: conda
   dependencies:
   - python >=3.6
@@ -21257,14 +27991,37 @@
   build_number: 0
   license: Apache-2.0
   license_family: Apache
   size: 366573
   timestamp: 1695848504604
   purls:
   - pkg:pypi/unicodedata2
+- platform: osx-arm64
+  name: unicodedata2
+  version: 15.1.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/unicodedata2-15.1.0-py310h2aa6e3c_0.conda
+  hash:
+    md5: 9dbba0c13148e8efbb80eb60186b2d8c
+    sha256: fd33715a75bc7d4ad863ac47341e9fdf8b78e47aa55c90f89a844c660aacc352
+  build: py310h2aa6e3c_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Apache-2.0
+  license_family: Apache
+  size: 377237
+  timestamp: 1695848435303
+  purls:
+  - pkg:pypi/unicodedata2
 - platform: win-64
   name: unicodedata2
   version: 15.1.0
   category: main
   manager: conda
   dependencies:
   - python >=3.10,<3.11.0a0
@@ -21330,14 +28087,38 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 94669
   timestamp: 1708239595549
   purls:
   - pkg:pypi/urllib3
+- platform: osx-arm64
+  name: urllib3
+  version: 2.2.1
+  category: main
+  manager: conda
+  dependencies:
+  - brotli-python >=1.0.9
+  - pysocks >=1.5.6,<2.0,!=1.5.7
+  - python >=3.7
+  url: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
+  hash:
+    md5: 08807a87fa7af10754d46f63b368e016
+    sha256: d4009dcc9327684d6409706ce17656afbeae690d8522d3c9bc4df57649a352cd
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 94669
+  timestamp: 1708239595549
+  purls:
+  - pkg:pypi/urllib3
 - platform: win-64
   name: urllib3
   version: 2.2.1
   category: main
   manager: conda
   dependencies:
   - brotli-python >=1.0.9
@@ -21458,14 +28239,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 32709
   timestamp: 1704731373922
   purls:
   - pkg:pypi/wcwidth
+- platform: osx-arm64
+  name: wcwidth
+  version: 0.2.13
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+  hash:
+    md5: 68f0738df502a14213624b288c60c9ad
+    sha256: b6cd2fee7e728e620ec736d8dfee29c6c9e2adbd4e695a31f1d8f834a83e57e3
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 32709
+  timestamp: 1704731373922
+  purls:
+  - pkg:pypi/wcwidth
 - platform: win-64
   name: wcwidth
   version: 0.2.13
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -21524,14 +28327,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 57963
   timestamp: 1711546009410
   purls:
   - pkg:pypi/wheel
+- platform: osx-arm64
+  name: wheel
+  version: 0.43.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
+  hash:
+    md5: 0b5293a157c2b5cd513dd1b03d8d3aae
+    sha256: cb318f066afd6fd64619f14c030569faf3f53e6f50abf743b4c865e7d95b96bc
+  build: pyhd8ed1ab_1
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 1
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 57963
+  timestamp: 1711546009410
+  purls:
+  - pkg:pypi/wheel
 - platform: win-64
   name: wheel
   version: 0.43.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -21605,14 +28430,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: GPL-2.0-or-later
   license_family: GPL
   size: 937077
   timestamp: 1660323305349
+- platform: osx-arm64
+  name: x264
+  version: 1!164.3095
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/x264-1!164.3095-h57fd34a_2.tar.bz2
+  hash:
+    md5: b1f6dccde5d3a1f911960b6e567113ff
+    sha256: debdf60bbcfa6a60201b12a1d53f36736821db281a28223a09e0685edcce105a
+  build: h57fd34a_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: GPL-2.0-or-later
+  license_family: GPL
+  size: 717038
+  timestamp: 1660323292329
 - platform: win-64
   name: x264
   version: 1!164.3095
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15
@@ -21664,14 +28507,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 3
   license: GPL-2.0-or-later
   license_family: GPL
   size: 3433205
   timestamp: 1646610148268
+- platform: osx-arm64
+  name: x265
+  version: '3.5'
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=12.0.1
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/x265-3.5-hbc6ce65_3.tar.bz2
+  hash:
+    md5: b1f7f2780feffe310b068c021e8ff9b2
+    sha256: 2fed6987dba7dee07bd9adc1a6f8e6c699efb851431bcb6ebad7de196e87841d
+  build: hbc6ce65_3
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 3
+  license: GPL-2.0-or-later
+  license_family: GPL
+  size: 1832744
+  timestamp: 1646609481185
 - platform: win-64
   name: x265
   version: '3.5'
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15
@@ -21965,14 +28827,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 13071
   timestamp: 1684638167647
+- platform: osx-arm64
+  name: xorg-libxau
+  version: 1.0.11
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/xorg-libxau-1.0.11-hb547adb_0.conda
+  hash:
+    md5: ca73dc4f01ea91e44e3ed76602c5ea61
+    sha256: 02c313a1cada46912e5b9bdb355cfb4534bfe22143b4ea4ecc419690e793023b
+  build: hb547adb_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 13667
+  timestamp: 1684638272445
 - platform: win-64
   name: xorg-libxau
   version: 1.0.11
   category: main
   manager: conda
   dependencies:
   - m2w64-gcc-libs
@@ -22022,14 +28902,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: MIT
   license_family: MIT
   size: 17225
   timestamp: 1610071995461
+- platform: osx-arm64
+  name: xorg-libxdmcp
+  version: 1.1.3
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/xorg-libxdmcp-1.1.3-h27ca646_0.tar.bz2
+  hash:
+    md5: 6738b13f7fadc18725965abdd4129c36
+    sha256: d9a2fb4762779994718832f05a7d62ab2dcf6103a312235267628b5187ce88f7
+  build: h27ca646_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  size: 18164
+  timestamp: 1610071737668
 - platform: win-64
   name: xorg-libxdmcp
   version: 1.1.3
   category: main
   manager: conda
   dependencies:
   - m2w64-gcc-libs
@@ -22247,14 +29145,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 46179
   timestamp: 1712210047952
   purls:
   - pkg:pypi/xyzservices
+- platform: osx-arm64
+  name: xyzservices
+  version: 2024.4.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/xyzservices-2024.4.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 93dffc47dadbe36a1a644f3f50d4979d
+    sha256: 4e095631b52a78bbd9b53f28eb79b0c8f448d9509cf0451e99c2f3f85576f114
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 46179
+  timestamp: 1712210047952
+  purls:
+  - pkg:pypi/xyzservices
 - platform: win-64
   name: xyzservices
   version: 2024.4.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -22304,14 +29224,31 @@
   build: h775f41a_0
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: LGPL-2.1 and GPL-2.0
   size: 238119
   timestamp: 1660346964847
+- platform: osx-arm64
+  name: xz
+  version: 5.2.6
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+  hash:
+    md5: 39c6b54e94014701dd157f4f576ed211
+    sha256: 59d78af0c3e071021cfe82dc40134c19dab8cdf804324b62940f5c8cd71803ec
+  build: h57fd34a_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: LGPL-2.1 and GPL-2.0
+  size: 235693
+  timestamp: 1660346961024
 - platform: win-64
   name: xz
   version: 5.2.6
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15
@@ -22360,14 +29297,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 2
   license: MIT
   license_family: MIT
   size: 84237
   timestamp: 1641347062780
+- platform: osx-arm64
+  name: yaml
+  version: 0.2.5
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/yaml-0.2.5-h3422bc3_2.tar.bz2
+  hash:
+    md5: 4bb3f014845110883a3c5ee811fd84b4
+    sha256: 93181a04ba8cfecfdfb162fc958436d868cc37db504c58078eab4c1a3e57fbb7
+  build: h3422bc3_2
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 2
+  license: MIT
+  license_family: MIT
+  size: 88016
+  timestamp: 1641347076660
 - platform: win-64
   name: yaml
   version: 0.2.5
   category: main
   manager: conda
   dependencies:
   - vc >=14.1,<15.0a0
@@ -22421,14 +29376,34 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 215707
   timestamp: 1702765897536
+- platform: osx-arm64
+  name: zfp
+  version: 1.0.1
+  category: main
+  manager: conda
+  dependencies:
+  - libcxx >=15
+  - llvm-openmp >=16.0.6
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/zfp-1.0.1-ha8f4885_0.conda
+  hash:
+    md5: ffa2d992521c35ea31a217e138f01b8b
+    sha256: 3b81ddab41d7174125f90739035784d8d8ff2e47b92906593a84a0858ce56090
+  build: ha8f4885_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 196830
+  timestamp: 1702766075336
 - platform: win-64
   name: zfp
   version: 1.0.1
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -22486,14 +29461,36 @@
   license: BSD-3-Clause
   license_family: BSD
   noarch: python
   size: 36325
   timestamp: 1681770298596
   purls:
   - pkg:pypi/zict
+- platform: osx-arm64
+  name: zict
+  version: 3.0.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/zict-3.0.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: cf30c2c15b82aacb07f9c09e28ff2275
+    sha256: 3d65c081514569ab3642ba7e6c2a6b4615778b596db6b1c82ee30a2d912539e5
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  noarch: python
+  size: 36325
+  timestamp: 1681770298596
+  purls:
+  - pkg:pypi/zict
 - platform: win-64
   name: zict
   version: 3.0.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -22552,14 +29549,36 @@
   license: MIT
   license_family: MIT
   noarch: python
   size: 18954
   timestamp: 1695255262261
   purls:
   - pkg:pypi/zipp
+- platform: osx-arm64
+  name: zipp
+  version: 3.17.0
+  category: main
+  manager: conda
+  dependencies:
+  - python >=3.8
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+  hash:
+    md5: 2e4d6bc0b14e10f895fc6791a7d9b26a
+    sha256: bced1423fdbf77bca0a735187d05d9b9812d2163f60ab426fc10f11f92ecbe26
+  build: pyhd8ed1ab_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: MIT
+  license_family: MIT
+  noarch: python
+  size: 18954
+  timestamp: 1695255262261
+  purls:
+  - pkg:pypi/zipp
 - platform: win-64
   name: zipp
   version: 3.17.0
   category: main
   manager: conda
   dependencies:
   - python >=3.8
@@ -22613,14 +29632,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 5
   license: Zlib
   license_family: Other
   size: 90764
   timestamp: 1686575574678
+- platform: osx-arm64
+  name: zlib
+  version: 1.2.13
+  category: main
+  manager: conda
+  dependencies:
+  - libzlib 1.2.13 h53f4e23_5
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/zlib-1.2.13-h53f4e23_5.conda
+  hash:
+    md5: a08383f223b10b71492d27566fafbf6c
+    sha256: de0ee1e24aa6867058d3b852a15c8d7f49f262f5828772700c647186d4a96bbe
+  build: h53f4e23_5
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 5
+  license: Zlib
+  license_family: Other
+  size: 79577
+  timestamp: 1686575471024
 - platform: win-64
   name: zlib
   version: 1.2.13
   category: main
   manager: conda
   dependencies:
   - libzlib 1.2.13 hcfcfb64_5
@@ -22672,14 +29710,32 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: Zlib
   license_family: Other
   size: 93171
   timestamp: 1679095009343
+- platform: osx-arm64
+  name: zlib-ng
+  version: 2.0.7
+  category: main
+  manager: conda
+  dependencies: []
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/zlib-ng-2.0.7-h1a8c8d9_0.conda
+  hash:
+    md5: 4852d8981e833f34c8ed32e4fb8e103b
+    sha256: c526e4b6351e351c89ed0c60ca43b9f04668363a58e355583dc7701efb4fca89
+  build: h1a8c8d9_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: Zlib
+  license_family: Other
+  size: 84057
+  timestamp: 1679095058609
 - platform: win-64
   name: zlib-ng
   version: 2.0.7
   category: main
   manager: conda
   dependencies:
   - ucrt >=10.0.20348.0
@@ -22733,14 +29789,33 @@
   arch: x86_64
   subdir: osx-64
   build_number: 0
   license: BSD-3-Clause
   license_family: BSD
   size: 499383
   timestamp: 1693151312586
+- platform: osx-arm64
+  name: zstd
+  version: 1.5.5
+  category: main
+  manager: conda
+  dependencies:
+  - libzlib >=1.2.13,<1.3.0a0
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
+  hash:
+    md5: 5b212cfb7f9d71d603ad891879dc7933
+    sha256: 7e1fe6057628bbb56849a6741455bbb88705bae6d6646257e57904ac5ee5a481
+  build: h4f39d0f_0
+  arch: aarch64
+  subdir: osx-arm64
+  build_number: 0
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 400508
+  timestamp: 1693151393180
 - platform: win-64
   name: zstd
   version: 1.5.5
   category: main
   manager: conda
   dependencies:
   - libzlib >=1.2.13,<1.3.0a0
```

### Comparing `fluidimage-0.4.6/pixi.toml` & `fluidimage-0.5.0/pixi.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "fluidimage"
 channels = ["conda-forge"]
-platforms = ["linux-64", "win-64", "osx-64"]
+platforms = ["linux-64", "win-64", "osx-64", "osx-arm64"]
 
 [tasks]
 # use as `pixi run install-editable`
 install-dependencies = "pixi install"
 install-editable = {cmd = "pip install -e . -v --no-build-isolation --no-deps", depends_on = ["install-dependencies"]}
-test = "export OMP_NUM_THREADS=1 && pytest src -v"
+test = "export OMP_NUM_THREADS=1 && pytest src -v -s"
 
 [dependencies]
 python = ">=3.9,<3.11"
 numpy = ">=1.26.3"
 transonic = ">=0.6.4"
 # should actually be >=0.6.2 (soon available)
 fluiddyn = ">=0.6.1"
```

### Comparing `fluidimage-0.4.6/pylintrc` & `fluidimage-0.5.0/pylintrc`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/pyproject.toml` & `fluidimage-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "transonic>=0.6.2",
     "pythran>=0.9.7",
 ]
 build-backend = 'mesonpy'
 
 [project]
 name = "fluidimage"
-version = "0.4.6"
+version = "0.5.0"
 description = "Fluid image processing with Python."
 authors = [
     {name = "Pierre Augier", email = "pierre.augier@legi.cnrs.fr"},
 ]
 dependencies = [
     "numpy >= 1.8",
     "matplotlib >= 3.5",
```

### Comparing `fluidimage-0.4.6/src/fluidimage/__init__.py` & `fluidimage-0.5.0/src/fluidimage/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/_opencv.py` & `fluidimage-0.5.0/src/fluidimage/_opencv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/_evaluate_subpix.py` & `fluidimage-0.5.0/src/fluidimage/calcul/_evaluate_subpix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/correl.cu` & `fluidimage-0.5.0/src/fluidimage/calcul/correl.cu`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/correl.py` & `fluidimage-0.5.0/src/fluidimage/calcul/correl.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/correl_pycuda.py` & `fluidimage-0.5.0/src/fluidimage/calcul/correl_pycuda.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/fft.py` & `fluidimage-0.5.0/src/fluidimage/calcul/fft.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/interpolate/griddata.py` & `fluidimage-0.5.0/src/fluidimage/calcul/interpolate/griddata.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py` & `fluidimage-0.5.0/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from .thin_plate_spline import (
     ThinPlateSpline,
     ThinPlateSplineNumpy,
-    compute_tps_coeff,
+    compute_tps_weights,
 )
 
 pi = np.pi
 
 
 def test_tps():
     n0 = 10
@@ -25,14 +25,14 @@
     XI, YI = np.meshgrid(xI, yI)
     XI = XI.ravel()
     YI = YI.ravel()
 
     new_positions = np.vstack([XI, YI])
 
     # calculate tps coeff
-    U_smooth, U_tps = compute_tps_coeff(centers, U, 0)
+    U_smooth, U_tps = compute_tps_weights(centers, U, 0)
     # evaluate interpolation on the new grid
     tps = ThinPlateSpline(new_positions, centers)
     tps.compute_field(U_tps)
     tps.compute_gradient(U_tps)
 
     ThinPlateSplineNumpy(new_positions, centers)
```

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/interpolate/thin_plate_spline.py` & `fluidimage-0.5.0/src/fluidimage/calcul/interpolate/thin_plate_spline.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 Translated and adapted from UVmat code (Joel Sommeria, LEGI, CNRS).
 
 This interpolation/smoothing (Duchon, 1976; NguyenDuc and Sommeria,
 1988) minimises a linear combination of the squared curvature and
 squared difference from the initial data.
 
 We first need to compute tps coefficients ``U_tps`` (function
-``compute_tps_coeff``). Interpolated data can then be obtained as the
+``compute_tps_weights``). Interpolated data can then be obtained as the
 matrix product ``dot(U_tps, EM)`` where the matrix ``EM`` is obtained
 by the function ``compute_tps_matrix``.  The spatial derivatives are
 obtained as ``dot(U_tps, EMDX)`` and ``dot(U_tps, EMDY)``, where
 ``EMDX`` and ``EMDY`` are obtained from the function
 ``compute_tps_matrix_dxy``. A helper class is also provided.
 
-.. autofunction:: compute_tps_coeff
+.. autofunction:: compute_tps_weights
 
 .. autoclass:: ThinPlateSpline
    :members:
 
 .. autofunction:: compute_tps_matrix_numpy
 
 .. autofunction:: compute_tps_matrices_dxy
@@ -161,68 +161,63 @@
         )
 
 else:
     print("Warning: function compute_tps_matrix_numpy not pythranized.")
     compute_tps_matrix = compute_tps_matrix_numpy
 
 
-def compute_tps_coeff(centers, U, smoothing_coef):
+def compute_tps_weights(centers, values, smoothing_coef):
     """Calculate the thin plate spline (tps) coefficients
 
     Parameters
     ----------
 
     centers : np.array
         ``[nb_dim,  N]`` array representing the positions of the N centers,
         sources of the TPS (nb_dim = space dimension).
 
-    U : np.array
+    values : np.array
         ``[N]`` array representing the values of the considered
         scalar measured at the centres ``centers``.
 
     smoothing_coef : float
         Smoothing parameter. The result is smoother for larger smoothing_coef.
 
     Returns
     -------
 
-    U_smooth : np.array
+    smoothed_values : np.array
          Values of the quantity U at the N centres after smoothing.
 
-    U_tps : np.array
+    tps_weights : np.array
          TPS weights of the centres and columns of the linear.
 
     """
-    nb_dim, N = centers.shape
-    U = np.hstack([U, np.zeros(nb_dim + 1)])
-    U = U.reshape([U.size, 1])
+    nb_dim, num_values = centers.shape
+    values = np.hstack([values, np.zeros(nb_dim + 1)])
+    values = values.reshape([values.size, 1])
     try:
         EM = compute_tps_matrix(centers, centers).T
     except TypeError as e:
         print(centers.dtype, centers.shape)
         raise e
 
-    smoothing_mat = smoothing_coef * np.eye(N, N)
-    smoothing_mat = np.hstack([smoothing_mat, np.zeros([N, nb_dim + 1])])
-    PM = np.hstack([np.ones([N, 1]), centers.T])
+    smoothing_mat = smoothing_coef * np.eye(num_values, num_values)
+    smoothing_mat = np.hstack([smoothing_mat, np.zeros([num_values, nb_dim + 1])])
+    PM = np.hstack([np.ones([num_values, 1]), centers.T])
     IM = np.vstack(
         [
             EM + smoothing_mat,
             np.hstack([PM.T, np.zeros([nb_dim + 1, nb_dim + 1])]),
         ]
     )
 
-    # print('det(IM)', np.linalg.det(IM))
-    # print('cond(IM)', np.linalg.cond(IM))
-
-    # U_tps, r, r2, r3 = np.linalg.lstsq(IM, U)
-    U_tps = np.linalg.solve(IM, U)
-
-    U_smooth = np.dot(EM, U_tps)
-    return U_smooth.ravel(), U_tps.ravel()
+    tps_weights = np.linalg.solve(IM, values)
+    smoothed_values = np.dot(EM, tps_weights)
+    return smoothed_values.ravel(), tps_weights.ravel()
 
 
 def compute_tps_matrices_dxy(dsites, centers):
     """Calculate the derivatives of thin plate spline (tps) interpolation
     at a set of points (limited to the 2D case)
 
     Parameters
```

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/mean_neighbors.py` & `fluidimage-0.5.0/src/fluidimage/calcul/mean_neighbors.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png` & `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/reduction_kernel.cu` & `fluidimage-0.5.0/src/fluidimage/calcul/reduction_kernel.cu`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/subpix.py` & `fluidimage-0.5.0/src/fluidimage/calcul/subpix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/test_correl.py` & `fluidimage-0.5.0/src/fluidimage/calcul/test_correl.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calcul/test_fft.py` & `fluidimage-0.5.0/src/fluidimage/calcul/test_fft.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/calib2d_simple.py` & `fluidimage-0.5.0/src/fluidimage/calibration/calib2d_simple.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/calib_cv.py` & `fluidimage-0.5.0/src/fluidimage/calibration/calib_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/calib_direct.py` & `fluidimage-0.5.0/src/fluidimage/calibration/calib_direct.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/calib_tsai.py` & `fluidimage-0.5.0/src/fluidimage/calibration/calib_tsai.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/test_calib_cv.py` & `fluidimage-0.5.0/src/fluidimage/calibration/test_calib_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/test_direct_stereo_reconstruction.py` & `fluidimage-0.5.0/src/fluidimage/calibration/test_direct_stereo_reconstruction.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/test_tsai_calibration.py` & `fluidimage-0.5.0/src/fluidimage/calibration/test_tsai_calibration.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/calibration/util.py` & `fluidimage-0.5.0/src/fluidimage/calibration/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/config.py` & `fluidimage-0.5.0/src/fluidimage/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+"""Handle Fluidimage configuration"""
+
 import os
 from configparser import ConfigParser
 
 
 def get_config():
+    """Get configuration from .fluidimagerc"""
     config = ConfigParser()
 
     home = os.path.expanduser("~")
     path_config = os.path.join(home, ".fluidimagerc")
 
-    if os.path.exists(path_config):
-        config.read(path_config)
+    if not os.path.exists(path_config):
+        return {}
+    config.read(path_config)
 
     config_dict = {}
     for section in config.sections():
         section_dict = {}
         for option in config.options(section):
             value = config.get(section, option)
             if value.lower in ["true", "false"]:
```

### Comparing `fluidimage-0.4.6/src/fluidimage/conftest.py` & `fluidimage-0.5.0/src/fluidimage/conftest.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/data_objects/display_piv.py` & `fluidimage-0.5.0/src/fluidimage/data_objects/display_piv.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,20 @@
             ax0.set_ylim(ylim)
 
         ax0.set_xlabel("pixels")
         ax0.set_ylabel("pixels")
 
         if piv_results is not None:
             if show_interp:
-                if hasattr(piv_results, "deltaxs_approx"):
+                if show_interp == "smooth":
+                    deltaxs = piv_results.deltaxs_smooth
+                    deltays = piv_results.deltays_smooth
+                    xs = piv_results.xs_smooth
+                    ys = piv_results.ys_smooth
+                elif hasattr(piv_results, "deltaxs_approx"):
                     deltaxs = piv_results.deltaxs_approx
                     deltays = piv_results.deltays_approx
                     xs = piv_results.ixvecs_approx
                     ys = piv_results.iyvecs_approx
                 else:
                     deltaxs = piv_results.deltaxs_final
                     deltays = piv_results.deltays_final
```

### Comparing `fluidimage-0.4.6/src/fluidimage/data_objects/display_pre.py` & `fluidimage-0.5.0/src/fluidimage/data_objects/display_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/data_objects/piv.py` & `fluidimage-0.5.0/src/fluidimage/data_objects/piv.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,28 +242,37 @@
       Positions in pixels of the vectors in ``deltaxs_approx``, ``deltays_approx``.
 
     deltaxs_final, deltays_final, ixvecs_final, iyvecs_final:
 
       Equivalent to the `_approx` variables but for the last pass
       and of size ``num_vectors``.
 
+    deltaxs_smooth, deltays_smooth:
+
+      Smoothed displacements at the positions ``xs_smooth``, ``ys_smooth``,
+      equal to ``xs``, ``ys`` except where the vectors are detected as wrong.
+      (present only for TPS interpolation).
     """
 
     _keys_to_be_saved = [
         "xs",
         "ys",
+        "xs_smooth",
+        "ys_smooth",
         "deltaxs",
         "deltays",
         "correls_max",
         "deltaxs_approx",
         "deltays_approx",
         "ixvecs_approx",
         "iyvecs_approx",
         "deltaxs_final",
         "deltays_final",
+        "deltaxs_smooth",
+        "deltays_smooth",
         "ixvecs_final",
         "iyvecs_final",
     ]
 
     _dict_to_be_saved = ["errors", "deltaxs_wrong", "deltays_wrong"]
 
     def __init__(
@@ -383,15 +392,18 @@
 
         g_piv = file.create_group(tag)
         g_piv.attrs["class_name"] = "HeavyPIVResults"
         g_piv.attrs["module_name"] = "fluidimage.data_objects.piv"
 
         for k in self._keys_to_be_saved:
             if k in self.__dict__ and self.__dict__[k] is not None:
-                g_piv.create_dataset(k, data=self.__dict__[k])
+                arr = self.__dict__[k]
+                if arr.dtype == np.float64:
+                    arr = arr.astype(np.float32)
+                g_piv.create_dataset(k, data=arr)
 
         for name_dict in self._dict_to_be_saved:
             try:
                 d = self.__dict__[name_dict]
                 if d is None:
                     raise KeyError
             except KeyError:
```

### Comparing `fluidimage-0.4.6/src/fluidimage/data_objects/preproc.py` & `fluidimage-0.5.0/src/fluidimage/data_objects/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/data_objects/tomo.py` & `fluidimage-0.5.0/src/fluidimage/data_objects/tomo.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/__init__.py` & `fluidimage-0.5.0/src/fluidimage/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/base.py` & `fluidimage-0.5.0/src/fluidimage/executors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,14 +449,15 @@
                 self._has_to_stop = True
                 for process in self.processes:
                     os.kill(process.pid, signal_number)
 
             signal.signal(12, handler_signals)
 
         self._start_processes()
+        self.nb_processes = len(self.processes)
         self._wait_for_all_processes()
         self._finalize_compute()
 
     def _poll_return_code(self, process):
         return process.poll()
 
     def _join_processes(self):
```

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/exec_async.py` & `fluidimage-0.5.0/src/fluidimage/executors/exec_async.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/exec_async_multiproc.py` & `fluidimage-0.5.0/src/fluidimage/executors/exec_async_multiproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/exec_async_seq_for_multi.py` & `fluidimage-0.5.0/src/fluidimage/executors/exec_async_seq_for_multi.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/exec_async_sequential.py` & `fluidimage-0.5.0/src/fluidimage/executors/exec_async_sequential.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/exec_async_servers.py` & `fluidimage-0.5.0/src/fluidimage/executors/exec_async_servers.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/exec_sequential.py` & `fluidimage-0.5.0/src/fluidimage/executors/exec_sequential.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/multi_exec_async.py` & `fluidimage-0.5.0/src/fluidimage/executors/multi_exec_async.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/multi_exec_subproc.py` & `fluidimage-0.5.0/src/fluidimage/executors/multi_exec_subproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/executors/servers.py` & `fluidimage-0.5.0/src/fluidimage/executors/servers.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/base_matplotlib.py` & `fluidimage-0.5.0/src/fluidimage/gui/base_matplotlib.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/imviewer.py` & `fluidimage-0.5.0/src/fluidimage/gui/imviewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/launcher/main.py` & `fluidimage-0.5.0/src/fluidimage/gui/launcher/main.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/launcher/mainwindow.py` & `fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/launcher/mainwindow.ui` & `fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/launcher/test_launcher.py` & `fluidimage-0.5.0/src/fluidimage/gui/launcher/test_launcher.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/monitor.py` & `fluidimage-0.5.0/src/fluidimage/gui/monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     TabbedContent,
     TabPane,
     Tree,
 )
 
 import fluidimage
 from fluidimage import ParamContainer
+from fluidimage.util import format_time_in_seconds
 
 
 def build_branch(branch, params_node):
     """Build the branches of the tree"""
     for key in params_node._get_key_attribs():
         branch.add_leaf(f"{key} = {repr(params_node[key])}")
 
@@ -49,23 +50,14 @@
     """Copy the documentation between 2 ParamContainer objects"""
     params_node._set_doc(params_node_with_doc._doc)
 
     for tag in params_node._tag_children:
         copy_doc(params_node[tag], params_node_with_doc[tag])
 
 
-def format_time_in_seconds(duration_in_s):
-    """return a formatted str of the duration"""
-    if duration_in_s < 60:
-        return f"{duration_in_s:.2f} s"
-    hours, remainder = divmod(duration_in_s, 3600)
-    minutes, seconds = divmod(remainder, 60)
-    return f"{int(hours):02}:{int(minutes):02}:{int(seconds):02}"
-
-
 class MonitorApp(App):
     """Fluidimage monitor Textual app"""
 
     progress_bar: ProgressBar
     tree_params: Tree
     timer_update_info: Timer
     digit_num_results: Digits
@@ -297,15 +289,15 @@
 
         if self.job_is_running:
             result = f"Started since {duration_str}"
         else:
             result = f"Total duration: {duration_str}"
 
         if self.num_results:
-            result += f" ({duration_in_s * self.info_job['nb_max_workers'] / self.num_results:.2f} s.CPU/result)"
+            result += f" ({duration_in_s * self.info_job['nb_cpus_allowed'] / self.num_results:.2f} s.CPU/result)"
 
         return result
 
     def action_launch_fluidpivviewer(self) -> None:
         """Launch fluidpivviewer from the result directory"""
         print("launching fluidpivviewer")
         subprocess.run(["fluidpivviewer", str(self.path_results)], check=False)
```

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/pg_main.py` & `fluidimage-0.5.0/src/fluidimage/gui/pg_main.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/pg_wrapper.py` & `fluidimage-0.5.0/src/fluidimage/gui/pg_wrapper.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/piv_viewer.py` & `fluidimage-0.5.0/src/fluidimage/gui/piv_viewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/test_imviewer.py` & `fluidimage-0.5.0/src/fluidimage/gui/test_imviewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/test_imviewer_pg.py` & `fluidimage-0.5.0/src/fluidimage/gui/test_imviewer_pg.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/test_monitor.py` & `fluidimage-0.5.0/src/fluidimage/gui/test_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 import sys
 
 import pytest
 
 from fluidimage.executors import supported_multi_executors
-from fluidimage.gui.monitor import MonitorApp, main, format_time_in_seconds
+from fluidimage.gui.monitor import MonitorApp, format_time_in_seconds, main
 from fluidimage.piv import TopologyPIV
 
 postfix = "test_monitor"
 
 
 def test_monitor_help(monkeypatch):
```

### Comparing `fluidimage-0.4.6/src/fluidimage/gui/test_piv_viewer.py` & `fluidimage-0.5.0/src/fluidimage/gui/test_piv_viewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/image2image.py` & `fluidimage-0.5.0/src/fluidimage/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/meson.build` & `fluidimage-0.5.0/src/fluidimage/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   'optical_flow.py',
   'piv.py',
   'preproc.py',
   'run_from_xml.py',
   'synthetic.py',
   'test_image2image.py',
   'test_run_from_xml.py',
+  'uvmat.py',
 ]
 
 py.install_sources(
   python_sources,
   subdir: 'fluidimage'
 )
```

### Comparing `fluidimage-0.4.6/src/fluidimage/postproc/piv.py` & `fluidimage-0.5.0/src/fluidimage/postproc/piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/postproc/postproc.py` & `fluidimage-0.5.0/src/fluidimage/postproc/postproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/postproc/test_piv.py` & `fluidimage-0.5.0/src/fluidimage/postproc/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/postproc/test_util.py` & `fluidimage-0.5.0/src/fluidimage/postproc/test_util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/postproc/util.py` & `fluidimage-0.5.0/src/fluidimage/postproc/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/postproc/vector_field.py` & `fluidimage-0.5.0/src/fluidimage/postproc/vector_field.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/preproc.py` & `fluidimage-0.5.0/src/fluidimage/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/reconstruct/tomo/mlos.py` & `fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/mlos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/reconstruct/tomo/test_mlos.py` & `fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/test_mlos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/run_from_xml.py` & `fluidimage-0.5.0/src/fluidimage/uvmat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,148 @@
-"""Uvmat interface
-==================
+"""UVmat interface
 
-From Matlab, something like::
+.. autofunction:: tidy_uvmat_instructions
 
-  system(['python -m fluidimage.run_from_xml ' path_to_instructions_xml])
+.. autoclass:: ActionBase
+   :members:
+   :private-members:
 
-
-.. todo::
-
-   UVmat civserie: input and output.
+.. autoclass:: ActionPIVFromUvmatXML
+   :members:
+   :private-members:
 
 """
 
-import argparse
 import os
 from abc import ABC, abstractmethod
+from logging import warning
 from time import time
 
-from fluiddyn import time_as_str
-from fluiddyn.util import import_class
 from fluiddyn.util.paramcontainer import tidy_container
 from fluidimage.topologies.piv import TopologyPIV
-
-from . import (  # SerieOfArraysFromFiles,
-    ParamContainer,
-    config_logging,
-    logger,
-    reset_logger,
-)
-
-# import numpy as np
-# import scipy
+from fluidimage.util import format_time_in_seconds
 
 
-def tidy_uvmat_instructions(params):
-    params._set_internal_attr("_tag", "instructions_uvmat")
+def tidy_uvmat_instructions(instructions):
+    """Clean up UVmat instructions with nicer names and a simpler organization"""
+    instructions._set_internal_attr("_tag", "instructions_uvmat")
 
-    # get nicer names and a simpler organization...
-    tidy_container(params)
+    tidy_container(instructions)
 
-    params.input_table = input_table = params.input_table.split(" & ")
+    instructions.input_table = input_table = instructions.input_table.split(" & ")
     for i in range(1, len(input_table)):
         if input_table[i].startswith("/"):
             input_table[i] = input_table[i][1:]
 
-    filename = "".join(input_table[2:])
     path_dir = os.path.join(*input_table[:2])
+    input_table[3] = "*"
+    filename = "".join(input_table[2:])
     path_file_input = os.path.abspath(os.path.join(path_dir, filename))
     path_dir_input = path_dir
-    params._set_attrib("path_dir_input", path_dir_input)
-    params._set_attrib("path_file_input", path_file_input)
-
-    params._set_attrib("path_dir_output", path_dir_input + params.output_dir_ext)
-
-    ir = params.index_range
-    if not hasattr(ir, "incr_i"):
-        ir._set_attrib("incr_i", 1)
+    instructions._set_attrib("path_dir_input", path_dir_input)
+    instructions._set_attrib("path_file_input", path_file_input)
+    instructions._set_attrib(
+        "path_dir_output", path_dir_input + instructions.output_dir_ext
+    )
 
-    if not hasattr(ir, "first_i"):
-        print("Warning: no attribute first_i in xml UVmat file.")
-        ir._set_attrib("first_i", 1)
 
-    if not hasattr(ir, "last_i"):
-        print("Warning: no attribute last_i in xml UVmat file.")
-        ir._set_attrib("last_i", None)
+class ActionBase(ABC):
+    """Abstract class to represent UVmat 'actions'"""
 
-    if not hasattr(ir, "first_j"):
-        str_subset = f"i:i+{ir.incr_i + 1}:{ir.incr_i}"
-        ind_start = ir.first_i
+    name: str
+    computer_cls: type
 
-        if ir.last_i is None:
-            ind_stop = None
+    @classmethod
+    @abstractmethod
+    def params_from_uvmat_xml(cls, instructions):
+        """Create fluidimage params from UVmat xml"""
+        print("UVmat instructions:", instructions._make_xml_text(), sep="\n")
+        params = cls.computer_cls.create_default_params()
+        params.saving.path = instructions.path_dir_output
+        params.saving.how = "recompute"
+        cls.set_params_series(params, instructions)
+        return params
+
+    @classmethod
+    def set_params_series(cls, params, instructions):
+        """Set params.series from UVmat xml"""
+        ir = instructions.index_range
+
+        pair_indices = instructions.action_input.pair_indices
+        pair_mode = pair_indices.list_pair_mode
+
+        if pair_mode in ["series(Di)", "pair j1-j2"]:
+            ind_start = ir.first_i
+
+            try:
+                ind_step = ir.incr_i
+            except AttributeError:
+                ind_step = 1
+
+            try:
+                ind_stop = ir.last_i + 1
+            except AttributeError:
+                ind_stop = None
+
+        elif pair_mode == "series(Dj)":
+
+            ind_start = ir.first_j
+
+            try:
+                ind_step = ir.incr_j
+            except AttributeError:
+                ind_step = 1
+
+            try:
+                ind_stop = ir.last_j + 1
+            except AttributeError:
+                ind_stop = None
+
+        if pair_mode == "pair j1-j2":
+            if not pair_indices.list_pair_civ1.startswith("j= a-b"):
+                raise NotImplementedError(f"{pair_indices.list_pair_civ1 = }")
+            if pair_indices.list_pair_civ1 != "j= a-b":
+                warning(
+                    f"Do not know how to handle UVmat XML: {pair_indices.list_pair_civ1 = }"
+                )
+            str_subset = "i,0:2"
+        elif pair_mode == "series(Di)":
+            str_subset = "i:i+2:1"
+        elif pair_mode == "series(Dj)":
+            if ir.first_i != ir.last_i:
+                raise NotImplementedError("ir.first_i != ir.last_i")
+            str_subset = "{ir.first_i},i:i+2:1"
         else:
-            ind_stop = ir.last_i - ir.incr_i + 1
-    else:
-        raise NotImplementedError
-
-    params._set_attrib("str_subset", str_subset)
-    params._set_attrib("ind_stop", ind_stop)
-    params._set_attrib("ind_start", ind_start)
+            raise NotImplementedError(f"{pair_indices.list_pair_mode = }")
 
+        params.series.path = instructions.path_file_input
+        params.series.str_subset = str_subset
+        params.series.ind_start = ind_start
+        params.series.ind_step = ind_step
+        params.series.ind_stop = ind_stop
 
-class ActionBase(ABC):
-
-    @abstractmethod
-    def __init__(self, instructions, args):
+    def __init__(self, params):
         """Initialize the action class"""
+        self.params = params
+        print("Initialize Fluidimage computations with parameters:")
+        print(self.params._make_xml_text())
+        self.computer = self.computer_cls(self.params)
 
-    @abstractmethod
     def compute(self):
         """Perform the computation"""
+        t = time()
+        self.computer.compute()
+        t = time() - t
+        print(f"elapsed time: {format_time_in_seconds(t)}")
 
 
 # class ActionAverage(ActionBase):
 #     """Compute the average and save as a png file."""
 
-#     def __init__(self, instructions, args):
+#     def __init__(self, instructions):
 #         self.instructions = instructions
 
 #         # create the serie of arrays
 #         logger.info("Create the serie of arrays")
 #         self.serie_arrays = SerieOfArraysFromFiles(
 #             path=instructions.path_dir_input,
 #             slicing=instructions.slicing,
@@ -140,151 +183,53 @@
 #         mean /= nb_fields
 
 #         logger.info("Save in file:\n%s", path_save)
 #         scipy.misc.imsave(path_save, mean)
 #         return mean
 
 
-def params_piv_from_uvmat_xml(instructions, args):
-    params = TopologyPIV.create_default_params()
-
-    params.series.path = instructions.path_file_input
-
-    params.series.str_subset = instructions.str_subset
-    params.series.ind_stop = instructions.ind_stop
-    params.series.ind_start = instructions.ind_start
-
-    params.saving.path = instructions.path_dir_output
-
-    n0 = int(instructions.action_input.civ1.search_box_size.split("\t")[0])
-    if n0 % 2 == 1:
-        n0 -= 1
-
-    params.piv0.shape_crop_im0 = n0
-
-    if hasattr(instructions.action_input, "patch2"):
-        params.multipass.subdom_size = (
-            instructions.action_input.patch2.sub_domain_size
-        )
-    else:
-        params.multipass.use_tps = False
-
-    if hasattr(instructions.action_input, "civ2"):
-        params.multipass.number = 2
-
-    modif_fluidimage_params(params, args)
-
-    return params
-
-
 class ActionPIVFromUvmatXML(ActionBase):
     """Compute the average and save as a png file."""
 
-    def __init__(self, instructions, args):
-        self.instructions = instructions
-        self.params = params_piv_from_uvmat_xml(instructions, args)
-        logger.info("Initialize Fluidimage computations with parameters:")
-        logger.info(self.params._make_xml_text())
-        self.topology = TopologyPIV(self.params)
-
-    def compute(self):
-        t = time()
-        self.topology.compute()
-        t = time() - t
-        print(f"elapsed time: {t} s")
-
-
-# actions_classes = {"aver_stat": ActionAverage, "civ_series": ActionPIVFromUvmatXML}
-actions_classes = {"civ_series": ActionPIVFromUvmatXML}
-
-programs = ["uvmat", "fluidimage"]
-
-
-def parse_args():
-    parser = argparse.ArgumentParser(
-        description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
-    )
-    parser.add_argument("path", help="Path file.", type=str, nargs="?")
-    parser.add_argument(
-        "-m",
-        "--mode",
-        help="'ask', 'new_dir', 'complete' or 'recompute'.",
-        type=str,
-        default=None,
-    )
-
-    return parser.parse_args()
+    name = "civ_series"
+    computer_cls = TopologyPIV
 
+    @classmethod
+    def params_from_uvmat_xml(cls, instructions):
+        params = super().params_from_uvmat_xml(instructions)
 
-def modif_fluidimage_params(params, args):
-    if args.mode is not None:
-        try:
-            params.saving.how = args.mode
-        except AttributeError:
-            pass
-
+        action_input = instructions.action_input
 
-def main():
-    reset_logger()
-    config_logging("info")
+        n0 = int(action_input.civ1.search_box_size.split("\t")[0])
+        if n0 % 2 == 1:
+            n0 -= 1
 
-    args = parse_args()
+        params.piv0.shape_crop_im0 = n0
 
-    path_instructions_xml = args.path
-
-    params = ParamContainer(path_file=path_instructions_xml)
-
-    program = None
-    try:
-        params.Action.ActionName
-    except AttributeError:
-        try:
-            program = params._value_text["program"]
-        except (AttributeError, KeyError):
-            pass
-    else:
-        program = "uvmat"
-
-    if program not in programs:
-        raise ValueError("Can not detect the program to launch.")
-
-    logger.info(
-        "\n%s: using instructions in xml file:\n%s",
-        time_as_str(2),
-        path_instructions_xml,
-    )
+        if hasattr(action_input, "patch2"):
+            params.multipass.subdom_size = action_input.patch2.sub_domain_size
+            params.multipass.smoothing_coef = action_input.patch2.field_smooth
+            params.multipass.threshold_tps = action_input.patch2.max_diff
+        else:
+            params.multipass.use_tps = False
 
-    kwargs_compute = {}
+        if hasattr(action_input, "civ2"):
+            params.multipass.number = 2
 
-    if program == "uvmat":
-        tidy_uvmat_instructions(params)
-        action_name = params.action.action_name
-        logger.info(
-            'Check if the action "%s" is implemented by FluidImage', action_name
-        )
-        if action_name not in actions_classes.keys():
-            raise NotImplementedError(
-                'action "' + action_name + '" is not yet implemented.'
-            )
-
-        cls = actions_classes[action_name]
-        action = cls(params, args)
-
-    elif program == "fluidimage":
-        cls = import_class(
-            params._value_text["module"], params._value_text["class"]
-        )
-        modif_fluidimage_params(params, args)
-        action = cls(params)
+        fix = params.fix
+        fix.correl_min = action_input.fix1.min_corr
 
         try:
-            compute_kwargs = params.compute_kwargs
+            fix.displacement_max = action_input.fix1.max_vel
         except AttributeError:
             pass
-        else:
-            kwargs_compute = compute_kwargs._make_dict_tree()
 
-    return action.compute(**kwargs_compute)
+        return params
 
 
-if __name__ == "__main__":
-    result = main()
+actions_classes = {
+    cls.name: cls
+    for cls in locals().values()
+    if isinstance(cls, type)
+    and issubclass(cls, ActionBase)
+    and cls is not ActionBase
+}
```

### Comparing `fluidimage-0.4.6/src/fluidimage/synthetic.py` & `fluidimage-0.5.0/src/fluidimage/synthetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+"""Production of synthetic images"""
+
 import numpy as np
 
 
 def make_synthetic_images(
     displacements,
     nb_particles,
     shape_im0,
     shape_im1=None,
     epsilon=0.0,
     part_size=np.sqrt(1 / 0.5),
 ):
+    """Produce synthetic images for testing PIV"""
     ny, nx = tuple(shape_im0)
 
     displacement_x, displacement_y = tuple(displacements)
 
     xs = np.arange(nx, dtype="float32")
     ys = np.arange(ny, dtype="float32")
```

### Comparing `fluidimage-0.4.6/src/fluidimage/test_image2image.py` & `fluidimage-0.5.0/src/fluidimage/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/__init__.py` & `fluidimage-0.5.0/src/fluidimage/topologies/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/base.py` & `fluidimage-0.5.0/src/fluidimage/topologies/base.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/bos.py` & `fluidimage-0.5.0/src/fluidimage/topologies/bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/example.py` & `fluidimage-0.5.0/src/fluidimage/topologies/example.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/image2image.py` & `fluidimage-0.5.0/src/fluidimage/topologies/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/launcher.py` & `fluidimage-0.5.0/src/fluidimage/topologies/launcher.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/log.py` & `fluidimage-0.5.0/src/fluidimage/topologies/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,21 @@
         self.works_ended = data_main_file.works_ended
         self.nb_cpus_allowed = data_main_file.nb_cpus_allowed
         self.nb_max_workers = data_main_file.nb_max_workers
         self.executor_name = data_main_file.executor_name
         self.topology_name = data_main_file.topology_name
 
         self.mem_start = data_main_file.mem_start
-        self.mem_end = data_main_file.mem_end
+
+        try:
+            self.duration = data_main_file.duration
+        except AttributeError:
+            pass
+        else:
+            self.mem_end = data_main_file.mem_end
 
         self.paths_log_files = sorted(path_log_dir.glob("process_*.txt"))
         for path_log_process in self.paths_log_files:
             data = DataLogFile(path_log_process)
             self.works.extend(data.works)
             self.works_ended.extend(data.works_ended)
```

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/meson.build` & `fluidimage-0.5.0/src/fluidimage/topologies/meson.build`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/nb_cpu_cores.py` & `fluidimage-0.5.0/src/fluidimage/topologies/nb_cpu_cores.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/optical_flow.py` & `fluidimage-0.5.0/src/fluidimage/topologies/optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/piv.py` & `fluidimage-0.5.0/src/fluidimage/topologies/piv.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import copy
 import sys
 from pathlib import Path
 
 from fluidimage import ParamContainer, SeriesOfArrays
 from fluidimage.data_objects.piv import ArrayCouple, get_name_piv
 from fluidimage.topologies import TopologyBaseFromSeries, prepare_path_dir_result
+from fluidimage.topologies.nb_cpu_cores import nb_cores
 from fluidimage.topologies.splitters import SplitterFromSeries
 from fluidimage.util import imread, logger
 from fluidimage.works import image2image
 from fluidimage.works.piv import WorkPIV
 
 
 class TopologyPIV(TopologyBaseFromSeries):
@@ -239,15 +240,23 @@
         """Make a text printed at exit"""
         txt = f"Stop compute after t = {time_since_start:.2f} s"
         try:
             nb_results = len(self.results)
         except AttributeError:
             nb_results = None
         if nb_results is not None and nb_results > 0:
-            txt += f" ({nb_results} piv fields, {time_since_start / nb_results:.2f} s/field)."
+            try:
+                num_processes = self.executor.nb_processes
+            except AttributeError:
+                num_processes = self.executor.nb_max_workers
+            num_cores_used = min(nb_cores, num_processes)
+            txt += (
+                f" ({nb_results} piv fields, {time_since_start / nb_results:.2f} s/field,"
+                f" {time_since_start * num_cores_used / nb_results:.2f} s.CPU/field)."
+            )
         else:
             txt += "."
         txt += "\npath results:\n" + str(Path(self.path_dir_result).resolve())
         return txt
 
 
 Topology = TopologyPIV
```

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/preproc.py` & `fluidimage-0.5.0/src/fluidimage/topologies/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/splitters.py` & `fluidimage-0.5.0/src/fluidimage/topologies/splitters.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/surface_tracking.py` & `fluidimage-0.5.0/src/fluidimage/topologies/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_bos.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_example.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_example.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_image2image.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_optical_flow.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_piv.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_preproc.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_splitters.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_splitters.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/topologies/test_surftracking.py` & `fluidimage-0.5.0/src/fluidimage/topologies/test_surftracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/util/__init__.py` & `fluidimage-0.5.0/src/fluidimage/util/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     log_error,
     log_memory_usage,
     logger,
     reset_logger,
 )
 from .util import (
     cstring,
+    format_time_in_seconds,
     get_txt_memory_usage,
     imread,
     imsave,
     print_memory_usage,
     safe_eval,
     str_short,
 )
@@ -42,8 +43,9 @@
     "cstring",
     "str_short",
     "DEBUG",
     "log_debug",
     "log_error",
     "config_logging",
     "safe_eval",
+    "format_time_in_seconds",
 ]
```

### Comparing `fluidimage-0.4.6/src/fluidimage/util/log.py` & `fluidimage-0.5.0/src/fluidimage/util/log.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/util/util.py` & `fluidimage-0.5.0/src/fluidimage/util/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 .. autofunction:: is_memory_full
 
 .. autofunction:: str_short
 
 .. autofunction:: safe_eval
 
+.. autofunction:: format_time_in_seconds
+
 """
 
 from pathlib import Path
 
 import psutil
 from IPython.lib.pretty import pretty
 from simpleeval import EvalWithCompoundTypes
@@ -127,7 +129,16 @@
 
 _evaluator = EvalWithCompoundTypes()
 
 
 def safe_eval(source):
     """Save eval with simpleeval"""
     return _evaluator.eval(source)
+
+
+def format_time_in_seconds(duration_in_s):
+    """return a formatted str of the duration"""
+    if duration_in_s < 60:
+        return f"{duration_in_s:.2f} s"
+    hours, remainder = divmod(duration_in_s, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    return f"{int(hours):02}:{int(minutes):02}:{int(seconds):02}"
```

### Comparing `fluidimage-0.4.6/src/fluidimage/works/__init__.py` & `fluidimage-0.5.0/src/fluidimage/works/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/bos.py` & `fluidimage-0.5.0/src/fluidimage/works/bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/image2image.py` & `fluidimage-0.5.0/src/fluidimage/works/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/optical_flow.py` & `fluidimage-0.5.0/src/fluidimage/works/optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/piv/fix.py` & `fluidimage-0.5.0/src/fluidimage/works/piv/fix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/piv/multipass.py` & `fluidimage-0.5.0/src/fluidimage/works/piv/multipass.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         params._set_child(
             "multipass",
             attribs={
                 "number": 1,
                 "coeff_zoom": 2,
                 "use_tps": "last",
                 "subdom_size": 200,
-                "smoothing_coef": 0.5,
-                "threshold_tps": 1.0,
+                "smoothing_coef": 2.0,
+                "threshold_tps": 1.5,
             },
         )
 
         params.multipass._set_doc(
             """Multipass PIV parameters:
 
 - number : int (default 1)
@@ -89,15 +89,15 @@
 - subdom_size : int
 
   Number of vectors in the subdomains used for the TPS method.
 
 - smoothing_coef : float
 
   Coefficient used for the TPS method. The result is smoother for larger
-  smoothing_coef.
+  smoothing_coef. 2 is often reasonable. Can typically be between 0 to 40.
 
 - threshold_tps :  float
 
   Allowed difference of displacement (in pixels) between smoothed and input
   field for TPS filter used in an iterative filtering method. Vectors too far
   from the corresponding interpolated vector are removed.
```

### Comparing `fluidimage-0.4.6/src/fluidimage/works/piv/singlepass.py` & `fluidimage-0.5.0/src/fluidimage/works/piv/singlepass.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,17 +453,16 @@
 
         if not any(selection):
             raise InterpError("Only nan.")
 
         xs = piv_results.xs[selection]
         ys = piv_results.ys[selection]
 
-        xs, ys = self._xymasked_from_xyoriginalimage(xs, ys)
-
-        centers = np.vstack([ys, xs])
+        xs_tmp, ys_tmp = self._xymasked_from_xyoriginalimage(xs, ys)
+        centers = np.vstack([ys_tmp, xs_tmp])
 
         deltaxs = piv_results.deltaxs[selection]
         deltays = piv_results.deltays[selection]
 
         if (
             self.params.multipass.use_tps is True
             or self.params.multipass.use_tps == "last"
@@ -479,47 +478,61 @@
             )
 
             tps = ThinPlateSplineSubdom(
                 centers,
                 subdom_size,
                 smoothing_coef,
                 threshold=threshold,
-                percent_buffer_area=0.25,
+                percent_buffer_area=20,
             )
             try:
                 (
                     deltaxs_smooth,
                     deltaxs_tps,
                     summary,
-                ) = tps.compute_tps_coeff_subdom(deltaxs)
+                ) = tps.compute_tps_weights_subdom(deltaxs)
                 (
                     deltays_smooth,
                     deltays_tps,
                     summary,
-                ) = tps.compute_tps_coeff_subdom(deltays)
+                ) = tps.compute_tps_weights_subdom(deltays)
             except np.linalg.LinAlgError:
                 print("LinAlgError in TPS: compute delta_approx with griddata")
                 deltaxs_approx = griddata(
                     centers[::-1], deltaxs, (self.ixvecs, self.iyvecs)
                 )
                 deltays_approx = griddata(
                     centers[::-1], deltays, (self.ixvecs, self.iyvecs)
                 )
             else:
-                piv_results.deltaxs_smooth = deltaxs_smooth
                 piv_results.deltaxs_tps = deltaxs_tps
-                piv_results.deltays_smooth = deltays_smooth
                 piv_results.deltays_tps = deltays_tps
 
                 new_positions = np.vstack([self.iyvecs_grid, self.ixvecs_grid])
 
                 tps.init_with_new_positions(new_positions)
 
-                deltaxs_approx = tps.compute_eval(deltaxs_tps)
-                deltays_approx = tps.compute_eval(deltays_tps)
+                deltaxs_approx = tps.interpolate(deltaxs_tps)
+                deltays_approx = tps.interpolate(deltays_tps)
+
+                if last:
+                    xs_smooth = piv_results.ixvecs_final.copy().astype(np.float32)
+                    xs_smooth[selection] = xs
+                    ys_smooth = piv_results.iyvecs_final.copy().astype(np.float32)
+                    ys_smooth[selection] = ys
+
+                    deltaxs_smooth_full = deltaxs_approx.copy()
+                    deltaxs_smooth_full[selection] = deltaxs_smooth
+                    deltays_smooth_full = deltays_approx.copy()
+                    deltays_smooth_full[selection] = deltays_smooth
+
+                    piv_results.xs_smooth = xs_smooth
+                    piv_results.ys_smooth = ys_smooth
+                    piv_results.deltaxs_smooth = deltaxs_smooth_full
+                    piv_results.deltays_smooth = deltays_smooth_full
 
                 print("TPS summary: ", end="")
                 nb_fixed_vectors_tot = summary.pop("nb_fixed_vectors_tot")
                 if nb_fixed_vectors_tot > 0:
                     print(f'{nb_fixed_vectors_tot} "erratic" vectors changed.')
                 else:
                     print("no erratic vector found.")
```

### Comparing `fluidimage-0.4.6/src/fluidimage/works/piv/test_piv.py` & `fluidimage-0.5.0/src/fluidimage/works/piv/test_piv.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     # for a very short computation
     params.piv0.shape_crop_im0 = 32
     params.piv0.grid.overlap = -3
 
     params.piv0.nb_peaks_to_search = 2
 
     params.multipass.number = 2
+    params.multipass.use_tps = True
 
     params.fix.displacement_max = 3
     params.fix.threshold_diff_neighbour = 2
 
     params.series.path = str(path_images / "Oseen*")
     params.series.str_subset = "i+1:i+3"
```

### Comparing `fluidimage-0.4.6/src/fluidimage/works/preproc/__init__.py` & `fluidimage-0.5.0/src/fluidimage/works/preproc/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/preproc/_toolbox_cv.py` & `fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/preproc/_toolbox_py.py` & `fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_py.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/preproc/io.py` & `fluidimage-0.5.0/src/fluidimage/works/preproc/io.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/preproc/toolbox.py` & `fluidimage-0.5.0/src/fluidimage/works/preproc/toolbox.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/surface_tracking.py` & `fluidimage-0.5.0/src/fluidimage/works/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/test_bos.py` & `fluidimage-0.5.0/src/fluidimage/works/test_bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/test_image2image.py` & `fluidimage-0.5.0/src/fluidimage/works/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/test_preproc.py` & `fluidimage-0.5.0/src/fluidimage/works/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/src/fluidimage/works/with_mask.py` & `fluidimage-0.5.0/src/fluidimage/works/with_mask.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.4.6/PKG-INFO` & `fluidimage-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidimage
-Version: 0.4.6
+Version: 0.5.0
 Summary: Fluid image processing with Python.
 Keywords: PIV
 Author-Email: Pierre Augier <pierre.augier@legi.cnrs.fr>
 License: CeCILL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

