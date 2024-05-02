# Comparing `tmp/burst2safe-0.3.1.tar.gz` & `tmp/burst2safe-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burst2safe-0.3.1.tar", last modified: Tue Apr 30 13:08:37 2024, max compression
+gzip compressed data, was "burst2safe-0.3.2.tar", last modified: Thu May  2 15:34:45 2024, max compression
```

## Comparing `burst2safe-0.3.1.tar` & `burst2safe-0.3.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.997810 burst2safe-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.921810 burst2safe-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.925810 burst2safe-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/build-and-deploy-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/build-and-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/bump-version.yml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/changelog-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/labeled-pr-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/pytest-golden.yml
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/pytest-integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/release-checklist-comment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-30 13:08:30.000000 burst2safe-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-30 13:08:30.000000 burst2safe-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-30 13:08:30.000000 burst2safe-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-30 13:08:36.997810 burst2safe-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-30 13:08:30.000000 burst2safe-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 13:08:30.000000 burst2safe-0.3.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-30 13:08:30.000000 burst2safe-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:08:36.997810 burst2safe-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.921810 burst2safe-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.925810 burst2safe-0.3.1/src/burst2safe/
--rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/burst2safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.921810 burst2safe-0.3.1/src/burst2safe/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.929810 burst2safe-0.3.1/src/burst2safe/data/support_236/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_236/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_236/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_236/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147288 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_236/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_236/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.929810 burst2safe-0.3.1/src/burst2safe/data/support_245/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_245/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_245/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_245/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147222 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_245/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_245/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.929810 burst2safe-0.3.1/src/burst2safe/data/support_260/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_260/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_260/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_260/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_260/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_260/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.933810 burst2safe-0.3.1/src/burst2safe/data/support_290/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_290/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_290/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_290/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_290/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_290/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.933810 burst2safe-0.3.1/src/burst2safe/data/support_340/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-rfi.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    61552 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_340/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.933810 burst2safe-0.3.1/src/burst2safe/data/support_371/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-rfi.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/data/support_371/s1-object-types.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/swath.py
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-30 13:08:30.000000 burst2safe-0.3.1/src/burst2safe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.997810 burst2safe-0.3.1/src/burst2safe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-30 13:08:36.000000 burst2safe-0.3.1/src/burst2safe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-30 13:08:36.000000 burst2safe-0.3.1/src/burst2safe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:08:36.000000 burst2safe-0.3.1/src/burst2safe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 13:08:36.000000 burst2safe-0.3.1/src/burst2safe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:08:36.000000 burst2safe-0.3.1/src/burst2safe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 13:08:36.000000 burst2safe-0.3.1/src/burst2safe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 13:08:36.000000 burst2safe-0.3.1/src/burst2safe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.937810 burst2safe-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.937810 burst2safe-0.3.1/tests/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/etc/identify_ipf_differences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_burst2safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.953810 burst2safe-0.3.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)  6288473 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6073763 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:08:36.989810 burst2safe-0.3.1/tests/test_data/ipf/
--rw-r--r--   0 runner    (1001) docker     (127)  5647017 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6067536 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6114849 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6350843 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6564579 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6345069 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_data/manifest_7C85.safe
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_golden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_ipf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_swath.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-30 13:08:30.000000 burst2safe-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.171597 burst2safe-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.099596 burst2safe-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.099596 burst2safe-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/build-and-deploy-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/build-and-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/bump-version.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/changelog-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/labeled-pr-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/pytest-golden.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/pytest-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/release-checklist-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-02 15:34:39.000000 burst2safe-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-02 15:34:39.000000 burst2safe-0.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-02 15:34:39.000000 burst2safe-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-02 15:34:45.171597 burst2safe-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-02 15:34:39.000000 burst2safe-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-02 15:34:39.000000 burst2safe-0.3.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 15:34:39.000000 burst2safe-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:34:45.175597 burst2safe-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.095596 burst2safe-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.103596 burst2safe-0.3.2/src/burst2safe/
+-rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.095596 burst2safe-0.3.2/src/burst2safe/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.103596 burst2safe-0.3.2/src/burst2safe/data/support_236/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_236/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_236/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_236/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147288 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_236/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_236/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.107596 burst2safe-0.3.2/src/burst2safe/data/support_245/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_245/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_245/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_245/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147222 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_245/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_245/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.107596 burst2safe-0.3.2/src/burst2safe/data/support_260/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_260/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_260/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_260/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_260/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_260/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.107596 burst2safe-0.3.2/src/burst2safe/data/support_290/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_290/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_290/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_290/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_290/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_290/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.107596 burst2safe-0.3.2/src/burst2safe/data/support_340/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-rfi.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    61552 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_340/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.111596 burst2safe-0.3.2/src/burst2safe/data/support_371/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-rfi.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/data/support_371/s1-object-types.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-02 15:34:39.000000 burst2safe-0.3.2/src/burst2safe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.171597 burst2safe-0.3.2/src/burst2safe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-02 15:34:44.000000 burst2safe-0.3.2/src/burst2safe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-02 15:34:45.000000 burst2safe-0.3.2/src/burst2safe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:34:44.000000 burst2safe-0.3.2/src/burst2safe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 15:34:44.000000 burst2safe-0.3.2/src/burst2safe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:34:44.000000 burst2safe-0.3.2/src/burst2safe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 15:34:44.000000 burst2safe-0.3.2/src/burst2safe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 15:34:44.000000 burst2safe-0.3.2/src/burst2safe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.111596 burst2safe-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.111596 burst2safe-0.3.2/tests/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/etc/identify_ipf_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.127596 burst2safe-0.3.2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  6288473 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6073763 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:34:45.163597 burst2safe-0.3.2/tests/test_data/ipf/
+-rw-r--r--   0 runner    (1001) docker     (127)  5647017 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6067536 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6114849 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6350843 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6564579 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6345069 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_data/manifest_7C85.safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_golden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_ipf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-02 15:34:39.000000 burst2safe-0.3.2/tests/test_utils.py
```

### Comparing `burst2safe-0.3.1/.github/workflows/build-and-deploy-test.yml` & `burst2safe-0.3.2/.github/workflows/build-and-deploy-test.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/.github/workflows/build-and-deploy.yml` & `burst2safe-0.3.2/.github/workflows/build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/.github/workflows/pytest-golden.yml` & `burst2safe-0.3.2/.github/workflows/pytest-golden.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/.github/workflows/pytest-integration.yml` & `burst2safe-0.3.2/.github/workflows/pytest-integration.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/.github/workflows/pytest.yml` & `burst2safe-0.3.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/.github/workflows/static-analysis.yml` & `burst2safe-0.3.2/.github/workflows/static-analysis.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/.gitignore` & `burst2safe-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/CHANGELOG.md` & `burst2safe-0.3.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/)
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.2]
+
+### Fixed
+* Bug introduced in `0.3.1` where the `download_bursts` function would not work for a single worker.
+
 ## [0.3.1]
 
 ### Fixed
 * Race condition in `download_bursts` function by switching to parallel, instead of threaded, downloads.
 
 ## [0.3.0]
```

### Comparing `burst2safe-0.3.1/LICENSE` & `burst2safe-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/PKG-INFO` & `burst2safe-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `burst2safe-0.3.1/README.md` & `burst2safe-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/pyproject.toml` & `burst2safe-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/base.py` & `burst2safe-0.3.2/src/burst2safe/base.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/burst2safe.py` & `burst2safe-0.3.2/src/burst2safe/burst2safe.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,16 @@
         downloads[burst_info.metadata_path] = burst_info.metadata_url
     download_info = [(value, key.parent, key.name) for key, value in downloads.items()]
     urls, dirs, names = zip(*download_info)
 
     session = asf_search.ASFSession()
     n_workers = min(len(urls), max(cpu_count() - 2, 1))
     if n_workers == 1:
-        asf_search.download_url(urls[0], dirs[0], names[1], session)
+        for url, dir, name in zip(urls, dirs, names):
+            asf_search.download_url(url, dir, name, session)
     else:
         with ProcessPoolExecutor(max_workers=n_workers) as executor:
             executor.map(asf_search.download_url, urls, dirs, names, [session] * len(urls))
 
 
 def burst2safe(
     granules: Optional[Iterable[str]] = None,
```

### Comparing `burst2safe-0.3.1/src/burst2safe/calibration.py` & `burst2safe-0.3.2/src/burst2safe/calibration.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_236/s1-level-1-calibration.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_236/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_236/s1-level-1-noise.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_236/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_236/s1-level-1-product.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_236/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_236/s1-object-types.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_236/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_245/s1-level-1-calibration.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_245/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_245/s1-level-1-noise.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_245/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_245/s1-level-1-product.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_245/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_245/s1-object-types.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_245/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_260/s1-level-1-calibration.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_260/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_260/s1-level-1-noise.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_260/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_260/s1-level-1-product.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_260/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_260/s1-object-types.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_260/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_290/s1-level-1-calibration.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_290/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_290/s1-level-1-noise.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_290/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_290/s1-level-1-product.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_290/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_290/s1-object-types.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_290/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-calibration.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-noise.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-product.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_340/s1-level-1-rfi.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_340/s1-level-1-rfi.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_340/s1-object-types.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_340/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-calibration.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-noise.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-product.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_371/s1-level-1-rfi.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_371/s1-level-1-rfi.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/data/support_371/s1-object-types.xsd` & `burst2safe-0.3.2/src/burst2safe/data/support_371/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/manifest.py` & `burst2safe-0.3.2/src/burst2safe/manifest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/measurement.py` & `burst2safe-0.3.2/src/burst2safe/measurement.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/noise.py` & `burst2safe-0.3.2/src/burst2safe/noise.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/product.py` & `burst2safe-0.3.2/src/burst2safe/product.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/rfi.py` & `burst2safe-0.3.2/src/burst2safe/rfi.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/safe.py` & `burst2safe-0.3.2/src/burst2safe/safe.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/swath.py` & `burst2safe-0.3.2/src/burst2safe/swath.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe/utils.py` & `burst2safe-0.3.2/src/burst2safe/utils.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/src/burst2safe.egg-info/PKG-INFO` & `burst2safe-0.3.2/src/burst2safe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `burst2safe-0.3.1/src/burst2safe.egg-info/SOURCES.txt` & `burst2safe-0.3.2/src/burst2safe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/conftest.py` & `burst2safe-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/etc/identify_ipf_differences.py` & `burst2safe-0.3.2/tests/etc/identify_ipf_differences.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/helpers.py` & `burst2safe-0.3.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_base.py` & `burst2safe-0.3.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml` & `burst2safe-0.3.2/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml` & `burst2safe-0.3.2/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml` & `burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml` & `burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml` & `burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml` & `burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml` & `burst2safe-0.3.2/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml` & `burst2safe-0.3.2/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_data/manifest_7C85.safe` & `burst2safe-0.3.2/tests/test_data/manifest_7C85.safe`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_golden.py` & `burst2safe-0.3.2/tests/test_golden.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_ipf.py` & `burst2safe-0.3.2/tests/test_ipf.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_manifest.py` & `burst2safe-0.3.2/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_measurement.py` & `burst2safe-0.3.2/tests/test_measurement.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_noise.py` & `burst2safe-0.3.2/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_product.py` & `burst2safe-0.3.2/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_safe.py` & `burst2safe-0.3.2/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_swath.py` & `burst2safe-0.3.2/tests/test_swath.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.1/tests/test_utils.py` & `burst2safe-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

