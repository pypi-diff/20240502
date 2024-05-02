# Comparing `tmp/roadtx-1.7.1.tar.gz` & `tmp/roadtx-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadtx-1.7.1.tar", last modified: Mon Apr 29 12:05:55 2024, max compression
+gzip compressed data, was "roadtx-1.8.0.tar", last modified: Wed May  1 14:39:32 2024, max compression
```

## Comparing `roadtx-1.7.1.tar` & `roadtx-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.526741 roadtx-1.7.1/
--rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-04-29 12:05:55.526741 roadtx-1.7.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.518741 roadtx-1.7.1/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.522741 roadtx-1.7.1/roadtools/roadtx/
--rw-r--r--   0 vsts      (1001) docker     (127)    17458 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/federation.py
--rw-r--r--   0 vsts      (1001) docker     (127)   208284 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/firstpartyscopes.json
--rw-r--r--   0 vsts      (1001) docker     (127)     7865 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/keepass.py
--rw-r--r--   0 vsts      (1001) docker     (127)    72108 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18740 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/selenium.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.522741 roadtx-1.7.1/roadtx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-29 12:05:52.000000 roadtx-1.7.1/roadtx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-29 12:05:55.526741 roadtx-1.7.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1157 2024-04-29 12:04:09.000000 roadtx-1.7.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.463863 roadtx-1.8.0/
+-rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-05-01 14:39:32.463863 roadtx-1.8.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.459863 roadtx-1.8.0/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.463863 roadtx-1.8.0/roadtools/roadtx/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17458 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/federation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   208284 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/firstpartyscopes.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     7865 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/keepass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81212 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23357 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/selenium.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.463863 roadtx-1.8.0/roadtx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-01 14:39:28.000000 roadtx-1.8.0/roadtx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-01 14:39:32.463863 roadtx-1.8.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1157 2024-05-01 14:37:27.000000 roadtx-1.8.0/setup.py
```

### Comparing `roadtx-1.7.1/PKG-INFO` & `roadtx-1.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.7.1
+Version: 1.8.0
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: roadlib>=0.23
+Requires-Dist: roadlib>=0.24
 Requires-Dist: requests
 Requires-Dist: selenium
 Requires-Dist: selenium-wire
 Requires-Dist: pyotp
 Requires-Dist: pycryptodomex
 Requires-Dist: signxml
 Requires-Dist: blinker<1.8.0
```

### Comparing `roadtx-1.7.1/roadtools/roadtx/federation.py` & `roadtx-1.8.0/roadtools/roadtx/federation.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.7.1/roadtools/roadtx/firstpartyscopes.json` & `roadtx-1.8.0/roadtools/roadtx/firstpartyscopes.json`

 * *Files identical despite different names*

### Comparing `roadtx-1.7.1/roadtools/roadtx/keepass.py` & `roadtx-1.8.0/roadtools/roadtx/keepass.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.7.1/roadtools/roadtx/main.py` & `roadtx-1.8.0/roadtools/roadtx/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import os
 import json
 import codecs
 import binascii
 import base64
 import time
+from collections import defaultdict
 from urllib.parse import quote_plus
 from roadtools.roadlib.auth import Authentication, get_data
 from roadtools.roadlib.constants import WELLKNOWN_CLIENTS, WELLKNOWN_RESOURCES, WELLKNOWN_USER_AGENTS
 from roadtools.roadlib.deviceauth import DeviceAuthentication
 from roadtools.roadtx.selenium import SeleniumAuthentication
 from roadtools.roadtx.federation import EncryptedPFX, SAMLSigner, encode_object_guid
 import pyotp
@@ -26,14 +27,48 @@
     subparsers = parser.add_subparsers(dest='command')
 
     # Construct authentication module options
     auth = Authentication()
     auth_parser = subparsers.add_parser('gettokens', aliases=['auth','gettoken'], help='Authenticate to Azure AD and get access/refresh tokens. Supports various authentication methods.')
     auth.get_sub_argparse(auth_parser, for_rr=False)
 
+    # Refresh token helper
+    rttsauth_parser = subparsers.add_parser('refreshtokento', help='Use cached refresh token to switch between resources or clients')
+    clienthelptext = 'Client ID (application ID) to use when authenticating. Accepts aliases (list with roadtx listaliases). Read from token file if not supplied'
+    rttsauth_parser.add_argument('-c',
+                                 '--client',
+                                 action='store',
+                                 help=clienthelptext)
+    rttsauth_parser.add_argument('-r',
+                                 '--resource',
+                                 action='store',
+                                 help='Resource to authenticate to. Either a full URL or alias (list with roadtx listaliases)',
+                                 default='https://graph.windows.net')
+    rttsauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password secret of the application if not a public app')
+    rttsauth_parser.add_argument('-s',
+                                 '--scope',
+                                 action='store',
+                                 help='Scope to use. Will automatically switch to v2.0 auth endpoint if specified. If unsure use -r instead.')
+    rttsauth_parser.add_argument('-t',
+                                 '--tenant',
+                                 action='store',
+                                 help='Tenant ID or domain to auth to')
+    rttsauth_parser.add_argument('--tokenfile',
+                                 action='store',
+                                 help='File to read and store the tokens from/to (default: .roadtools_auth)',
+                                 default='.roadtools_auth')
+    rttsauth_parser.add_argument('--tokens-stdout',
+                                 action='store_true',
+                                 help='Do not store tokens on disk, pipe to stdout instead')
+    rttsauth_parser.add_argument('-ua', '--user-agent', action='store',
+                                 help='Custom user agent to use. Default: Python requests user agent')
+    rttsauth_parser.add_argument('--cae',
+                                 action='store_true',
+                                 help='Request Continuous Access Evaluation tokens (requires use of scope parameter instead of resource)')
+
     # Construct device module
     device_parser = subparsers.add_parser('device', help='Register or join devices to Azure AD')
     device_parser.add_argument('-a',
                                '--action',
                                action='store',
                                choices=['join','register','delete'],
                                default='join',
@@ -127,49 +162,74 @@
                                 help='Do not store tokens on disk, pipe to stdout instead')
     prtauth_parser.add_argument('-ua', '--user-agent', action='store',
                                 help='Custom user agent to use. Default: Python requests user agent')
     prtauth_parser.add_argument('-t',
                                 '--tenant',
                                 action='store',
                                 help='Tenant ID or domain to auth to')
+    prtauth_parser.add_argument('--cae',
+                                action='store_true',
+                                help='Request Continuous Access Evaluation tokens')
+
 
+    prtauth_parser.add_argument('-v3', '--prt-protocol-v3', action='store_true', help='Use PRT protocol version v3')
 
     # Application auth
-    # appauth_parser = subparsers.add_parser('appauth', help='Authenticate as an application')
-    # helptext = 'Client ID (application ID) to use when authenticating.'
-    # appauth_parser.add_argument('-c',
-    #                             '--client',
-    #                             action='store',
-    #                             help=helptext,
-    #                             default='1b730954-1685-4b74-9bfd-dac224a7b894')
-    # appauth_parser.add_argument('-r',
-    #                             '--resource',
-    #                             action='store',
-    #                             help='Resource to authenticate to. Either a full URL or alias (list with roadtx listaliases)',
-    #                             default='https://graph.windows.net')
-    # appauth_parser.add_argument('-s',
-    #                             '--scope',
-    #                             action='store',
-    #                             help='Token scope. Either a full URL or alias (msgraph, aadgraph, devicereg) to use the default.')
-    # appauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password secret of the appliction')
-    # appauth_parser.add_argument('-t',
-    #                             '--tenant',
-    #                             action='store',
-    #                             help='Tenant ID or domain to auth to',
-    #                             required=True)
+    appauth_parser = subparsers.add_parser('appauth', help='Authenticate as an application')
+    helptext = 'Client ID (application ID) to use when authenticating.'
+    appauth_parser.add_argument('-c',
+                                '--client',
+                                action='store',
+                                help=helptext,
+                                default='1b730954-1685-4b74-9bfd-dac224a7b894')
+    appauth_parser.add_argument('-p',
+                                '--password',
+                                action='store',
+                                help="Client secret or password credential for the application, if not using certificates")
+    appauth_parser.add_argument('-r',
+                                '--resource',
+                                action='store',
+                                help='Resource to authenticate to. Either a full URL or alias (list with roadtx listaliases)',
+                                default='https://graph.windows.net')
+    appauth_parser.add_argument('-s',
+                                '--scope',
+                                action='store',
+                                help='Scope to use. Will automatically switch to v2.0 auth endpoint if specified. If unsure use -r instead.')
+    appauth_parser.add_argument('-t',
+                                '--tenant',
+                                action='store',
+                                help='Tenant ID or domain to auth to',
+                                required=True)
+    appauth_parser.add_argument('--cert-pem', action='store', metavar='file', help='Certificate file with Application certificate')
+    appauth_parser.add_argument('--key-pem', action='store', metavar='file', help='Private key file for Application')
+    appauth_parser.add_argument('--cert-pfx', action='store', metavar='file', help='Application cert and key as PFX file')
+    appauth_parser.add_argument('--pfx-pass', action='store', metavar='password', help='PFX file password')
+    appauth_parser.add_argument('--pfx-base64', action='store', metavar='BASE64', help='PFX file as base64 string')
+    appauth_parser.add_argument('--cae',
+                                action='store_true',
+                                help='Request Continuous Access Evaluation tokens (requires use of scope parameter instead of resource)')
+    appauth_parser.add_argument('-ua', '--user-agent', action='store',
+                                help='Custom user agent to use. Default: Python requests user agent')
+    appauth_parser.add_argument('--tokenfile',
+                                action='store',
+                                help='File to store the credentials (default: .roadtools_auth)',
+                                default='.roadtools_auth')
+    appauth_parser.add_argument('--tokens-stdout',
+                                action='store_true',
+                                help='Do not store tokens on disk, pipe to stdout instead')
 
     # Code grant flow auth
     codeauth_parser = subparsers.add_parser('codeauth', help='Code grant flow - exchange code for auth tokens')
     clienthelptext = 'Client ID (application ID) to use when authenticating. Accepts aliases (list with roadtx listaliases)'
     codeauth_parser.add_argument('-c',
                                  '--client',
                                  action='store',
                                  help=clienthelptext,
                                  default='1b730954-1685-4b74-9bfd-dac224a7b894')
-    codeauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password secret of the appliction if not a public app')
+    codeauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password secret of the application if not a public app')
     codeauth_parser.add_argument('-r',
                                  '--resource',
                                  action='store',
                                  help='Resource to authenticate to. Either a full URL or alias (list with roadtx listaliases)',
                                  default='https://graph.windows.net')
     codeauth_parser.add_argument('-s',
                                  '--scope',
@@ -185,14 +245,17 @@
     codeauth_parser.add_argument('--tokenfile',
                                  action='store',
                                  help='File to store the credentials (default: .roadtools_auth)',
                                  default='.roadtools_auth')
     codeauth_parser.add_argument('--tokens-stdout',
                                  action='store_true',
                                  help='Do not store tokens on disk, pipe to stdout instead')
+    codeauth_parser.add_argument('--cae',
+                                 action='store_true',
+                                 help='Request Continuous Access Evaluation tokens (requires use of scope parameter instead of resource)')
     codeauth_parser.add_argument('code',
                                  action='store',
                                  help="Code to auth with that you got from Azure AD")
 
     # Bulk enrollment token
     bulkenrollment_parser = subparsers.add_parser('bulkenrollmenttoken', help='Request / use bulk enrollment tokens')
     bulkenrollment_parser.add_argument('--access-token', action='store', help='Access token for the device registration service. If not specified, taken from .roadtools_auth or file specified with --tokenfile')
@@ -266,15 +329,15 @@
     describe_parser = subparsers.add_parser('describe', help='Decode and describe an access token')
     describe_parser.add_argument('-t', '--token', default=None, action='store', metavar='TOKEN', help='Token data to describe. Defaults to reading from stdin')
     describe_parser.add_argument('-f', '--tokenfile', action='store', help='File to read the token from (default: .roadtools_auth)', default='.roadtools_auth')
     describe_parser.add_argument('-v', '--verbose', action='store_true', help='Show extra information')
 
     # Find scope
     getscope_parser = subparsers.add_parser('getscope', aliases=['findscope'], help='Find first-party apps with the right pre-approved scope')
-    getscope_parser.add_argument('-s', '--scope', default=None, action='store', required=True, metavar='SCOPE', help='Desired scope (API URL + scope on that API, for example https://graph.microsoft.com/files.read)')
+    getscope_parser.add_argument('-s', '--scope', default=None, action='store', required=False, metavar='SCOPE', help='Desired scope (API URL + scope on that API, for example https://graph.microsoft.com/files.read). If omitted, all known scopes will be listed.')
     getscope_parser.add_argument('--foci', action='store_true', help='Only list FOCI clients')
     getscope_parser.add_argument('--csv', action='store_true', help='Output in CSV format')
 
     # Get OTP
     otpparser = subparsers.add_parser('getotp', help='Get OTP code from seed, either supplied or from KeePass file')
     otpparser.add_argument('-u', '--username', action='store', help='User to query from KeePass file')
     otpparser.add_argument('-s', '--otpseed', action='store', help='OTP secret seed')
@@ -332,14 +395,17 @@
                                 help='Do not close the browser window after timeout. Useful if you want to browse online apps with the obtained credentials')
     intauth_parser.add_argument('--capture-code',
                                 action='store_true',
                                 help='Do not attempt to redeem any authentication code but print it instead')
     intauth_parser.add_argument('--federated',
                                 action='store_true',
                                 help='Fill in password on Federation server login page (assumes AD FS)')
+    intauth_parser.add_argument('--cae',
+                                action='store_true',
+                                help='Request Continuous Access Evaluation tokens (requires use of scope parameter instead of resource)')
 
     # Interactive auth using Selenium - creds from keepass
     kdbauth_parser = subparsers.add_parser('keepassauth', help='Selenium based authentication with credentials from a KeePass database')
     kdbauth_parser.add_argument('-u', '--username', action='store', help='User to authenticate as (must exist as username in KeePass)')
     kdbauth_parser.add_argument('-kp', '--keepass', action='store', metavar='KPFILE', default='roadtx.kdbx', help='KeePass file (default: roadtx.kdbx)')
     kdbauth_parser.add_argument('-kpp', '--keepass-password', action='store', metavar='KPPASS', help='KeePass file password. Can also be provided via KPPASS environment variable.')
     kdbauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
@@ -384,14 +450,17 @@
                                 help='Do not attempt to redeem any authentication code but print it instead')
     kdbauth_parser.add_argument('--federated',
                                 action='store_true',
                                 help='Fill in password on Federation server login page (assumes AD FS)')
     kdbauth_parser.add_argument('--device-code',
                                 action='store',
                                 help='Authenticate with the given device code')
+    kdbauth_parser.add_argument('--cae',
+                                action='store_true',
+                                help='Request Continuous Access Evaluation tokens (requires use of scope parameter instead of resource)')
 
 
 
     # Interactive auth using Selenium - inject PRT
     browserprtauth_parser = subparsers.add_parser('browserprtauth', help='Selenium based auth with automatic PRT usage. Emulates Edge browser with PRT')
     browserprtauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
     browserprtauth_parser.add_argument('-c',
@@ -439,14 +508,17 @@
                                        help='Path to geckodriver file on disk (download from: https://github.com/mozilla/geckodriver/releases)')
     browserprtauth_parser.add_argument('-k', '--keep-open',
                                        action='store_true',
                                        help='Do not close the browser window after timeout. Useful if you want to browse online apps with the obtained credentials')
     browserprtauth_parser.add_argument('--capture-code',
                                        action='store_true',
                                        help='Do not attempt to redeem any authentication code but print it instead')
+    browserprtauth_parser.add_argument('--cae',
+                                       action='store_true',
+                                       help='Request Continuous Access Evaluation tokens (requires use of scope parameter instead of resource)')
 
     # Interactive auth using Selenium - inject PRT to other user
     injauth_parser = subparsers.add_parser('browserprtinject', help='Selenium based auth with automatic PRT injection. Can be used with other users to add device state to session')
     injauth_parser.add_argument('-u', '--username', action='store', metavar='USER', help='User to authenticate (optional, otherwise you have to specify it by hand)')
     injauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password of the user (can be left out if using PRT, or KeePass creds)')
     injauth_parser.add_argument('-kp', '--keepass', action='store', metavar='KPFILE', default='roadtx.kdbx', help='KeePass file (default: roadtx.kdbx)')
     injauth_parser.add_argument('-kpp', '--keepass-password', action='store', metavar='KPPASS', help='KeePass file password. Can also be provided via KPPASS environment variable.')
@@ -493,14 +565,17 @@
     injauth_parser.add_argument('--tokenfile',
                                 action='store',
                                 help='File to store the credentials (default: .roadtools_auth)',
                                 default='.roadtools_auth')
     injauth_parser.add_argument('--tokens-stdout',
                                 action='store_true',
                                 help='Do not store tokens on disk, pipe to stdout instead')
+    injauth_parser.add_argument('--cae',
+                                action='store_true',
+                                help='Request Continuous Access Evaluation tokens (requires use of scope parameter instead of resource)')
 
     # Interactive auth using Selenium - enrich PRT
     enrauth_parser = subparsers.add_parser('prtenrich', help='Interactive authentication to add MFA claim to a PRT')
     enrauth_parser.add_argument('-u', '--username', action='store', metavar='USER', help='User in the prt')
     enrauth_parser.add_argument('-kp', '--keepass', action='store', metavar='KPFILE', default='roadtx.kdbx', help='KeePass file (default: roadtx.kdbx)')
     enrauth_parser.add_argument('-kpp', '--keepass-password', action='store', metavar='KPPASS', help='KeePass file password. Can also be provided via KPPASS environment variable.')
     enrauth_parser.add_argument('-d', '--driver-path',
@@ -582,14 +657,66 @@
                 print(f'Requesting token with scope {auth.scope}')
             else:
                 print(f'Requesting token for resource {auth.resource_uri}')
         res = auth.get_tokens(args)
         if not res:
             return
         auth.save_tokens(args)
+    elif args.command == 'refreshtokento':
+        try:
+            with codecs.open('.roadtools_auth', 'r', 'utf-8') as infile:
+                tokenobject = json.load(infile)
+            _, tokendata = auth.parse_accesstoken(tokenobject['accessToken'])
+        except FileNotFoundError:
+            print('This command requires the .roadtools_auth file, which was not found. Use the gettokens command to supply a refresh token manually.')
+            return
+        auth.set_client_id(tokenobject['_clientId'])
+        auth.set_resource_uri(args.resource)
+        auth.outfile = args.tokenfile
+        # Tenant from arguments or from tokenfile
+        if args.tenant:
+            auth.tenant = args.tenant
+        elif 'tenantId' in tokenobject:
+            auth.tenant = tokenobject['tenantId']
+        if args.cae:
+            auth.use_cae = args.cae
+        if not args.tokens_stdout:
+            if args.scope:
+                print(f'Requesting token with scope {args.scope}')
+            else:
+                print(f'Requesting token for resource {auth.resource_uri}')
+        if args.scope:
+            auth.scope = args.scope
+            auth.authenticate_with_refresh_native_v2(tokenobject['refreshToken'], client_secret=args.password)
+        else:
+            auth.authenticate_with_refresh_native(tokenobject['refreshToken'], client_secret=args.password)
+        auth.save_tokens(args)
+    elif args.command == 'appauth':
+        auth.set_client_id(args.client)
+        auth.set_resource_uri(args.resource)
+        auth.scope = args.scope
+        auth.use_cae = args.cae
+        auth.tenant = args.tenant
+        auth.outfile = args.tokenfile
+        if args.password:
+            # Password based flow
+            if args.scope:
+                auth.authenticate_as_app_native_v2(client_secret=args.password)
+            else:
+                auth.authenticate_as_app_native(client_secret=args.password)
+        else:
+            if not auth.loadappcert(args.cert_pem, args.key_pem, args.cert_pfx, args.pfx_pass, args.pfx_base64):
+                return
+            if args.scope:
+                assertion = auth.generate_app_assertion(use_v2=True)
+                auth.authenticate_as_app_native_v2(assertion=assertion)
+            else:
+                assertion = auth.generate_app_assertion(use_v2=False)
+                auth.authenticate_as_app_native(assertion=assertion)
+        auth.save_tokens(args)
     elif args.command == 'device':
         if args.action in ('register', 'join'):
             if args.access_token:
                 tokenobject, tokendata = auth.parse_accesstoken(args.access_token)
             else:
                 try:
                     with codecs.open('.roadtools_auth', 'r', 'utf-8') as infile:
@@ -662,14 +789,15 @@
                 print('You must either supply a PRT and session key on the command line or a file that contains them')
                 return
             print("Renewing PRT")
             prtdata = deviceauth.renew_prt()
             deviceauth.saveprt(prtdata, args.prt_file)
     elif args.command == 'prtauth':
         auth.set_user_agent(args.user_agent)
+        auth.use_cae = args.cae
         if args.tenant:
             auth.tenant = args.tenant
         if args.prt and args.prt_sessionkey:
             deviceauth.setprt(args.prt, args.prt_sessionkey)
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
@@ -718,14 +846,16 @@
                 print('Decrypted data (hex)')
                 print(binascii.hexlify(data))
 
     elif args.command == 'codeauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.tenant = args.tenant
+        if args.cae:
+            auth.use_cae = args.cae
         if args.scope:
             # Switch to identity platform v2 and use scope instead of resource
             auth.scope = args.scope
             auth.authenticate_with_code_native_v2(args.code, args.redirect_url, client_secret=args.password)
         else:
             auth.authenticate_with_code_native(args.code, args.redirect_url, client_secret=args.password)
         auth.outfile = args.tokenfile
@@ -760,14 +890,15 @@
         for alias, useragent in WELLKNOWN_USER_AGENTS.items():
             print(f"{alias:<15} - {useragent}")
     elif args.command == 'interactiveauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.set_user_agent(args.user_agent)
         auth.tenant = args.tenant
+        auth.use_cae = args.cae
         # Intercept if custom UA is set
         custom_ua = args.user_agent is not None
         selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url, proxy=seleniumproxy)
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
@@ -787,21 +918,23 @@
             result = selauth.selenium_login_with_custom_useragent(url, args.username, args.password, capture=args.capture_code, federated=args.federated)
         else:
             result = selauth.selenium_login(url, args.username, args.password, capture=args.capture_code, federated=args.federated)
         if args.capture_code:
             if result:
                 print(f'Captured auth code: {result}')
             return
-        auth.outfile = args.tokenfile
-        auth.save_tokens(args)
+        elif result:
+            auth.outfile = args.tokenfile
+            auth.save_tokens(args)
     elif args.command == 'keepassauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.set_user_agent(args.user_agent)
         auth.tenant = args.tenant
+        auth.use_cae = args.cae
         # Intercept if custom UA is set
         custom_ua = args.user_agent is not None
         selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url, proxy=seleniumproxy)
         password, otpseed = selauth.get_keepass_cred(args.username, args.keepass, args.keepass_password)
         if args.auth_url:
             url = args.auth_url
         else:
@@ -821,14 +954,16 @@
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'browserprtauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.set_user_agent(args.user_agent)
         auth.tenant = args.tenant
+        auth.use_cae = args.cae
+        auth.scope = args.scope
         if args.prt and args.prt_sessionkey:
             deviceauth.setprt(args.prt, args.prt_sessionkey)
         elif args.prt_cookie:
             pass
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
@@ -866,14 +1001,15 @@
                 return
             return
     elif args.command == 'browserprtinject':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.set_user_agent(args.user_agent)
         auth.tenant = args.tenant
+        auth.use_cae = args.cae
         if args.prt and args.prt_sessionkey:
             deviceauth.setprt(args.prt, args.prt_sessionkey)
         elif args.prt_cookie:
             pass
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
@@ -999,28 +1135,58 @@
         print(json.dumps(body, sort_keys=True, indent=4))
     elif args.command in ('getscope', 'findscope'):
         # Load scope data
         current_dir = os.path.abspath(os.path.dirname(__file__))
         datafile = os.path.join(current_dir, 'firstpartyscopes.json')
         with codecs.open(datafile,'r','utf-8') as infile:
             data = json.load(infile)
+
+        if not args.scope:
+            results = set()
+
+            app_resource_ids = defaultdict(set)
+            for resource, app_id in data['resourceidentifiers'].items():
+                app_resource_ids[app_id].add(resource)
+
+            for app in data['apps'].values():
+                if args.foci and not app['foci']:
+                    continue
+
+                for app_id, scopes in app['scopes'].items():
+                    for resource in app_resource_ids.get(app_id, [f'https://{app_id}']):
+                        resource = resource.rstrip('/')
+                        for scope in map(str.lower, scopes):
+                            results.add(f'{resource}/{scope}')
+
+            if args.csv:
+                print('"scope"')
+            else:
+                print("Listing all possible scopes")
+
+            for scope in sorted(results):
+                print(f'"{scope}"' if args.csv else scope)
+
+            return
+
         try:
             resource, scope = args.scope.lower().rsplit('/', 1)
         except ValueError:
             print("No resource (API) specified in scope, defaulting to Microsoft Graph")
             resource = "https://graph.microsoft.com"
             scope = args.scope
+
         try:
             resourceid = data['resourceidentifiers'][resource.lower()]
         except KeyError:
             try:
                 resourceid = data['resourceidentifiers'][resource.lower() + '/']
             except KeyError:
                 print(f'The API {resource} is not a known resource')
                 return
+
         # Loop through scopes
         results = []
         for appid, app in data['apps'].items():
             # Skip foci apps
             if args.foci and not app['foci']:
                 continue
             try:
@@ -1157,13 +1323,9 @@
             print('You must either supply a PRT and session key on the command line or a file that contains them')
             return
         challenge = auth.get_srv_challenge()['Nonce']
         cookie = auth.create_prt_cookie_kdf_ver_2(deviceauth.prt, deviceauth.session_key, challenge)
         print(f"PRT cookie: {cookie}")
         print("Can be used in external browsers using the x-ms-RefreshTokenCredential header or cookie. Note that a PRT cookie is only valid for 5 minutes.")
 
-
-
-
-
 if __name__ == '__main__':
     main()
```

### Comparing `roadtx-1.7.1/roadtools/roadtx/selenium.py` & `roadtx-1.8.0/roadtools/roadtx/selenium.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,35 @@
 from seleniumwire import webdriver as webdriver_wire
 from seleniumwire.thirdparty.mitmproxy.net.http import encoding
 from selenium import webdriver
 from selenium.webdriver.firefox.service import Service
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
+from selenium.common import exceptions
 from selenium.common.exceptions import TimeoutException, StaleElementReferenceException
 import pyotp
 
+# Decorator for selenium functions
+def selenium_wrap(func):
+    def wrapped(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except exceptions.NoSuchWindowException as exc:
+            if 'Browsing context has been discarded' in str(exc):
+                print('Browser window was closed by the user')
+                return False
+            raise exc
+        except exceptions.WebDriverException as exc:
+            if 'Failed to decode response from marionette' in str(exc):
+                print('Browser window closed by the user')
+                return False
+            raise exc
+    return wrapped
+
 class SeleniumAuthentication():
     def __init__(self, auth, deviceauth, redirurl, proxy=None):
         if proxy and proxy.startswith('http'):
             proxy = proxy.replace('http://','').replace('https://','')
         self.proxy = proxy
         self.auth = auth
         self.deviceauth = deviceauth
@@ -108,14 +126,15 @@
         userpassword = entry['Password']
         try:
             otpseed = entry['otp']
         except KeyError:
             otpseed = None
         return userpassword, otpseed
 
+    @selenium_wrap
     def selenium_login(self, url, identity=None, password=None, otpseed=None, keep=False, capture=False, federated=False, devicecode=None):
         '''
         Selenium based login with optional autofill of whatever is provided
         '''
         driver = self.driver
         # Change if using device code auth
         if devicecode:
@@ -155,14 +174,16 @@
             res = urlparse(driver.current_url)
             params = parse_qs(res.query)
             code = params['code'][0]
             if not keep:
                 driver.close()
             if capture:
                 return code
+            if self.auth.scope:
+                return self.auth.authenticate_with_code_native_v2(code, self.redirurl)
             return self.auth.authenticate_with_code_native(code, self.redirurl)
         except TimeoutException:
             pass
 
         if otpseed:
             try:
                 els = WebDriverWait(driver, 2).until(lambda d: d.find_element(By.CSS_SELECTOR, '[data-value="PhoneAppOTP"]'))
@@ -202,14 +223,16 @@
                 res = urlparse(driver.current_url)
                 params = parse_qs(res.query)
                 code = params['code'][0]
                 if not keep:
                     driver.close()
                 if capture:
                     return code
+                if self.auth.scope:
+                    return self.auth.authenticate_with_code_native_v2(code, self.redirurl)
                 return self.auth.authenticate_with_code_native(code, self.redirurl)
             except TimeoutException:
                 if not keep:
                     driver.close()
                     raise AuthenticationException('Authentication did not complete within time limit')
         return False
 
@@ -219,15 +242,14 @@
         '''
         def interceptor(request):
             del request.headers['User-Agent']
             request.headers['User-Agent'] = self.auth.user_agent
         self.driver.request_interceptor = interceptor
         return self.selenium_login(url, identity=identity, password=password, otpseed=otpseed, keep=keep, capture=capture, federated=federated, devicecode=devicecode)
 
-
     def selenium_login_with_prt(self, url, identity=None, password=None, otpseed=None, keep=False, prtcookie=None, capture=False):
         '''
         Selenium login with PRT injection.
         '''
         def interceptor(request):
             del request.headers['User-Agent']
             if self.auth.user_agent:
@@ -301,31 +323,32 @@
             else:
                 existing = ''
             request.headers['Cookie'] = f'ESTSAUTHPERSISTENT={estscookie}; ' + existing
 
         self.driver.request_interceptor = interceptor
         return self.selenium_login(url, identity, password, otpseed, keep=keep, capture=capture)
 
+    @selenium_wrap
     def selenium_enrich_prt(self, url, otpseed=None):
         '''
         Selenium authentication to add NGC MFA claim to a PRT or token.
         Single factor auth is handled via PRT injection, MFA seed can come
         from keepass or manually. Result is refresh token that can be used to request
         a new PRT, or an access token to the desired resource (depends on supplied url).
         '''
         def interceptor(request):
             del request.headers['User-Agent']
             if self.auth.user_agent:
                 request.headers['User-Agent'] = self.auth.user_agent
             else:
                 request.headers['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; WebView/3.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36 Edge/18.19044'
-            request.headers['Sec-Ch-Ua'] = '" Not;A Brand";v="99", "Microsoft Edge";v="103", "Chromium";v="103"'
-            request.headers['Sec-Ch-Ua-Mobile'] =  '?0'
-            request.headers['Sec-Ch-Ua-Platform'] =  '"Windows"'
-            request.headers['Sec-Ch-Ua-Platform-Version'] = '"10.0.0"'
+                request.headers['Sec-Ch-Ua'] = '" Not;A Brand";v="99", "Microsoft Edge";v="103", "Chromium";v="103"'
+                request.headers['Sec-Ch-Ua-Mobile'] =  '?0'
+                request.headers['Sec-Ch-Ua-Platform'] =  '"Windows"'
+                request.headers['Sec-Ch-Ua-Platform-Version'] = '"10.0.0"'
 
             if request.url.startswith('https://login.microsoftonline.com') and self.deviceauth.prt:
                 if '/authorize' in request.url or '/login' in request.url or '/kmsi' in request.url or '/reprocess' in request.url or '/resume' in request.url:
                     if 'sso_nonce' in request.url:
                         res = urlparse(request.url)
                         params = parse_qs(res.query)
                         cookie = self.auth.create_prt_cookie_kdf_ver_2(self.deviceauth.prt,
@@ -371,7 +394,72 @@
                 # No MFA?
                 pass
         
         el = WebDriverWait(driver, 6000).until(lambda d: d.find_element(by=By.CSS_SELECTOR, value='form[name="hiddenform"] input[name="code"]'))
         code = el.get_property("value")
         driver.close()
         return self.auth.authenticate_with_code_encrypted(code, self.deviceauth.session_key, self.redirurl)
+
+    @selenium_wrap
+    def selenium_login_owatoken(self, owatoken):
+        def interceptor(request):
+            if request.url == 'https://outlook.office.com/owa/?init':
+                # Replace with owa request
+                req_url = "https://outlook.office.com:443/owa/"
+                req_cookies = {
+                    "ClientId": "AF0E07DCF04B42D3A1F0BA42E387B211",
+                    "OIDC": "1",
+                    "OpenIdConnect.nonce.v3.LTNEDyBePk9sAdZIbnys6v-YAcgFNTLDF9tdXKxWVp8":
+                    "638357308291354513.0509bcb8-3602-48c0-be52-fd59799eca11",
+                    "X-OWA-RedirectHistory": "ArLym14BkQ97-Jbm2wg"
+                }
+                req_headers = {
+                    "Cache-Control": "max-age=0",
+                    "Upgrade-Insecure-Requests": "1",
+                    "Origin": "https://login.microsoftonline.com",
+                    "Content-Type": "application/x-www-form-urlencoded",
+                    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+                    "Sec-Fetch-Site": "cross-site",
+                    "Sec-Fetch-Mode": "navigate",
+                    "Sec-Fetch-Dest": "document",
+                    "Referer": "https://login.microsoftonline.com/",
+                    "Accept-Encoding": "gzip, deflate, br",
+                    "Accept-Language": "en-US,en;q=0.9",
+                    "Priority": "u=0, i"
+                }
+                if self.auth.user_agent:
+                    req_headers['User-Agent'] = self.auth.user_agent
+                else:
+                    req_headers['User-Agent'] = request.headers['User-Agent']
+                req_data = {
+                    "code": "ohnoesthisisempty",
+                    "id_token": owatoken,
+                    "Astate": "DctBFoAgCABRrNdxSBBJOI6abVt2_Vj82U0CgD1sIVEE2iUm2oSsOItWZTlJyccchnJRwWqTcCwt-NzqzX3NzpziPfL79fwD",
+                    "session_state": "56f4cbb9-6cc9-4150-a4b3-5b2865f916c9",
+                    "correlation_id": "2c13357a-eab7-97ed-bd48-8b50a6979bfc"
+                }
+                res = requests.post(req_url, allow_redirects=False, headers=req_headers, cookies=req_cookies, data=req_data, timeout=30.0)
+                request.create_response(
+                    status_code=res.status_code,
+                    headers=dict(res.headers),
+                    body=res.content
+                )
+        def resp_interceptor(request, response):
+            if request.url == 'https://outlook.office.com/owa/':
+                if response.headers.get('X-Ms-Diagnostics') and response.headers.get('Location','').startswith('https://login.microsoftonline.com'):
+                    diag = response.headers.get('X-Ms-Diagnostics')
+                    print(f'Error during auth: {diag}')
+                    del response.headers['Location']
+                    body = '<html><body><div name="youshouldquit">An error occurred (see command line)</div></body></html>'
+                    response.body = encoding.encode(body, response.headers.get('Content-Encoding', 'identity'))
+                    del response.headers['Content-Length']
+                    response.headers['Content-Length'] = len(response.body)
+
+
+        self.driver.request_interceptor = interceptor
+        self.driver.response_interceptor = resp_interceptor
+
+        driver = self.driver
+        driver.get("https://outlook.office.com/owa/?init")
+        el = WebDriverWait(driver, 6000).until(lambda d: d.find_element(by=By.CSS_SELECTOR, value='div[name="youshouldquit"]'))
+        driver.close()
+
```

### Comparing `roadtx-1.7.1/roadtx.egg-info/PKG-INFO` & `roadtx-1.8.0/roadtx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.7.1
+Version: 1.8.0
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: roadlib>=0.23
+Requires-Dist: roadlib>=0.24
 Requires-Dist: requests
 Requires-Dist: selenium
 Requires-Dist: selenium-wire
 Requires-Dist: pyotp
 Requires-Dist: pycryptodomex
 Requires-Dist: signxml
 Requires-Dist: blinker<1.8.0
```

### Comparing `roadtx-1.7.1/setup.py` & `roadtx-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadtx',
-      version='1.7.1',
+      version='1.8.0',
       description='ROADtools Token eXchange',
       author='Dirk-jan Mollema',
       author_email='dirkjan@outsidersecurity.nl',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
@@ -14,15 +14,15 @@
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
       ],
       packages=['roadtools.roadtx'],
       package_data={'roadtools.roadtx': ['firstpartyscopes.json']},
       install_requires=[
-          'roadlib>=0.23',
+          'roadlib>=0.24',
           'requests',
           'selenium',
           'selenium-wire',
           'pyotp',
           'pycryptodomex',
           'signxml',
           'blinker<1.8.0'
```

