# Comparing `tmp/heaserver_accounts-1.1.0.tar.gz` & `tmp/heaserver_accounts-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_accounts-1.1.0.tar", last modified: Wed Apr 24 18:02:43 2024, max compression
+gzip compressed data, was "heaserver_accounts-1.1.1.tar", last modified: Thu May  2 20:42:09 2024, max compression
```

## Comparing `heaserver_accounts-1.1.0.tar` & `heaserver_accounts-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.398248 heaserver_accounts-1.1.0/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/.gitignore
--rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5916 2024-04-24 18:02:43.397247 heaserver_accounts-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4608 2024-04-24 17:52:12.000000 heaserver_accounts-1.1.0/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/RELEASING.md
--rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.330245 heaserver_accounts-1.1.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.330245 heaserver_accounts-1.1.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.351247 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7797 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-24 18:02:43.399248 heaserver_accounts-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-04-24 18:02:07.000000 heaserver_accounts-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.332245 heaserver_accounts-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.331245 heaserver_accounts-1.1.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.354251 heaserver_accounts-1.1.0/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0    45175 2024-04-24 17:47:43.000000 heaserver_accounts-1.1.0/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.356246 heaserver_accounts-1.1.0/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0    11652 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.0/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.395248 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     5916 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 18:02:43.000000 heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.332245 heaserver_accounts-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.333245 heaserver_accounts-1.1.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:02:43.393247 heaserver_accounts-1.1.0/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.0/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     7626 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.0/tests/heaserver/accounttest/test_all.py
--rw-rw-rw-   0        0        0     5460 2024-04-23 22:20:38.000000 heaserver_accounts-1.1.0/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.814577 heaserver_accounts-1.1.1/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5973 2024-05-02 20:42:09.813521 heaserver_accounts-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4665 2024-05-02 20:08:33.000000 heaserver_accounts-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/RELEASING.md
+-rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.620346 heaserver_accounts-1.1.1/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.620346 heaserver_accounts-1.1.1/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.750656 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7797 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:42:09.815101 heaserver_accounts-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-05-02 20:40:26.000000 heaserver_accounts-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.623341 heaserver_accounts-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.622339 heaserver_accounts-1.1.1/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.754325 heaserver_accounts-1.1.1/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0    47097 2024-05-02 20:39:51.000000 heaserver_accounts-1.1.1/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.755951 heaserver_accounts-1.1.1/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0    11957 2024-05-02 20:08:33.000000 heaserver_accounts-1.1.1/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.811946 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     5973 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.624339 heaserver_accounts-1.1.1/tests/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.624339 heaserver_accounts-1.1.1/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.809834 heaserver_accounts-1.1.1/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     7626 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.1/tests/heaserver/accounttest/test_all.py
+-rw-rw-rw-   0        0        0     5462 2024-05-02 20:39:51.000000 heaserver_accounts-1.1.1/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver_accounts-1.1.0/Dockerfile` & `heaserver_accounts-1.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.0/LICENSE` & `heaserver_accounts-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.0/PKG-INFO` & `heaserver_accounts-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.0
+Requires-Dist: heaserver~=1.5.1
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.1
+* Fixed new bucket form submission.
+
 ## Version 1.1.0
 * Removed the PUT and DELETE account calls because neither works.
 
 ## Version 1.0.8
 * Addressed occasional slowdown getting one account.
 
 ## Version 1.0.7
```

### Comparing `heaserver_accounts-1.1.0/README.md` & `heaserver_accounts-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.1
+* Fixed new bucket form submission.
+
 ## Version 1.1.0
 * Removed the PUT and DELETE account calls because neither works.
 
 ## Version 1.0.8
 * Addressed occasional slowdown getting one account.
 
 ## Version 1.0.7
```

### Comparing `heaserver_accounts-1.1.0/RELEASING.md` & `heaserver_accounts-1.1.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.0/integrationtests/heaserver/accountintegrationtest/testcase.py` & `heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.0/run-swaggerui.py` & `heaserver_accounts-1.1.1/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.0/setup.py` & `heaserver_accounts-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.1.0',
+    version='1.1.1',
     description="Manages account information",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver~=1.5.0'
+        'heaserver~=1.5.1'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver_accounts-1.1.0/src/heaserver/account/service.py` & `heaserver_accounts-1.1.1/src/heaserver/account/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from heaserver.service.oidcclaimhdrs import SUB
 from heaserver.service.runner import init_cmd_line, routes, start, web
 from heaserver.service.db import aws, awsservicelib
 from heaserver.service.wstl import builder_factory, action
 from heaserver.service import response, client
 from heaserver.service.appproperty import HEA_DB, HEA_CACHE
 from heaserver.service.heaobjectsupport import new_heaobject_from_type
-from heaobject.account import AWSAccount
+from heaobject.account import AWSAccount  #, AccountView
 from heaobject.bucket import AWSBucket
 from heaobject.storage import AWSStorage
 from heaobject.root import DesktopObjectDict
 from heaobject.volume import AWSFileSystem
 from heaobject.user import NONE_USER
 from yarl import URL
 from aiohttp.web import Request, Response
@@ -33,14 +33,48 @@
 
     :param request: the HTTP request.
     :return: Always returns status code 200.
     """
     return response.status_ok(None)
 
 
+# @routes.get('/accounts')
+# @routes.get('/accounts/')
+# @action(name='heaserver-accounts-account-get-actual', rel='hea-actual', path='{+actual_object_uri}')
+# async def get_accounts(request: web.Request) -> web.Response:
+#     async with DesktopObjectActionLifecycle(request=request,
+#                                                 code='hea-get',
+#                                                 description=f'Getting all accounts',
+#                                                 activity_cb=publish_desktop_object) as activity:
+#         logger = logging.getLogger(__name__)
+#         sub = request.headers.get(SUB, NONE_USER)
+#         account_ids = request.query.getall('account_id', [])
+#         try:
+#             aws_accounts = await _aws_account_ids_to_aws_accounts(request, tuple(a.split('^')[1] for a in account_ids))
+#         except IndexError:
+#             return response.status_bad_request(f'Invalid account_id query parameter {", ".join(account_ids)}')
+#         activity.new_object_type_name = AWSAccount.get_type_name()
+#         activity.new_object_uri = 'accounts/'
+#         account_views: list[AccountView] = []
+#         for aws_account in aws_accounts:
+#             av = AccountView()
+#             av.actual_object_id = aws_account.id
+#             av.actual_object_type_name = aws_account.type
+#             av.actual_object_uri = f'awsaccounts/{aws_account.id}'
+#             av.display_name = aws_account.display_name
+#             av.owner = aws_account.owner
+#             av.shares = aws_account.shares
+#             av.created = aws_account.created
+#             av.modified = aws_account.modified
+#             av.name = aws_account.name
+#             av.type_display_name = aws_account.type_display_name
+#             account_views.append(av)
+#         return await response.get_all(request, [a.to_dict() for a in account_views],
+#                                       permissions=[a.get_permissions(sub) for a in account_views])
+
 @routes.options('/awsaccounts/{id}')
 async def get_awsaccount_options(request: web.Request) -> web.Response:
     """
     ---
     summary: Allowed HTTP methods.
     tags:
         - heaserver-accounts-awsaccount
@@ -94,29 +128,28 @@
                                                 code='hea-get',
                                                 description=f'Getting AWS account {id_}',
                                                 activity_cb=publish_desktop_object) as activity:
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'id^{request.match_info["id"]}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
-            account_dict, volume_id = cached_value
+            account, volume_id = cached_value
         else:
             account, volume_id = await _get_awsaccount_by_id(request)
             logger.debug('Got account %s and volume %s', account, volume_id)
             if account is None:
                 raise response.status_not_found()
-            account_dict = account.to_dict()
-            request.app[HEA_CACHE][cache_key] = (account_dict, volume_id)
-            request.app[HEA_CACHE][(sub, f'volume_id^{volume_id}')] = (account_dict, volume_id)
+            request.app[HEA_CACHE][cache_key] = (account, volume_id)
+            request.app[HEA_CACHE][(sub, f'volume_id^{volume_id}')] = (account, volume_id)
         request.match_info['volume_id'] = volume_id
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_id = id_
         activity.new_object_uri = f'awsaccounts/{id_}'
         activity.new_volume_id = volume_id
-        return await response.get(request, account_dict)
+        return await response.get(request, account.to_dict(), account.get_permissions(sub))
 
 
 @routes.get('/awsaccounts/byname/{name}')
 @action('heaserver-accounts-awsaccount-get-self', rel='self hea-account', path='awsaccounts/{id}')
 @action(name='heaserver-accounts-awsaccount-get-volume', rel='hea-volume', path='volumes/{volume_id}')
 async def get_awsaccount_by_name(request: web.Request) -> web.Response:
     """
@@ -143,28 +176,27 @@
     async with DesktopObjectActionLifecycle(request=request,
                                                     code='hea-get',
                                                     description=f'Getting AWS account {name}',
                                                     activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, f'id^{name}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
-            account_dict, volume_id = cached_value
+            account, volume_id = cached_value
         else:
             account, volume_id = await _get_account_by_name(request)
             request.match_info['volume_id'] = volume_id
             if account is None:
                 raise response.status_not_found()
-            account_dict = account.to_dict()
-            request.app[HEA_CACHE][cache_key] = (account_dict, volume_id)
-            request.app[HEA_CACHE][(sub, f'volume_id^{volume_id}')] = (account_dict, volume_id)
+            request.app[HEA_CACHE][cache_key] = (account, volume_id)
+            request.app[HEA_CACHE][(sub, f'volume_id^{volume_id}')] = (account, volume_id)
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_id = name
         activity.new_object_uri = f'awsaccounts/{name}'
         activity.new_volume_id = volume_id
-    return await response.get(request, account_dict)
+    return await response.get(request, account.to_dict(), account.get_permissions(sub))
 
 
 @routes.get('/awsaccounts')
 @routes.get('/awsaccounts/')
 @action('heaserver-accounts-awsaccount-get-open-choices', rel='hea-opener-choices hea-context-menu', path='awsaccounts/{id}/opener')
 @action('heaserver-accounts-awsaccount-get-properties', rel='hea-properties hea-context-menu')
 @action('heaserver-accounts-awsaccount-get-create-choices', rel='hea-creator-choices hea-context-menu', path='awsaccounts/{id}/creator')
@@ -183,40 +215,22 @@
       '200':
         $ref: '#/components/responses/200'
     """
     async with DesktopObjectActionLifecycle(request=request,
                                                 code='hea-get',
                                                 description=f'Getting all AWS accounts',
                                                 activity_cb=publish_desktop_object) as activity:
-        logger = logging.getLogger(__name__)
+
         sub = request.headers.get(SUB, NONE_USER)
-        account_ids_ = request.query.getall('account_id', None)
-        account_ids = tuple(account_ids_) if account_ids_ is not None else None
-        cache_key = (sub, None, account_ids)
-        account_dicts = request.app[HEA_CACHE].get(cache_key) if account_ids is None else None
-        if account_dicts is None:
-            db = request.app[HEA_DB]
-            account_dicts: list[DesktopObjectDict] = []
-            volume_ids = [volume.id async for volume in db.get_volumes(request, AWSFileSystem,
-                                                                       account_ids=account_ids,
-                                                                       account_type_names=[AWSAccount.get_type_name()] * len(account_ids) if account_ids is not None else None)]
-            logger.debug('Checking volumes %s for accounts %s', volume_ids, account_ids)
-            account_id_to_account = {}
-            async for aws_account, volume_id in db.get_accounts(request, volume_ids):
-                if not account_ids or aws_account.id in account_ids:
-                    account_dict = aws_account.to_dict()
-                    account_id_to_account[account_dict['id']] = account_dict
-                    request.app[HEA_CACHE][(sub, f'id^{account_dict["id"]}')] = (account_dict, volume_id)
-            account_dicts_ = list(account_id_to_account.values())
-            if account_dicts is None:
-                request.app[HEA_CACHE][cache_key] = account_dicts_
-            account_dicts = account_dicts_
+        account_ids = request.query.getall('account_id', [])
+        accounts = await _aws_account_ids_to_aws_accounts(request, account_ids)
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_uri = 'awsaccounts/'
-        return await response.get_all(request, account_dicts)
+        return await response.get_all(request, [a.to_dict() for a in accounts],
+                                      permissions=[a.get_permissions(sub) for a in accounts])
 
 
 @routes.get('/volumes/{volume_id}/awsaccounts/me')
 @action('heaserver-accounts-awsaccount-get-open-choices', rel='hea-opener-choices hea-context-menu',
         path='volumes/{volume_id}/awsaccounts/me/opener')
 @action('heaserver-accounts-awsaccount-get-properties', rel='hea-properties hea-context-menu')
 @action('heaserver-accounts-awsaccount-get-create-choices', rel='hea-creator-choices hea-context-menu', path='awsaccounts/{id}/creator')
@@ -256,27 +270,26 @@
                                                 description=f'Getting my AWS account',
                                                 activity_cb=publish_desktop_object) as activity:
         volume_id = request.match_info['volume_id']
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'volume_id^{volume_id}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
-            account_dict, volume_id = cached_value
+            account, volume_id = cached_value
         else:
             account = await _get_account(request, volume_id)
             if account is None:
                 raise response.status_not_found()
-            account_dict = account.to_dict()
-            request.app[HEA_CACHE][cache_key] = (account_dict, volume_id)
-            request.app[HEA_CACHE][(sub, f'id^{account.id}')] = (account_dict, volume_id)
+            request.app[HEA_CACHE][cache_key] = (account, volume_id)
+            request.app[HEA_CACHE][(sub, f'id^{account.id}')] = (account, volume_id)
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_volume_id = volume_id
-        activity.new_object_uri = f'volumes/{account_dict["id"]}'
-        activity.new_object_id = account_dict["id"]
-        return await response.get(request, account_dict)
+        activity.new_object_uri = f'volumes/{account.id}'
+        activity.new_object_id = account.id
+        return await response.get(request, account.to_dict(), account.get_permissions(sub))
 
 
 @routes.get('/awsaccounts/{id}/opener')
 @action('heaserver-accounts-awsaccount-open-buckets',
         rel=f'hea-opener hea-context-aws hea-default {AWSBucket.get_mime_type()}', path='volumes/{volume_id}/bucketitems/')
 @action('heaserver-accounts-awsaccount-open-storage',
         rel=f'hea-opener hea-context-aws {AWSStorage.get_mime_type()}', path='volumes/{volume_id}/storage/')
@@ -359,24 +372,23 @@
     async with DesktopObjectActionLifecycle(request=request,
                                                     code='hea-get',
                                                     description=f'Getting my AWS account',
                                                     activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, f'id^{id_}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
-            account_dict, volume_id = cached_value
+            account, volume_id = cached_value
         else:
             account = await _get_account(request, volume_id)
             if account is None:
                 raise response.status_not_found()
-            account_dict = account.to_dict()
         activity.new_object_type_name = AWSAccount.get_type_name()
-        activity.new_object_uri = f'awsaccounts/{account_dict["id"]}'
+        activity.new_object_uri = f'awsaccounts/{account.id}'
         activity.new_volume_id = volume_id
-        activity.new_object_id = account_dict["id"]
+        activity.new_object_id = account.id
         return await response.get_multiple_choices(request)
 
 
 # @routes.post('/volumes/{volume_id}/awsaccounts/me')
 # async def post_account_awsaccounts(request: web.Request) -> web.Response:
 #     """
 #     Posts the awsaccounts information given the correct access key and secret access key.
@@ -533,24 +545,23 @@
                                                 code='hea-get',
                                                 description="Getting user's AWS account",
                                                 activity_cb=publish_desktop_object) as activity:
             sub = request.headers.get(SUB, NONE_USER)
             cache_key = (sub, f'volume_id^{volume_id}')
             cached_value = request.app[HEA_CACHE].get(cache_key)
             if cached_value is not None:
-                account_dict, _ = cached_value
+                account, _ = cached_value
             else:
                 account = await _get_account(request, volume_id)
                 if account is None:
                     raise response.status_not_found()
-                account_dict = account.to_dict()
             activity.new_object_type_name = AWSAccount.get_type_name()
-            activity.new_object_uri = f'awsaccounts/{account_dict["id"]}'
+            activity.new_object_uri = f'awsaccounts/{account.id}'
             activity.new_volume_id = volume_id
-            activity.new_object_id = account_dict["id"]
+            activity.new_object_id = account.id
             return await response.get_multiple_choices(request)
 
 
 @routes.get('/volumes/{volume_id}/awsaccounts/me/newbucket')
 @routes.get('/volumes/{volume_id}/awsaccounts/me/newbucket/')
 @action('heaserver-accounts-awsaccount-new-bucket-form')
 async def get_new_bucket_form_by_volume_id(request: web.Request) -> web.Response:
@@ -586,28 +597,27 @@
                                             code='hea-get',
                                             description="Getting user's AWS account",
                                             activity_cb=publish_desktop_object) as activity:
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'volume_id^{volume_id}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
-            account_dict, _ = cached_value
+            account, _ = cached_value
             return await response.get(request, cached_value)
         else:
             account = await _get_account(request, volume_id)
             if account is None:
                 return response.status_not_found()
-            account_dict = account.to_dict()
-            request.app[HEA_CACHE][cache_key] = account_dict
-            request.app[HEA_CACHE][(sub, f'id^{account.id}')] = account_dict
-        activity.new_object_id = account_dict['id']
+            request.app[HEA_CACHE][cache_key] = (account, volume_id)
+            request.app[HEA_CACHE][(sub, f'id^{account.id}')] = (account, volume_id)
+        activity.new_object_id = account.id
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_volume_id = volume_id
-        activity.new_object_uri = f'awsaccounts/{account_dict["id"]}'
-        return await response.get(request, account_dict)
+        activity.new_object_uri = f'awsaccounts/{account.id}'
+        return await response.get(request, account.to_dict(), permissions=account.get_permissions(sub))
 
 
 @routes.get('/awsaccounts/{id}/newbucket')
 @routes.get('/awsaccounts/{id}/newbucket/')
 @action('heaserver-accounts-awsaccount-new-bucket-form')
 async def get_new_bucket_form(request: web.Request) -> web.Response:
     """
@@ -633,26 +643,25 @@
                                                 code='hea-get',
                                                 description=f'Getting AWS account {id_}',
                                                 activity_cb=publish_desktop_object) as activity:
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'id^{request.match_info["id"]}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
-            account_dict, volume_id = cached_value
+            account, volume_id = cached_value
         else:
             account, volume_id = await _get_awsaccount_by_id(request)
             if account is None:
                 return response.status_not_found()
-            account_dict = account.to_dict()
-            request.app[HEA_CACHE][cache_key] = account_dict
+            request.app[HEA_CACHE][cache_key] = (account, volume_id)
         activity.new_object_id = id_
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_uri = f'awsaccounts/{id_}'
         activity.new_volume_id = volume_id
-        return await response.get(request, account_dict)
+        return await response.get(request, account.to_dict(), account.get_permissions(sub))
 
 
 @routes.post('/volumes/{volume_id}/awsaccounts/me/newbucket')
 @routes.post('/volumes/{volume_id}/awsaccounts/me/newbucket/')
 async def post_new_bucket_by_volume_id(request: web.Request) -> web.Response:
     """
     Gets form for creating a new bucket in this account.
@@ -953,7 +962,31 @@
             # account_status = org_client.describe_create_account_status(CreateAccountRequestId=create_account_response['CreateAccountStatus']['Id'])
             # if account_status['CreateAccountStatus']['State'] == 'FAILED':    # go to boto3 link above to see response syntax
             #     web.HTTPBadRequest()      # the response syntax contains reasons for failure, see boto3 link above to see possible reasons
             # else:
             #     return web.HTTPCreated()  # it may not actually be created, but it likely isn't a failure which means it will be created after a minute or two more, see boto3 docs
     except BotoClientError as e:
         return web.HTTPBadRequest()  # see boto3 link above to see possible  exceptions
+
+
+async def _aws_account_ids_to_aws_accounts(request: web.Request, aws_account_ids: list[str]) -> list[AWSAccount]:
+    logger = logging.getLogger(__name__)
+    sub = request.headers.get(SUB, NONE_USER)
+    cache_key = (sub, None, aws_account_ids)
+    accounts = request.app[HEA_CACHE].get(cache_key) if aws_account_ids is None else None
+    if accounts is None:
+        db = request.app[HEA_DB]
+        accounts: list[AWSAccount] = []
+        volume_ids = [volume.id async for volume in db.get_volumes(request, AWSFileSystem,
+                                                                   account_ids=aws_account_ids,
+                                                                   account_type_names=[AWSAccount.get_type_name()] * len(aws_account_ids) if aws_account_ids is not None else None)]
+        logger.debug('Checking volumes %s for accounts %s', volume_ids, aws_account_ids)
+        account_id_to_account = {}
+        async for aws_account, volume_id in db.get_accounts(request, volume_ids):
+            if not aws_account_ids or aws_account.id in aws_account_ids:
+                account_id_to_account[aws_account.id] = aws_account
+                request.app[HEA_CACHE][(sub, f'id^{aws_account.id}')] = (aws_account, volume_id)
+        accounts_ = list(account_id_to_account.values())
+        if accounts is None:
+            request.app[HEA_CACHE][cache_key] = accounts_
+        accounts = accounts_
+    return accounts
```

### Comparing `heaserver_accounts-1.1.0/src/heaserver/account/wstl/all.json` & `heaserver_accounts-1.1.1/src/heaserver/account/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'wstl'": "{'actions': {insert: [(2, OrderedDict([('name', "*

 * *           "'heaserver-accounts-account-get-actual'), ('description', 'Get the actual object'), "*

 * *           "('type', 'safe'), ('action', 'read'), ('target', 'item read cj'), ('prompt', 'Get "*

 * *           "actual')]))]}}"}*

```diff
@@ -14,14 +14,22 @@
                 "prompt": "View account",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
                 "description": "Get the actual object",
+                "name": "heaserver-accounts-account-get-actual",
+                "prompt": "Get actual",
+                "target": "item read cj",
+                "type": "safe"
+            },
+            {
+                "action": "read",
+                "description": "Get the actual object",
                 "name": "heaserver-accounts-bucketitem-get-actual",
                 "prompt": "Get actual",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
```

### Comparing `heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.0
+Requires-Dist: heaserver~=1.5.1
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.1
+* Fixed new bucket form submission.
+
 ## Version 1.1.0
 * Removed the PUT and DELETE account calls because neither works.
 
 ## Version 1.0.8
 * Addressed occasional slowdown getting one account.
 
 ## Version 1.0.7
```

### Comparing `heaserver_accounts-1.1.0/src/heaserver_accounts.egg-info/SOURCES.txt` & `heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.0/tests/heaserver/accounttest/test_all.py` & `heaserver_accounts-1.1.1/tests/heaserver/accounttest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.0/tests/heaserver/accounttest/testcase.py` & `heaserver_accounts-1.1.1/tests/heaserver/accounttest/testcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'credential_id': None,  # Let boto3 try to find the user's credentials.
         'account': {
             'type': AccountAssociation.get_type_name(),
             'actual_object_type_name': AWSAccount.get_type_name(),
             'actual_object_id': "123456789012"
         }
+
     }],
     'awsaccounts': [
         {
             "alternate_contact_name": None,
             "alternate_email_address": None,
             "alternate_phone_number": None,
             "created": None,
```

