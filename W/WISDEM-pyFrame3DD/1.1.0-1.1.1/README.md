# Comparing `tmp/wisdem_pyframe3dd-1.1.0.tar.gz` & `tmp/wisdem_pyframe3dd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisdem_pyframe3dd-1.1.0.tar", last modified: Wed Jan 17 22:54:07 2024, max compression
+gzip compressed data, was "wisdem_pyframe3dd-1.1.1.tar", last modified: Wed May  1 21:42:25 2024, max compression
```

## Comparing `wisdem_pyframe3dd-1.1.0.tar` & `wisdem_pyframe3dd-1.1.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0      405 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      301 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1515 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     4757 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/.github/workflows/CI_pyFrame3DD.yml
--rw-r--r--   0        0        0     2293 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/.github/workflows/Publish_pyFrame3DD.yml
--rw-r--r--   0        0        0      345 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/.gitignore
--rw-r--r--   0        0        0    33890 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2436 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/README.md
--rw-r--r--   0        0        0      131 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/environment.yml
--rw-r--r--   0        0        0     4817 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/examples/exB.3dd
--rw-r--r--   0        0        0     7415 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/examples/exB.py
--rw-r--r--   0        0        0     1050 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/meson.build
--rw-r--r--   0        0        0      704 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/meson_options.txt
--rw-r--r--   0        0        0      108 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/__init__.py
--rw-r--r--   0        0        0      861 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/meson.build
--rw-r--r--   0        0        0    45130 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/pyframe3dd.py
--rw-r--r--   0        0        0    28457 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGmatrix.c
--rw-r--r--   0        0        0    10963 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGmatrix.h
--rw-r--r--   0        0        0     8074 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGutil.c
--rw-r--r--   0        0        0     4049 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGutil.h
--rw-r--r--   0        0        0      879 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/Makefile
--rw-r--r--   0        0        0    28485 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/NRutil.c
--rw-r--r--   0        0        0     4932 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/NRutil.h
--rw-r--r--   0        0        0     1513 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/common.h
--rw-r--r--   0        0        0     5507 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/coordtrans.c
--rw-r--r--   0        0        0     2412 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/coordtrans.h
--rw-r--r--   0        0        0    17858 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/eig.c
--rw-r--r--   0        0        0     3024 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/eig.h
--rw-r--r--   0        0        0    33581 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd.c
--rw-r--r--   0        0        0     8995 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd.h
--rw-r--r--   0        0        0   137211 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd_io.c
--rw-r--r--   0        0        0    19213 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd_io.h
--rw-r--r--   0        0        0    28017 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/main.c
--rw-r--r--   0        0        0     1067 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/microstran/config.h
--rw-r--r--   0        0        0     2621 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/microstran/vec3.h
--rw-r--r--   0        0        0    17613 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/preframe.c
--rw-r--r--   0        0        0    28461 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_HPGmatrix.c
--rw-r--r--   0        0        0    10966 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_HPGmatrix.h
--rw-r--r--   0        0        0    17974 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_eig.c
--rw-r--r--   0        0        0     3026 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_eig.h
--rw-r--r--   0        0        0    34134 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_frame3dd.c
--rw-r--r--   0        0        0     9229 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_frame3dd.h
--rw-r--r--   0        0        0    56090 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_io.c
--rw-r--r--   0        0        0     9709 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_io.h
--rw-r--r--   0        0        0    27074 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_main.c
--rw-r--r--   0        0        0     3033 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_structs.h
--rw-r--r--   0        0        0     3631 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3983 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/test/test_beam_theory.py
--rw-r--r--   0        0        0     8836 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/test/test_breakdown.py
--rw-r--r--   0        0        0    55631 2024-01-17 22:53:02.000000 wisdem_pyframe3dd-1.1.0/test/test_frame.py
--rw-r--r--   0        0        0     3980 2024-01-17 22:54:07.565786 wisdem_pyframe3dd-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      405 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      301 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1515 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      197 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/.github/tools/cibw_repair_wheel_command_windows.sh
+-rw-r--r--   0        0        0     5126 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/.github/workflows/CI_pyFrame3DD.yml
+-rw-r--r--   0        0        0     2780 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/.github/workflows/Publish_pyFrame3DD.yml
+-rw-r--r--   0        0        0      345 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/.gitignore
+-rw-r--r--   0        0        0    33890 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2436 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/README.md
+-rw-r--r--   0        0        0      131 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/environment.yml
+-rw-r--r--   0        0        0     4817 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/examples/exB.3dd
+-rw-r--r--   0        0        0     7415 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/examples/exB.py
+-rw-r--r--   0        0        0     1050 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/meson.build
+-rw-r--r--   0        0        0      704 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/meson_options.txt
+-rw-r--r--   0        0        0      108 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/__init__.py
+-rw-r--r--   0        0        0      835 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/meson.build
+-rw-r--r--   0        0        0    45130 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/pyframe3dd.py
+-rw-r--r--   0        0        0    28457 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGmatrix.c
+-rw-r--r--   0        0        0    10963 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGmatrix.h
+-rw-r--r--   0        0        0     8074 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGutil.c
+-rw-r--r--   0        0        0     4049 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGutil.h
+-rw-r--r--   0        0        0      885 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/Makefile
+-rw-r--r--   0        0        0    28485 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/NRutil.c
+-rw-r--r--   0        0        0     4932 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/NRutil.h
+-rw-r--r--   0        0        0     1513 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/common.h
+-rw-r--r--   0        0        0     5507 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/coordtrans.c
+-rw-r--r--   0        0        0     2412 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/coordtrans.h
+-rw-r--r--   0        0        0    17858 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/eig.c
+-rw-r--r--   0        0        0     3024 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/eig.h
+-rw-r--r--   0        0        0    33581 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd.c
+-rw-r--r--   0        0        0     8995 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd.h
+-rw-r--r--   0        0        0   137211 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd_io.c
+-rw-r--r--   0        0        0    19213 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd_io.h
+-rw-r--r--   0        0        0    28017 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/main.c
+-rw-r--r--   0        0        0     1067 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/microstran/config.h
+-rw-r--r--   0        0        0     2621 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/microstran/vec3.h
+-rw-r--r--   0        0        0    17613 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/preframe.c
+-rw-r--r--   0        0        0    28461 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_HPGmatrix.c
+-rw-r--r--   0        0        0    10966 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_HPGmatrix.h
+-rw-r--r--   0        0        0    17974 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_eig.c
+-rw-r--r--   0        0        0     3026 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_eig.h
+-rw-r--r--   0        0        0    34134 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_frame3dd.c
+-rw-r--r--   0        0        0     9229 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_frame3dd.h
+-rw-r--r--   0        0        0    56090 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_io.c
+-rw-r--r--   0        0        0     9709 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_io.h
+-rw-r--r--   0        0        0    27074 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_main.c
+-rw-r--r--   0        0        0     3033 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_structs.h
+-rw-r--r--   0        0        0     4066 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3841 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/test/test_beam_theory.py
+-rw-r--r--   0        0        0     8606 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/test/test_breakdown.py
+-rw-r--r--   0        0        0    55767 2024-05-01 21:33:47.000000 wisdem_pyframe3dd-1.1.1/test/test_frame.py
+-rw-r--r--   0        0        0     3980 2024-05-01 21:42:25.379710 wisdem_pyframe3dd-1.1.1/PKG-INFO
```

### Comparing `wisdem_pyframe3dd-1.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `wisdem_pyframe3dd-1.1.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/.github/workflows/CI_pyFrame3DD.yml` & `wisdem_pyframe3dd-1.1.1/.github/workflows/CI_pyFrame3DD.yml`

 * *Files 13% similar despite different names*

```diff
@@ -12,50 +12,59 @@
             run:
                 shell: bash -l {0}
                 
         strategy:
             fail-fast: false #true
             matrix:
                 os: ["ubuntu-latest", "macOS-latest", "windows-latest"]
-                python-version: ["3.9", "3.10", "3.11"]
+                python-version: ["3.9", "3.10", "3.11", "3.12"]
 
         steps:
             - name: Setup C/C++ Compiler
+              if: false == contains( matrix.os, 'windows')
               id: install_cc
-              uses: rlalik/setup-cpp-compiler@v1.2
+              uses: rlalik/setup-cpp-compiler@master
               with:
-                  compiler: gcc #clang
+                  compiler: clang
+          
+            - name: Install mingw-w64 on Windows
+              if: contains( matrix.os, 'windows')
+              uses: msys2/setup-msys2@v2
+              with:
+                  path-type: inherit
+                  install: |
+                      mingw-w64-x86_64-gcc
 
             - name: checkout repository
               uses: actions/checkout@v4
 
+            - name: Set compilers
+              if: false == contains( matrix.os, 'windows')
+              run: |
+                  echo "CC=${{ steps.install_cc.outputs.cc }}" >> $GITHUB_ENV
+                  echo "CXX=${{ steps.install_cc.outputs.cxx }}" >> $GITHUB_ENV
+                  
             - name: Set up Python ${{ matrix.python-version }}
-              uses: actions/setup-python@v4
+              uses: actions/setup-python@v5
               id: cp
               with:
                   python-version: ${{ matrix.python-version }}
                   update-environment: true
-              
+
             - name: Editable Pip Install pyFrame3DD
-              env:
-                  CC: '${{ steps.install_cc.outputs.cc }}'
-                  CXX: '${{ steps.install_cc.outputs.cxx }}'
               run: |
                   '${{ steps.cp.outputs.python-path }}' -m pip install --upgrade pip
                   '${{ steps.cp.outputs.python-path }}' -m pip install meson-python meson numpy ninja wheel
                   '${{ steps.cp.outputs.python-path }}' -m pip install --no-build-isolation -e .[test]
-
+                  
             - name: Editable Test run
               run: |
                   '${{ steps.cp.outputs.python-path }}' -m pytest test
                   
             - name: Pip Install pyFrame3DD
-              env:
-                  CC: '${{ steps.install_cc.outputs.cc }}'
-                  CXX: '${{ steps.install_cc.outputs.cxx }}'
               run: |
                   '${{ steps.cp.outputs.python-path }}' -m pip uninstall pyframe3dd
                   '${{ steps.cp.outputs.python-path }}' -m pip install -v .[test]
 
             #- name: Setup tmate session
             #  uses: mxschmitt/action-tmate@v3
             #  with:
@@ -74,15 +83,15 @@
             run:
                 shell: bash -el {0}
                 
         strategy:
             fail-fast: false #true
             matrix:
                 os: ["ubuntu-latest", "macOS-latest", "windows-latest"]
-                python-version: ["3.9", "3.10", "3.11"]
+                python-version: ["3.9", "3.10", "3.11", "3.12"]
 
         steps:
             - name: checkout repository
               uses: actions/checkout@v3
 
             - uses: conda-incubator/setup-miniconda@v2
               # https://github.com/marketplace/actions/setup-miniconda
```

### Comparing `wisdem_pyframe3dd-1.1.0/.github/workflows/Publish_pyFrame3DD.yml` & `wisdem_pyframe3dd-1.1.1/.github/workflows/Publish_pyFrame3DD.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 name: Build and upload to PyPI
+# https://github.com/pypa/cibuildwheel/blob/main/examples/github-deploy.yml
+# Best comparable example: https://github.com/pdfo/pdfo
 
-# Build on every branch push, tag push, and pull request change:
-#on: [push, pull_request]
-# Alternatively, to publish when a (published) GitHub Release is created, use the following:
-on:
-    release:
-        types:
-            - published
+# Build on every pull request (no need for every push) and release change:
+on: [pull_request, release]
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: false
       matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        os: [ubuntu-latest, windows-latest, macos-13, macos-14]
 
     steps:
-      - name: Setup C/C++ Compiler
+      - name: Install compiler
+        if: false == contains( matrix.os, 'windows')
         id: install_cc
-        uses: rlalik/setup-cpp-compiler@v1.2
+        uses: rlalik/setup-cpp-compiler@master
         with:
-            compiler: gcc #clang
+          compiler: clang
+          
+      - name: Install mingw-w64 on Windows
+        if: contains( matrix.os, 'windows')
+        uses: msys2/setup-msys2@v2
+        with:
+          path-type: inherit
+          install: |
+            mingw-w64-x86_64-gcc
             
       - name: Checkout
         uses: actions/checkout@v4
 
-      - name: Build wheels
+      - name: Build wheels mac and linux
+        if: false == contains( matrix.os, 'windows')
+        uses: pypa/cibuildwheel@v2.17.0
         env:
-            CC: '${{ steps.install_cc.outputs.cc }}'
-            CXX: '${{ steps.install_cc.outputs.cxx }}'
-        uses: pypa/cibuildwheel@v2.16.2
+          CC: ${{ steps.install_cc.outputs.cc }}
+          CXX: ${{ steps.install_cc.outputs.cxx }}
 
+      - name: Build wheels windows
+        if: contains( matrix.os, 'windows')
+        uses: pypa/cibuildwheel@v2.17.0
+          
       - uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
           
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Build sdist
         run: pipx run build --sdist
 
       - uses: actions/upload-artifact@v4
         with:
           name: cibw-sdist
```

### Comparing `wisdem_pyframe3dd-1.1.0/LICENSE.txt` & `wisdem_pyframe3dd-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/README.md` & `wisdem_pyframe3dd-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/examples/exB.3dd` & `wisdem_pyframe3dd-1.1.1/examples/exB.3dd`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/examples/exB.py` & `wisdem_pyframe3dd-1.1.1/examples/exB.py`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/meson.build` & `wisdem_pyframe3dd-1.1.1/meson.build`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/meson_options.txt` & `wisdem_pyframe3dd-1.1.1/meson_options.txt`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/pyframe3dd.py` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/pyframe3dd.py`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGmatrix.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGmatrix.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGmatrix.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGmatrix.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGutil.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGutil.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/HPGutil.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/HPGutil.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/Makefile` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 CC ?= clang #gcc
-CFLAGS = -c -g -O2 -fPIC
+CFLAGS = -c -g -O2 -fPIC -Wall
 
 OBS   = coordtrans.o HPGutil.o NRutil.o 
 PYOBS = py_main.o py_io.o py_frame3dd.o py_eig.o py_HPGmatrix.o 
 EOBS  = main.o frame3dd.o frame3dd_io.o eig.o HPGmatrix.o 
 
 ifeq ($(OS),Windows_NT)
     ARCHFLAGS=-D WIN64
```

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/NRutil.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/NRutil.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/NRutil.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/NRutil.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/common.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/common.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/coordtrans.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/coordtrans.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/coordtrans.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/coordtrans.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/eig.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/eig.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/eig.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/eig.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd_io.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd_io.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/frame3dd_io.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/frame3dd_io.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/main.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/main.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/microstran/config.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/microstran/config.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/microstran/vec3.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/microstran/vec3.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/preframe.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/preframe.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_HPGmatrix.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_HPGmatrix.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_HPGmatrix.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_HPGmatrix.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_eig.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_eig.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_eig.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_eig.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_frame3dd.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_frame3dd.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_frame3dd.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_frame3dd.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_io.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_io.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_io.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_io.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_main.c` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_main.c`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyframe3dd/src/py_structs.h` & `wisdem_pyframe3dd-1.1.1/pyframe3dd/src/py_structs.h`

 * *Files identical despite different names*

### Comparing `wisdem_pyframe3dd-1.1.0/pyproject.toml` & `wisdem_pyframe3dd-1.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["numpy", "ninja", "meson>=1.1", "meson-python", "wheel"]
 build-backend = "mesonpy"
 
 [project]
 name = "WISDEM-pyFrame3DD"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python bindings to Frame3DD, a code for static and dynamic structural analysis of 2D and 3D frames and trusses, with permission from Prof Henri Gavin"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPL-3.0-only"}
 keywords = ["wind", "turbine", "mdao", "design", "optimization"]
 authors = [
   {name = "NREL WISDEM Team", email = "systems.engineering@nrel.gov" }
@@ -112,9 +112,19 @@
 skip_glob = ['__init__.py']
 atomic = true
 #lines_after_imports = 2
 #lines_between_types = 1
 #src_paths=isort,test
 
 [tool.cibuildwheel]
-skip = ["cp36-*", "cp37-*", "cp38-*", "*-win32"]
-build-frontend = "build"
+skip = ["pp*", "cp36-*", "cp37-*", "cp38-*", "*-win32", "*-win_arm64"] #, "*-musllinux*"]
+build-frontend = { name = "build", args = ["-w","-n","-x"] }
+before-build = "pip install numpy ninja meson meson-python"
+build-verbosity = "3"
+
+# https://github.com/pdfo/pdfo
+[[tool.cibuildwheel.overrides]]
+select = "*-win_amd64"
+environment = { PKG_CONFIG_PATH="c:/opt/64/lib/pkgconfig" }
+
+[tool.cibuildwheel.windows]
+repair-wheel-command = "bash .github/tools/cibw_repair_wheel_command_windows.sh {wheel} {dest_dir}"
```

### Comparing `wisdem_pyframe3dd-1.1.0/test/test_beam_theory.py` & `wisdem_pyframe3dd-1.1.1/test/test_beam_theory.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,9 @@
         self.assertAlmostEqual(freq[1], anal[0], -1)
         self.assertAlmostEqual(freq[2], anal[1], -1)
         self.assertAlmostEqual(freq[3], anal[1], -1)
         self.assertAlmostEqual(freq[4], anal[2], -2)
         self.assertAlmostEqual(freq[5], anal[2], -2)
     
 
-
-
-
-def suite():
-    suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(FrameTestEXA))
-    return suite
-
 if __name__ == '__main__':
-    unittest.TextTestRunner().run(suite())
+    unittest.main()
```

### Comparing `wisdem_pyframe3dd-1.1.0/test/test_breakdown.py` & `wisdem_pyframe3dd-1.1.1/test/test_breakdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,23 +209,14 @@
 
         npt.assert_almost_equal(rxns_mass.Fx, rxns_force.Fx)
         npt.assert_almost_equal(rxns_mass.Fy, rxns_force.Fy)
         npt.assert_almost_equal(rxns_mass.Fz, rxns_force.Fz)
         npt.assert_almost_equal(rxns_mass.Mxx, rxns_force.Mxx)
         npt.assert_almost_equal(rxns_mass.Myy, rxns_force.Myy)
         npt.assert_almost_equal(rxns_mass.Mzz, rxns_force.Mzz)
-        
-def suite():
-    suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(TestBreakdown))
-    return suite
 
 
-if __name__ == "__main__":
-    result = unittest.TextTestRunner().run(suite())
 
-    if result.wasSuccessful():
-        exit(0)
-    else:
-        exit(1)
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `wisdem_pyframe3dd-1.1.0/test/test_frame.py` & `wisdem_pyframe3dd-1.1.1/test/test_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -913,15 +913,22 @@
 
         # Check that the load cases are equivalent
         self.assertEqual(reactions.Fz[0,0], reactions.Fz[1,0])
         self.assertAlmostEqual(2*reactions.Fz[0,0], reactions.Fz[2,0])
 
 
 def suite():
-    suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(FrameTestEXA))
-    suite.addTest(unittest.makeSuite(FrameTestEXB))
-    suite.addTest(unittest.makeSuite(GravityAdd))
-    return suite
+    suite = [
+        unittest.TestLoader().loadTestsFromTestCase(FrameTestEXA),
+        unittest.TestLoader().loadTestsFromTestCase(FrameTestEXB),
+        unittest.TestLoader().loadTestsFromTestCase(GravityAdd),
+    ]
+    return unittest.TestSuite(suite)
+
+if __name__ == "__main__":
+    result = unittest.TextTestRunner().run(suite())
+
+    if result.wasSuccessful():
+        exit(0)
+    else:
+        exit(1)
 
-if __name__ == '__main__':
-    unittest.TextTestRunner().run(suite())
```

### Comparing `wisdem_pyframe3dd-1.1.0/PKG-INFO` & `wisdem_pyframe3dd-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: WISDEM-pyFrame3DD
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python bindings to Frame3DD, a code for static and dynamic structural analysis of 2D and 3D frames and trusses, with permission from Prof Henri Gavin
-Keywords: wind turbine mdao design optimization
+Keywords: wind,turbine,mdao,design,optimization
 Author-Email: NREL WISDEM Team <systems.engineering@nrel.gov>
 Maintainer-Email: NREL WISDEM Team <systems.engineering@nrel.gov>
 License: GPL-3.0-only
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

