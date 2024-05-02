# Comparing `tmp/featureform_enterprise-0.13.3rc2.tar.gz` & `tmp/featureform_enterprise-0.13.8rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform_enterprise-0.13.3rc2.tar", last modified: Tue Apr 30 20:34:20 2024, max compression
+gzip compressed data, was "featureform_enterprise-0.13.8rc0.tar", last modified: Thu May  2 14:44:57 2024, max compression
```

## Comparing `featureform_enterprise-0.13.3rc2.tar` & `featureform_enterprise-0.13.8rc0.tar`

### file list

```diff
@@ -1,407 +1,407 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.165511 featureform_enterprise-0.13.3rc2/
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-30 20:34:20.165511 featureform_enterprise-0.13.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-30 20:34:20.165511 featureform_enterprise-0.13.3rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.081511 featureform_enterprise-0.13.3rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.089511 featureform_enterprise-0.13.3rc2/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    38226 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.073511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.089511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.093511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.077511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.077511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.093511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/DkMZG6iKzRiMRJuCdvb4X/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.093511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.137511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
--rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
--rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
--rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
--rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
--rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
--rw-r--r--   0 runner    (1001) docker     (127)  4221299 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/_app-c972f4bb01d17484.js
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/query-f3c47b8d51f1458e.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/search-e03b34f74065bab5.js
--rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js
--rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
--rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.145511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.149511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.149511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.149511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.149511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/group/
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/group/[groupName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/groups.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.149511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/role/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/role/[roleName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/roles.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.149511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/user/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/user/[userName].html
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/users.html
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/query.html
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.153511 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    61862 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/base_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/clearIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/clickhouse-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/creature.png
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/localmode.png
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/welcomebackground.png
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-30 20:34:15.000000 featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/tasks.html
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.157511 featureform_enterprise-0.13.3rc2/src/featureform/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.157511 featureform_enterprise-0.13.3rc2/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-04-30 20:32:48.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (127)    30651 2024-04-30 20:32:49.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    57679 2024-04-30 20:32:49.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   112854 2024-04-30 20:32:49.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-30 20:32:48.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-04-30 20:32:49.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/serving_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-30 20:32:49.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/serving_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-30 20:32:49.000000 featureform_enterprise-0.13.3rc2/src/featureform/proto/serving_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)   201798 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    84139 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/status_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/variant_names_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.165511 featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-30 20:34:20.000000 featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34746 2024-04-30 20:34:20.000000 featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:34:20.000000 featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 20:34:20.000000 featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 20:34:20.000000 featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 20:34:20.000000 featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:20.165511 featureform_enterprise-0.13.3rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_autogenerated_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    43785 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_multi_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_ondemand_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_resource_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_source_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_source_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_training_set_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-30 20:31:56.000000 featureform_enterprise-0.13.3rc2/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.288123 featureform_enterprise-0.13.8rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-02 14:44:57.288123 featureform_enterprise-0.13.8rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-02 14:44:57.292123 featureform_enterprise-0.13.8rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.200123 featureform_enterprise-0.13.8rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.208123 featureform_enterprise-0.13.8rc0/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38226 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.200123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.208123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.208123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.200123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.200123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.208123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.208123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/WuUFdOFgDayRm_IpzsrHl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.256123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)    83441 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73108 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
+-rw-r--r--   0 runner    (1001) docker     (127)   199780 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
+-rw-r--r--   0 runner    (1001) docker     (127)   130088 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   108180 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.264123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/404-8d282ae638ce5722.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.264123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-7bfcb609b1affd61.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4221299 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-c972f4bb01d17484.js
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_error-e18771d792fd8fe7.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.264123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.264123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.264123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.264123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/connections-f98076127418a04b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/query-f3c47b8d51f1458e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/search-e03b34f74065bab5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.7b558400037bbf48.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.79939abf3c1e11a8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.dbf25fee2d30d81a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.503837d41162f24d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.9a929c1c9b2638ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.1f58545eb203e18f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.5a6e695471cb4195.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.e90979a55a3b2795.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.cb40bb8da99d6066.js
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a9e892235dc65f7b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.a271ae92c5d426c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.bb3235d2b44fb9b3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.b941e6f1f8370030.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.758f2e9ec02ed81c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    81048 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/group/[groupName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/groups.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/role/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/role/[roleName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/roles.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.268123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/user/[userName].html
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/users.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.276123 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    61862 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/amazon_dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26573 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60161 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/base_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/clearIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/clickhouse-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35853 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/creature.png
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/localmode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   175958 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/welcomebackground.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-02 14:44:52.000000 featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.280123 featureform_enterprise-0.13.8rc0/src/featureform/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.280123 featureform_enterprise-0.13.8rc0/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-05-02 14:43:21.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    31633 2024-05-02 14:43:22.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60198 2024-05-02 14:43:22.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   112854 2024-05-02 14:43:22.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-02 14:43:21.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-05-02 14:43:22.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/serving_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-02 14:43:22.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/serving_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-05-02 14:43:22.000000 featureform_enterprise-0.13.8rc0/src/featureform/proto/serving_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201949 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83829 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/status_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33892 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/variant_names_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.288123 featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-02 14:44:57.000000 featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34746 2024-05-02 14:44:57.000000 featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:44:57.000000 featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 14:44:57.000000 featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-02 14:44:57.000000 featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 14:44:57.000000 featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:57.288123 featureform_enterprise-0.13.8rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_autogenerated_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43785 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_multi_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_ondemand_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_resource_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_source_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_source_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28897 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_training_set_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-02 14:42:32.000000 featureform_enterprise-0.13.8rc0/tests/test_updating_provider.py
```

### Comparing `featureform_enterprise-0.13.3rc2/LICENSE` & `featureform_enterprise-0.13.8rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/PKG-INFO` & `featureform_enterprise-0.13.8rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.3rc2
+Version: 0.13.8rc0
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `featureform_enterprise-0.13.3rc2/README.md` & `featureform_enterprise-0.13.8rc0/README.md`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/setup.cfg` & `featureform_enterprise-0.13.8rc0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform-enterprise
-version = 0.13.3rc2
+version = 0.13.8-rc
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Enterprise Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls =
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/__init__.py` & `featureform_enterprise-0.13.8rc0/src/featureform/__init__.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/cli.py` & `featureform_enterprise-0.13.8rc0/src/featureform/cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/client.py` & `featureform_enterprise-0.13.8rc0/src/featureform/client.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/404.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/404.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/404-8d282ae638ce5722.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/[type]/[entity].html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-44302760e55a8032.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-44302760e55a8032.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/[type].html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/[type].html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-7bfcb609b1affd61.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-44302760e55a8032.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/_app-c972f4bb01d17484.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-c972f4bb01d17484.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/group/[groupName]-4ba8b6abfb4b13ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/role/[roleName]-a4f4cefefad41418.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/roles-a560426c6514c003.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/user/[userName]-5a66d4c05c9e7453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-142e8557e4889163.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.9d4c892d6ec3e998.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.1110d811936eb535.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.1cceaa6cbbc063ac.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.eb2d7c5e73071e92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.7cda0a8b4fd10c8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.d3bb3d49b9c1d80b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.a8dc93d57de022d3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.5c26573759f9c121.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.7c2ee867e260f0e7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.b157974fb0a5a751.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.5b503b684163ddee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.3767e3821cef0636.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.588ecfde90e6c6a6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.b830bba5a58a571f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.e5835ab195bd9150.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.c9f609621defe122.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.cbb253b90d4065f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.12fc5c16e5a165ee.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.24015a609992c2a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.a83f04a28cfc5c13.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.95f68b8f15b82829.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.e02e26748402cb2f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.a21b937dd852d3c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.f36b9b8a53d85766.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.51b85e9ce6ac77e9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.0f747e26266b02a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.0dcb315084b7163e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.b594f920dc05a67e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.588914f5988d8070.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.ee070d344f3affd6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.1cb9d96b33822dc8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.0d5ec818ecef9324.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.628102c989f49555.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.d2924ae4e73b1223.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.3f60a647075d636f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.24b8d9cafb06d199.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.8c0ef98ac4f8e8a2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.40ae09135f82f50e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.8aaf8e216bf41dfe.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.841bb10e71e1c449.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.bc56944969bce274.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.ca9c2b431c04ca17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.b5f4b6f514528d1d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.3b8da30965ace8d0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.a4e379d50aabc89d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.31cb364f97f4e824.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.e13b9d3271de18f9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.e2654a73b0584dec.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.da3b3e0fae942646.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.399f0ab013510453.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a7425f8edef285f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.155ab93349c67ccd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.c6479c75f219ea50.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.58f937c9dbd9989e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.a021feea122d3ab8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.15c4fc0252344391.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.746dde9caa36bd3a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.7866c582058e46fd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.7724b491752c429c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.d1dd2d2dd76819de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.c6da2507c50d21c4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.d3fa954b1b6c7ddf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.a7092d9f281d4e48.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.8ccf09a496d63a6f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1d47fcfbbb4f7aae.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.63e1bd7540f5f024.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.ec6db56efdb346a0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e29c5a5287592d58.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.d0376c6facb31ca5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.b47b77184d88114f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.78c84ccf0f96ba85.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.c75feab6b678db77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.508502701a02090a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.d426610fe97ba28f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f181bbcd52749298.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.75b381c93a6b3e68.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.16f39c180893252d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.650dab668c7e4fd7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.64a2195a59fd1547.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.80cf156f114fd8cf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.b64600096e2ca9ed.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.01d852003dbb136c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.5aae66009f81a97f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.f89efc1289945c39.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.da89585e43cc625e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.c33d2207767fa3ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.dffcd987fd2af796.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.9a225e869035cf5e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.33073eaf6ea575b1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.bb74c766d6f802c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.746cbe8d4f665f4e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.cfac9943bd3aa8c6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.8b59c21ed9aa0df8.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e3cb4a5604d89cfa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.12cb2d9917a6aab2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.a3b5dc1c4d26ae4c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.a43af9cbcc3d056e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.fb4387bc9a5ead37.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.794412054be66c77.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.47962934ccb42723.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.0df6c8ce29df587c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.40eef7387c672247.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.c777981c76bf526a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.80fd5c9b26494fb4.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b0db7f0ee3f15673.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.8b1345b4f614c39f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.31982856fa816d70.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.f17164273275fd38.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.2f587faa9c12f894.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.02e16f89cc645033.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.dd5a243970406aba.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.acb704c99ae042b7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.52a0bfb16d6c2b98.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.9a0f06e32359ab5f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.69a4a948327f0b94.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.8c3fb04cf18de9ad.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.fdc98b1cdb606d74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.8fca60ed2df5e72a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.c6bd9f3fa6de96e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.74938f19e891fdf5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.fc51859d62024c0c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.722d26c11b333d29.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.a38fd3d408351597.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.374dabbd7a65bb7e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.79a60949255a30ef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b8f96e57ccaae943.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.c394be68ff73cffa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.2017f4173ae7ddfb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.b409945670f221f7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.83a26a43f4df0850.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.51aa798f8d7e5f9d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.67ac42fc89d5c984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.83317f3b3977639c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.b5b55f9072af7a5d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.859e58b02983b520.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.478f7d5866f2865d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.7494238f7c6ad706.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.199e2ba708699dcb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.98e2ba9a44a80b8d.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.36058e7553ffa345.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.48de1152e01ba572.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.7a521a109d6461ca.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.c091a192bf82f926.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.badf407c7a6f2db0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.213c3d6af366a76e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.93772d4fe83877f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.3a384d03bec6f703.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.9cdb03119b332984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.e79ec6009494dfce.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.7766acfcd5f91811.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.e0ae21e641671328.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.26d85ff3fe699cbb.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.f36a4d3fb726f719.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.fcda67b8e3d7ff14.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.72882aebe76845de.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.2e295de118cafdef.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.e1cdb5c5cec33e2e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.7e7c3d8167ac74f6.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.790c6f46fa4e9d8b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.1f694c1ce3fcc4d1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.3aa230ff56d754c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.ae739446f2d00124.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.e221063f635f2e9f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.e3b79e7ad6d1e67b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.67dc98b63dd3081e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.49c692f8bc2d227f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.60d8ff3f62a0dde3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.241341676d07c7c5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.edc1a3543d37dac7.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.2ae7f1f871d749d9.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.11864bd2178e2c08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.cf7ba940ae593d96.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.d61bc93d9240911c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.7dc2e8495b82afa0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.cc6c20111eef392b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.28dda31a087b27dc.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.2a65ffecac1e4433.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.f3ac4fdc10100a71.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.e5cbb81e295d94aa.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.8fd37bd46bcdef8e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.021da63363b275e2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.7047500798cae5bd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.37b21bb61cb7da6e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.987edd5fb1761cdf.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.f4f05ad29882de17.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.74a04f9bd98b3d92.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.63c6b3c7dbad89c3.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.a961a8a3e36733d2.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.5c35ca803e68095b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.b314e238d6967a8f.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.1d0f9c7b17d4bc2b.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.790da421b54213dd.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.a9cf0d3dab52d046.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.8efe0bec8cec6f08.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.cfc4809f40a5b725.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2127ec25c75e4984.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.62a04a024d699193.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.f45aa85f3888e4f5.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.a26c328f4cf8b171.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.ea05c1dd27403a55.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.d6af4f6428d66d9a.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.74e478ac085e3404.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.92e6c66e598bc5b0.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.5be2e1ec1d76cc74.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.aa5faeff88cffc63.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.97f81f55c7dda273.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.2eea9520afb8e6ea.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.df4e0a4839a040a1.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.e1a7f78fb87ff37c.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.4ddc9ac973a0065e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-4ca33bb86fc5510e.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/group/[groupName].html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/groups.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/groups.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/role/[roleName].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/groups-7ef899e78a46642d.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/groups","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/role/[roleName].html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/roles.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/role/%5BroleName%5D-a4f4cefefad41418.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/role/[roleName]","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/roles.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/connections.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/roles-a560426c6514c003.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/roles","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/user/[userName].html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/users.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/admin/users.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/user/[userName].html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/users-313d4735cfc2c71a.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/user/%5BuserName%5D-5a66d4c05c9e7453.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/users","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/user/[userName]","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/connections.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/tasks.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/connections-f98076127418a04b.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/index.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/index-142e8557e4889163.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/query.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/query.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/query-f3c47b8d51f1458e.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/query-f3c47b8d51f1458e.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/query","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/search.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/admin/group/[groupName].html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/search-e03b34f74065bab5.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/admin/group/%5BgroupName%5D-4ba8b6abfb4b13ca.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/admin/group/[groupName]","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_White.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/amazon_dynamoDB.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/amazon_dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/base_logo.png` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/base_logo.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/clearIcon.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/clearIcon.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/clickhouse-logo.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/clickhouse-logo.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/creature.png` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/creature.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/favicon.ico` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/logo192.png` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/logo512.png` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/static/welcomebackground.png` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/static/welcomebackground.png`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/dashboard/out/tasks.html` & `featureform_enterprise-0.13.8rc0/src/featureform/dashboard/out/search.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/tasks-cb5a5f315eeb0c01.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js" defer=""></script><script src="/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-4ca33bb86fc5510e.js" defer=""></script><script src="/_next/static/chunks/framework-f44ba79936f400b5.js" defer=""></script><script src="/_next/static/chunks/main-b492e665e4469b62.js" defer=""></script><script src="/_next/static/chunks/pages/_app-c972f4bb01d17484.js" defer=""></script><script src="/_next/static/chunks/pages/search-e03b34f74065bab5.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js" defer=""></script><script src="/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js" defer=""></script><style id="jss-server-side">.jss11 {
   top: 70px;
   width: 100%;
   height: 550px;
   position: absolute;
   margin-left: auto;
   margin-right: auto;
 }
@@ -82,8 +82,8 @@
   justify-self: flex-end;
 }
 .jss1 {
   top: 70px;
   width: 100%;
   height: 100%;
   position: relative;
-}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/tasks","query":{},"buildId":"DkMZG6iKzRiMRJuCdvb4X","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+}</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><style data-emotion="css-global o6gwfi">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:rgba(0, 0, 0, 0.87);font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#fff;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#fff;}</style><div class="jss2"><style data-emotion="css 3ys12l">.css-3ys12l{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><style data-emotion="css fydjzv">.css-fydjzv{background-color:#fff;color:rgba(0, 0, 0, 0.87);-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:0px 2px 4px -1px rgba(0,0,0,0.2),0px 4px 5px 0px rgba(0,0,0,0.14),0px 1px 10px 0px rgba(0,0,0,0.12);display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:absolute;z-index:1100;top:0;left:auto;right:0;background-color:#1976d2;color:#fff;}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation4 MuiAppBar-root MuiAppBar-colorPrimary MuiAppBar-positionAbsolute jss3 css-fydjzv" style="background-color:#FC195C"><style data-emotion="css i6s8oy">.css-i6s8oy{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;}@media (min-width:600px){.css-i6s8oy{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-i6s8oy{min-height:48px;}}}@media (min-width:600px){.css-i6s8oy{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular jss6 css-i6s8oy"><div class="jss7"><style data-emotion="css 11gnq51">.css-11gnq51{height:50px;width:50px;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;}@media (min-width:0px){.css-11gnq51{display:none;}}@media (min-width:600px){.css-11gnq51{display:block;}}</style><img class="MuiBox-root css-11gnq51" src="/static/base_logo.png" alt="Featureform" style="cursor:pointer;nowrap:"/></div><div class="jss9"></div><div></div></div></header></div>explicitly check for null</div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"WuUFdOFgDayRm_IpzsrHl","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/deploy.py` & `featureform_enterprise-0.13.8rc0/src/featureform/deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/exceptions.py` & `featureform_enterprise-0.13.8rc0/src/featureform/exceptions.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/format.py` & `featureform_enterprise-0.13.8rc0/src/featureform/format.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/get.py` & `featureform_enterprise-0.13.8rc0/src/featureform/get.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/grpc_client.py` & `featureform_enterprise-0.13.8rc0/src/featureform/grpc_client.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/lib/auth.py` & `featureform_enterprise-0.13.8rc0/src/featureform/lib/auth.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/list.py` & `featureform_enterprise-0.13.8rc0/src/featureform/list.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata.proto` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata.proto`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,14 @@
     }
 }
 
 message FeatureVariant {
     string name = 1;
     string variant = 2;
     NameVariant source = 3;
-    string type = 4;
     string entity = 5;
     google.protobuf.Timestamp created = 6;
     string owner = 7;
     string description = 8;
     string provider = 9;
     ResourceStatus status = 10;
     repeated NameVariant trainingsets = 11;
@@ -241,19 +240,43 @@
         Stream stream = 21;
     }
     google.protobuf.Timestamp last_updated = 13;
     string schedule = 14;
     Tags tags = 15;
     Properties properties = 16;
     ComputationMode mode = 18;
-    bool is_embedding = 19;
-    int32 dimension = 20;
     string task_id = 23 [deprecated=true];
     repeated string task_id_list = 24;
     FeatureParameters additional_parameters = 22;
+    ValueType type = 25;
+}
+
+message ValueType {
+    oneof Type {
+        ScalarType scalar = 1;
+        VectorType vector = 2;
+    }
+}
+
+enum ScalarType {
+    NULL = 0;
+    INT = 1;
+    FLOAT32 = 2;
+    FLOAT64 = 3;
+    STRING = 4;
+    BOOL = 5;
+    INT32 = 6;
+    INT64 = 7;
+    DATETIME = 8;
+}
+
+message VectorType {
+    ScalarType scalar = 1;
+    int32 dimension = 2;
+    bool is_embedding = 3;
 }
 
 message FeatureParameters {
     oneof feature_type {
         PrecomputedFeatureParameters precomputed = 1;
         OndemandFeatureParameters ondemand = 2;
     }
@@ -280,29 +303,29 @@
     repeated string variants = 4;
 }
 
 message LabelVariant {
     string name = 1;
     string variant = 2;
     string description = 3;
-    string type = 4;
     NameVariant source = 5;
     string entity = 6;
     google.protobuf.Timestamp created = 7;
     string owner = 8;
     string provider = 9;
     ResourceStatus status = 10;
     repeated NameVariant trainingsets = 11;
     oneof location {
         Columns columns = 12;
         Stream stream = 16;
     }
     Tags tags = 13;
     Properties properties = 14;
     string task_id = 15 [deprecated=true];
+    ValueType type = 18;
     repeated string task_id_list = 17;
 }
 
 message Provider {
     string name = 1;
     string description = 2;
     string type = 3;
@@ -475,8 +498,8 @@
 
 message StreamingLabelVariant {
     string name = 1;
     string variant = 2;
     string value = 3;
     string entity = 4;
     google.protobuf.Timestamp ts = 5;
-}
+}
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata_pb2.py` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n featureform/proto/metadata.proto\x12\"featureform.serving.metadata.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x19google/protobuf/any.proto\"T\n\x0eOktaAuthConfig\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12\x1f\n\x17\x61uthorization_server_id\x18\x02 \x01(\t\x12\x11\n\tclient_id\x18\x03 \x01(\t\"\x17\n\x15PassThroughAuthConfig\"\xad\x01\n\nAuthConfig\x12\x42\n\x04okta\x18\x01 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.OktaAuthConfigH\x00\x12Q\n\x0cpass_through\x18\x02 \x01(\x0b\x32\x39.featureform.serving.metadata.proto.PassThroughAuthConfigH\x00\x42\x08\n\x06\x63onfig\"\x14\n\x04Name\x12\x0c\n\x04name\x18\x01 \x01(\t\"S\n\x0b\x45rrorStatus\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12%\n\x07\x64\x65tails\x18\x03 \x03(\x0b\x32\x14.google.protobuf.Any\"\x9f\x02\n\x0eResourceStatus\x12I\n\x06status\x18\x01 \x01(\x0e\x32\x39.featureform.serving.metadata.proto.ResourceStatus.Status\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12\x45\n\x0c\x65rror_status\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.ErrorStatus\"d\n\x06Status\x12\r\n\tNO_STATUS\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\t\n\x05READY\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04\x12\x0b\n\x07RUNNING\x10\x05\x12\r\n\tCANCELLED\x10\x06\"\x98\x01\n\nResourceID\x12\x41\n\x08resource\x18\x01 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12G\n\rresource_type\x18\x02 \x01(\x0e\x32\x30.featureform.serving.metadata.proto.ResourceType\"\x9b\x01\n\x10SetStatusRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\"n\n\x15ScheduleChangeRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x10\n\x08schedule\x18\x02 \x01(\t\",\n\x0bNameVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\"\x07\n\x05\x45mpty\"\x86\x01\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"4\n\x07\x43olumns\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\n\n\x02ts\x18\x03 \x01(\t\"\x1f\n\x0ePythonFunction\x12\r\n\x05query\x18\x01 \x01(\x0c\"\"\n\x06Stream\x12\x18\n\x10offline_provider\x18\x01 \x01(\t\"\xdc\x02\n\x0fResourceVariant\x12M\n\x0f\x66\x65\x61ture_variant\x18\x01 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.FeatureVariantH\x00\x12I\n\rlabel_variant\x18\x02 \x01(\x0b\x32\x30.featureform.serving.metadata.proto.LabelVariantH\x00\x12V\n\x14training_set_variant\x18\x03 \x01(\x0b\x32\x36.featureform.serving.metadata.proto.TrainingSetVariantH\x00\x12K\n\x0esource_variant\x18\x04 \x01(\x0b\x32\x31.featureform.serving.metadata.proto.SourceVariantH\x00\x42\n\n\x08resource\"\xfb\x07\n\x0e\x46\x65\x61tureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12?\n\x06source\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x05 \x01(\t\x12+\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x46\n\x08\x66unction\x18\x11 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.PythonFunctionH\x00\x12<\n\x06stream\x18\x15 \x01(\x0b\x32*.featureform.serving.metadata.proto.StreamH\x00\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x36\n\x04tags\x18\x0f \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x10 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x41\n\x04mode\x18\x12 \x01(\x0e\x32\x33.featureform.serving.metadata.proto.ComputationMode\x12\x14\n\x0cis_embedding\x18\x13 \x01(\x08\x12\x11\n\tdimension\x18\x14 \x01(\x05\x12\x13\n\x07task_id\x18\x17 \x01(\tB\x02\x18\x01\x12\x14\n\x0ctask_id_list\x18\x18 \x03(\t\x12T\n\x15\x61\x64\x64itional_parameters\x18\x16 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.FeatureParametersB\n\n\x08location\"\xcf\x01\n\x11\x46\x65\x61tureParameters\x12W\n\x0bprecomputed\x18\x01 \x01(\x0b\x32@.featureform.serving.metadata.proto.PrecomputedFeatureParametersH\x00\x12Q\n\x08ondemand\x18\x02 \x01(\x0b\x32=.featureform.serving.metadata.proto.OndemandFeatureParametersH\x00\x42\x0e\n\x0c\x66\x65\x61ture_type\"\x1e\n\x1cPrecomputedFeatureParameters\"/\n\x19OndemandFeatureParameters\x12\x12\n\ndefinition\x18\x01 \x01(\t\"d\n\nFeatureLag\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\x03lag\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x84\x01\n\x05Label\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xab\x05\n\x0cLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12?\n\x06source\x18\x05 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0e\n\x06\x65ntity\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12<\n\x06stream\x18\x10 \x01(\x0b\x32*.featureform.serving.metadata.proto.StreamH\x00\x12\x36\n\x04tags\x18\r \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x0e \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x13\n\x07task_id\x18\x0f \x01(\tB\x02\x18\x01\x12\x14\n\x0ctask_id_list\x18\x11 \x03(\tB\n\n\x08location\"\xc3\x04\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08software\x18\x04 \x01(\t\x12\x0c\n\x04team\x18\x05 \x01(\t\x12\x19\n\x11serialized_config\x18\x06 \x01(\x0c\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12@\n\x07sources\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x0c \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\r \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x8a\x01\n\x0bTrainingSet\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\x8e\x05\n\x12TrainingSetVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12+\n\x07\x63reated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08provider\x18\x06 \x01(\t\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x05label\x18\t \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x44\n\x0c\x66\x65\x61ture_lags\x18\x0f \x03(\x0b\x32..featureform.serving.metadata.proto.FeatureLag\x12\x36\n\x04tags\x18\x10 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x11 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x13\n\x07task_id\x18\x12 \x01(\tB\x02\x18\x01\x12\x14\n\x0ctask_id_list\x18\x13 \x03(\t\"\xb6\x03\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x42\n\x06status\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x07 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x08 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xf1\x02\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x06 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x07 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xe1\x03\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12@\n\x07sources\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x08 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\t \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x85\x01\n\x06Source\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xf3\x06\n\rSourceVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12L\n\x0etransformation\x18\x0e \x01(\x0b\x32\x32.featureform.serving.metadata.proto.TransformationH\x00\x12\x46\n\x0bprimaryData\x18\x0f \x01(\x0b\x32/.featureform.serving.metadata.proto.PrimaryDataH\x00\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x10\n\x08provider\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06status\x18\x08 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\r\n\x05table\x18\t \x01(\t\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0c \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x10 \x01(\t\x12\x36\n\x04tags\x18\x11 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x12 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x13\n\x07task_id\x18\x13 \x01(\tB\x02\x18\x01\x12\x33\n\x10max_job_duration\x18\x14 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x14\n\x0ctask_id_list\x18\x15 \x03(\tB\x0c\n\ndefinition\"\x95\x02\n\x0eTransformation\x12R\n\x11SQLTransformation\x18\x01 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.SQLTransformationH\x00\x12P\n\x10\x44\x46Transformation\x18\x02 \x01(\x0b\x32\x34.featureform.serving.metadata.proto.DFTransformationH\x00\x12M\n\x0fkubernetes_args\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.KubernetesArgsH\x01\x42\x06\n\x04typeB\x06\n\x04\x61rgs\"o\n\x17KubernetesResourceSpecs\x12\x13\n\x0b\x63pu_request\x18\x01 \x01(\t\x12\x11\n\tcpu_limit\x18\x02 \x01(\t\x12\x16\n\x0ememory_request\x18\x03 \x01(\t\x12\x14\n\x0cmemory_limit\x18\x04 \x01(\t\"r\n\x0eKubernetesArgs\x12\x14\n\x0c\x64ocker_image\x18\x01 \x01(\t\x12J\n\x05specs\x18\x02 \x01(\x0b\x32;.featureform.serving.metadata.proto.KubernetesResourceSpecs\"c\n\x11SQLTransformation\x12\r\n\x05query\x18\x01 \x01(\t\x12?\n\x06source\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"w\n\x10\x44\x46Transformation\x12\r\n\x05query\x18\x01 \x01(\x0c\x12?\n\x06inputs\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x13\n\x0bsource_text\x18\x03 \x01(\t\"_\n\x0bPrimaryData\x12\x44\n\x05table\x18\x01 \x01(\x0b\x32\x33.featureform.serving.metadata.proto.PrimarySQLTableH\x00\x42\n\n\x08location\"\x1f\n\x0fPrimarySQLTable\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x13\n\x04Tags\x12\x0b\n\x03tag\x18\x01 \x03(\t\"+\n\x08Property\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x42\x07\n\x05value\"\xbb\x01\n\nProperties\x12N\n\x08property\x18\x01 \x03(\x0b\x32<.featureform.serving.metadata.proto.Properties.PropertyEntry\x1a]\n\rPropertyEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.featureform.serving.metadata.proto.Property:\x02\x38\x01\"\x7f\n\x17StreamingFeatureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\t\x12&\n\x02ts\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"}\n\x15StreamingLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x04 \x01(\t\x12&\n\x02ts\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp*\xc9\x01\n\x0cResourceType\x12\x0b\n\x07\x46\x45\x41TURE\x10\x00\x12\t\n\x05LABEL\x10\x01\x12\x10\n\x0cTRAINING_SET\x10\x02\x12\n\n\x06SOURCE\x10\x03\x12\x13\n\x0f\x46\x45\x41TURE_VARIANT\x10\x04\x12\x11\n\rLABEL_VARIANT\x10\x05\x12\x18\n\x14TRAINING_SET_VARIANT\x10\x06\x12\x12\n\x0eSOURCE_VARIANT\x10\x07\x12\x0c\n\x08PROVIDER\x10\x08\x12\n\n\x06\x45NTITY\x10\t\x12\t\n\x05MODEL\x10\n\x12\x08\n\x04USER\x10\x0b*F\n\x0f\x43omputationMode\x12\x0f\n\x0bPRECOMPUTED\x10\x00\x12\x13\n\x0f\x43LIENT_COMPUTED\x10\x01\x12\r\n\tSTREAMING\x10\x02\x32\xef\x1b\n\x08Metadata\x12j\n\rGetAuthConfig\x12).featureform.serving.metadata.proto.Empty\x1a..featureform.serving.metadata.proto.AuthConfig\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12y\n\rGetEquivalent\x12\x33.featureform.serving.metadata.proto.ResourceVariant\x1a\x33.featureform.serving.metadata.proto.ResourceVariant\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12t\n\x11SetResourceStatus\x12\x34.featureform.serving.metadata.proto.SetStatusRequest\x1a).featureform.serving.metadata.proto.Empty2\xe6\x1c\n\x03\x41pi\x12j\n\rGetAuthConfig\x12).featureform.serving.metadata.proto.Empty\x1a..featureform.serving.metadata.proto.AuthConfig\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12y\n\rGetEquivalent\x12\x33.featureform.serving.metadata.proto.ResourceVariant\x1a\x33.featureform.serving.metadata.proto.ResourceVariant\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12y\n\rWriteFeatures\x12;.featureform.serving.metadata.proto.StreamingFeatureVariant\x1a).featureform.serving.metadata.proto.Empty(\x01\x12u\n\x0bWriteLabels\x12\x39.featureform.serving.metadata.proto.StreamingLabelVariant\x1a).featureform.serving.metadata.proto.Empty(\x01\x42\'Z%github.com/featureform/metadata/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n featureform/proto/metadata.proto\x12\"featureform.serving.metadata.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x19google/protobuf/any.proto\"T\n\x0eOktaAuthConfig\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12\x1f\n\x17\x61uthorization_server_id\x18\x02 \x01(\t\x12\x11\n\tclient_id\x18\x03 \x01(\t\"\x17\n\x15PassThroughAuthConfig\"\xad\x01\n\nAuthConfig\x12\x42\n\x04okta\x18\x01 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.OktaAuthConfigH\x00\x12Q\n\x0cpass_through\x18\x02 \x01(\x0b\x32\x39.featureform.serving.metadata.proto.PassThroughAuthConfigH\x00\x42\x08\n\x06\x63onfig\"\x14\n\x04Name\x12\x0c\n\x04name\x18\x01 \x01(\t\"S\n\x0b\x45rrorStatus\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12%\n\x07\x64\x65tails\x18\x03 \x03(\x0b\x32\x14.google.protobuf.Any\"\x9f\x02\n\x0eResourceStatus\x12I\n\x06status\x18\x01 \x01(\x0e\x32\x39.featureform.serving.metadata.proto.ResourceStatus.Status\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12\x45\n\x0c\x65rror_status\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.ErrorStatus\"d\n\x06Status\x12\r\n\tNO_STATUS\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\t\n\x05READY\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04\x12\x0b\n\x07RUNNING\x10\x05\x12\r\n\tCANCELLED\x10\x06\"\x98\x01\n\nResourceID\x12\x41\n\x08resource\x18\x01 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12G\n\rresource_type\x18\x02 \x01(\x0e\x32\x30.featureform.serving.metadata.proto.ResourceType\"\x9b\x01\n\x10SetStatusRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\"n\n\x15ScheduleChangeRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x10\n\x08schedule\x18\x02 \x01(\t\",\n\x0bNameVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\"\x07\n\x05\x45mpty\"\x86\x01\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"4\n\x07\x43olumns\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\n\n\x02ts\x18\x03 \x01(\t\"\x1f\n\x0ePythonFunction\x12\r\n\x05query\x18\x01 \x01(\x0c\"\"\n\x06Stream\x12\x18\n\x10offline_provider\x18\x01 \x01(\t\"\xdc\x02\n\x0fResourceVariant\x12M\n\x0f\x66\x65\x61ture_variant\x18\x01 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.FeatureVariantH\x00\x12I\n\rlabel_variant\x18\x02 \x01(\x0b\x32\x30.featureform.serving.metadata.proto.LabelVariantH\x00\x12V\n\x14training_set_variant\x18\x03 \x01(\x0b\x32\x36.featureform.serving.metadata.proto.TrainingSetVariantH\x00\x12K\n\x0esource_variant\x18\x04 \x01(\x0b\x32\x31.featureform.serving.metadata.proto.SourceVariantH\x00\x42\n\n\x08resource\"\x81\x08\n\x0e\x46\x65\x61tureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12?\n\x06source\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0e\n\x06\x65ntity\x18\x05 \x01(\t\x12+\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x46\n\x08\x66unction\x18\x11 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.PythonFunctionH\x00\x12<\n\x06stream\x18\x15 \x01(\x0b\x32*.featureform.serving.metadata.proto.StreamH\x00\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x36\n\x04tags\x18\x0f \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x10 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x41\n\x04mode\x18\x12 \x01(\x0e\x32\x33.featureform.serving.metadata.proto.ComputationMode\x12\x13\n\x07task_id\x18\x17 \x01(\tB\x02\x18\x01\x12\x14\n\x0ctask_id_list\x18\x18 \x03(\t\x12T\n\x15\x61\x64\x64itional_parameters\x18\x16 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.FeatureParameters\x12;\n\x04type\x18\x19 \x01(\x0b\x32-.featureform.serving.metadata.proto.ValueTypeB\n\n\x08location\"\x97\x01\n\tValueType\x12@\n\x06scalar\x18\x01 \x01(\x0e\x32..featureform.serving.metadata.proto.ScalarTypeH\x00\x12@\n\x06vector\x18\x02 \x01(\x0b\x32..featureform.serving.metadata.proto.VectorTypeH\x00\x42\x06\n\x04Type\"u\n\nVectorType\x12>\n\x06scalar\x18\x01 \x01(\x0e\x32..featureform.serving.metadata.proto.ScalarType\x12\x11\n\tdimension\x18\x02 \x01(\x05\x12\x14\n\x0cis_embedding\x18\x03 \x01(\x08\"\xcf\x01\n\x11\x46\x65\x61tureParameters\x12W\n\x0bprecomputed\x18\x01 \x01(\x0b\x32@.featureform.serving.metadata.proto.PrecomputedFeatureParametersH\x00\x12Q\n\x08ondemand\x18\x02 \x01(\x0b\x32=.featureform.serving.metadata.proto.OndemandFeatureParametersH\x00\x42\x0e\n\x0c\x66\x65\x61ture_type\"\x1e\n\x1cPrecomputedFeatureParameters\"/\n\x19OndemandFeatureParameters\x12\x12\n\ndefinition\x18\x01 \x01(\t\"d\n\nFeatureLag\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\x03lag\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x84\x01\n\x05Label\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xda\x05\n\x0cLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12?\n\x06source\x18\x05 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0e\n\x06\x65ntity\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12<\n\x06stream\x18\x10 \x01(\x0b\x32*.featureform.serving.metadata.proto.StreamH\x00\x12\x36\n\x04tags\x18\r \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x0e \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x13\n\x07task_id\x18\x0f \x01(\tB\x02\x18\x01\x12;\n\x04type\x18\x12 \x01(\x0b\x32-.featureform.serving.metadata.proto.ValueType\x12\x14\n\x0ctask_id_list\x18\x11 \x03(\tB\n\n\x08location\"\xc3\x04\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08software\x18\x04 \x01(\t\x12\x0c\n\x04team\x18\x05 \x01(\t\x12\x19\n\x11serialized_config\x18\x06 \x01(\x0c\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12@\n\x07sources\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x0c \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\r \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x8a\x01\n\x0bTrainingSet\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\x8e\x05\n\x12TrainingSetVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12+\n\x07\x63reated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08provider\x18\x06 \x01(\t\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x05label\x18\t \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x44\n\x0c\x66\x65\x61ture_lags\x18\x0f \x03(\x0b\x32..featureform.serving.metadata.proto.FeatureLag\x12\x36\n\x04tags\x18\x10 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x11 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x13\n\x07task_id\x18\x12 \x01(\tB\x02\x18\x01\x12\x14\n\x0ctask_id_list\x18\x13 \x03(\t\"\xb6\x03\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x42\n\x06status\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x07 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x08 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xf1\x02\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x06 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x07 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xe1\x03\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12@\n\x07sources\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x08 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\t \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x85\x01\n\x06Source\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xf3\x06\n\rSourceVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12L\n\x0etransformation\x18\x0e \x01(\x0b\x32\x32.featureform.serving.metadata.proto.TransformationH\x00\x12\x46\n\x0bprimaryData\x18\x0f \x01(\x0b\x32/.featureform.serving.metadata.proto.PrimaryDataH\x00\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x10\n\x08provider\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06status\x18\x08 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\r\n\x05table\x18\t \x01(\t\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0c \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x10 \x01(\t\x12\x36\n\x04tags\x18\x11 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x12 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x13\n\x07task_id\x18\x13 \x01(\tB\x02\x18\x01\x12\x33\n\x10max_job_duration\x18\x14 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x14\n\x0ctask_id_list\x18\x15 \x03(\tB\x0c\n\ndefinition\"\x95\x02\n\x0eTransformation\x12R\n\x11SQLTransformation\x18\x01 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.SQLTransformationH\x00\x12P\n\x10\x44\x46Transformation\x18\x02 \x01(\x0b\x32\x34.featureform.serving.metadata.proto.DFTransformationH\x00\x12M\n\x0fkubernetes_args\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.KubernetesArgsH\x01\x42\x06\n\x04typeB\x06\n\x04\x61rgs\"o\n\x17KubernetesResourceSpecs\x12\x13\n\x0b\x63pu_request\x18\x01 \x01(\t\x12\x11\n\tcpu_limit\x18\x02 \x01(\t\x12\x16\n\x0ememory_request\x18\x03 \x01(\t\x12\x14\n\x0cmemory_limit\x18\x04 \x01(\t\"r\n\x0eKubernetesArgs\x12\x14\n\x0c\x64ocker_image\x18\x01 \x01(\t\x12J\n\x05specs\x18\x02 \x01(\x0b\x32;.featureform.serving.metadata.proto.KubernetesResourceSpecs\"c\n\x11SQLTransformation\x12\r\n\x05query\x18\x01 \x01(\t\x12?\n\x06source\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"w\n\x10\x44\x46Transformation\x12\r\n\x05query\x18\x01 \x01(\x0c\x12?\n\x06inputs\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x13\n\x0bsource_text\x18\x03 \x01(\t\"_\n\x0bPrimaryData\x12\x44\n\x05table\x18\x01 \x01(\x0b\x32\x33.featureform.serving.metadata.proto.PrimarySQLTableH\x00\x42\n\n\x08location\"\x1f\n\x0fPrimarySQLTable\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x13\n\x04Tags\x12\x0b\n\x03tag\x18\x01 \x03(\t\"+\n\x08Property\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x42\x07\n\x05value\"\xbb\x01\n\nProperties\x12N\n\x08property\x18\x01 \x03(\x0b\x32<.featureform.serving.metadata.proto.Properties.PropertyEntry\x1a]\n\rPropertyEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.featureform.serving.metadata.proto.Property:\x02\x38\x01\"\x7f\n\x17StreamingFeatureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\t\x12&\n\x02ts\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"}\n\x15StreamingLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x04 \x01(\t\x12&\n\x02ts\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp*\xc9\x01\n\x0cResourceType\x12\x0b\n\x07\x46\x45\x41TURE\x10\x00\x12\t\n\x05LABEL\x10\x01\x12\x10\n\x0cTRAINING_SET\x10\x02\x12\n\n\x06SOURCE\x10\x03\x12\x13\n\x0f\x46\x45\x41TURE_VARIANT\x10\x04\x12\x11\n\rLABEL_VARIANT\x10\x05\x12\x18\n\x14TRAINING_SET_VARIANT\x10\x06\x12\x12\n\x0eSOURCE_VARIANT\x10\x07\x12\x0c\n\x08PROVIDER\x10\x08\x12\n\n\x06\x45NTITY\x10\t\x12\t\n\x05MODEL\x10\n\x12\x08\n\x04USER\x10\x0b*F\n\x0f\x43omputationMode\x12\x0f\n\x0bPRECOMPUTED\x10\x00\x12\x13\n\x0f\x43LIENT_COMPUTED\x10\x01\x12\r\n\tSTREAMING\x10\x02*s\n\nScalarType\x12\x08\n\x04NULL\x10\x00\x12\x07\n\x03INT\x10\x01\x12\x0b\n\x07\x46LOAT32\x10\x02\x12\x0b\n\x07\x46LOAT64\x10\x03\x12\n\n\x06STRING\x10\x04\x12\x08\n\x04\x42OOL\x10\x05\x12\t\n\x05INT32\x10\x06\x12\t\n\x05INT64\x10\x07\x12\x0c\n\x08\x44\x41TETIME\x10\x08\x32\xef\x1b\n\x08Metadata\x12j\n\rGetAuthConfig\x12).featureform.serving.metadata.proto.Empty\x1a..featureform.serving.metadata.proto.AuthConfig\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12y\n\rGetEquivalent\x12\x33.featureform.serving.metadata.proto.ResourceVariant\x1a\x33.featureform.serving.metadata.proto.ResourceVariant\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12t\n\x11SetResourceStatus\x12\x34.featureform.serving.metadata.proto.SetStatusRequest\x1a).featureform.serving.metadata.proto.Empty2\xe6\x1c\n\x03\x41pi\x12j\n\rGetAuthConfig\x12).featureform.serving.metadata.proto.Empty\x1a..featureform.serving.metadata.proto.AuthConfig\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12y\n\rGetEquivalent\x12\x33.featureform.serving.metadata.proto.ResourceVariant\x1a\x33.featureform.serving.metadata.proto.ResourceVariant\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12y\n\rWriteFeatures\x12;.featureform.serving.metadata.proto.StreamingFeatureVariant\x1a).featureform.serving.metadata.proto.Empty(\x01\x12u\n\x0bWriteLabels\x12\x39.featureform.serving.metadata.proto.StreamingLabelVariant\x1a).featureform.serving.metadata.proto.Empty(\x01\x42\'Z%github.com/featureform/metadata/protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'featureform.proto.metadata_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z%github.com/featureform/metadata/proto'
@@ -31,18 +31,20 @@
   _globals['_LABELVARIANT'].fields_by_name['task_id']._serialized_options = b'\030\001'
   _globals['_TRAININGSETVARIANT'].fields_by_name['task_id']._options = None
   _globals['_TRAININGSETVARIANT'].fields_by_name['task_id']._serialized_options = b'\030\001'
   _globals['_SOURCEVARIANT'].fields_by_name['task_id']._options = None
   _globals['_SOURCEVARIANT'].fields_by_name['task_id']._serialized_options = b'\030\001'
   _globals['_PROPERTIES_PROPERTYENTRY']._options = None
   _globals['_PROPERTIES_PROPERTYENTRY']._serialized_options = b'8\001'
-  _globals['_RESOURCETYPE']._serialized_start=9248
-  _globals['_RESOURCETYPE']._serialized_end=9449
-  _globals['_COMPUTATIONMODE']._serialized_start=9451
-  _globals['_COMPUTATIONMODE']._serialized_end=9521
+  _globals['_RESOURCETYPE']._serialized_start=9574
+  _globals['_RESOURCETYPE']._serialized_end=9775
+  _globals['_COMPUTATIONMODE']._serialized_start=9777
+  _globals['_COMPUTATIONMODE']._serialized_end=9847
+  _globals['_SCALARTYPE']._serialized_start=9849
+  _globals['_SCALARTYPE']._serialized_end=9964
   _globals['_OKTAAUTHCONFIG']._serialized_start=164
   _globals['_OKTAAUTHCONFIG']._serialized_end=248
   _globals['_PASSTHROUGHAUTHCONFIG']._serialized_start=250
   _globals['_PASSTHROUGHAUTHCONFIG']._serialized_end=273
   _globals['_AUTHCONFIG']._serialized_start=276
   _globals['_AUTHCONFIG']._serialized_end=449
   _globals['_NAME']._serialized_start=451
@@ -70,67 +72,71 @@
   _globals['_PYTHONFUNCTION']._serialized_start=1519
   _globals['_PYTHONFUNCTION']._serialized_end=1550
   _globals['_STREAM']._serialized_start=1552
   _globals['_STREAM']._serialized_end=1586
   _globals['_RESOURCEVARIANT']._serialized_start=1589
   _globals['_RESOURCEVARIANT']._serialized_end=1937
   _globals['_FEATUREVARIANT']._serialized_start=1940
-  _globals['_FEATUREVARIANT']._serialized_end=2959
-  _globals['_FEATUREPARAMETERS']._serialized_start=2962
-  _globals['_FEATUREPARAMETERS']._serialized_end=3169
-  _globals['_PRECOMPUTEDFEATUREPARAMETERS']._serialized_start=3171
-  _globals['_PRECOMPUTEDFEATUREPARAMETERS']._serialized_end=3201
-  _globals['_ONDEMANDFEATUREPARAMETERS']._serialized_start=3203
-  _globals['_ONDEMANDFEATUREPARAMETERS']._serialized_end=3250
-  _globals['_FEATURELAG']._serialized_start=3252
-  _globals['_FEATURELAG']._serialized_end=3352
-  _globals['_LABEL']._serialized_start=3355
-  _globals['_LABEL']._serialized_end=3487
-  _globals['_LABELVARIANT']._serialized_start=3490
-  _globals['_LABELVARIANT']._serialized_end=4173
-  _globals['_PROVIDER']._serialized_start=4176
-  _globals['_PROVIDER']._serialized_end=4755
-  _globals['_TRAININGSET']._serialized_start=4758
-  _globals['_TRAININGSET']._serialized_end=4896
-  _globals['_TRAININGSETVARIANT']._serialized_start=4899
-  _globals['_TRAININGSETVARIANT']._serialized_end=5553
-  _globals['_ENTITY']._serialized_start=5556
-  _globals['_ENTITY']._serialized_end=5994
-  _globals['_MODEL']._serialized_start=5997
-  _globals['_MODEL']._serialized_end=6366
-  _globals['_USER']._serialized_start=6369
-  _globals['_USER']._serialized_end=6850
-  _globals['_SOURCE']._serialized_start=6853
-  _globals['_SOURCE']._serialized_end=6986
-  _globals['_SOURCEVARIANT']._serialized_start=6989
-  _globals['_SOURCEVARIANT']._serialized_end=7872
-  _globals['_TRANSFORMATION']._serialized_start=7875
-  _globals['_TRANSFORMATION']._serialized_end=8152
-  _globals['_KUBERNETESRESOURCESPECS']._serialized_start=8154
-  _globals['_KUBERNETESRESOURCESPECS']._serialized_end=8265
-  _globals['_KUBERNETESARGS']._serialized_start=8267
-  _globals['_KUBERNETESARGS']._serialized_end=8381
-  _globals['_SQLTRANSFORMATION']._serialized_start=8383
-  _globals['_SQLTRANSFORMATION']._serialized_end=8482
-  _globals['_DFTRANSFORMATION']._serialized_start=8484
-  _globals['_DFTRANSFORMATION']._serialized_end=8603
-  _globals['_PRIMARYDATA']._serialized_start=8605
-  _globals['_PRIMARYDATA']._serialized_end=8700
-  _globals['_PRIMARYSQLTABLE']._serialized_start=8702
-  _globals['_PRIMARYSQLTABLE']._serialized_end=8733
-  _globals['_TAGS']._serialized_start=8735
-  _globals['_TAGS']._serialized_end=8754
-  _globals['_PROPERTY']._serialized_start=8756
-  _globals['_PROPERTY']._serialized_end=8799
-  _globals['_PROPERTIES']._serialized_start=8802
-  _globals['_PROPERTIES']._serialized_end=8989
-  _globals['_PROPERTIES_PROPERTYENTRY']._serialized_start=8896
-  _globals['_PROPERTIES_PROPERTYENTRY']._serialized_end=8989
-  _globals['_STREAMINGFEATUREVARIANT']._serialized_start=8991
-  _globals['_STREAMINGFEATUREVARIANT']._serialized_end=9118
-  _globals['_STREAMINGLABELVARIANT']._serialized_start=9120
-  _globals['_STREAMINGLABELVARIANT']._serialized_end=9245
-  _globals['_METADATA']._serialized_start=9524
-  _globals['_METADATA']._serialized_end=13091
-  _globals['_API']._serialized_start=13094
-  _globals['_API']._serialized_end=16780
+  _globals['_FEATUREVARIANT']._serialized_end=2965
+  _globals['_VALUETYPE']._serialized_start=2968
+  _globals['_VALUETYPE']._serialized_end=3119
+  _globals['_VECTORTYPE']._serialized_start=3121
+  _globals['_VECTORTYPE']._serialized_end=3238
+  _globals['_FEATUREPARAMETERS']._serialized_start=3241
+  _globals['_FEATUREPARAMETERS']._serialized_end=3448
+  _globals['_PRECOMPUTEDFEATUREPARAMETERS']._serialized_start=3450
+  _globals['_PRECOMPUTEDFEATUREPARAMETERS']._serialized_end=3480
+  _globals['_ONDEMANDFEATUREPARAMETERS']._serialized_start=3482
+  _globals['_ONDEMANDFEATUREPARAMETERS']._serialized_end=3529
+  _globals['_FEATURELAG']._serialized_start=3531
+  _globals['_FEATURELAG']._serialized_end=3631
+  _globals['_LABEL']._serialized_start=3634
+  _globals['_LABEL']._serialized_end=3766
+  _globals['_LABELVARIANT']._serialized_start=3769
+  _globals['_LABELVARIANT']._serialized_end=4499
+  _globals['_PROVIDER']._serialized_start=4502
+  _globals['_PROVIDER']._serialized_end=5081
+  _globals['_TRAININGSET']._serialized_start=5084
+  _globals['_TRAININGSET']._serialized_end=5222
+  _globals['_TRAININGSETVARIANT']._serialized_start=5225
+  _globals['_TRAININGSETVARIANT']._serialized_end=5879
+  _globals['_ENTITY']._serialized_start=5882
+  _globals['_ENTITY']._serialized_end=6320
+  _globals['_MODEL']._serialized_start=6323
+  _globals['_MODEL']._serialized_end=6692
+  _globals['_USER']._serialized_start=6695
+  _globals['_USER']._serialized_end=7176
+  _globals['_SOURCE']._serialized_start=7179
+  _globals['_SOURCE']._serialized_end=7312
+  _globals['_SOURCEVARIANT']._serialized_start=7315
+  _globals['_SOURCEVARIANT']._serialized_end=8198
+  _globals['_TRANSFORMATION']._serialized_start=8201
+  _globals['_TRANSFORMATION']._serialized_end=8478
+  _globals['_KUBERNETESRESOURCESPECS']._serialized_start=8480
+  _globals['_KUBERNETESRESOURCESPECS']._serialized_end=8591
+  _globals['_KUBERNETESARGS']._serialized_start=8593
+  _globals['_KUBERNETESARGS']._serialized_end=8707
+  _globals['_SQLTRANSFORMATION']._serialized_start=8709
+  _globals['_SQLTRANSFORMATION']._serialized_end=8808
+  _globals['_DFTRANSFORMATION']._serialized_start=8810
+  _globals['_DFTRANSFORMATION']._serialized_end=8929
+  _globals['_PRIMARYDATA']._serialized_start=8931
+  _globals['_PRIMARYDATA']._serialized_end=9026
+  _globals['_PRIMARYSQLTABLE']._serialized_start=9028
+  _globals['_PRIMARYSQLTABLE']._serialized_end=9059
+  _globals['_TAGS']._serialized_start=9061
+  _globals['_TAGS']._serialized_end=9080
+  _globals['_PROPERTY']._serialized_start=9082
+  _globals['_PROPERTY']._serialized_end=9125
+  _globals['_PROPERTIES']._serialized_start=9128
+  _globals['_PROPERTIES']._serialized_end=9315
+  _globals['_PROPERTIES_PROPERTYENTRY']._serialized_start=9222
+  _globals['_PROPERTIES_PROPERTYENTRY']._serialized_end=9315
+  _globals['_STREAMINGFEATUREVARIANT']._serialized_start=9317
+  _globals['_STREAMINGFEATUREVARIANT']._serialized_end=9444
+  _globals['_STREAMINGLABELVARIANT']._serialized_start=9446
+  _globals['_STREAMINGLABELVARIANT']._serialized_end=9571
+  _globals['_METADATA']._serialized_start=9967
+  _globals['_METADATA']._serialized_end=13534
+  _globals['_API']._serialized_start=13537
+  _globals['_API']._serialized_end=17223
 # @@protoc_insertion_point(module_scope)
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata_pb2.pyi` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,43 @@
 class ComputationMode(_ComputationMode, metaclass=_ComputationModeEnumTypeWrapper): ...
 
 PRECOMPUTED: ComputationMode.ValueType  # 0
 CLIENT_COMPUTED: ComputationMode.ValueType  # 1
 STREAMING: ComputationMode.ValueType  # 2
 global___ComputationMode = ComputationMode
 
+class _ScalarType:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _ScalarTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ScalarType.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    NULL: _ScalarType.ValueType  # 0
+    INT: _ScalarType.ValueType  # 1
+    FLOAT32: _ScalarType.ValueType  # 2
+    FLOAT64: _ScalarType.ValueType  # 3
+    STRING: _ScalarType.ValueType  # 4
+    BOOL: _ScalarType.ValueType  # 5
+    INT32: _ScalarType.ValueType  # 6
+    INT64: _ScalarType.ValueType  # 7
+    DATETIME: _ScalarType.ValueType  # 8
+
+class ScalarType(_ScalarType, metaclass=_ScalarTypeEnumTypeWrapper): ...
+
+NULL: ScalarType.ValueType  # 0
+INT: ScalarType.ValueType  # 1
+FLOAT32: ScalarType.ValueType  # 2
+FLOAT64: ScalarType.ValueType  # 3
+STRING: ScalarType.ValueType  # 4
+BOOL: ScalarType.ValueType  # 5
+INT32: ScalarType.ValueType  # 6
+INT64: ScalarType.ValueType  # 7
+DATETIME: ScalarType.ValueType  # 8
+global___ScalarType = ScalarType
+
 @typing.final
 class OktaAuthConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DOMAIN_FIELD_NUMBER: builtins.int
     AUTHORIZATION_SERVER_ID_FIELD_NUMBER: builtins.int
     CLIENT_ID_FIELD_NUMBER: builtins.int
@@ -424,15 +453,14 @@
 @typing.final
 class FeatureVariant(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     VARIANT_FIELD_NUMBER: builtins.int
     SOURCE_FIELD_NUMBER: builtins.int
-    TYPE_FIELD_NUMBER: builtins.int
     ENTITY_FIELD_NUMBER: builtins.int
     CREATED_FIELD_NUMBER: builtins.int
     OWNER_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     PROVIDER_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     TRAININGSETS_FIELD_NUMBER: builtins.int
@@ -440,30 +468,26 @@
     FUNCTION_FIELD_NUMBER: builtins.int
     STREAM_FIELD_NUMBER: builtins.int
     LAST_UPDATED_FIELD_NUMBER: builtins.int
     SCHEDULE_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     MODE_FIELD_NUMBER: builtins.int
-    IS_EMBEDDING_FIELD_NUMBER: builtins.int
-    DIMENSION_FIELD_NUMBER: builtins.int
     TASK_ID_FIELD_NUMBER: builtins.int
     TASK_ID_LIST_FIELD_NUMBER: builtins.int
     ADDITIONAL_PARAMETERS_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
     variant: builtins.str
-    type: builtins.str
     entity: builtins.str
     owner: builtins.str
     description: builtins.str
     provider: builtins.str
     schedule: builtins.str
     mode: global___ComputationMode.ValueType
-    is_embedding: builtins.bool
-    dimension: builtins.int
     task_id: builtins.str
     @property
     def source(self) -> global___NameVariant: ...
     @property
     def created(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
     def status(self) -> global___ResourceStatus: ...
@@ -481,21 +505,22 @@
     def tags(self) -> global___Tags: ...
     @property
     def properties(self) -> global___Properties: ...
     @property
     def task_id_list(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def additional_parameters(self) -> global___FeatureParameters: ...
+    @property
+    def type(self) -> global___ValueType: ...
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         variant: builtins.str = ...,
         source: global___NameVariant | None = ...,
-        type: builtins.str = ...,
         entity: builtins.str = ...,
         created: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         owner: builtins.str = ...,
         description: builtins.str = ...,
         provider: builtins.str = ...,
         status: global___ResourceStatus | None = ...,
         trainingsets: collections.abc.Iterable[global___NameVariant] | None = ...,
@@ -503,27 +528,68 @@
         function: global___PythonFunction | None = ...,
         stream: global___Stream | None = ...,
         last_updated: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         schedule: builtins.str = ...,
         tags: global___Tags | None = ...,
         properties: global___Properties | None = ...,
         mode: global___ComputationMode.ValueType = ...,
-        is_embedding: builtins.bool = ...,
-        dimension: builtins.int = ...,
         task_id: builtins.str = ...,
         task_id_list: collections.abc.Iterable[builtins.str] | None = ...,
         additional_parameters: global___FeatureParameters | None = ...,
+        type: global___ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["additional_parameters", b"additional_parameters", "columns", b"columns", "created", b"created", "function", b"function", "last_updated", b"last_updated", "location", b"location", "properties", b"properties", "source", b"source", "status", b"status", "stream", b"stream", "tags", b"tags"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["additional_parameters", b"additional_parameters", "columns", b"columns", "created", b"created", "description", b"description", "dimension", b"dimension", "entity", b"entity", "function", b"function", "is_embedding", b"is_embedding", "last_updated", b"last_updated", "location", b"location", "mode", b"mode", "name", b"name", "owner", b"owner", "properties", b"properties", "provider", b"provider", "schedule", b"schedule", "source", b"source", "status", b"status", "stream", b"stream", "tags", b"tags", "task_id", b"task_id", "task_id_list", b"task_id_list", "trainingsets", b"trainingsets", "type", b"type", "variant", b"variant"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["additional_parameters", b"additional_parameters", "columns", b"columns", "created", b"created", "function", b"function", "last_updated", b"last_updated", "location", b"location", "properties", b"properties", "source", b"source", "status", b"status", "stream", b"stream", "tags", b"tags", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["additional_parameters", b"additional_parameters", "columns", b"columns", "created", b"created", "description", b"description", "entity", b"entity", "function", b"function", "last_updated", b"last_updated", "location", b"location", "mode", b"mode", "name", b"name", "owner", b"owner", "properties", b"properties", "provider", b"provider", "schedule", b"schedule", "source", b"source", "status", b"status", "stream", b"stream", "tags", b"tags", "task_id", b"task_id", "task_id_list", b"task_id_list", "trainingsets", b"trainingsets", "type", b"type", "variant", b"variant"]) -> None: ...
     def WhichOneof(self, oneof_group: typing.Literal["location", b"location"]) -> typing.Literal["columns", "function", "stream"] | None: ...
 
 global___FeatureVariant = FeatureVariant
 
 @typing.final
+class ValueType(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SCALAR_FIELD_NUMBER: builtins.int
+    VECTOR_FIELD_NUMBER: builtins.int
+    scalar: global___ScalarType.ValueType
+    @property
+    def vector(self) -> global___VectorType: ...
+    def __init__(
+        self,
+        *,
+        scalar: global___ScalarType.ValueType = ...,
+        vector: global___VectorType | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing.Literal["Type", b"Type", "scalar", b"scalar", "vector", b"vector"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["Type", b"Type", "scalar", b"scalar", "vector", b"vector"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["Type", b"Type"]) -> typing.Literal["scalar", "vector"] | None: ...
+
+global___ValueType = ValueType
+
+@typing.final
+class VectorType(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SCALAR_FIELD_NUMBER: builtins.int
+    DIMENSION_FIELD_NUMBER: builtins.int
+    IS_EMBEDDING_FIELD_NUMBER: builtins.int
+    scalar: global___ScalarType.ValueType
+    dimension: builtins.int
+    is_embedding: builtins.bool
+    def __init__(
+        self,
+        *,
+        scalar: global___ScalarType.ValueType = ...,
+        dimension: builtins.int = ...,
+        is_embedding: builtins.bool = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dimension", b"dimension", "is_embedding", b"is_embedding", "scalar", b"scalar"]) -> None: ...
+
+global___VectorType = VectorType
+
+@typing.final
 class FeatureParameters(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PRECOMPUTED_FIELD_NUMBER: builtins.int
     ONDEMAND_FIELD_NUMBER: builtins.int
     @property
     def precomputed(self) -> global___PrecomputedFeatureParameters: ...
@@ -622,32 +688,31 @@
 @typing.final
 class LabelVariant(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     VARIANT_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
-    TYPE_FIELD_NUMBER: builtins.int
     SOURCE_FIELD_NUMBER: builtins.int
     ENTITY_FIELD_NUMBER: builtins.int
     CREATED_FIELD_NUMBER: builtins.int
     OWNER_FIELD_NUMBER: builtins.int
     PROVIDER_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     TRAININGSETS_FIELD_NUMBER: builtins.int
     COLUMNS_FIELD_NUMBER: builtins.int
     STREAM_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     TASK_ID_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
     TASK_ID_LIST_FIELD_NUMBER: builtins.int
     name: builtins.str
     variant: builtins.str
     description: builtins.str
-    type: builtins.str
     entity: builtins.str
     owner: builtins.str
     provider: builtins.str
     task_id: builtins.str
     @property
     def source(self) -> global___NameVariant: ...
     @property
@@ -661,37 +726,39 @@
     @property
     def stream(self) -> global___Stream: ...
     @property
     def tags(self) -> global___Tags: ...
     @property
     def properties(self) -> global___Properties: ...
     @property
+    def type(self) -> global___ValueType: ...
+    @property
     def task_id_list(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         variant: builtins.str = ...,
         description: builtins.str = ...,
-        type: builtins.str = ...,
         source: global___NameVariant | None = ...,
         entity: builtins.str = ...,
         created: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         owner: builtins.str = ...,
         provider: builtins.str = ...,
         status: global___ResourceStatus | None = ...,
         trainingsets: collections.abc.Iterable[global___NameVariant] | None = ...,
         columns: global___Columns | None = ...,
         stream: global___Stream | None = ...,
         tags: global___Tags | None = ...,
         properties: global___Properties | None = ...,
         task_id: builtins.str = ...,
+        type: global___ValueType | None = ...,
         task_id_list: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["columns", b"columns", "created", b"created", "location", b"location", "properties", b"properties", "source", b"source", "status", b"status", "stream", b"stream", "tags", b"tags"]) -> builtins.bool: ...
+    def HasField(self, field_name: typing.Literal["columns", b"columns", "created", b"created", "location", b"location", "properties", b"properties", "source", b"source", "status", b"status", "stream", b"stream", "tags", b"tags", "type", b"type"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing.Literal["columns", b"columns", "created", b"created", "description", b"description", "entity", b"entity", "location", b"location", "name", b"name", "owner", b"owner", "properties", b"properties", "provider", b"provider", "source", b"source", "status", b"status", "stream", b"stream", "tags", b"tags", "task_id", b"task_id", "task_id_list", b"task_id_list", "trainingsets", b"trainingsets", "type", b"type", "variant", b"variant"]) -> None: ...
     def WhichOneof(self, oneof_group: typing.Literal["location", b"location"]) -> typing.Literal["columns", "stream"] | None: ...
 
 global___LabelVariant = LabelVariant
 
 @typing.final
 class Provider(google.protobuf.message.Message):
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/metadata_pb2_grpc.py` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/metadata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/serving.proto` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/serving.proto`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/serving_pb2.py` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/serving_pb2.pyi` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/proto/serving_pb2_grpc.py` & `featureform_enterprise-0.13.8rc0/src/featureform/proto/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/register.py` & `featureform_enterprise-0.13.8rc0/src/featureform/register.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .list import *
 from .parse import *
 from .proto import metadata_pb2_grpc as ff_grpc
 from .resources import *
 from .search import search
 from .status_display import display_statuses
 from .tls import insecure_channel, secure_channel
-from .types import pd_to_ff_datatype
+from .types import pd_to_ff_datatype, VectorType
 from .variant_names_generator import get_current_timestamp_variant
 from .variant_names_generator import get_random_name
 
 NameVariant = Tuple[str, str]
 
 s3_config = S3StoreConfig("", "", AWSStaticCredentials("id", "secret"))
 NON_INFERENCE_STORES = [s3_config.type()]
@@ -4078,22 +4078,25 @@
                 )
             if isinstance(feature["type"], ScalarType):
                 feature["type"] = feature["type"].value
             desc = feature.get("description", "")
             feature_tags = feature.get("tags", [])
             feature_properties = feature.get("properties", {})
             additional_Parameters = self._get_additional_parameters(ondemand_feature)
+            is_embedding = feature.get("is_embedding", False)
+            dims = feature.get("dims", 0)
+            value_type = ScalarType(feature["type"])
+            if dims > 0:
+                value_type = VectorType(value_type, dims, is_embedding)
             resource = FeatureVariant(
                 created=None,
                 name=feature["name"],
                 variant=variant,
                 source=source,
-                value_type=feature["type"],
-                is_embedding=feature.get("is_embedding", False),
-                dims=feature.get("dims", 0),
+                value_type=value_type,
                 entity=entity,
                 owner=owner,
                 provider=inference_store,
                 description=desc,
                 schedule=schedule,
                 location=ResourceColumnMapping(
                     entity=entity_column,
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/resources.py` & `featureform_enterprise-0.13.8rc0/src/featureform/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import dill
 import grpc
 from google.protobuf.duration_pb2 import Duration
 from google.rpc import error_details_pb2
 
 
 from . import feature_flag
+from .types import VectorType, type_from_proto
 from .enums import *
 from .exceptions import *
 from .version import check_up_to_date
 
 NameVariant = Tuple[str, str]
 
 # Constants for Pyspark Versions
@@ -1754,39 +1755,34 @@
 
 
 @typechecked
 @dataclass
 class FeatureVariant(ResourceVariant):
     name: str
     source: Any
-    value_type: str
+    value_type: Union[VectorType, ScalarType, str]
     entity: str
     owner: str
     location: ResourceLocation
     description: str
     variant: str
     provider: Optional[str] = None
     created: str = None
-    is_embedding: bool = False
-    dims: int = 0
     tags: list = None
     properties: dict = None
     schedule: str = ""
     schedule_obj: Schedule = None
     status: str = "NO_STATUS"
     error: Optional[str] = None
     additional_parameters: Optional[Additional_Parameters] = None
     server_status: Optional[ServerStatus] = None
 
     def __post_init__(self):
-        col_types = [member.value for member in ScalarType]
-        if self.value_type not in col_types:
-            raise ValueError(
-                f"Invalid feature type ({self.value_type}) must be one of: {col_types}"
-            )
+        if isinstance(self.value_type, str):
+            self.value_type = ScalarType(self.value_type)
 
     def update_schedule(self, schedule) -> None:
         self.schedule_obj = Schedule(
             name=self.name,
             variant=self.variant,
             resource_type=4,
             schedule_string=schedule,
@@ -1806,17 +1802,15 @@
         feature = next(stub.GetFeatureVariants(iter([name_variant])))
 
         return FeatureVariant(
             created=None,
             name=feature.name,
             variant=feature.variant,
             source=(feature.source.name, feature.source.variant),
-            value_type=feature.type,
-            is_embedding=feature.is_embedding,
-            dims=feature.dimension,
+            value_type=type_from_proto(feature.type),
             entity=feature.entity,
             owner=feature.owner,
             provider=feature.provider,
             location=ResourceColumnMapping("", "", ""),
             description=feature.description,
             tags=list(feature.tags.tag),
             properties={k: v for k, v in feature.properties.property.items()},
@@ -1833,17 +1827,15 @@
         serialized = pb.FeatureVariant(
             name=self.name,
             variant=self.variant,
             source=pb.NameVariant(
                 name=self.source[0],
                 variant=self.source[1],
             ),
-            type=self.value_type,
-            is_embedding=self.is_embedding,
-            dimension=self.dims,
+            type=self.value_type.to_proto(),
             entity=self.entity,
             owner=self.owner,
             description=self.description,
             schedule=self.schedule,
             provider=self.provider,
             columns=self.location.proto(),
             mode=ComputationMode.PRECOMPUTED.proto(),
@@ -2129,34 +2121,31 @@
 
 
 @typechecked
 @dataclass
 class LabelVariant(ResourceVariant):
     name: str
     source: Any
-    value_type: str
+    value_type: Union[VectorType, ScalarType, str]
     entity: str
     owner: str
     description: str
     tags: list
     properties: dict
     location: ResourceLocation
     variant: str
     provider: Optional[str] = None
     created: str = None
     status: str = "NO_STATUS"
     error: Optional[str] = None
     server_status: Optional[ServerStatus] = None
 
     def __post_init__(self):
-        col_types = [member.value for member in ScalarType]
-        if self.value_type not in col_types:
-            raise ValueError(
-                f"Invalid label type ({self.value_type}) must be one of: {col_types}"
-            )
+        if isinstance(self.value_type, str):
+            self.value_type = ScalarType(self.value_type)
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
@@ -2166,15 +2155,15 @@
         name_variant = pb.NameVariant(name=self.name, variant=self.variant)
         label = next(stub.GetLabelVariants(iter([name_variant])))
 
         return LabelVariant(
             name=label.name,
             variant=label.variant,
             source=(label.source.name, label.source.variant),
-            value_type=label.type,
+            value_type=type_from_proto(label.type),
             entity=label.entity,
             owner=label.owner,
             provider=label.provider,
             location=ResourceColumnMapping("", "", ""),
             description=label.description,
             tags=list(label.tags.tag),
             properties={k: v for k, v in label.properties.property.items()},
@@ -2190,15 +2179,15 @@
             name=self.name,
             variant=self.variant,
             source=pb.NameVariant(
                 name=self.source[0],
                 variant=self.source[1],
             ),
             provider=self.provider,
-            type=self.value_type,
+            type=self.value_type.to_proto(),
             entity=self.entity,
             owner=self.owner,
             description=self.description,
             columns=self.location.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
             status=pb.ResourceStatus(status=pb.ResourceStatus.NO_STATUS),
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/search.py` & `featureform_enterprise-0.13.8rc0/src/featureform/search.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/serving.py` & `featureform_enterprise-0.13.8rc0/src/featureform/serving.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/status_display.py` & `featureform_enterprise-0.13.8rc0/src/featureform/status_display.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/tls.py` & `featureform_enterprise-0.13.8rc0/src/featureform/tls.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/train_test_split.py` & `featureform_enterprise-0.13.8rc0/src/featureform/train_test_split.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/type_objects.py` & `featureform_enterprise-0.13.8rc0/src/featureform/type_objects.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/variant_names_generator.py` & `featureform_enterprise-0.13.8rc0/src/featureform/variant_names_generator.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform/version.py` & `featureform_enterprise-0.13.8rc0/src/featureform/version.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/PKG-INFO` & `featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform-enterprise
-Version: 0.13.3rc2
+Version: 0.13.8rc0
 Summary: Package for the Featureform Enterprise Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/featureform/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `featureform_enterprise-0.13.3rc2/src/featureform_enterprise.egg-info/SOURCES.txt` & `featureform_enterprise-0.13.8rc0/src/featureform_enterprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 src/featureform/dashboard/out/index.html
 src/featureform/dashboard/out/query.html
 src/featureform/dashboard/out/robots.txt
 src/featureform/dashboard/out/search.html
 src/featureform/dashboard/out/site.webmanifest
 src/featureform/dashboard/out/tasks.html
 src/featureform/dashboard/out/[type]/[entity].html
-src/featureform/dashboard/out/_next/static/DkMZG6iKzRiMRJuCdvb4X/_buildManifest.js
-src/featureform/dashboard/out/_next/static/DkMZG6iKzRiMRJuCdvb4X/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+src/featureform/dashboard/out/_next/static/WuUFdOFgDayRm_IpzsrHl/_buildManifest.js
+src/featureform/dashboard/out/_next/static/WuUFdOFgDayRm_IpzsrHl/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/chunks/72a30a16.feed22892a5cf9b7.js
 src/featureform/dashboard/out/_next/static/chunks/7679.f81bbdabe01d6434.js
 src/featureform/dashboard/out/_next/static/chunks/7856.a10f149ec0da2cc4.js
 src/featureform/dashboard/out/_next/static/chunks/ad7f724d.8aaacf4430f8899f.js
 src/featureform/dashboard/out/_next/static/chunks/framework-f44ba79936f400b5.js
 src/featureform/dashboard/out/_next/static/chunks/main-b492e665e4469b62.js
 src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
```

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_auth.py` & `featureform_enterprise-0.13.8rc0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_autogenerated_variants.py` & `featureform_enterprise-0.13.8rc0/tests/test_autogenerated_variants.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_class_api.py` & `featureform_enterprise-0.13.8rc0/tests/test_class_api.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_cli.py` & `featureform_enterprise-0.13.8rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_client.py` & `featureform_enterprise-0.13.8rc0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_deploy.py` & `featureform_enterprise-0.13.8rc0/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_enums.py` & `featureform_enterprise-0.13.8rc0/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_executor_resources.py` & `featureform_enterprise-0.13.8rc0/tests/test_executor_resources.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_getting_model.py` & `featureform_enterprise-0.13.8rc0/tests/test_getting_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_multi_feature.py` & `featureform_enterprise-0.13.8rc0/tests/test_multi_feature.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_ondemand_features.py` & `featureform_enterprise-0.13.8rc0/tests/test_ondemand_features.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_parse.py` & `featureform_enterprise-0.13.8rc0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_resource_registration.py` & `featureform_enterprise-0.13.8rc0/tests/test_resource_registration.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_search.py` & `featureform_enterprise-0.13.8rc0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_serving_model.py` & `featureform_enterprise-0.13.8rc0/tests/test_serving_model.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_source_columns.py` & `featureform_enterprise-0.13.8rc0/tests/test_source_columns.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_source_dataframe.py` & `featureform_enterprise-0.13.8rc0/tests/test_source_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_spark_provider.py` & `featureform_enterprise-0.13.8rc0/tests/test_spark_provider.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_tags_and_properties.py` & `featureform_enterprise-0.13.8rc0/tests/test_tags_and_properties.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_train_test_split.py` & `featureform_enterprise-0.13.8rc0/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_training_set_dataframe.py` & `featureform_enterprise-0.13.8rc0/tests/test_training_set_dataframe.py`

 * *Files identical despite different names*

### Comparing `featureform_enterprise-0.13.3rc2/tests/test_updating_provider.py` & `featureform_enterprise-0.13.8rc0/tests/test_updating_provider.py`

 * *Files identical despite different names*

