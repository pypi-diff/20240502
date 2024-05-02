# Comparing `tmp/pyorthogonalrouting-1.0.0.tar.gz` & `tmp/pyorthogonalrouting-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorthogonalrouting-1.0.0.tar", last modified: Thu Apr 25 14:29:18 2024, max compression
+gzip compressed data, was "pyorthogonalrouting-1.1.1.tar", last modified: Thu May  2 17:17:23 2024, max compression
```

## Comparing `pyorthogonalrouting-1.0.0.tar` & `pyorthogonalrouting-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-25 14:29:18.645678 pyorthogonalrouting-1.0.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2024-04-06 14:22:10.000000 pyorthogonalrouting-1.0.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2268 2024-04-25 14:29:18.645503 pyorthogonalrouting-1.0.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1795 2024-04-06 15:02:25.000000 pyorthogonalrouting-1.0.0/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      795 2024-04-25 13:10:53.000000 pyorthogonalrouting-1.0.0/pyproject.toml
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-04-25 14:29:18.645717 pyorthogonalrouting-1.0.0/setup.cfg
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-25 14:29:18.634997 pyorthogonalrouting-1.0.0/src/
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-25 14:29:18.643797 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      607 2024-04-11 13:00:44.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      648 2024-04-10 14:41:49.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/ConnectorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4004 2024-04-08 00:38:06.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Functions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6405 2024-04-10 15:08:08.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Grid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      247 2024-04-04 20:00:23.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/LeftTopRightBottom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      390 2024-03-31 20:46:11.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Line.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6353 2024-04-13 14:41:34.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/OrthogonalConnector.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1039 2024-03-31 20:47:20.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      567 2024-04-02 23:26:15.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/OrthogonalConnectorOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      589 2024-04-07 17:06:45.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Point.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11420 2024-04-12 20:46:55.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/PointGraph.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2340 2024-04-11 20:33:20.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/PointNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2024-03-31 20:46:23.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Rect.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5423 2024-04-08 20:44:33.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Rectangle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      300 2024-03-31 20:44:39.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Size.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       53 2024-04-06 14:24:59.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-04-25 02:33:04.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-25 14:29:18.645191 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/enumerations/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      209 2024-03-31 20:53:59.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/enumerations/BendDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      134 2024-04-01 17:04:50.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/enumerations/Direction.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      154 2024-04-02 23:01:12.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/enumerations/Side.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-31 19:08:00.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/enumerations/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/enumerations/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-25 14:29:18.645321 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2268 2024-04-25 14:29:18.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1158 2024-04-25 14:29:18.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-04-25 14:29:18.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       20 2024-04-25 14:29:18.000000 pyorthogonalrouting-1.0.0/src/pyorthogonalrouting.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.821650 pyorthogonalrouting-1.1.1/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2024-04-06 14:22:10.000000 pyorthogonalrouting-1.1.1/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2320 2024-05-02 17:17:23.821460 pyorthogonalrouting-1.1.1/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1811 2024-04-25 14:31:09.000000 pyorthogonalrouting-1.1.1/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      817 2024-04-29 00:18:49.000000 pyorthogonalrouting-1.1.1/pyproject.toml
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-05-02 17:17:23.821691 pyorthogonalrouting-1.1.1/setup.cfg
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.813644 pyorthogonalrouting-1.1.1/src/
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.819620 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      607 2024-04-11 13:00:44.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2545 2024-05-01 18:51:12.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Configuration.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      648 2024-04-10 14:41:49.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/ConnectorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4004 2024-04-08 00:38:06.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Functions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6405 2024-04-10 15:08:08.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Grid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      247 2024-04-04 20:00:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/LeftTopRightBottom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      390 2024-03-31 20:46:11.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Line.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6353 2024-04-13 14:41:34.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnector.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1039 2024-03-31 20:47:20.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2024-04-29 00:35:04.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      589 2024-04-07 17:06:45.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Point.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11420 2024-04-12 20:46:55.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointGraph.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2340 2024-04-11 20:33:20.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1036 2024-04-30 00:38:15.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Rect.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5423 2024-04-08 20:44:33.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Rectangle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      424 2024-04-29 01:42:33.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Size.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       53 2024-04-06 14:24:59.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-05-01 18:57:25.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.821128 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      209 2024-03-31 20:53:59.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/BendDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      134 2024-04-01 17:04:50.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/Direction.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      154 2024-04-02 23:01:12.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/Side.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-31 19:08:00.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/enumerations/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-05 23:04:28.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-02 17:17:23.821274 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2320 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1245 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       21 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       20 2024-05-02 17:17:23.000000 pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/top_level.txt
```

### Comparing `pyorthogonalrouting-1.0.0/LICENSE` & `pyorthogonalrouting-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/PKG-INFO` & `pyorthogonalrouting-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyorthogonalrouting
-Version: 1.0.0
+Version: 1.1.1
 Summary: Yet another orthogonal router
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/py-orthogonal-routing
 Keywords: orthogonal,routing,python,pyut
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: codeallybasic==1.3.1
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/py-orthogonal-routing/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/py-orthogonal-routing/tree/master)
-[![PyPI version](https://badge.fury.io/py/pyutmodelv2.svg)](https://badge.fury.io/py/pyutmodelv2)
+[![PyPI version](https://badge.fury.io/py/pyorthogonalrouting.svg)](https://badge.fury.io/py/pyorthogonalrouting)
 
 This is a port of [Orthogonal Connectors](https://gist.github.com/jose-mdz/4a8894c152383b9d7a870c24a04447e4).
 
 ## Developer Notes
 This project uses [buildlackey](https://github.com/hasii2011/buildlackey) for day-to-day development builds
 
 ___
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.0.0 Summary: Yet
+Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.1.1 Summary: Yet
 another orthogonal router Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/py-orthogonal-routing Keywords:
 orthogonal,routing,python,pyut Description-Content-Type: text/markdown License-
-File: LICENSE ![](https://github.com/hasii2011/code-ally-basic/blob/master/
-developer/agpl-license-web-badge-version-2-256x48.png "AGPL") [![Maintenance]
-(https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/
-Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
-dl.circleci.com/status-badge/img/gh/hasii2011/py-orthogonal-routing/tree/
-master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/
-hasii2011/py-orthogonal-routing/tree/master) [![PyPI version](https://
-badge.fury.io/py/pyutmodelv2.svg)](https://badge.fury.io/py/pyutmodelv2) This
-is a port of [Orthogonal Connectors](https://gist.github.com/jose-mdz/
-4a8894c152383b9d7a870c24a04447e4). ## Developer Notes This project uses
-[buildlackey](https://github.com/hasii2011/buildlackey) for day-to-day
-development builds ___ ## Note For all kinds of problems, requests,
-enhancements, bug reports, etc., drop me an e-mail. Written by _H_u_m_b_e_r_t_o_ _A_.
-_S_a_n_c_h_e_z_ _I_I (C) 2024 ![Humberto's Modified Logo](https://
-raw.githubusercontent.com/wiki/hasii2011/gittodoistclone/images/
+File: LICENSE Requires-Dist: codeallybasic==1.3.1 ![](https://github.com/
+hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-
+2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/badge/
+Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
+commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
+hasii2011/py-orthogonal-routing/tree/master.svg?style=shield)](https://
+dl.circleci.com/status-badge/redirect/gh/hasii2011/py-orthogonal-routing/tree/
+master) [![PyPI version](https://badge.fury.io/py/pyorthogonalrouting.svg)]
+(https://badge.fury.io/py/pyorthogonalrouting) This is a port of [Orthogonal
+Connectors](https://gist.github.com/jose-mdz/4a8894c152383b9d7a870c24a04447e4).
+## Developer Notes This project uses [buildlackey](https://github.com/
+hasii2011/buildlackey) for day-to-day development builds ___ ## Note For all
+kinds of problems, requests, enhancements, bug reports, etc., drop me an e-
+mail. Written by _H_u_m_b_e_r_t_o_ _A_._ _S_a_n_c_h_e_z_ _I_I (C) 2024 ![Humberto's Modified Logo]
+(https://raw.githubusercontent.com/wiki/hasii2011/gittodoistclone/images/
 SillyGitHub.png) I am concerned about GitHub's Copilot project I urge you to
 read about the [Give up GitHub](https://GiveUpGitHub.org) campaign from [the
 Software Freedom Conservancy](https://sfconservancy.org). While I do not
 advocate for all the issues listed there, I do not like that a company like
 Microsoft may profit from open source projects. I continue to use GitHub
 because it offers the services I need for free. But I continue to monitor their
 terms of service. Any use of this project's code by GitHub Copilot, past or
```

### Comparing `pyorthogonalrouting-1.0.0/README.md` & `pyorthogonalrouting-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/py-orthogonal-routing/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/py-orthogonal-routing/tree/master)
-[![PyPI version](https://badge.fury.io/py/pyutmodelv2.svg)](https://badge.fury.io/py/pyutmodelv2)
+[![PyPI version](https://badge.fury.io/py/pyorthogonalrouting.svg)](https://badge.fury.io/py/pyorthogonalrouting)
 
 This is a port of [Orthogonal Connectors](https://gist.github.com/jose-mdz/4a8894c152383b9d7a870c24a04447e4).
 
 ## Developer Notes
 This project uses [buildlackey](https://github.com/hasii2011/buildlackey) for day-to-day development builds
 
 ___
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-
 license-web-badge-version-2-256x48.png "AGPL") [![Maintenance](https://
 img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
 StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
 status-badge/img/gh/hasii2011/py-orthogonal-routing/tree/
 master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/
 hasii2011/py-orthogonal-routing/tree/master) [![PyPI version](https://
-badge.fury.io/py/pyutmodelv2.svg)](https://badge.fury.io/py/pyutmodelv2) This
-is a port of [Orthogonal Connectors](https://gist.github.com/jose-mdz/
-4a8894c152383b9d7a870c24a04447e4). ## Developer Notes This project uses
-[buildlackey](https://github.com/hasii2011/buildlackey) for day-to-day
-development builds ___ ## Note For all kinds of problems, requests,
+badge.fury.io/py/pyorthogonalrouting.svg)](https://badge.fury.io/py/
+pyorthogonalrouting) This is a port of [Orthogonal Connectors](https://
+gist.github.com/jose-mdz/4a8894c152383b9d7a870c24a04447e4). ## Developer Notes
+This project uses [buildlackey](https://github.com/hasii2011/buildlackey) for
+day-to-day development builds ___ ## Note For all kinds of problems, requests,
 enhancements, bug reports, etc., drop me an e-mail. Written by _H_u_m_b_e_r_t_o_ _A_.
 _S_a_n_c_h_e_z_ _I_I (C) 2024 ![Humberto's Modified Logo](https://
 raw.githubusercontent.com/wiki/hasii2011/gittodoistclone/images/
 SillyGitHub.png) I am concerned about GitHub's Copilot project I urge you to
 read about the [Give up GitHub](https://GiveUpGitHub.org) campaign from [the
 Software Freedom Conservancy](https://sfconservancy.org). While I do not
 advocate for all the issues listed there, I do not like that a company like
```

### Comparing `pyorthogonalrouting-1.0.0/pyproject.toml` & `pyorthogonalrouting-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = 'Yet another orthogonal router'
 readme = "README.md"
 license = {text = 'GNU AFFERO GENERAL PUBLIC LICENSE'}
 authors = [{name = 'Humberto A. Sanchez II', email = 'Humbert.A.Sanchez.II@gmail.com'}]
 maintainers = [{name = 'Humberto A. Sanchez II', email = 'Humbert.A.Sanchez.II@gmail.com'}]
 keywords = ['orthogonal', 'routing', 'python', 'pyut']
 
-dependencies = []
+dependencies = ['codeallybasic==1.3.1']
 
 [project.urls]
 Repository = 'https://github.com/hasii2011/py-orthogonal-routing'
 
 
 [tool.setuptools.packages.find]
 where = ['src']
```

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Common.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Common.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/ConnectorPoint.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/ConnectorPoint.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Functions.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Functions.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Grid.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Grid.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/OrthogonalConnector.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnector.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorByProduct.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/OrthogonalConnectorOptions.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/OrthogonalConnectorOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 
 
 @dataclass(slots=True)
 class OrthogonalConnectorOptions:
 
     pointA:             ConnectorPoint = NO_CONNECTOR_POINT
     pointB:             ConnectorPoint = NO_CONNECTOR_POINT
-    shapeMargin:        int            = 0
-    globalBoundsMargin: int            = 0
+    shapeMargin:        int            = 20
+    globalBoundsMargin: int            = 50
     globalBounds:       Rect           = NO_RECT
```

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Point.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Point.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/PointGraph.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointGraph.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/PointNode.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/PointNode.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting/Rectangle.py` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting/Rectangle.py`

 * *Files identical despite different names*

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting.egg-info/PKG-INFO` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyorthogonalrouting
-Version: 1.0.0
+Version: 1.1.1
 Summary: Yet another orthogonal router
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/py-orthogonal-routing
 Keywords: orthogonal,routing,python,pyut
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: codeallybasic==1.3.1
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/py-orthogonal-routing/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/py-orthogonal-routing/tree/master)
-[![PyPI version](https://badge.fury.io/py/pyutmodelv2.svg)](https://badge.fury.io/py/pyutmodelv2)
+[![PyPI version](https://badge.fury.io/py/pyorthogonalrouting.svg)](https://badge.fury.io/py/pyorthogonalrouting)
 
 This is a port of [Orthogonal Connectors](https://gist.github.com/jose-mdz/4a8894c152383b9d7a870c24a04447e4).
 
 ## Developer Notes
 This project uses [buildlackey](https://github.com/hasii2011/buildlackey) for day-to-day development builds
 
 ___
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.0.0 Summary: Yet
+Metadata-Version: 2.1 Name: pyorthogonalrouting Version: 1.1.1 Summary: Yet
 another orthogonal router Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/py-orthogonal-routing Keywords:
 orthogonal,routing,python,pyut Description-Content-Type: text/markdown License-
-File: LICENSE ![](https://github.com/hasii2011/code-ally-basic/blob/master/
-developer/agpl-license-web-badge-version-2-256x48.png "AGPL") [![Maintenance]
-(https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/
-Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
-dl.circleci.com/status-badge/img/gh/hasii2011/py-orthogonal-routing/tree/
-master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/
-hasii2011/py-orthogonal-routing/tree/master) [![PyPI version](https://
-badge.fury.io/py/pyutmodelv2.svg)](https://badge.fury.io/py/pyutmodelv2) This
-is a port of [Orthogonal Connectors](https://gist.github.com/jose-mdz/
-4a8894c152383b9d7a870c24a04447e4). ## Developer Notes This project uses
-[buildlackey](https://github.com/hasii2011/buildlackey) for day-to-day
-development builds ___ ## Note For all kinds of problems, requests,
-enhancements, bug reports, etc., drop me an e-mail. Written by _H_u_m_b_e_r_t_o_ _A_.
-_S_a_n_c_h_e_z_ _I_I (C) 2024 ![Humberto's Modified Logo](https://
-raw.githubusercontent.com/wiki/hasii2011/gittodoistclone/images/
+File: LICENSE Requires-Dist: codeallybasic==1.3.1 ![](https://github.com/
+hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-
+2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/badge/
+Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
+commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
+hasii2011/py-orthogonal-routing/tree/master.svg?style=shield)](https://
+dl.circleci.com/status-badge/redirect/gh/hasii2011/py-orthogonal-routing/tree/
+master) [![PyPI version](https://badge.fury.io/py/pyorthogonalrouting.svg)]
+(https://badge.fury.io/py/pyorthogonalrouting) This is a port of [Orthogonal
+Connectors](https://gist.github.com/jose-mdz/4a8894c152383b9d7a870c24a04447e4).
+## Developer Notes This project uses [buildlackey](https://github.com/
+hasii2011/buildlackey) for day-to-day development builds ___ ## Note For all
+kinds of problems, requests, enhancements, bug reports, etc., drop me an e-
+mail. Written by _H_u_m_b_e_r_t_o_ _A_._ _S_a_n_c_h_e_z_ _I_I (C) 2024 ![Humberto's Modified Logo]
+(https://raw.githubusercontent.com/wiki/hasii2011/gittodoistclone/images/
 SillyGitHub.png) I am concerned about GitHub's Copilot project I urge you to
 read about the [Give up GitHub](https://GiveUpGitHub.org) campaign from [the
 Software Freedom Conservancy](https://sfconservancy.org). While I do not
 advocate for all the issues listed there, I do not like that a company like
 Microsoft may profit from open source projects. I continue to use GitHub
 because it offers the services I need for free. But I continue to monitor their
 terms of service. Any use of this project's code by GitHub Copilot, past or
```

### Comparing `pyorthogonalrouting-1.0.0/src/pyorthogonalrouting.egg-info/SOURCES.txt` & `pyorthogonalrouting-1.1.1/src/pyorthogonalrouting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/pyorthogonalrouting/Common.py
+src/pyorthogonalrouting/Configuration.py
 src/pyorthogonalrouting/ConnectorPoint.py
 src/pyorthogonalrouting/Functions.py
 src/pyorthogonalrouting/Grid.py
 src/pyorthogonalrouting/LeftTopRightBottom.py
 src/pyorthogonalrouting/Line.py
 src/pyorthogonalrouting/OrthogonalConnector.py
 src/pyorthogonalrouting/OrthogonalConnectorByProduct.py
@@ -18,13 +19,14 @@
 src/pyorthogonalrouting/Size.py
 src/pyorthogonalrouting/__init__.py
 src/pyorthogonalrouting/_version.py
 src/pyorthogonalrouting/py.typed
 src/pyorthogonalrouting.egg-info/PKG-INFO
 src/pyorthogonalrouting.egg-info/SOURCES.txt
 src/pyorthogonalrouting.egg-info/dependency_links.txt
+src/pyorthogonalrouting.egg-info/requires.txt
 src/pyorthogonalrouting.egg-info/top_level.txt
 src/pyorthogonalrouting/enumerations/BendDirection.py
 src/pyorthogonalrouting/enumerations/Direction.py
 src/pyorthogonalrouting/enumerations/Side.py
 src/pyorthogonalrouting/enumerations/__init__.py
 src/pyorthogonalrouting/enumerations/py.typed
```

