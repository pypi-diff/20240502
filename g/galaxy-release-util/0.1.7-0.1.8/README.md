# Comparing `tmp/galaxy-release-util-0.1.7.tar.gz` & `tmp/galaxy_release_util-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-release-util-0.1.7.tar", last modified: Thu Feb 22 03:03:21 2024, max compression
+gzip compressed data, was "galaxy_release_util-0.1.8.tar", last modified: Thu May  2 09:54:22 2024, max compression
```

## Comparing `galaxy-release-util-0.1.7.tar` & `galaxy_release_util-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:21.438790 galaxy-release-util-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-02-22 03:03:21.438790 galaxy-release-util-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:21.434790 galaxy-release-util-0.1.7/galaxy_release_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22145 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/bootstrap_history.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:21.438790 galaxy-release-util-0.1.7/galaxy_release_util/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/cli/release_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/github_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    27969 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/point_release.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/galaxy_release_util/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:21.438790 galaxy-release-util-0.1.7/galaxy_release_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-02-22 03:03:21.000000 galaxy-release-util-0.1.7/galaxy_release_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-22 03:03:21.000000 galaxy-release-util-0.1.7/galaxy_release_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:03:21.000000 galaxy-release-util-0.1.7/galaxy_release_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:03:21.000000 galaxy-release-util-0.1.7/galaxy_release_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 03:03:21.000000 galaxy-release-util-0.1.7/galaxy_release_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-22 03:03:21.000000 galaxy-release-util-0.1.7/galaxy_release_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-22 03:03:21.438790 galaxy-release-util-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:03:21.438790 galaxy-release-util-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-22 03:03:12.000000 galaxy-release-util-0.1.7/tests/test_release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/galaxy_release_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/bootstrap_history.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/galaxy_release_util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/cli/release_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/github_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28017 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/point_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/galaxy_release_util/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 09:54:22.000000 galaxy_release_util-0.1.8/galaxy_release_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:54:22.553325 galaxy_release_util-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-02 09:54:15.000000 galaxy_release_util-0.1.8/tests/test_release.py
```

### Comparing `galaxy-release-util-0.1.7/HISTORY.rst` & `galaxy_release_util-0.1.8/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 History
 -------
 
 .. to_doc
 
 
 ------------------
-0.1.6 (02-21-2024)
+0.1.8 (02-05-2024)
+------------------
+* Add mypy to CI under python 3.8 by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/11
+* Misc. updates  by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/12
+* Misc. updates to script generating the release publication issue by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/13
+* Fix link to docs on point releases by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/14
+
+------------------
+0.1.7 (21-02-2024)
 ------------------
 * Misc. updates to script by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/9
 
 ------------------
 0.1.6 (14-02-2024)
 ------------------
 * Ignore commit without PR by @mvdbeek in https://github.com/galaxyproject/galaxy-release-util/pull/4
```

### Comparing `galaxy-release-util-0.1.7/LICENSE.txt` & `galaxy_release_util-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.7/PKG-INFO` & `galaxy_release_util-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,15 +63,23 @@
 History
 -------
 
 .. to_doc
 
 
 ------------------
-0.1.6 (02-21-2024)
+0.1.8 (02-05-2024)
+------------------
+* Add mypy to CI under python 3.8 by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/11
+* Misc. updates  by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/12
+* Misc. updates to script generating the release publication issue by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/13
+* Fix link to docs on point releases by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/14
+
+------------------
+0.1.7 (21-02-2024)
 ------------------
 * Misc. updates to script by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/9
 
 ------------------
 0.1.6 (14-02-2024)
 ------------------
 * Ignore commit without PR by @mvdbeek in https://github.com/galaxyproject/galaxy-release-util/pull/4
```

### Comparing `galaxy-release-util-0.1.7/README.rst` & `galaxy_release_util-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.7/galaxy_release_util/bootstrap_history.py` & `galaxy_release_util-0.1.8/galaxy_release_util/bootstrap_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
 Feature description.
 
 Feature3
 --------
 
 Feature description.
 
-Also check out the `${release} user release notes <${release}_announce_user.html>`__
+Also check out the `${release} user release notes <${release}_announce_user.html>`__.
+Are you an admin? Check out `some admin relevant PRs <https://github.com/galaxyproject/galaxy/pulls?q=label%3Ahighlight%2Fadmin+milestone%3A${release}+is%3Aclosed+is%3Apr>`__.
 
 Get Galaxy
 ===========================================================
 
 The code lives at `GitHub <https://github.com/galaxyproject/galaxy>`__ and you should have `Git <https://git-scm.com/>`__ to obtain it.
 
 To get a new Galaxy repository run:
@@ -225,31 +226,31 @@
 - [X] **Prep**
 
     - [X] ~~Create this release issue ``make release-issue``.~~
     - [X] ~~Set freeze date (${freeze_date}).~~
 
 - [ ] **Branch Release (on or around ${freeze_date})**
 
-    - [ ] Ensure all [blocking milestone PRs](https://github.com/galaxyproject/galaxy/pulls?q=is%3Aopen+is%3Apr+milestone%3A${version}) have been merged, delayed, or closed.
+    - [ ] Ensure all [blocking milestone pull requests](https://github.com/galaxyproject/galaxy/pulls?q=is%3Aopen+is%3Apr+milestone%3A${version}) have been merged, delayed, or closed.
 
           make release-check-blocking-prs
 
     - [ ] Add latest database revision identifier (for ``release_${version}`` and ``${version}``) to ``REVISION_TAGS`` in ``galaxy/model/migrations/dbscript.py``.
 
     - [ ] Merge the latest release into dev and push upstream.
 
           make release-merge-stable-to-next RELEASE_PREVIOUS=release_${previous_version}
           make release-push-dev
 
     - [ ] Create and push release branch:
 
           make release-create-rc
 
-    - [ ] Open PRs from your fork of branch ``version-${version}`` to upstream ``release_${version}`` and of ``version-${next_version}.dev`` to ``dev``.
-    - [ ] Update ``MILESTONE_NUMBER`` in the [maintenance bot](https://github.com/galaxyproject/galaxy/blob/dev/.github/workflows/maintenance_bot.yaml) to `${next_version}` so it properly tags new PRs.
+    - [ ] Open pull requests from your fork of branch ``version-${version}`` to upstream ``release_${version}`` and of ``version-${next_version}.dev`` to ``dev``.
+    - [ ] Update ``MILESTONE_NUMBER`` in the [maintenance bot](https://github.com/galaxyproject/galaxy/blob/dev/.github/workflows/maintenance_bot.yaml) to `${next_version}` so it properly tags new pull requests.
 
 - [ ] **Issue Review Timeline Notes**
 
     - [ ] Ensure any security fixes will be ready prior to ${freeze_date} + 1 week, to allow time for notification prior to release.
     - [ ] Ensure ownership of outstanding bugfixes and track progress during freeze.
 
 - [ ] **Deploy and Test Release**
@@ -261,52 +262,49 @@
     - [ ] [Update BioBlend CI testing](https://github.com/galaxyproject/bioblend/blob/main/.github/workflows/test.yaml) to include a ``release_${version}`` target: add ``- release_${version}`` to the ``galaxy_version`` list in ``.github/workflows/test.yaml`` .
     - [ ] Update GALAXY_RELEASE in IUC and devteam github workflows
         - [ ] https://github.com/galaxyproject/tools-iuc/blob/master/.github/workflows/
         - [ ] https://github.com/galaxyproject/tools-devteam/blob/master/.github/workflows/
 
 - [ ] **Create Release Notes**
 
-    - [ ] Review merged PRs and ensure they all have a milestones attached. [Link](https://github.com/galaxyproject/galaxy/pulls?utf8=%E2%9C%93&q=is%3Apr+is%3Amerged+no%3Amilestone+-label%3Amerge+)
-    - [ ] Checkout release branch
+    - [ ] Review merged pull requests and ensure they all have a milestone attached. [Link](https://github.com/galaxyproject/galaxy/pulls?utf8=%E2%9C%93&q=is%3Apr+is%3Amerged+no%3Amilestone+-label%3Amerge+)
+    - [ ] Switch to release branch and create a new branch for release notes
 
           git checkout release_${version} -b ${version}_release_notes
     - [ ] Bootstrap the release notes
 
           make release-bootstrap-history RELEASE_CURR=${version}
     - [ ] Open newly created files and manually curate major topics and release notes.
     - [ ] Run ``python scripts/release-diff.py release_${previous_version}`` and add configuration changes to release notes.
     - [ ] Add new release to doc/source/releases/index.rst
-    - [ ] Commit release notes.
-
-          git add docs/; git commit -m "Release notes for $version"; git push upstream ${version}_release_notes
-    - [ ] Open a pull request for new release note branch.
+    - [ ] Open a pull request for the release notes branch.
     - [ ] Merge release note pull request.
 
 - [ ] **Do Release**
 
     - [ ] Ensure all [blocking milestone issues](https://github.com/galaxyproject/galaxy/issues?q=is%3Aopen+is%3Aissue+milestone%3A${version}) have been resolved.
 
           make release-check-blocking-issues RELEASE_CURR=${version}
-    - [ ] Ensure all [blocking milestone PRs](https://github.com/galaxyproject/galaxy/pulls?q=is%3Aopen+is%3Apr+milestone%3A${version}) have been merged or closed.
+    - [ ] Ensure all [blocking milestone pull requests](https://github.com/galaxyproject/galaxy/pulls?q=is%3Aopen+is%3Apr+milestone%3A${version}) have been merged or closed.
 
           make release-check-blocking-prs RELEASE_CURR=${version}
-    - [ ] Ensure all PRs merged into the pre-release branch during the freeze have [milestones attached](https://github.com/galaxyproject/galaxy/pulls?q=is%3Apr+is%3Aclosed+base%3Arelease_${version}+is%3Amerged+no%3Amilestone) and that they are the not [${next_version} milestones](https://github.com/galaxyproject/galaxy/pulls?q=is%3Apr+is%3Aclosed+base%3Arelease_${version}+is%3Amerged+milestone%3A${next_version})
-    - [ ] Ensure release notes include all PRs added during the freeze by re-running the release note bootstrapping:
+    - [ ] Ensure all pull requests merged into the pre-release branch during the freeze have [milestones attached](https://github.com/galaxyproject/galaxy/pulls?q=is%3Apr+is%3Aclosed+base%3Arelease_${version}+is%3Amerged+no%3Amilestone) and that they are the not [${next_version} milestones](https://github.com/galaxyproject/galaxy/pulls?q=is%3Apr+is%3Aclosed+base%3Arelease_${version}+is%3Amerged+milestone%3A${next_version})
+    - [ ] Ensure release notes include all pull requests added during the freeze by re-running the release note bootstrapping:
 
           make release-bootstrap-history
     - [ ] Ensure previous release is merged into current. [GitHub branch comparison](https://github.com/galaxyproject/galaxy/compare/release_${version}...release_${previous_version})
     - [ ] Create and push release tag:
 
           make release-create
 
     - [ ] Create dev packages:
 
           cd packages && ./build_packages.sh
 
-    - [ ] Create the first point release (v${version}.0) using the instructions at https://docs.galaxyproject.org/en/master/dev/create_release.html
+    - [ ] Create the first point release (v${version}.0) using the instructions at https://docs.galaxyproject.org/en/master/dev/create_point_release.html
     - [ ] Open PR against planemo with a pin to the new packages
 
 - [ ] **Do Docker Release**
 
     - [ ] Change the [dev branch](https://github.com/bgruening/docker-galaxy-stable/tree/dev) of the Galaxy Docker container to ${next_version}
     - [ ] Merge dev into master
```

### Comparing `galaxy-release-util-0.1.7/galaxy_release_util/cli/options.py` & `galaxy_release_util-0.1.8/galaxy_release_util/cli/options.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.7/galaxy_release_util/github_client.py` & `galaxy_release_util-0.1.8/galaxy_release_util/github_client.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.7/galaxy_release_util/metadata.py` & `galaxy_release_util-0.1.8/galaxy_release_util/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.7/galaxy_release_util/point_release.py` & `galaxy_release_util-0.1.8/galaxy_release_util/point_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,44 +168,43 @@
 
     settings = frontend.get_default_settings(Parser)  # type: ignore[attr-defined] ## upstream type stubs not updated?
     document = utils.new_document(str(package.history_rst), settings)
     Parser().parse(package.history_rst.read_text(), document)
     changelog_items: List[ChangelogItem] = []
     root_section = document[0]
     assert isinstance(root_section, docutils.nodes.section)
-    assert root_section.tagname == "section"
-    for release in root_section.children:
+    for node in root_section.children:
         # ignore title and comment
-        assert isinstance(release, (docutils.nodes.title, docutils.nodes.comment, docutils.nodes.section)), release
-        if release.tagname == "section":
-            assert release[0].tagname == "title"
-            release_version = release[0].astext()
+        assert isinstance(node, (docutils.nodes.title, docutils.nodes.comment, docutils.nodes.section)), node
+        if isinstance(node, docutils.nodes.section):
+            release_version = node[0].astext()
             current_date = None
             if " (" in release_version:
                 version_str, current_date = release_version.split(" (")
                 current_date = current_date.split(")")[0]
             else:
                 # this should be a dev-release without changelog items
                 # we will just omit this later
                 version_str = release_version
             current_version = Version(version_str)
             package.add_release(ReleaseItem(version=current_version, date=current_date))
-            changes = []
-            for changelog_item in release[1:]:
+            changes: List = []
+            for changelog_item in node[1:]:
                 # could be bullet list or a nested section with bugfix, docs, etc
-                if changelog_item.tagname == "bullet_list":
+                if isinstance(changelog_item, docutils.nodes.bullet_list):
                     for child in changelog_item.children:
                         add_changelog_item(changes, child)
-                elif changelog_item.tagname == "paragraph":
+                elif isinstance(changelog_item, docutils.nodes.paragraph):
                     changes = changelog_item.rawsource.splitlines()
-                elif changelog_item.tagname == "section":
+                elif isinstance(changelog_item, docutils.nodes.section):
                     kind = changelog_item[0].astext()
                     section_delimiter = "=" * len(kind)
                     changes.append(f"\n{section_delimiter}\n{kind}\n{section_delimiter}\n")
                     for section_changelog_item in changelog_item[1:]:
+                        assert isinstance(section_changelog_item, docutils.nodes.bullet_list)
                         for child in section_changelog_item:
                             add_changelog_item(changes, child)
             changelog_items.append(ChangelogItem(version=current_version, date=current_date, changes=changes))
 
     # Filter out dev release versions without changelog,
     # we're going to add these back after committing the release version
     clean_changelog_items: List[ChangelogItem] = []
```

### Comparing `galaxy-release-util-0.1.7/galaxy_release_util.egg-info/PKG-INFO` & `galaxy_release_util-0.1.8/galaxy_release_util.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,15 +63,23 @@
 History
 -------
 
 .. to_doc
 
 
 ------------------
-0.1.6 (02-21-2024)
+0.1.8 (02-05-2024)
+------------------
+* Add mypy to CI under python 3.8 by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/11
+* Misc. updates  by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/12
+* Misc. updates to script generating the release publication issue by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/13
+* Fix link to docs on point releases by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/14
+
+------------------
+0.1.7 (21-02-2024)
 ------------------
 * Misc. updates to script by @jdavcs in https://github.com/galaxyproject/galaxy-release-util/pull/9
 
 ------------------
 0.1.6 (14-02-2024)
 ------------------
 * Ignore commit without PR by @mvdbeek in https://github.com/galaxyproject/galaxy-release-util/pull/4
```

### Comparing `galaxy-release-util-0.1.7/galaxy_release_util.egg-info/SOURCES.txt` & `galaxy_release_util-0.1.8/galaxy_release_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.7/setup.cfg` & `galaxy_release_util-0.1.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-release-util
 url = https://github.com/galaxyproject/galaxy-release-util
-version = 0.1.7
+version = 0.1.8
 
 [options]
 include_package_data = True
 install_requires = 
 	build
 	click
 	docutils
```

### Comparing `galaxy-release-util-0.1.7/tests/test_release.py` & `galaxy_release_util-0.1.8/tests/test_release.py`

 * *Files identical despite different names*

