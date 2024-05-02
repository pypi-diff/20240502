# Comparing `tmp/crc-bonfire-5.7.1.tar.gz` & `tmp/crc_bonfire-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-bonfire-5.7.1.tar", last modified: Fri Mar 22 20:16:46 2024, max compression
+gzip compressed data, was "crc_bonfire-5.7.2.tar", last modified: Thu May  2 18:50:23 2024, max compression
```

## Comparing `crc-bonfire-5.7.1.tar` & `crc_bonfire-5.7.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.339609 crc-bonfire-5.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.343609 crc-bonfire-5.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    22882 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21622 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.343609 crc-bonfire-5.7.1/bonfire/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47966 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/elastic_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/openshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/qontract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/bonfire/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/resources/default-iqe-cji.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/resources/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/resources/local-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/resources/reservation-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/bonfire/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/build_deploy.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/cicd/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/cicd/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/cicd/bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/crc_bonfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22882 2024-03-22 20:16:46.000000 crc-bonfire-5.7.1/crc_bonfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-22 20:16:46.000000 crc-bonfire-5.7.1/crc_bonfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 20:16:46.000000 crc-bonfire-5.7.1/crc_bonfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 20:16:46.000000 crc-bonfire-5.7.1/crc_bonfire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-22 20:16:46.000000 crc-bonfire-5.7.1/crc_bonfire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 20:16:46.000000 crc-bonfire-5.7.1/crc_bonfire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/entry_points.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-22 20:16:46.351609 crc-bonfire-5.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/tests/data/namespace_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/tests/data/reservation_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/tests/test_app_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/tests/test_bonfire.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/tests/test_get_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:16:46.347609 crc-bonfire-5.7.1/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-22 20:16:35.000000 crc-bonfire-5.7.1/utils/search_replace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.958171 crc_bonfire-5.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.962171 crc_bonfire-5.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.962171 crc_bonfire-5.7.2/bonfire/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47966 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/elastic_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29373 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/qontract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.962171 crc_bonfire-5.7.2/bonfire/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/default-iqe-cji.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/local-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/resources/reservation-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/bonfire/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/build_deploy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/cicd/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/cicd/bootstrap.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/crc_bonfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 18:50:23.000000 crc_bonfire-5.7.2/crc_bonfire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2975380 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/entry_points.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/data/namespace_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/data/reservation_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_app_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:23.966171 crc_bonfire-5.7.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-02 18:50:11.000000 crc_bonfire-5.7.2/utils/search_replace.py
```

### Comparing `crc-bonfire-5.7.1/.github/workflows/release.yml` & `crc_bonfire-5.7.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/.github/workflows/tests.yml` & `crc_bonfire-5.7.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/.gitignore` & `crc_bonfire-5.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/CONTRIBUTING.md` & `crc_bonfire-5.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/Dockerfile` & `crc_bonfire-5.7.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/PKG-INFO` & `crc_bonfire-5.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.7.1
+Version: 5.7.2
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Home-page: https://www.github.com/RedHatInsights/bonfire
 Author: Brandon Squizzato
 Author-email: bsquizza@redhat.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -239,15 +239,15 @@
 * `--frontends=true` -- by default, bonfire will not deploy Frontend resources. Use this flag to enable the deployment of app frontends.
 * `--set-image-tag <image uri>=<tag>` -- use this to change the image tag of a container image that appears in your templates. This does a search/replace for all occurences of `<image uri>` and sets the tag to be `<tag>`
 * `--target-env` -- this changes which deploy target `bonfire` looks up to determine the parameters to apply when processing app templates. By default, the target env is set to `insights-ephemeral`
 * `--ref-env` -- this changes which deploy target `bonfire` looks up to determine the git ref to fetch for your app configuration. For example, using `--ref-env insights-stage` would cause bonfire to deploy the stage git ref of your app and `--ref-env insights-production` would cause bonfire to deploy the production git ref of your app. If a target matching the environment is not found, `bonfire` defaults back to deploying the 'main'/'master' branch.
 * `--set-template-ref <component>=<ref>` -- use this to change the git ref deployed for just a single component.
 * `--set-parameter <component>/<name>=<value>` -- use this to set a parameter value on a specific component's template.
 * `--optional-deps-method <hybrid|all|none>` -- change the way that bonfire processes ClowdApp optional dependencies (see "Dependency Processing" section)
-* `--prefer PARAM_NAME=PARAM_VALUE` -- in cases where bonfire finds more than one deployment target, use this to set the parameter names and values that should be used to select a "preferred" deployment target. This option can be passed in multiple times. `bonfire` will select the target with the highest amount of "preferred parameters" on it. Default is currently set to `ENV=frontends` to select "stable" frontends in the consoledot environments.
+* `--prefer PARAM_NAME=PARAM_VALUE` -- in cases where bonfire finds more than one deployment target, use this to set the parameter names and values that should be used to select a "preferred" deployment target. This option can be passed in multiple times. `bonfire` will select the target with the highest amount of "preferred parameters" on it. Default is currently set to `ENV_NAME=frontends` to select "stable" frontends in the consoledot environments.
 
 
 # Interactions with Ephemeral Namespace Operator
 
 `bonfire` creates/modifies `NamespaceReservation` resources on the cluster to reserve and release namespaces. The template for the object that bonfire applies into the cluster can be found [here](bonfire/resources/reservation-template.yaml)
 
 For more information about how the ephemeral namespace operator works, see its documentation [here](https://github.com/RedHatInsights/ephemeral-namespace-operator)
```

### Comparing `crc-bonfire-5.7.1/README.md` & `crc_bonfire-5.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 * `--frontends=true` -- by default, bonfire will not deploy Frontend resources. Use this flag to enable the deployment of app frontends.
 * `--set-image-tag <image uri>=<tag>` -- use this to change the image tag of a container image that appears in your templates. This does a search/replace for all occurences of `<image uri>` and sets the tag to be `<tag>`
 * `--target-env` -- this changes which deploy target `bonfire` looks up to determine the parameters to apply when processing app templates. By default, the target env is set to `insights-ephemeral`
 * `--ref-env` -- this changes which deploy target `bonfire` looks up to determine the git ref to fetch for your app configuration. For example, using `--ref-env insights-stage` would cause bonfire to deploy the stage git ref of your app and `--ref-env insights-production` would cause bonfire to deploy the production git ref of your app. If a target matching the environment is not found, `bonfire` defaults back to deploying the 'main'/'master' branch.
 * `--set-template-ref <component>=<ref>` -- use this to change the git ref deployed for just a single component.
 * `--set-parameter <component>/<name>=<value>` -- use this to set a parameter value on a specific component's template.
 * `--optional-deps-method <hybrid|all|none>` -- change the way that bonfire processes ClowdApp optional dependencies (see "Dependency Processing" section)
-* `--prefer PARAM_NAME=PARAM_VALUE` -- in cases where bonfire finds more than one deployment target, use this to set the parameter names and values that should be used to select a "preferred" deployment target. This option can be passed in multiple times. `bonfire` will select the target with the highest amount of "preferred parameters" on it. Default is currently set to `ENV=frontends` to select "stable" frontends in the consoledot environments.
+* `--prefer PARAM_NAME=PARAM_VALUE` -- in cases where bonfire finds more than one deployment target, use this to set the parameter names and values that should be used to select a "preferred" deployment target. This option can be passed in multiple times. `bonfire` will select the target with the highest amount of "preferred parameters" on it. Default is currently set to `ENV_NAME=frontends` to select "stable" frontends in the consoledot environments.
 
 
 # Interactions with Ephemeral Namespace Operator
 
 `bonfire` creates/modifies `NamespaceReservation` resources on the cluster to reserve and release namespaces. The template for the object that bonfire applies into the cluster can be found [here](bonfire/resources/reservation-template.yaml)
 
 For more information about how the ephemeral namespace operator works, see its documentation [here](https://github.com/RedHatInsights/ephemeral-namespace-operator)
```

### Comparing `crc-bonfire-5.7.1/bonfire/bonfire.py` & `crc_bonfire-5.7.2/bonfire/bonfire.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/config.py` & `crc_bonfire-5.7.2/bonfire/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 EPHEMERAL_CLUSTER_CLOWDENV_TEMPLATE = resource_filename(
     "bonfire", "resources/ephemeral-cluster-clowdenvironment.yaml"
 )
 DEFAULT_IQE_CJI_TEMPLATE = resource_filename("bonfire", "resources/default-iqe-cji.yaml")
 DEFAULT_CONFIG_DATA = resource_filename("bonfire", "resources/default_config.yaml")
 DEFAULT_RESERVATION_TEMPLATE = resource_filename("bonfire", "resources/reservation-template.yaml")
 
-DEFAULT_GRAPHQL_URL = "https://app-interface.apps.appsrep05ue1.zqxk.p1.openshiftapps.com/graphql"
+DEFAULT_GRAPHQL_URL = (
+    "https://app-interface.apps.rosa.appsrep09ue1.03r5.p3.openshiftapps.com/graphql"
+)
 
 DEFAULT_ELASTICSEARCH_HOST = "https://localhost:9200/"
 DEFAULT_ELASTICSEARCH_INDEX = "search-bonfire"
 DEFAULT_ENABLE_TELEMETRY = "false"
 
 DEFAULT_CLIENT_ID = "bonfire"
```

### Comparing `crc-bonfire-5.7.1/bonfire/elastic_logging.py` & `crc_bonfire-5.7.2/bonfire/elastic_logging.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/local.py` & `crc_bonfire-5.7.2/bonfire/local.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/namespaces.py` & `crc_bonfire-5.7.2/bonfire/namespaces.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/openshift.py` & `crc_bonfire-5.7.2/bonfire/openshift.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/processor.py` & `crc_bonfire-5.7.2/bonfire/processor.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/qontract.py` & `crc_bonfire-5.7.2/bonfire/qontract.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/resources/default-iqe-cji.yaml` & `crc_bonfire-5.7.2/bonfire/resources/default-iqe-cji.yaml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/resources/default_config.yaml` & `crc_bonfire-5.7.2/bonfire/resources/default_config.yaml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml` & `crc_bonfire-5.7.2/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/resources/local-cluster-clowdenvironment.yaml` & `crc_bonfire-5.7.2/bonfire/resources/local-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/secrets.py` & `crc_bonfire-5.7.2/bonfire/secrets.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/bonfire/utils.py` & `crc_bonfire-5.7.2/bonfire/utils.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/cicd/README.md` & `crc_bonfire-5.7.2/cicd/README.md`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/crc_bonfire.egg-info/PKG-INFO` & `crc_bonfire-5.7.2/crc_bonfire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 5.7.1
+Version: 5.7.2
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Home-page: https://www.github.com/RedHatInsights/bonfire
 Author: Brandon Squizzato
 Author-email: bsquizza@redhat.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -239,15 +239,15 @@
 * `--frontends=true` -- by default, bonfire will not deploy Frontend resources. Use this flag to enable the deployment of app frontends.
 * `--set-image-tag <image uri>=<tag>` -- use this to change the image tag of a container image that appears in your templates. This does a search/replace for all occurences of `<image uri>` and sets the tag to be `<tag>`
 * `--target-env` -- this changes which deploy target `bonfire` looks up to determine the parameters to apply when processing app templates. By default, the target env is set to `insights-ephemeral`
 * `--ref-env` -- this changes which deploy target `bonfire` looks up to determine the git ref to fetch for your app configuration. For example, using `--ref-env insights-stage` would cause bonfire to deploy the stage git ref of your app and `--ref-env insights-production` would cause bonfire to deploy the production git ref of your app. If a target matching the environment is not found, `bonfire` defaults back to deploying the 'main'/'master' branch.
 * `--set-template-ref <component>=<ref>` -- use this to change the git ref deployed for just a single component.
 * `--set-parameter <component>/<name>=<value>` -- use this to set a parameter value on a specific component's template.
 * `--optional-deps-method <hybrid|all|none>` -- change the way that bonfire processes ClowdApp optional dependencies (see "Dependency Processing" section)
-* `--prefer PARAM_NAME=PARAM_VALUE` -- in cases where bonfire finds more than one deployment target, use this to set the parameter names and values that should be used to select a "preferred" deployment target. This option can be passed in multiple times. `bonfire` will select the target with the highest amount of "preferred parameters" on it. Default is currently set to `ENV=frontends` to select "stable" frontends in the consoledot environments.
+* `--prefer PARAM_NAME=PARAM_VALUE` -- in cases where bonfire finds more than one deployment target, use this to set the parameter names and values that should be used to select a "preferred" deployment target. This option can be passed in multiple times. `bonfire` will select the target with the highest amount of "preferred parameters" on it. Default is currently set to `ENV_NAME=frontends` to select "stable" frontends in the consoledot environments.
 
 
 # Interactions with Ephemeral Namespace Operator
 
 `bonfire` creates/modifies `NamespaceReservation` resources on the cluster to reserve and release namespaces. The template for the object that bonfire applies into the cluster can be found [here](bonfire/resources/reservation-template.yaml)
 
 For more information about how the ephemeral namespace operator works, see its documentation [here](https://github.com/RedHatInsights/ephemeral-namespace-operator)
```

### Comparing `crc-bonfire-5.7.1/crc_bonfire.egg-info/SOURCES.txt` & `crc_bonfire-5.7.2/crc_bonfire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/demo.gif` & `crc_bonfire-5.7.2/demo.gif`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/entrypoint.sh` & `crc_bonfire-5.7.2/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/setup.cfg` & `crc_bonfire-5.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/tests/data/namespace_data.json` & `crc_bonfire-5.7.2/tests/data/namespace_data.json`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/tests/data/reservation_data.json` & `crc_bonfire-5.7.2/tests/data/reservation_data.json`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/tests/test_app_configs.py` & `crc_bonfire-5.7.2/tests/test_app_configs.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/tests/test_bonfire.py` & `crc_bonfire-5.7.2/tests/test_bonfire.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/tests/test_get_apps.py` & `crc_bonfire-5.7.2/tests/test_get_apps.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/tests/test_processor.py` & `crc_bonfire-5.7.2/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/tests/test_utils.py` & `crc_bonfire-5.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-5.7.1/utils/search_replace.py` & `crc_bonfire-5.7.2/utils/search_replace.py`

 * *Files identical despite different names*

