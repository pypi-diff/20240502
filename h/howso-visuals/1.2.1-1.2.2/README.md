# Comparing `tmp/howso-visuals-1.2.1.tar.gz` & `tmp/howso_visuals-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "howso-visuals-1.2.1.tar", last modified: Wed Feb 21 18:22:43 2024, max compression
+gzip compressed data, was "howso_visuals-1.2.2.tar", last modified: Tue Apr 30 13:36:01 2024, max compression
```

## Comparing `howso-visuals-1.2.1.tar` & `howso_visuals-1.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.469706 howso-visuals-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.461706 howso-visuals-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.461706 howso-visuals-1.2.1/.github/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.github/templates/version_summary.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.github/workflows/build-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.github/workflows/build-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.github/workflows/rebuild-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)   193755 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33893 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-02-21 18:22:43.469706 howso-visuals-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/bin/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/config/latest-mt-debug-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/config/latest-mt-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/config/latest-mt-noavx-debug-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/config/latest-st-debug-howso.yml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/config/latest-st-howso.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/config/powershell/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/config/powershell/Download-Tzdata.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/config/powershell/Helper-Functions.ps1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.457706 howso-visuals-1.2.1/howso/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/howso/visuals/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/howso/visuals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/howso/visuals/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/howso/visuals/data/iris.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/howso/visuals/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/howso/visuals/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/howso/visuals/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    24016 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/howso/visuals/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:22:43.465706 howso-visuals-1.2.1/howso_visuals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-02-21 18:22:43.000000 howso-visuals-1.2.1/howso_visuals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-21 18:22:43.000000 howso-visuals-1.2.1/howso_visuals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 18:22:43.000000 howso-visuals-1.2.1/howso_visuals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-21 18:22:43.000000 howso-visuals-1.2.1/howso_visuals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-21 18:22:43.000000 howso-visuals-1.2.1/howso_visuals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.10-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.11-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.8-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.8.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.9-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-21 18:22:35.000000 howso-visuals-1.2.1/requirements-3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 18:22:43.469706 howso-visuals-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.224062 howso_visuals-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.216062 howso_visuals-1.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.216062 howso_visuals-1.2.2/.github/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/templates/version_summary.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/build-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/build-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.github/workflows/rebuild-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)   199837 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33893 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-04-30 13:36:01.224062 howso_visuals-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/bin/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-mt-debug-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-mt-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-mt-noavx-debug-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-st-debug-howso.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/latest-st-howso.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/config/powershell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/powershell/Download-Tzdata.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/config/powershell/Helper-Functions.ps1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.212062 howso_visuals-1.2.2/howso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso/visuals/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso/visuals/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/data/iris.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso/visuals/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24016 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/howso/visuals/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:36:01.220062 howso_visuals-1.2.2/howso_visuals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40889 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 13:36:01.000000 howso_visuals-1.2.2/howso_visuals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    65614 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.10-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    65365 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.11-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    65365 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.12-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    65866 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.9-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35209 2024-04-30 13:35:57.000000 howso_visuals-1.2.2/requirements-3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:36:01.224062 howso_visuals-1.2.2/setup.cfg
```

### Comparing `howso-visuals-1.2.1/.github/templates/version_summary.md` & `howso_visuals-1.2.2/.github/templates/version_summary.md`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/.github/workflows/build-pr.yml` & `howso_visuals-1.2.2/.github/workflows/build-pr.yml`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/.github/workflows/build-release.yml` & `howso_visuals-1.2.2/.github/workflows/build-release.yml`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/.github/workflows/build.yml` & `howso_visuals-1.2.2/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         .
       env:
         SETUPTOOLS_SCM_PRETEND_VERSION: ${{ needs.metadata.outputs.version }}
 
     - name: Upload Tarball Artifact
       uses: actions/upload-artifact@v3
       with:
-        name: "howso-visuals-${{ needs.metadata.outputs.version }}"
-        path: "dist/howso-visuals-${{ needs.metadata.outputs.version }}.tar.gz"
+        name: "howso_visuals-${{ needs.metadata.outputs.version }}"
+        path: "dist/howso_visuals-${{ needs.metadata.outputs.version }}.tar.gz"
         if-no-files-found: error
 
     - name: Upload Wheel Artifact
       uses: actions/upload-artifact@v3
       with:
         name: "howso_visuals-${{ needs.metadata.outputs.version }}-py3-none-any"
         path: "dist/howso_visuals-${{ needs.metadata.outputs.version }}-py3-none-any.whl"
@@ -92,70 +92,84 @@
   workflow-summary:
     needs: ['metadata']
     uses: "howsoai/.github/.github/workflows/workflow-summary.yml@main"
     secrets: inherit
     with:
       upstream-details: ${{ needs.metadata.outputs.upstream-details }}
 
-  pytest-linux-3-8-st:
+  pytest-linux-3-9-st:
     needs: ['metadata', 'build']
     uses: howsoai/.github/.github/workflows/pytest.yml@main
     secrets: inherit
     with:
       platform: 'howso-ubuntu-runner-latest'
       platform-pretty: 'Linux'
       amalgam-plat-arch: 'linux-amd64'
-      python-version: '3.8'
+      python-version: '3.9'
       config-fp: './config/latest-st-debug-howso.yml'
       config-pretty: 'ST'
       workers: 'auto'
       upstream-details: ${{ needs.metadata.outputs.upstream-details }}
 
-  pytest-linux-3-11-mt:
+  pytest-linux-3-12-mt:
     needs: ['metadata', 'build']
     uses: howsoai/.github/.github/workflows/pytest.yml@main
     secrets: inherit
     with:
       platform: 'howso-ubuntu-runner-latest'
       platform-pretty: 'Linux'
       amalgam-plat-arch: 'linux-amd64'
-      python-version: '3.11'
+      python-version: '3.12'
       config-fp: './config/latest-mt-debug-howso.yml'
       config-pretty: 'MT'
       upstream-details: ${{ needs.metadata.outputs.upstream-details }}
 
-  pytest-windows-3-11-mt:
+  pytest-windows-3-12-mt:
     needs: ['metadata', 'build']
     uses: howsoai/.github/.github/workflows/pytest.yml@main
     secrets: inherit
     with:
       platform: 'howso-windows-runner-latest'
       platform-pretty: 'Windows'
       amalgam-plat-arch: 'windows-amd64'
-      python-version: '3.11'
+      python-version: '3.12'
       config-fp: './config/latest-mt-debug-howso.yml'
       config-pretty: 'MT'
       upstream-details: ${{ needs.metadata.outputs.upstream-details }}
 
-  pytest-macos-3-11-mt:
+  pytest-macos-3-12-mt:
     needs: ['metadata', 'build']
     uses: howsoai/.github/.github/workflows/pytest.yml@main
     secrets: inherit
     with:
       platform: 'macos-latest-large'
       platform-pretty: 'MacOS'
       amalgam-plat-arch: 'darwin-amd64'
-      python-version: '3.11'
+      python-version: '3.12'
       config-fp: './config/latest-mt-noavx-debug-howso.yml'
       config-pretty: 'MT'
       upstream-details: ${{ needs.metadata.outputs.upstream-details }}
 
+  generate-changelog:
+    if: inputs.build-type == 'release'
+    secrets: inherit
+    needs:
+      - metadata
+    uses: "howsoai/.github/.github/workflows/release-notes.yml@main"
+
   release:
     if: inputs.build-type == 'release'
-    needs: ['metadata', 'build']
+    needs:
+      - metadata
+      - build
+      - generate-changelog
+      - pytest-linux-3-9-st
+      - pytest-linux-3-12-mt
+      - pytest-windows-3-12-mt
+      - pytest-macos-3-12-mt
     runs-on: ubuntu-latest
     environment:
       name: pypi
     permissions:
       contents: write
       id-token: write
 
@@ -171,17 +185,17 @@
     - name: Create Release
       uses: ncipollo/release-action@v1
       with:
         tag: ${{ needs.metadata.outputs.version }}
         commit: ${{ github.sha }}
         name: "${{ github.event.repository.name }} ${{ needs.metadata.outputs.version }}"
         artifactErrorsFailBuild: true
-        generateReleaseNotes: true
+        body: ${{ needs.generate-changelog.outputs.changelog }}
         makeLatest: legacy
-        artifacts: "./tmp/howso-visuals-*/howso-visuals-*.tar.gz,./tmp/howso_visuals-*/howso_visuals-*.whl"
+        artifacts: "./tmp/howso_visuals-*/howso_visuals-*.tar.gz,./tmp/howso_visuals-*/howso_visuals-*.whl"
         artifactContentType: application/gzip
 
     - name: Clean up dir
       run: |
         mkdir -p dist
         find ./tmp -type f -name '*.whl' -exec cp -t ./dist {} +
         find ./tmp -type f -name '*.tar.gz' -exec cp -t ./dist {} +
```

### Comparing `howso-visuals-1.2.1/.github/workflows/rebuild-requirements.yml` & `howso_visuals-1.2.2/.github/workflows/rebuild-requirements.yml`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/.gitignore` & `howso_visuals-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/LICENSE-3RD-PARTY.txt` & `howso_visuals-1.2.2/LICENSE-3RD-PARTY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,83 @@
+build
+1.2.1
+MIT License
+Filipe Laíns <lains@riseup.net>, Bernát Gábor <gaborjbernat@gmail.com>, layday <layday@protonmail.com>, Henry Schreiner <henryschreineriii@gmail.com>
+https://build.pypa.io
+A simple, correct Python build frontend
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/build-1.2.1.dist-info/LICENSE
+Copyright © 2019 Filipe Laíns <filipe.lains@gmail.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice (including the next
+paragraph) shall be included in all copies or substantial portions of the
+Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+click
+8.1.7
+BSD License
+UNKNOWN
+https://palletsprojects.com/p/click/
+Composable command line interface toolkit
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/click-8.1.7.dist-info/LICENSE.rst
+Copyright 2014 Pallets
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are
+met:
+
+1.  Redistributions of source code must retain the above copyright
+    notice, this list of conditions and the following disclaimer.
+
+2.  Redistributions in binary form must reproduce the above copyright
+    notice, this list of conditions and the following disclaimer in the
+    documentation and/or other materials provided with the distribution.
+
+3.  Neither the name of the copyright holder nor the names of its
+    contributors may be used to endorse or promote products derived from
+    this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
+TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
+NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
 contourpy
-1.2.0
+1.2.1
 BSD License
 Ian Thomas <ianthomas23@gmail.com>
 https://github.com/contourpy/contourpy
 Python library for calculating contours of 2D quadrilateral grids
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/contourpy-1.2.0.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/contourpy-1.2.1.dist-info/LICENSE
 BSD 3-Clause License
 
-Copyright (c) 2021-2023, ContourPy Developers.
+Copyright (c) 2021-2024, ContourPy Developers.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
@@ -38,15 +104,15 @@
 
 cycler
 0.12.1
 BSD License
 Thomas A Caswell <matplotlib-users@python.org>
 https://matplotlib.org/cycler/
 Composable style cycles
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/cycler-0.12.1.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/cycler-0.12.1.dist-info/LICENSE
 Copyright (c) 2015, matplotlib project
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
@@ -68,20 +134,20 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 fonttools
-4.47.2
+4.51.0
 MIT License
 Just van Rossum
 http://github.com/fonttools/fonttools
 Tools to manipulate font files
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/fonttools-4.47.2.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/fonttools-4.51.0.dist-info/LICENSE
 MIT License
 
 Copyright (c) 2017 Just van Rossum
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -103,15 +169,15 @@
 
 kiwisolver
 1.4.5
 BSD License
 The Nucleic Development Team <sccolbert@gmail.com>
 https://github.com/nucleic/kiwi
 A fast implementation of the Cassowary constraint solver
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/kiwisolver-1.4.5.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/kiwisolver-1.4.5.dist-info/LICENSE
 =========================
  The Kiwi licensing terms
 =========================
 Kiwi is licensed under the terms of the Modified BSD License (also known as
 New or Revised BSD), as follows:
 
 Copyright (c) 2013, Nucleic Development Team
@@ -178,20 +244,20 @@
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file LICENSE, distributed with this software.
 #------------------------------------------------------------------------------
 
 
 matplotlib
-3.8.2
+3.8.4
 Python Software Foundation License
 John D. Hunter, Michael Droettboom
 https://matplotlib.org
 Python plotting package
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/matplotlib-3.8.2.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/matplotlib-3.8.4.dist-info/LICENSE
 License agreement for matplotlib versions 1.3.0 and later
 =========================================================
 
 1. This LICENSE AGREEMENT is between the Matplotlib Development Team
 ("MDT"), and the Individual or Organization ("Licensee") accessing and
 otherwise using matplotlib software in source or binary form and its
 associated documentation.
@@ -285,20 +351,20 @@
 products or services of Licensee, or any third party.
 
 8. By copying, installing or otherwise using matplotlib,
 Licensee agrees to be bound by the terms and conditions of this License
 Agreement.
 
 numpy
-1.26.3
+1.26.4
 BSD License
 Travis E. Oliphant et al.
 https://numpy.org
 Fundamental package for array computing in Python
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/numpy-1.26.3.dist-info/LICENSE.txt
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/numpy-1.26.4.dist-info/LICENSE.txt
 Copyright (c) 2005-2023, NumPy Developers.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
@@ -356,19 +422,14 @@
 installed in built numpy packages:
 
 Name: Meson
 Files: vendored-meson/meson/*
 License: Apache 2.0
   For license text, see vendored-meson/meson/COPYING
 
-Name: meson-python
-Files: vendored-meson/meson-python/*
-License: MIT
-  For license text, see vendored-meson/meson-python/LICENSE
-
 Name: spin
 Files: .spin/cmds.py
 License: BSD-3
   For license text, see .spin/LICENSE
 
 ----
 
@@ -1270,32 +1331,32 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
     Lesser General Public License for more details.
     https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html
 
 
 packaging
-23.2
+24.0
 Apache Software License; BSD License
 Donald Stufft <donald@stufft.io>
 https://github.com/pypa/packaging
 Core utilities for Python packages
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/packaging-23.2.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/packaging-24.0.dist-info/LICENSE
 This software is made available under the terms of *either* of the licenses
 found in LICENSE.APACHE or LICENSE.BSD. Contributions to this software is made
 under the terms of *both* these licenses.
 
 
 pandas
-2.1.4
+2.2.2
 BSD License
 The Pandas Development Team <pandas-dev@python.org>
 https://pandas.pydata.org
 Powerful data structures for data analysis, time series, and statistics
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/pandas-2.1.4.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/pandas-2.2.2.dist-info/LICENSE
 BSD 3-Clause License
 
 Copyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team
 All rights reserved.
 
 Copyright (c) 2011-2023, Open source contributors.
 
@@ -1322,28 +1383,28 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 pillow
-10.2.0
+10.3.0
 Historical Permission Notice and Disclaimer (HPND)
-"Jeffrey A. Clark (Alex)" <aclark@aclark.net>
+"Jeffrey A. Clark" <aclark@aclark.net>
 https://python-pillow.org
 Python Imaging Library (Fork)
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/pillow-10.2.0.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/pillow-10.3.0.dist-info/LICENSE
 The Python Imaging Library (PIL) is
 
     Copyright © 1997-2011 by Secret Labs AB
-    Copyright © 1995-2011 by Fredrik Lundh
+    Copyright © 1995-2011 by Fredrik Lundh and contributors
 
 Pillow is the friendly PIL fork. It is
 
-    Copyright © 2010-2024 by Jeffrey A. Clark (Alex) and contributors.
+    Copyright © 2010-2024 by Jeffrey A. Clark and contributors
 
 Like PIL, Pillow is licensed under the open source HPND License:
 
 By obtaining, using, and/or copying this software and/or its associated
 documentation, you agree that you have read, understood, and will comply
 with the following terms and conditions:
 
@@ -2673,21 +2734,58 @@
 Gailly and Mark Adler; it does not include third-party code.
 
 If you redistribute modified sources, we would appreciate that you include in
 the file ChangeLog history information documenting your changes.  Please read
 the FAQ for more information on the distribution of modified source versions.
 
 
+pip-tools
+7.4.1
+BSD License
+Vincent Driessen <me@nvie.com>
+https://github.com/jazzband/pip-tools/
+pip-tools keeps your pinned dependencies fresh.
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/pip_tools-7.4.1.dist-info/LICENSE
+BSD 3-Clause License
+
+Copyright (c). All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+    1. Redistributions of source code must retain the above copyright notice,
+       this list of conditions and the following disclaimer.
+
+    2. Redistributions in binary form must reproduce the above copyright
+       notice, this list of conditions and the following disclaimer in the
+       documentation and/or other materials provided with the distribution.
+
+    3. Neither the name of pip-tools nor the names of its contributors may be
+       used to endorse or promote products derived from this software without
+       specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
 plotly
-5.18.0
+5.21.0
 MIT License
 Chris P
 https://plotly.com/python/
 An open-source, interactive data visualization library for Python
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/plotly-5.18.0.dist-info/LICENSE.txt
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/plotly-5.21.0.dist-info/LICENSE.txt
 The MIT License (MIT)
 
 Copyright (c) 2016-2018 Plotly, Inc
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -2704,20 +2802,20 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 
 
 pyparsing
-3.1.1
+3.1.2
 MIT License
 Paul McGuire <ptmcg.gm+pyparsing@gmail.com>
 https://github.com/pyparsing/pyparsing/
 pyparsing module - Classes and methods to define and execute parsing grammars
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/pyparsing-3.1.1.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/pyparsing-3.1.2.dist-info/LICENSE
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
 the following conditions:
@@ -2730,21 +2828,51 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
+pyproject_hooks
+1.0.0
+MIT License
+Thomas Kluyver <thomas@kluyver.me.uk>
+https://github.com/pypa/pyproject-hooks
+Wrappers to call pyproject.toml-based build backend hooks.
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
+The MIT License (MIT)
+
+Copyright (c) 2017 Thomas Kluyver
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
 python-dateutil
-2.8.2
+2.9.0.post0
 Apache Software License; BSD License
 Gustavo Niemeyer
 https://github.com/dateutil/dateutil
 Extensions to the standard Python datetime module
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/python_dateutil-2.8.2.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/python_dateutil-2.9.0.post0.dist-info/LICENSE
 Copyright 2017- Paul Ganssle <paul@ganssle.io>
 Copyright 2017- dateutil contributors (see AUTHORS file)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
@@ -2793,20 +2921,20 @@
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 The above BSD License Applies to all code, even that also covered by Apache 2.0.
 
 pytz
-2023.3.post1
+2024.1
 MIT License
 Stuart Bishop
 http://pythonhosted.org/pytz
 World timezone definitions, modern and historical
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/pytz-2023.3.post1.dist-info/LICENSE.txt
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/pytz-2024.1.dist-info/LICENSE.txt
 Copyright (c) 2003-2019 Stuart Bishop <stuart@stuartbishop.net>
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
@@ -2821,21 +2949,21 @@
 THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
 scipy
-1.11.4
+1.13.0
 BSD License
 UNKNOWN
 https://scipy.org/
 Fundamental algorithms for scientific computing in Python
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/scipy-1.11.4.dist-info/LICENSE.txt
-Copyright (c) 2001-2002 Enthought, Inc. 2003-2023, SciPy Developers.
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/scipy-1.13.0.dist-info/LICENSE.txt
+Copyright (c) 2001-2002 Enthought, Inc. 2003-2024, SciPy Developers.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
@@ -3768,15 +3896,15 @@
 
 seaborn
 0.12.2
 BSD License
 Michael Waskom <mwaskom@gmail.com>
 https://github.com/mwaskom/seaborn
 Statistical data visualization
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/seaborn-0.12.2.dist-info/LICENSE.md
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/seaborn-0.12.2.dist-info/LICENSE.md
 Copyright (c) 2012-2021, Michael L. Waskom
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
@@ -3804,15 +3932,15 @@
 
 six
 1.16.0
 MIT License
 Benjamin Peterson
 https://github.com/benjaminp/six
 Python 2 and 3 compatibility utilities
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/six-1.16.0.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/six-1.16.0.dist-info/LICENSE
 Copyright (c) 2010-2020 Benjamin Peterson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
@@ -3831,15 +3959,15 @@
 
 tenacity
 8.2.3
 Apache Software License
 Julien Danjou
 https://github.com/jd/tenacity
 Retry code until it succeeds
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/tenacity-8.2.3.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/tenacity-8.2.3.dist-info/LICENSE
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -4036,20 +4164,20 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 tzdata
-2023.4
+2024.1
 Apache Software License
 Python Software Foundation
 https://github.com/python/tzdata
 Provider of IANA time zone data
-/opt/hostedtoolcache/Python/3.11.7/x64/lib/python3.11/site-packages/tzdata-2023.4.dist-info/LICENSE
+/home/runner/.pyenv/versions/3.12.1/lib/python3.12/site-packages/tzdata-2024.1.dist-info/LICENSE
 Apache Software License 2.0
 
 Copyright (c) 2020, Paul Ganssle (Google)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `howso-visuals-1.2.1/LICENSE.txt` & `howso_visuals-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/PKG-INFO` & `howso_visuals-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: howso-visuals
-Version: 1.2.1
+Version: 1.2.2
 Summary: Visualization utilities for use with Howso Engine.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
            Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
         of this license document, but changing it is not allowed.
@@ -667,15 +667,15 @@
 Project-URL: homepage, https://howso.com
 Project-URL: documentation, https://docs.howso.com/
 Project-URL: repository, https://github.com/howsoai/howso-visuals-py
 Keywords: machine,learning,artificial,intelligence,data,visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
 Requires-Dist: seaborn~=0.12.0
 Requires-Dist: plotly
 Requires-Dist: scipy
 Provides-Extra: dev
```

### Comparing `howso-visuals-1.2.1/README.md` & `howso_visuals-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/config/powershell/Download-Tzdata.ps1` & `howso_visuals-1.2.2/config/powershell/Download-Tzdata.ps1`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Write-Host "OS: $OS"
     
     $TzDataPath = "$Path/tzdata"
     if(-not (Test-Path "$TzDataPath")) {
         New-Item -ItemType Directory -Force -Path "$TzDataPath" | Out-Null
         $LocalTarGz = "$Path/tzdata.tar.gz"
         $ProgressPreference = 'SilentlyContinue'
-        Invoke-WebRequest -Uri "https://data.iana.org/time-zones/releases/tzdata2023c.tar.gz" -Outfile "$LocalTarGz"
+        Invoke-WebRequest -Uri "https://data.iana.org/time-zones/releases/tzdata2024a.tar.gz" -Outfile "$LocalTarGz"
         $ProgressPreference = 'Continue'
         Invoke-NativeCommand -Cmd "tar" -Arguments @("-xzf", "$LocalTarGz", "-C", "$TzDataPath")
         Remove-Item -Path "$LocalTarGz"
         Write-Host "tzdata written to: $TzDataPath"
 
         if ($OS.equals("windows")) {
             $TimeZoneFile = "$TzDataPath/windowsZones.xml"
```

### Comparing `howso-visuals-1.2.1/config/powershell/Helper-Functions.ps1` & `howso_visuals-1.2.2/config/powershell/Helper-Functions.ps1`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/howso/visuals/data/iris.csv` & `howso_visuals-1.2.2/howso/visuals/data/iris.csv`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/howso/visuals/tests/conftest.py` & `howso_visuals-1.2.2/howso/visuals/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/howso/visuals/tests/test_plot.py` & `howso_visuals-1.2.2/howso/visuals/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/howso/visuals/visuals.py` & `howso_visuals-1.2.2/howso/visuals/visuals.py`

 * *Files identical despite different names*

### Comparing `howso-visuals-1.2.1/howso_visuals.egg-info/PKG-INFO` & `howso_visuals-1.2.2/howso_visuals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: howso-visuals
-Version: 1.2.1
+Version: 1.2.2
 Summary: Visualization utilities for use with Howso Engine.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
            Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
         of this license document, but changing it is not allowed.
@@ -667,15 +667,15 @@
 Project-URL: homepage, https://howso.com
 Project-URL: documentation, https://docs.howso.com/
 Project-URL: repository, https://github.com/howsoai/howso-visuals-py
 Keywords: machine,learning,artificial,intelligence,data,visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
 Requires-Dist: seaborn~=0.12.0
 Requires-Dist: plotly
 Requires-Dist: scipy
 Provides-Extra: dev
```

### Comparing `howso-visuals-1.2.1/howso_visuals.egg-info/SOURCES.txt` & `howso_visuals-1.2.2/howso_visuals.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 LICENSE.txt
 README.md
 pyproject.toml
 requirements-3.10-dev.txt
 requirements-3.10.txt
 requirements-3.11-dev.txt
 requirements-3.11.txt
-requirements-3.8-dev.txt
-requirements-3.8.txt
+requirements-3.12-dev.txt
+requirements-3.12.txt
 requirements-3.9-dev.txt
 requirements-3.9.txt
 .github/CODEOWNERS
 .github/templates/version_summary.md
 .github/workflows/build-pr.yml
 .github/workflows/build-release.yml
 .github/workflows/build.yml
```

### Comparing `howso-visuals-1.2.1/pyproject.toml` & `howso_visuals-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name="howso-visuals"
 dynamic = ["version"]
 readme = "README.md"
 description = "Visualization utilities for use with Howso Engine."
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 keywords = ["machine", "learning", "artificial", "intelligence", "data", "visualization"]
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Programming Language :: Python :: 3"
 ]
```

