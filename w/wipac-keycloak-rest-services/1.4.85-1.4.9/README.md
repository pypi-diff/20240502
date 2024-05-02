# Comparing `tmp/wipac-keycloak-rest-services-1.4.85.tar.gz` & `tmp/wipac-keycloak-rest-services-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-keycloak-rest-services-1.4.85.tar", last modified: Thu May  2 01:16:10 2024, max compression
+gzip compressed data, was "wipac-keycloak-rest-services-1.4.9.tar", last modified: Wed Jul 19 15:00:02 2023, max compression
```

## Comparing `wipac-keycloak-rest-services-1.4.85.tar` & `wipac-keycloak-rest-services-1.4.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 01:16:10.835881 wipac-keycloak-rest-services-1.4.85/
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-02 01:16:10.835881 wipac-keycloak-rest-services-1.4.85/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3139 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 01:16:10.835881 wipac-keycloak-rest-services-1.4.85/krs/
--rw-r--r--   0 root         (0) root         (0)      514 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20266 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/apps.py
--rw-r--r--   0 root         (0) root         (0)    16594 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     3215 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/email.py
--rw-r--r--   0 root         (0) root         (0)    15570 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/groups.py
--rw-r--r--   0 root         (0) root         (0)     9012 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/institutions.py
--rw-r--r--   0 root         (0) root         (0)    22784 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/ldap.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/py.typed
--rw-r--r--   0 root         (0) root         (0)     5722 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/token.py
--rw-r--r--   0 root         (0) root         (0)     9389 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/users.py
--rw-r--r--   0 root         (0) root         (0)      860 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/krs/util.py
--rw-r--r--   0 root         (0) root         (0)     2306 2024-05-02 01:16:10.835881 wipac-keycloak-rest-services-1.4.85/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-02 01:16:08.000000 wipac-keycloak-rest-services-1.4.85/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 01:16:10.835881 wipac-keycloak-rest-services-1.4.85/wipac_keycloak_rest_services.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-02 01:16:10.000000 wipac-keycloak-rest-services-1.4.85/wipac_keycloak_rest_services.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-05-02 01:16:10.000000 wipac-keycloak-rest-services-1.4.85/wipac_keycloak_rest_services.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 01:16:10.000000 wipac-keycloak-rest-services-1.4.85/wipac_keycloak_rest_services.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-02 01:16:10.000000 wipac-keycloak-rest-services-1.4.85/wipac_keycloak_rest_services.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-02 01:16:10.000000 wipac-keycloak-rest-services-1.4.85/wipac_keycloak_rest_services.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 15:00:02.559593 wipac-keycloak-rest-services-1.4.9/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-19 15:00:02.559593 wipac-keycloak-rest-services-1.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 15:00:02.559593 wipac-keycloak-rest-services-1.4.9/krs/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-19 14:59:58.000000 wipac-keycloak-rest-services-1.4.9/krs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20266 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/apps.py
+-rw-r--r--   0 root         (0) root         (0)    15733 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/email.py
+-rw-r--r--   0 root         (0) root         (0)    10971 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/groups.py
+-rw-r--r--   0 root         (0) root         (0)     8766 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/institutions.py
+-rw-r--r--   0 root         (0) root         (0)    22784 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/ldap.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/token.py
+-rw-r--r--   0 root         (0) root         (0)     9213 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/krs/users.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-07-19 15:00:02.559593 wipac-keycloak-rest-services-1.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-19 14:59:57.000000 wipac-keycloak-rest-services-1.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 15:00:02.559593 wipac-keycloak-rest-services-1.4.9/wipac_keycloak_rest_services.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-19 15:00:02.000000 wipac-keycloak-rest-services-1.4.9/wipac_keycloak_rest_services.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-19 15:00:02.000000 wipac-keycloak-rest-services-1.4.9/wipac_keycloak_rest_services.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 15:00:02.000000 wipac-keycloak-rest-services-1.4.9/wipac_keycloak_rest_services.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-19 15:00:02.000000 wipac-keycloak-rest-services-1.4.9/wipac_keycloak_rest_services.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-19 15:00:02.000000 wipac-keycloak-rest-services-1.4.9/wipac_keycloak_rest_services.egg-info/top_level.txt
```

### Comparing `wipac-keycloak-rest-services-1.4.85/LICENSE` & `wipac-keycloak-rest-services-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.85/PKG-INFO` & `wipac-keycloak-rest-services-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.85
+Version: 1.4.9
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
 Project-URL: Source, https://github.com/WIPACrepo/keycloak-rest-services
 Keywords: keycloak,rest,tools,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: actions
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/wipac-keycloak-rest-services)](https://pypi.org/project/wipac-keycloak-rest-services/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/WIPACrepo/keycloak-rest-services?include_prereleases)](https://github.com/WIPACrepo/keycloak-rest-services/) [![PyPI - License](https://img.shields.io/pypi/l/wipac-keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/WIPACrepo/keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/) [![GitHub issues](https://img.shields.io/github/issues/WIPACrepo/keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/WIPACrepo/keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
@@ -40,15 +40,14 @@
 
 Then, start instances of Keycloak, LDAP, and RabbitMQ in other terminals:
 
     ./resources/start-keycloak.sh
     ./resources/start-ldap.sh
     ./resources/start-rabbitmq.sh
 
-Note that version of Keycloak server used for testing is set in `resources/keycloak-image/Dockerfile`.
 
 Keycloak may take a minute to start. If it does not, check your network settings,
 as it does not play well with VPNs and other more exotic network situations.
 
 Finally, run the tests:
 
     source ./resources/pytest-env.sh
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_1m2to9fx_/tmpe5_9k6_t_TarContainer/0/2", line 94, column 0: CDATA terminal not found*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.85
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.9
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Python: <3.13,>=3.9
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
 actions License-File: LICENSE [![PyPI](https://img.shields.io/pypi/v/wipac-
 keycloak-rest-services)](https://pypi.org/project/wipac-keycloak-rest-services/
 ) [![GitHub release (latest by date including pre-releases)](https://
 img.shields.io/github/v/release/WIPACrepo/keycloak-rest-
 services?include_prereleases)](https://github.com/WIPACrepo/keycloak-rest-
 services/) [![PyPI - License](https://img.shields.io/pypi/l/wipac-keycloak-
@@ -27,24 +27,23 @@
 (https://github.com/WIPACrepo/keycloak-rest-services/
 pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) # keycloak-rest-services
 Services surrounding Keycloak, that use the REST API to read/update state. ##
 Running Tests The tests run automatically in CircleCI, but for those that want
 to run them locally, there is a way. First, build and load the local python
 environment: ./setupenv.sh . env/bin/activate Then, start instances of
 Keycloak, LDAP, and RabbitMQ in other terminals: ./resources/start-keycloak.sh
-./resources/start-ldap.sh ./resources/start-rabbitmq.sh Note that version of
-Keycloak server used for testing is set in `resources/keycloak-image/
-Dockerfile`. Keycloak may take a minute to start. If it does not, check your
-network settings, as it does not play well with VPNs and other more exotic
-network situations. Finally, run the tests: source ./resources/pytest-env.sh
-pytest ### Getting Test Coverage If you want a coverage report, instead of
-running pytest directly, run it under the coverage tool: keycloak_url=http://
-localhost:8080 username=admin password=admin coverage run -m pytest coverage
-html --include='krs*' ## Manually Running Scripts It is possible to manually
-run all of the basic operations for controlling users and groups. 1. Bootstrap
-Keycloak If you do not already have a Keycloak instance, start a test instance
-as shown above. Then, run the bootstrap script to create a realm and the REST
-service account: ```bash keycloak_url=http://localhost:8080 username=admin
-password=admin realm=test python3 -m krs.bootstrap ``` Save the `client_secret`
-that gets printed, as you will need this. 2. User and group actions Now you can
-actually run the scripts, which take the format: ```bash keycloak_url=http://
-localhost:8080 client_id=rest-access client_secret= realm=test python -m krs.
+./resources/start-ldap.sh ./resources/start-rabbitmq.sh Keycloak may take a
+minute to start. If it does not, check your network settings, as it does not
+play well with VPNs and other more exotic network situations. Finally, run the
+tests: source ./resources/pytest-env.sh pytest ### Getting Test Coverage If you
+want a coverage report, instead of running pytest directly, run it under the
+coverage tool: keycloak_url=http://localhost:8080 username=admin password=admin
+coverage run -m pytest coverage html --include='krs*' ## Manually Running
+Scripts It is possible to manually run all of the basic operations for
+controlling users and groups. 1. Bootstrap Keycloak If you do not already have
+a Keycloak instance, start a test instance as shown above. Then, run the
+bootstrap script to create a realm and the REST service account: ```bash
+keycloak_url=http://localhost:8080 username=admin password=admin realm=test
+python3 -m krs.bootstrap ``` Save the `client_secret` that gets printed, as you
+will need this. 2. User and group actions Now you can actually run the scripts,
+which take the format: ```bash keycloak_url=http://localhost:8080
+client_id=rest-access client_secret= realm=test python -m krs.
```

### Comparing `wipac-keycloak-rest-services-1.4.85/README.md` & `wipac-keycloak-rest-services-1.4.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 Then, start instances of Keycloak, LDAP, and RabbitMQ in other terminals:
 
     ./resources/start-keycloak.sh
     ./resources/start-ldap.sh
     ./resources/start-rabbitmq.sh
 
-Note that version of Keycloak server used for testing is set in `resources/keycloak-image/Dockerfile`.
 
 Keycloak may take a minute to start. If it does not, check your network settings,
 as it does not play well with VPNs and other more exotic network situations.
 
 Finally, run the tests:
 
     source ./resources/pytest-env.sh
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_1m2to9fx_/tmpe5_9k6_t_TarContainer/0/3.md", line 70, column 0: CDATA terminal not found*

```diff
@@ -13,24 +13,23 @@
 keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/
 pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) # keycloak-rest-services
 Services surrounding Keycloak, that use the REST API to read/update state. ##
 Running Tests The tests run automatically in CircleCI, but for those that want
 to run them locally, there is a way. First, build and load the local python
 environment: ./setupenv.sh . env/bin/activate Then, start instances of
 Keycloak, LDAP, and RabbitMQ in other terminals: ./resources/start-keycloak.sh
-./resources/start-ldap.sh ./resources/start-rabbitmq.sh Note that version of
-Keycloak server used for testing is set in `resources/keycloak-image/
-Dockerfile`. Keycloak may take a minute to start. If it does not, check your
-network settings, as it does not play well with VPNs and other more exotic
-network situations. Finally, run the tests: source ./resources/pytest-env.sh
-pytest ### Getting Test Coverage If you want a coverage report, instead of
-running pytest directly, run it under the coverage tool: keycloak_url=http://
-localhost:8080 username=admin password=admin coverage run -m pytest coverage
-html --include='krs*' ## Manually Running Scripts It is possible to manually
-run all of the basic operations for controlling users and groups. 1. Bootstrap
-Keycloak If you do not already have a Keycloak instance, start a test instance
-as shown above. Then, run the bootstrap script to create a realm and the REST
-service account: ```bash keycloak_url=http://localhost:8080 username=admin
-password=admin realm=test python3 -m krs.bootstrap ``` Save the `client_secret`
-that gets printed, as you will need this. 2. User and group actions Now you can
-actually run the scripts, which take the format: ```bash keycloak_url=http://
-localhost:8080 client_id=rest-access client_secret= realm=test python -m krs.
+./resources/start-ldap.sh ./resources/start-rabbitmq.sh Keycloak may take a
+minute to start. If it does not, check your network settings, as it does not
+play well with VPNs and other more exotic network situations. Finally, run the
+tests: source ./resources/pytest-env.sh pytest ### Getting Test Coverage If you
+want a coverage report, instead of running pytest directly, run it under the
+coverage tool: keycloak_url=http://localhost:8080 username=admin password=admin
+coverage run -m pytest coverage html --include='krs*' ## Manually Running
+Scripts It is possible to manually run all of the basic operations for
+controlling users and groups. 1. Bootstrap Keycloak If you do not already have
+a Keycloak instance, start a test instance as shown above. Then, run the
+bootstrap script to create a realm and the REST service account: ```bash
+keycloak_url=http://localhost:8080 username=admin password=admin realm=test
+python3 -m krs.bootstrap ``` Save the `client_secret` that gets printed, as you
+will need this. 2. User and group actions Now you can actually run the scripts,
+which take the format: ```bash keycloak_url=http://localhost:8080
+client_id=rest-access client_secret= realm=test python -m krs.
```

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/__init__.py` & `wipac-keycloak-rest-services-1.4.9/krs/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.4.85"
+__version__ = "1.4.9"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/apps.py` & `wipac-keycloak-rest-services-1.4.9/krs/apps.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/bootstrap.py` & `wipac-keycloak-rest-services-1.4.9/krs/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,28 +58,14 @@
     except requests.exceptions.HTTPError:
         print(f'creating realm "{realm}"')
         url = f'{cfg["KEYCLOAK_URL"]}/auth/admin/realms/'
         r = requests.post(url, json={'realm': realm, 'enabled': True},
                           headers={'Authorization': f'bearer {token}'})
         r.raise_for_status()
         print(f'realm "{realm}" created')
-
-        # Enable unmanaged user attributes. Starting with KeyCloak 24, User Profile
-        # is enabled by default. This means that by default KeyCloak only allows user
-        # attributes that are defined by the user attribute schema. This behavior is
-        # different in our production realm because declarative-user-profile was disabled
-        # when our realm was created. So, enable unmanaged user attributes to make the
-        # test realm behave like our production realm.
-        url = f'{cfg["KEYCLOAK_URL"]}/auth/admin/realms/{realm}/users/profile'
-        r = requests.get(url, headers={'Authorization': f'bearer {token}'})
-        r.raise_for_status()
-        json = r.json()
-        json["unmanagedAttributePolicy"] = "ENABLED"
-        requests.put(url, json=json, headers={'Authorization': f'bearer {token}'})
-        r.raise_for_status()
     else:
         print(f'realm "{realm}" already exists')
 
 
 def delete_realm(realm, token=None):
     cfg = from_environment({
         'KEYCLOAK_URL': None,
```

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/email.py` & `wipac-keycloak-rest-services-1.4.9/krs/email.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,37 +35,36 @@
     </style>
   </head>
   <body>
     <header>
       <img alt="IceCube Logo" src="https://res.cloudinary.com/icecube/images/c_scale,w_456,h_120/v1611782268/IC-webheader/IC-webheader.png" srcset="https://res.cloudinary.com/icecube/images/c_scale,w_456,h_120/v1611782268/IC-webheader/IC-webheader.png 1x, https://res.cloudinary.com/icecube/images/c_scale,w_912,h_240/v1611782268/IC-webheader/IC-webheader.png 2x" width="228" height="60" />
     </header>
     <div class="main">
-      <h2>{headline}</h2>
+      <h2>IceCube Identity Management</h2>
       <p>{}</p>
     </div>
     <footer>
       <p>This message was sent via an automated system and does not accept replies.
         For questions, email <a href="mailto:help@icecube.wisc.edu">help@icecube.wisc.edu</a>.
       </p>
       <p class="copyright">© WIPAC, University of Wisconsin-Madison</p>
     </footer>
   </body>
 </html>
 """
 
 
-def send_email(recipient, subject, content, headline="IceCube Identity Management", sender=None):
+def send_email(recipient, subject, content, sender=None):
     """
     Send an email message.
 
     Args:
         recipient (dict): Dict with name and email, or just a string email address
         subject (str): Email subject
         content (str): Email content
-        headline (str): Message headline used in HTML email body
         sender (dict): (optional) Dict with name and email, or just a string email address
     """
     config = from_environment({
         'EMAIL_SENDER': 'no-reply@icecube.wisc.edu',
         'EMAIL_SMTP_SERVER': 'localhost',
         'EMAIL_SMTP_TIMEOUT': 5,  # email should be mostly instant
     })
@@ -74,32 +73,24 @@
         sender = config['EMAIL_SENDER']
 
     msg = EmailMessage()
     msg['Subject'] = subject
     msg['Date'] = localtime()
 
     if isinstance(sender, dict):
-        if '@' in sender['email']:
-            username, domain = sender['email'].split('@')
-        else:
-            username = sender['email']
-            domain = ''
+        username, domain = sender['email'].split('@')
         msg['From'] = Address(sender['name'], username, domain)
     else:
         msg['From'] = sender
 
     if isinstance(recipient, dict):
-        if '@' in recipient['email']:
-            username, domain = recipient['email'].split('@')
-        else:
-            username = recipient['email']
-            domain = ''
+        username, domain = recipient['email'].split('@')
         msg['To'] = (Address(recipient['name'], username, domain),)
     else:
         msg['To'] = recipient
 
     msg.set_content(TEMPLATE.format(content))
-    msg.add_alternative(HTML_TEMPLATE.format(content.replace('\n', '<br>'), headline=headline),
+    msg.add_alternative(HTML_TEMPLATE.format(content.replace('\n', '<br>')),
                         subtype='html')
 
     with smtplib.SMTP(config['EMAIL_SMTP_SERVER'], timeout=config['EMAIL_SMTP_TIMEOUT']) as s:
         s.send_message(msg)
```

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/institutions.py` & `wipac-keycloak-rest-services-1.4.9/krs/institutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,15 @@
     Args:
         experiment (str): experiment name (default: list all experiments)
         filter_func (callable): given a group path and set of attrs, a callable to return true/false
 
     Returns:
         dict: group_path: attrs
     """
-    # Starting with KeyCloak 23, GET /admin/realms/{realm}/groups doesn't populate
-    # subgroups unless "search" parameter is used. It is not clear whether it's
-    # a bug or a feature https://github.com/keycloak/keycloak/issues/27694
-    url = '/groups?briefRepresentation=false&max=10000&search='
+    url = '/groups?briefRepresentation=false&max=10000'
     group_hierarchy = await rest_client.request('GET', url)
     logger.debug('raw list_insts: %r', group_hierarchy)
     ret = {}
 
     def add_groups(groups):
         for g in groups:
             if g['subGroups']:
```

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/ldap.py` & `wipac-keycloak-rest-services-1.4.9/krs/ldap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/rabbitmq.py` & `wipac-keycloak-rest-services-1.4.9/krs/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/token.py` & `wipac-keycloak-rest-services-1.4.9/krs/token.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.85/krs/users.py` & `wipac-keycloak-rest-services-1.4.9/krs/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 """
 User actions against Keycloak.
-
-This code uses custom keycloak attributes that are documented here:
-https://bookstack.icecube.wisc.edu/ops/books/services/page/custom-keycloak-attributes
 """
 import asyncio
 import logging
 from unidecode import unidecode
 
 import requests.exceptions
 
@@ -38,24 +35,25 @@
 async def list_users(search=None, rest_client=None):
     """
     List users in Keycloak.
 
     Returns:
         dict: username: user info
     """
+    start = 0
     inc = 50
     ret = {}
+    data = [0]*inc
 
-    num_users = await rest_client.request('GET', '/users/count')
-
-    for start in range(0, num_users, inc):
-        url = f'/users?&max={min(inc, num_users - start)}&first={start}'
+    while len(data) == inc:
+        url = f'/users?&max={inc}&first={start}'
         if search:
             url += f'&search={search}'
         data = await rest_client.request('GET', url)
+        start += inc
         for u in data:
             _fix_attributes(u)
             ret[u['username']] = u
     return ret
 
 
 async def user_info(username, rest_client=None):
@@ -93,14 +91,15 @@
         attribs = {}
     attribs['canonical_email'] = unidecode(first_name + '.' + last_name).lower().replace(' ', '.') + "@icecube.wisc.edu"
 
     try:
         await user_info(username, rest_client=rest_client)
     except Exception:
         logger.info(f'creating user "{username}"')
+        logger.info(username)
         user = {
             'email': email,
             'firstName': first_name,
             'lastName': last_name,
             'username': username,
             'enabled': True,
             'attributes': attribs,
```

### Comparing `wipac-keycloak-rest-services-1.4.85/setup.cfg` & `wipac-keycloak-rest-services-1.4.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [wipac:cicd_setup_builder]
 pypi_name = wipac-keycloak-rest-services
-python_min = 3.9
+python_min = 3.8
 package_dirs = krs
 author = WIPAC Developers
 author_email = developers@icecube.wisc.edu
 keywords_spaced = keycloak rest tools utilities
 
 [metadata]
 name = wipac-keycloak-rest-services
@@ -20,18 +20,18 @@
 	rest
 	tools
 	utilities
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
+	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: 3.12
 download_url = https://pypi.org/project/wipac-keycloak-rest-services/
 project_urls = 
 	Tracker = https://github.com/WIPACrepo/keycloak-rest-services/issues
 	Source = https://github.com/WIPACrepo/keycloak-rest-services
 
 [semantic_release]
 version_variable = krs/__init__.py:__version__
@@ -45,33 +45,31 @@
 
 [options]
 install_requires = 
 	aio_pika
 	ldap3
 	motor
 	requests
-	unidecode
 	wipac-dev-tools
 	wipac-rest-tools
-python_requires = >=3.9, <3.13
+python_requires = >=3.8, <3.12
 packages = find:
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-asyncio
 	pytest-cov
 	pytest-mock
 	coverage
 	flake8
 actions = 
-	asyncache
 	google-api-python-client
 	google-auth-oauthlib
-	jsonpath_ng
+	unidecode
 
 [options.package_data]
 * = py.typed
 
 [options.packages.find]
 include = 
 	krs
```

### Comparing `wipac-keycloak-rest-services-1.4.85/wipac_keycloak_rest_services.egg-info/PKG-INFO` & `wipac-keycloak-rest-services-1.4.9/wipac_keycloak_rest_services.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.85
+Version: 1.4.9
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
 Project-URL: Source, https://github.com/WIPACrepo/keycloak-rest-services
 Keywords: keycloak,rest,tools,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: actions
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/wipac-keycloak-rest-services)](https://pypi.org/project/wipac-keycloak-rest-services/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/WIPACrepo/keycloak-rest-services?include_prereleases)](https://github.com/WIPACrepo/keycloak-rest-services/) [![PyPI - License](https://img.shields.io/pypi/l/wipac-keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/WIPACrepo/keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/) [![GitHub issues](https://img.shields.io/github/issues/WIPACrepo/keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/WIPACrepo/keycloak-rest-services)](https://github.com/WIPACrepo/keycloak-rest-services/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
@@ -40,15 +40,14 @@
 
 Then, start instances of Keycloak, LDAP, and RabbitMQ in other terminals:
 
     ./resources/start-keycloak.sh
     ./resources/start-ldap.sh
     ./resources/start-rabbitmq.sh
 
-Note that version of Keycloak server used for testing is set in `resources/keycloak-image/Dockerfile`.
 
 Keycloak may take a minute to start. If it does not, check your network settings,
 as it does not play well with VPNs and other more exotic network situations.
 
 Finally, run the tests:
 
     source ./resources/pytest-env.sh
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_1m2to9fx_/tmpe5_9k6_t_TarContainer/0/20", line 94, column 0: CDATA terminal not found*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.85
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.9
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Python: <3.13,>=3.9
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
 actions License-File: LICENSE [![PyPI](https://img.shields.io/pypi/v/wipac-
 keycloak-rest-services)](https://pypi.org/project/wipac-keycloak-rest-services/
 ) [![GitHub release (latest by date including pre-releases)](https://
 img.shields.io/github/v/release/WIPACrepo/keycloak-rest-
 services?include_prereleases)](https://github.com/WIPACrepo/keycloak-rest-
 services/) [![PyPI - License](https://img.shields.io/pypi/l/wipac-keycloak-
@@ -27,24 +27,23 @@
 (https://github.com/WIPACrepo/keycloak-rest-services/
 pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) # keycloak-rest-services
 Services surrounding Keycloak, that use the REST API to read/update state. ##
 Running Tests The tests run automatically in CircleCI, but for those that want
 to run them locally, there is a way. First, build and load the local python
 environment: ./setupenv.sh . env/bin/activate Then, start instances of
 Keycloak, LDAP, and RabbitMQ in other terminals: ./resources/start-keycloak.sh
-./resources/start-ldap.sh ./resources/start-rabbitmq.sh Note that version of
-Keycloak server used for testing is set in `resources/keycloak-image/
-Dockerfile`. Keycloak may take a minute to start. If it does not, check your
-network settings, as it does not play well with VPNs and other more exotic
-network situations. Finally, run the tests: source ./resources/pytest-env.sh
-pytest ### Getting Test Coverage If you want a coverage report, instead of
-running pytest directly, run it under the coverage tool: keycloak_url=http://
-localhost:8080 username=admin password=admin coverage run -m pytest coverage
-html --include='krs*' ## Manually Running Scripts It is possible to manually
-run all of the basic operations for controlling users and groups. 1. Bootstrap
-Keycloak If you do not already have a Keycloak instance, start a test instance
-as shown above. Then, run the bootstrap script to create a realm and the REST
-service account: ```bash keycloak_url=http://localhost:8080 username=admin
-password=admin realm=test python3 -m krs.bootstrap ``` Save the `client_secret`
-that gets printed, as you will need this. 2. User and group actions Now you can
-actually run the scripts, which take the format: ```bash keycloak_url=http://
-localhost:8080 client_id=rest-access client_secret= realm=test python -m krs.
+./resources/start-ldap.sh ./resources/start-rabbitmq.sh Keycloak may take a
+minute to start. If it does not, check your network settings, as it does not
+play well with VPNs and other more exotic network situations. Finally, run the
+tests: source ./resources/pytest-env.sh pytest ### Getting Test Coverage If you
+want a coverage report, instead of running pytest directly, run it under the
+coverage tool: keycloak_url=http://localhost:8080 username=admin password=admin
+coverage run -m pytest coverage html --include='krs*' ## Manually Running
+Scripts It is possible to manually run all of the basic operations for
+controlling users and groups. 1. Bootstrap Keycloak If you do not already have
+a Keycloak instance, start a test instance as shown above. Then, run the
+bootstrap script to create a realm and the REST service account: ```bash
+keycloak_url=http://localhost:8080 username=admin password=admin realm=test
+python3 -m krs.bootstrap ``` Save the `client_secret` that gets printed, as you
+will need this. 2. User and group actions Now you can actually run the scripts,
+which take the format: ```bash keycloak_url=http://localhost:8080
+client_id=rest-access client_secret= realm=test python -m krs.
```

