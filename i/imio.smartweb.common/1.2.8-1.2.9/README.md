# Comparing `tmp/imio.smartweb.common-1.2.8.tar.gz` & `tmp/imio.smartweb.common-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.smartweb.common-1.2.8.tar", last modified: Fri Feb  2 08:33:28 2024, max compression
+gzip compressed data, was "imio.smartweb.common-1.2.9.tar", last modified: Thu Feb  8 12:40:36 2024, max compression
```

## Comparing `imio.smartweb.common-1.2.8.tar` & `imio.smartweb.common-1.2.9.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.827051 imio.smartweb.common-1.2.8/
--rw-r--r--   0 thom       (501) staff       (20)     8177 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/CHANGES.rst
--rw-r--r--   0 thom       (501) staff       (20)       64 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/CONTRIBUTORS.rst
--rw-r--r--   0 thom       (501) staff       (20)      586 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/DEVELOP.rst
--rw-r--r--   0 thom       (501) staff       (20)    18092 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/LICENSE.GPL
--rw-r--r--   0 thom       (501) staff       (20)      655 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/LICENSE.rst
--rw-r--r--   0 thom       (501) staff       (20)      106 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/MANIFEST.in
--rw-r--r--   0 thom       (501) staff       (20)    12495 2024-02-02 08:33:28.827203 imio.smartweb.common-1.2.8/PKG-INFO
--rw-r--r--   0 thom       (501) staff       (20)     3161 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/README.rst
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.781885 imio.smartweb.common-1.2.8/docs/
--rw-r--r--   0 thom       (501) staff       (20)     7966 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/docs/conf.py
--rw-r--r--   0 thom       (501) staff       (20)       83 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/docs/index.rst
--rw-r--r--   0 thom       (501) staff       (20)       64 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/requirements.txt
--rw-r--r--   0 thom       (501) staff       (20)      518 2024-02-02 08:33:28.827811 imio.smartweb.common-1.2.8/setup.cfg
--rw-r--r--   0 thom       (501) staff       (20)     2800 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/setup.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.766828 imio.smartweb.common-1.2.8/src/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.782252 imio.smartweb.common-1.2.8/src/imio/
--rw-r--r--   0 thom       (501) staff       (20)       80 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/__init__.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.785241 imio.smartweb.common-1.2.8/src/imio/smartweb/
--rw-r--r--   0 thom       (501) staff       (20)       80 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/__init__.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.792775 imio.smartweb.common-1.2.8/src/imio/smartweb/common/
--rw-r--r--   0 thom       (501) staff       (20)     2709 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)      610 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/adapters.py
--rw-r--r--   0 thom       (501) staff       (20)      254 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/adapters.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.794159 imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/
--rw-r--r--   0 thom       (501) staff       (20)       24 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)      531 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)      825 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/iam.py
--rw-r--r--   0 thom       (501) staff       (20)      824 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/topics.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.796435 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)     2667 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)     2676 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/cropping.py
--rw-r--r--   0 thom       (501) staff       (20)      151 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/description.pt
--rw-r--r--   0 thom       (501) staff       (20)      517 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/description.py
--rw-r--r--   0 thom       (501) staff       (20)     4168 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/forms.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.796783 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/overrides/
--rw-r--r--   0 thom       (501) staff       (20)     1818 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.798423 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)     1062 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)     1672 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/form.py
--rw-r--r--   0 thom       (501) staff       (20)      205 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/utils.py
--rw-r--r--   0 thom       (501) staff       (20)     1815 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/views.py
--rw-r--r--   0 thom       (501) staff       (20)      297 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/scaling.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.801653 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/
--rw-r--r--   0 thom       (501) staff       (20)      351 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/Makefile
--rw-r--r--   0 thom       (501) staff       (20)      755 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/package.json
--rw-r--r--   0 thom       (501) staff       (20)   403548 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js
--rw-r--r--   0 thom       (501) staff       (20)      397 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css
--rw-r--r--   0 thom       (501) staff       (20)      804 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js
--rw-r--r--   0 thom       (501) staff       (20)      921 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css
--rw-r--r--   0 thom       (501) staff       (20)     1134 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.803017 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/
--rw-r--r--   0 thom       (501) staff       (20)     1380 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/edit.js
--rw-r--r--   0 thom       (501) staff       (20)      402 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/edit.less
--rw-r--r--   0 thom       (501) staff       (20)     2045 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/view.js
--rw-r--r--   0 thom       (501) staff       (20)     1401 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/view.less
--rw-r--r--   0 thom       (501) staff       (20)     1045 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/webpack.config.js
--rw-r--r--   0 thom       (501) staff       (20)      895 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/caching.py
--rw-r--r--   0 thom       (501) staff       (20)      435 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/config.py
--rw-r--r--   0 thom       (501) staff       (20)      796 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)    11341 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/contact_utils.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.804592 imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)      236 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)      642 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/utils.py
--rw-r--r--   0 thom       (501) staff       (20)      642 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/widget.pt
--rw-r--r--   0 thom       (501) staff       (20)      938 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/widget.py
--rw-r--r--   0 thom       (501) staff       (20)     1148 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/indexers.py
--rw-r--r--   0 thom       (501) staff       (20)      324 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/indexers.zcml
--rw-r--r--   0 thom       (501) staff       (20)     1417 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/interfaces.py
--rw-r--r--   0 thom       (501) staff       (20)      260 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/permissions.zcml
--rw-r--r--   0 thom       (501) staff       (20)     3476 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/privacy.py
--rw-r--r--   0 thom       (501) staff       (20)     1772 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/privacy.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.770159 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.806698 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/
--rw-r--r--   0 thom       (501) staff       (20)     1193 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/actions.xml
--rw-r--r--   0 thom       (501) staff       (20)      185 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/browserlayer.xml
--rw-r--r--   0 thom       (501) staff       (20)      576 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/catalog.xml
--rw-r--r--   0 thom       (501) staff       (20)      432 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/metadata.xml
--rw-r--r--   0 thom       (501) staff       (20)    46630 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/registry.xml
--rw-r--r--   0 thom       (501) staff       (20)     1595 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/rolemap.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.807352 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/
--rw-r--r--   0 thom       (501) staff       (20)      163 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/metadata.xml
--rw-r--r--   0 thom       (501) staff       (20)     1010 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/registry.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.808316 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/types/
--rw-r--r--   0 thom       (501) staff       (20)      229 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/types/Collection.xml
--rw-r--r--   0 thom       (501) staff       (20)      358 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/types/Document.xml
--rw-r--r--   0 thom       (501) staff       (20)      312 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/types/Folder.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.808654 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/uninstall/
--rw-r--r--   0 thom       (501) staff       (20)      130 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 thom       (501) staff       (20)     1278 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.809831 imio.smartweb.common-1.2.8/src/imio/smartweb/common/rest/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/rest/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)      301 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/rest/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)     3349 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/rest/search_filters.py
--rw-r--r--   0 thom       (501) staff       (20)     1269 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/rest/utils.py
--rw-r--r--   0 thom       (501) staff       (20)     1053 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/setuphandlers.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.811305 imio.smartweb.common-1.2.8/src/imio/smartweb/common/sharing/
--rw-r--r--   0 thom       (501) staff       (20)       56 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/sharing/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)      255 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/sharing/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)      509 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/sharing/localroles.py
--rw-r--r--   0 thom       (501) staff       (20)      452 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/sharing/permissions.py
--rw-r--r--   0 thom       (501) staff       (20)      224 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/sharing/permissions.zcml
--rw-r--r--   0 thom       (501) staff       (20)     2608 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/subscribers.py
--rw-r--r--   0 thom       (501) staff       (20)      860 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/subscribers.zcml
--rw-r--r--   0 thom       (501) staff       (20)     1964 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/testing.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.816355 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/__init__.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.817375 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/resources/
--rw-r--r--   0 thom       (501) staff       (20)     1185 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/resources/image.png
--rw-r--r--   0 thom       (501) staff       (20)    30604 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/resources/image_1400x800.png
--rw-r--r--   0 thom       (501) staff       (20)    32643 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/resources/image_1800x700.png
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.817734 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/robot/
--rw-r--r--   0 thom       (501) staff       (20)     2011 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/robot/test_example.robot
--rw-r--r--   0 thom       (501) staff       (20)     4736 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_cropping.py
--rw-r--r--   0 thom       (501) staff       (20)     2493 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_description.py
--rw-r--r--   0 thom       (501) staff       (20)     2413 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_forms.py
--rw-r--r--   0 thom       (501) staff       (20)     4960 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_indexes.py
--rw-r--r--   0 thom       (501) staff       (20)     3370 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_local_roles.py
--rw-r--r--   0 thom       (501) staff       (20)     1578 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_permissions.py
--rw-r--r--   0 thom       (501) staff       (20)     2953 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_privacy.py
--rw-r--r--   0 thom       (501) staff       (20)     3799 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_rest.py
--rw-r--r--   0 thom       (501) staff       (20)      955 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_robot.py
--rw-r--r--   0 thom       (501) staff       (20)     2102 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_setup.py
--rw-r--r--   0 thom       (501) staff       (20)     1699 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_subscribers.py
--rw-r--r--   0 thom       (501) staff       (20)     1570 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_text.py
--rw-r--r--   0 thom       (501) staff       (20)     9314 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_utils.py
--rw-r--r--   0 thom       (501) staff       (20)     1738 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_viewlets.py
--rw-r--r--   0 thom       (501) staff       (20)      848 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_vocabularies.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.818815 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)    12591 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/configure.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.776933 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.819135 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/
--rw-r--r--   0 thom       (501) staff       (20)     1346 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.819455 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/
--rw-r--r--   0 thom       (501) staff       (20)      721 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.772824 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.819771 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/
--rw-r--r--   0 thom       (501) staff       (20)      587 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.773234 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.820739 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/
--rw-r--r--   0 thom       (501) staff       (20)      965 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml
--rw-r--r--   0 thom       (501) staff       (20)      888 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml
--rw-r--r--   0 thom       (501) staff       (20)     2366 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.773651 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.821065 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/
--rw-r--r--   0 thom       (501) staff       (20)      565 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.774046 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.821380 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/
--rw-r--r--   0 thom       (501) staff       (20)      535 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.774450 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.821699 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/
--rw-r--r--   0 thom       (501) staff       (20)      224 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/syndication.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.774845 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.822021 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/
--rw-r--r--   0 thom       (501) staff       (20)      372 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/patched-faceted-jquery.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.775260 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.822339 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/
--rw-r--r--   0 thom       (501) staff       (20)      890 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/scales.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.822665 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1017_to_1018/
--rw-r--r--   0 thom       (501) staff       (20)      453 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1017_to_1018/registry.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.775892 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.822983 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/registry/
--rw-r--r--   0 thom       (501) staff       (20)      938 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/registry/scales.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.776290 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.823303 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/registry/
--rw-r--r--   0 thom       (501) staff       (20)      937 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/registry/scales.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.776696 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1023_to_1024/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.823623 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1023_to_1024/registry/
--rw-r--r--   0 thom       (501) staff       (20)      296 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1023_to_1024/registry/scales.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.777096 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.823935 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/registry/
--rw-r--r--   0 thom       (501) staff       (20)     1077 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/registry/scales.xml
--rw-r--r--   0 thom       (501) staff       (20)     5297 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/upgrades.py
--rw-r--r--   0 thom       (501) staff       (20)     5841 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/utils.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.826802 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/
--rw-r--r--   0 thom       (501) staff       (20)       24 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)       33 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/analytics.pt
--rw-r--r--   0 thom       (501) staff       (20)     1278 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/colophon.pt
--rw-r--r--   0 thom       (501) staff       (20)      586 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/colophon.py
--rw-r--r--   0 thom       (501) staff       (20)     1758 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)     1212 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/privacy.pt
--rw-r--r--   0 thom       (501) staff       (20)      449 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/privacy.py
--rw-r--r--   0 thom       (501) staff       (20)      181 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/skip_to_content.pt
--rw-r--r--   0 thom       (501) staff       (20)      496 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/skip_to_content.py
--rw-r--r--   0 thom       (501) staff       (20)     3835 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/vocabularies.py
--rw-r--r--   0 thom       (501) staff       (20)      940 2024-02-02 08:33:27.000000 imio.smartweb.common-1.2.8/src/imio/smartweb/common/vocabularies.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:33:28.784907 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/
--rw-r--r--   0 thom       (501) staff       (20)    12495 2024-02-02 08:33:28.000000 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/PKG-INFO
--rw-r--r--   0 thom       (501) staff       (20)     7058 2024-02-02 08:33:28.000000 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/SOURCES.txt
--rw-r--r--   0 thom       (501) staff       (20)        1 2024-02-02 08:33:28.000000 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/dependency_links.txt
--rw-r--r--   0 thom       (501) staff       (20)       19 2024-02-02 08:33:28.000000 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/namespace_packages.txt
--rw-r--r--   0 thom       (501) staff       (20)        1 2024-02-02 08:33:28.000000 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/not-zip-safe
--rw-r--r--   0 thom       (501) staff       (20)      445 2024-02-02 08:33:28.000000 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/requires.txt
--rw-r--r--   0 thom       (501) staff       (20)        5 2024-02-02 08:33:28.000000 imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/top_level.txt
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     8284 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/CHANGES.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)       64 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)      586 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/DEVELOP.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)    18092 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/LICENSE.GPL
+-rw-rw-r--   0 remi      (1000) remi      (1000)      655 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/LICENSE.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)      106 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/MANIFEST.in
+-rw-rw-r--   0 remi      (1000) remi      (1000)    12602 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3161 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/README.rst
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/docs/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7966 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/docs/conf.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       83 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/docs/index.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)       64 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/requirements.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      518 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/setup.cfg
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2800 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/setup.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/
+-rw-rw-r--   0 remi      (1000) remi      (1000)       80 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/__init__.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/
+-rw-rw-r--   0 remi      (1000) remi      (1000)       80 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/__init__.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2709 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      610 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/adapters.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      254 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/adapters.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/
+-rw-rw-r--   0 remi      (1000) remi      (1000)       24 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      531 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      825 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/iam.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      824 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/topics.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2667 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2676 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/cropping.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      151 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/description.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      517 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/description.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4168 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/forms.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/overrides/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1818 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1062 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1672 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/form.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      205 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/utils.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1815 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/views.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      297 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/scaling.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      351 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/Makefile
+-rw-rw-r--   0 remi      (1000) remi      (1000)      755 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/package.json
+-rw-rw-r--   0 remi      (1000) remi      (1000)   403548 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js
+-rw-rw-r--   0 remi      (1000) remi      (1000)      397 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css
+-rw-rw-r--   0 remi      (1000) remi      (1000)      804 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js
+-rw-rw-r--   0 remi      (1000) remi      (1000)      921 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1134 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1380 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/edit.js
+-rw-rw-r--   0 remi      (1000) remi      (1000)      402 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/edit.less
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2045 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/view.js
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1401 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/view.less
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1045 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/webpack.config.js
+-rw-rw-r--   0 remi      (1000) remi      (1000)      895 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/caching.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      435 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/config.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      796 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)    11341 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/contact_utils.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      236 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      642 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/utils.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      642 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/widget.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      938 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/widget.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1148 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/indexers.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      324 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/indexers.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1417 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/interfaces.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      260 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/permissions.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3476 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/privacy.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1772 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/privacy.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1193 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/actions.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      185 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/browserlayer.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      576 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/catalog.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      432 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/metadata.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)    46630 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/registry.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1595 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/rolemap.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      163 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/metadata.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1010 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/registry.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/types/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      229 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/types/Collection.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      358 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/types/Document.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      312 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/types/Folder.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/uninstall/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      130 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1278 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/rest/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/rest/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      301 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/rest/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3349 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/rest/search_filters.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1269 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/rest/utils.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1053 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/setuphandlers.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/sharing/
+-rw-rw-r--   0 remi      (1000) remi      (1000)       56 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/sharing/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      255 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/sharing/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      509 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/sharing/localroles.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      452 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/sharing/permissions.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      224 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/sharing/permissions.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2608 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/subscribers.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      860 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/subscribers.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1964 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/testing.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.384767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/__init__.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/resources/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1185 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/resources/image.png
+-rw-rw-r--   0 remi      (1000) remi      (1000)    30604 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/resources/image_1400x800.png
+-rw-rw-r--   0 remi      (1000) remi      (1000)    32643 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/resources/image_1800x700.png
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/robot/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2011 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/robot/test_example.robot
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4736 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_cropping.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2493 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_description.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2413 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_forms.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4960 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_indexes.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3370 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_local_roles.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1578 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_permissions.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2953 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_privacy.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3799 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_rest.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      955 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_robot.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2102 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_setup.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1699 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_subscribers.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1570 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_text.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     9314 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_utils.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1738 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_viewlets.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      848 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_vocabularies.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    12785 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/configure.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1346 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      721 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      587 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      965 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      888 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2366 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      565 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      535 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      224 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/syndication.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      372 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/patched-faceted-jquery.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      890 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/scales.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1017_to_1018/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      453 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1017_to_1018/registry.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      938 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/registry/scales.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      937 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/registry/scales.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1023_to_1024/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1023_to_1024/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      296 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1023_to_1024/registry/scales.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/registry/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1077 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/registry/scales.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     5474 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/upgrades.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     5841 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/utils.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.388767 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/
+-rw-rw-r--   0 remi      (1000) remi      (1000)       24 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       33 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/analytics.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1278 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/colophon.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      586 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/colophon.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1758 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1212 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/privacy.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      449 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/privacy.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      181 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/skip_to_content.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      496 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/skip_to_content.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3835 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/vocabularies.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      940 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio/smartweb/common/vocabularies.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-08 12:40:36.380767 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/
+-rw-rw-r--   0 remi      (1000) remi      (1000)    12602 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7058 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       19 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/namespace_packages.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/not-zip-safe
+-rw-rw-r--   0 remi      (1000) remi      (1000)      445 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        5 2024-02-08 12:40:36.000000 imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/top_level.txt
```

### Comparing `imio.smartweb.common-1.2.8/CHANGES.rst` & `imio.smartweb.common-1.2.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.2.9 (2024-02-08)
+------------------
+
+- WEB-4064 : Reindex SolR because of changes in schema
+  [remdub]
+
+
 1.2.8 (2024-02-02)
 ------------------
 
 - Fix skip content sr-only
   [thomlamb]
 
 1.2.7 (2024-01-16)
```

### Comparing `imio.smartweb.common-1.2.8/DEVELOP.rst` & `imio.smartweb.common-1.2.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/LICENSE.GPL` & `imio.smartweb.common-1.2.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/LICENSE.rst` & `imio.smartweb.common-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/PKG-INFO` & `imio.smartweb.common-1.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.common
-Version: 1.2.8
+Version: 1.2.9
 Summary: Common utilities, vocabularies, taxonomies for imio.smartweb & co products
 Home-page: https://github.com/imio/imio.smartweb.common
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.common
 Project-URL: Source, https://github.com/imio/imio.smartweb.common
@@ -131,14 +131,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-02-08)
+------------------
+
+- WEB-4064 : Reindex SolR because of changes in schema
+  [remdub]
+
+
 1.2.8 (2024-02-02)
 ------------------
 
 - Fix skip content sr-only
   [thomlamb]
 
 1.2.7 (2024-01-16)
```

### Comparing `imio.smartweb.common-1.2.8/README.rst` & `imio.smartweb.common-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/docs/conf.py` & `imio.smartweb.common-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/setup.cfg` & `imio.smartweb.common-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/setup.py` & `imio.smartweb.common-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.common",
-    version="1.2.8",
+    version="1.2.9",
     description="Common utilities, vocabularies, taxonomies for imio.smartweb & co products",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/__init__.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/__init__.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/adapters.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/adapters.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/configure.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/iam.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/iam.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/behaviors/topics.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/behaviors/topics.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/configure.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/cropping.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/description.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/description.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/forms.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/configure.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/form.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/form.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/privacy/views.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/privacy/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/package.json` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/package.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/edit.js` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/edit.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/view.js` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/view.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/src/view.less` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/src/view.less`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/browser/static/webpack.config.js` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/browser/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/caching.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/caching.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/configure.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/contact_utils.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/contact_utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/utils.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/widget.pt` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/widget.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/faceted/widget.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/faceted/widget.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/indexers.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/interfaces.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/privacy.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/privacy.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/privacy.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/privacy.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/actions.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/catalog.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/registry.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/default/rolemap.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles/testing/registry.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles/testing/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/profiles.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/rest/search_filters.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/rest/search_filters.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/rest/utils.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/rest/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/setuphandlers.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/subscribers.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/subscribers.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/testing.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/testing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/resources/image.png` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/resources/image.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/resources/image_1400x800.png` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/resources/image_1400x800.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/resources/image_1800x700.png` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/resources/image_1800x700.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/robot/test_example.robot` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_cropping.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_description.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_forms.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_indexes.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_local_roles.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_permissions.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_privacy.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_privacy.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_rest.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_robot.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_setup.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_subscribers.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_text.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_utils.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_viewlets.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_viewlets.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/tests/test_vocabularies.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/configure.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/configure.zcml`

 * *Files 0% similar despite different names*

```diff
@@ -372,8 +372,16 @@
       profile="imio.smartweb.common:default">
     <genericsetup:upgradeDepends
         title="Add 'carre' scales dimensions"
         import_profile="imio.smartweb.common.upgrades:upgrade_1025_to_1026"
         />
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeStep
+      title="Reindex SolR"
+      source="1026"
+      destination="1027"
+      handler=".upgrades.reindex_solr"
+      profile="imio.smartweb.common:default"
+      />
+
 </configure>
```

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/scales.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/scales.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/registry/scales.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1018_to_1019/registry/scales.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/registry/scales.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1022_to_1023/registry/scales.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/registry/scales.xml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/profiles/1025_to_1026/registry/scales.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/upgrades/upgrades.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/upgrades/upgrades.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,7 +142,14 @@
                 "Image",
             ]
         )
         for brain in brains:
             obj = brain.getObject()
             obj.setEffectiveDate(obj.created())
             obj.reindexObject(idxs=["effective"])
+
+
+def reindex_solr(context):
+    portal = api.portal.get()
+    maintenance = portal.unrestrictedTraverse("@@solr-maintenance")
+    maintenance.clear()
+    maintenance.reindex()
```

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/utils.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/colophon.pt` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/colophon.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/colophon.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/colophon.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/configure.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/viewlets/privacy.pt` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/viewlets/privacy.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/vocabularies.py` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio/smartweb/common/vocabularies.zcml` & `imio.smartweb.common-1.2.9/src/imio/smartweb/common/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/PKG-INFO` & `imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.common
-Version: 1.2.8
+Version: 1.2.9
 Summary: Common utilities, vocabularies, taxonomies for imio.smartweb & co products
 Home-page: https://github.com/imio/imio.smartweb.common
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.common
 Project-URL: Source, https://github.com/imio/imio.smartweb.common
@@ -131,14 +131,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-02-08)
+------------------
+
+- WEB-4064 : Reindex SolR because of changes in schema
+  [remdub]
+
+
 1.2.8 (2024-02-02)
 ------------------
 
 - Fix skip content sr-only
   [thomlamb]
 
 1.2.7 (2024-01-16)
```

### Comparing `imio.smartweb.common-1.2.8/src/imio.smartweb.common.egg-info/SOURCES.txt` & `imio.smartweb.common-1.2.9/src/imio.smartweb.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

