# Comparing `tmp/python_amcards-1.3.2.tar.gz` & `tmp/python_amcards-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_amcards-1.3.2.tar", last modified: Wed Apr 24 17:58:41 2024, max compression
+gzip compressed data, was "python_amcards-1.3.3.tar", last modified: Thu May  2 02:36:18 2024, max compression
```

## Comparing `python_amcards-1.3.2.tar` & `python_amcards-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-24 17:58:41.656062 python_amcards-1.3.2/
--rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python_amcards-1.3.2/LICENSE
--rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-24 17:58:41.655798 python_amcards-1.3.2/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)     2466 2023-05-19 17:59:31.000000 python_amcards-1.3.2/README.rst
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-24 17:58:41.654203 python_amcards-1.3.2/amcards/
--rw-r--r--   0 simonesestili   (501) staff       (20)     5466 2024-04-18 04:14:42.000000 python_amcards-1.3.2/amcards/__helpers.py
--rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python_amcards-1.3.2/amcards/__init__.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    61560 2024-04-18 05:21:04.000000 python_amcards-1.3.2/amcards/amcards.py
--rw-r--r--   0 simonesestili   (501) staff       (20)     1978 2024-04-18 05:21:12.000000 python_amcards-1.3.2/amcards/exceptions.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    30973 2024-04-24 17:56:43.000000 python_amcards-1.3.2/amcards/models.py
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-24 17:58:41.655496 python_amcards-1.3.2/python_amcards.egg-info/
--rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-24 17:58:41.000000 python_amcards-1.3.2/python_amcards.egg-info/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)      316 2024-04-24 17:58:41.000000 python_amcards-1.3.2/python_amcards.egg-info/SOURCES.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        1 2024-04-24 17:58:41.000000 python_amcards-1.3.2/python_amcards.egg-info/dependency_links.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       12 2024-04-24 17:58:41.000000 python_amcards-1.3.2/python_amcards.egg-info/requires.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        8 2024-04-24 17:58:41.000000 python_amcards-1.3.2/python_amcards.egg-info/top_level.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       38 2024-04-24 17:58:41.656120 python_amcards-1.3.2/setup.cfg
--rw-r--r--   0 simonesestili   (501) staff       (20)      874 2024-04-24 17:58:34.000000 python_amcards-1.3.2/setup.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-05-02 02:36:18.308967 python_amcards-1.3.3/
+-rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python_amcards-1.3.3/LICENSE
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-05-02 02:36:18.308636 python_amcards-1.3.3/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)     2466 2023-05-19 17:59:31.000000 python_amcards-1.3.3/README.rst
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-05-02 02:36:18.307151 python_amcards-1.3.3/amcards/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     5466 2024-04-18 04:14:42.000000 python_amcards-1.3.3/amcards/__helpers.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python_amcards-1.3.3/amcards/__init__.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    63018 2024-05-02 02:32:51.000000 python_amcards-1.3.3/amcards/amcards.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)     1978 2024-04-18 05:21:12.000000 python_amcards-1.3.3/amcards/exceptions.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    30973 2024-04-24 17:56:43.000000 python_amcards-1.3.3/amcards/models.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-05-02 02:36:18.308016 python_amcards-1.3.3/python_amcards.egg-info/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-05-02 02:36:18.000000 python_amcards-1.3.3/python_amcards.egg-info/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)      316 2024-05-02 02:36:18.000000 python_amcards-1.3.3/python_amcards.egg-info/SOURCES.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        1 2024-05-02 02:36:18.000000 python_amcards-1.3.3/python_amcards.egg-info/dependency_links.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       12 2024-05-02 02:36:18.000000 python_amcards-1.3.3/python_amcards.egg-info/requires.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        8 2024-05-02 02:36:18.000000 python_amcards-1.3.3/python_amcards.egg-info/top_level.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       38 2024-05-02 02:36:18.309026 python_amcards-1.3.3/setup.cfg
+-rw-r--r--   0 simonesestili   (501) staff       (20)      874 2024-05-02 02:36:09.000000 python_amcards-1.3.3/setup.py
```

### Comparing `python_amcards-1.3.2/LICENSE` & `python_amcards-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.2/PKG-INFO` & `python_amcards-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.3.2
+Version: 1.3.3
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `python_amcards-1.3.2/README.rst` & `python_amcards-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.2/amcards/__helpers.py` & `python_amcards-1.3.3/amcards/__helpers.py`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.2/amcards/amcards.py` & `python_amcards-1.3.3/amcards/amcards.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,17 @@
         params = {
             'limit': limit,
             'offset': skip,
         } | (filters or {})
 
         res = requests.get(url=f'{DOMAIN}/.api/v1/credittransaction/', headers=self._HEADERS, params=params)
         if not res.ok:
-            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            if res.status_code == 401:
+                raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            raise exceptions.AMcardsException(f'Something went wrong when fetching credit transactions. AMcards Status Code: {res.status_code}, AMcards Body: {res.text}.')
 
         credit_transactions_json = res.json().get('objects', [])
         return [CreditTransaction._from_json(credit_transaction_json) for credit_transaction_json in credit_transactions_json]
 
     def credit_transaction_count(self, filters: dict = None) -> int:
         """Fetches count of client's AMcards credit transactions.
 
@@ -139,15 +141,17 @@
         """
         params = {
             'limit': 1,
         } | (filters or {})
 
         res = requests.get(url=f'{DOMAIN}/.api/v1/credittransaction/', headers=self._HEADERS, params=params)
         if not res.ok:
-            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            if res.status_code == 401:
+                raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            raise exceptions.AMcardsException(f'Something went wrong when fetching credit transaction count. AMcards Status Code: {res.status_code}, AMcards Body: {res.text}.')
 
         return res.json()['meta']['total_count']
 
     def templates(self, limit: int = 25, skip: int = 0) -> List[Template]:
         """Fetches client's AMcards templates.
 
         :param int limit: Defaults to ``25``. Max number of templates to be fetched.
@@ -157,15 +161,17 @@
         :rtype: List[:py:class:`Template <amcards.models.Template>`]
 
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
         res = requests.get(url=f'{DOMAIN}/.api/v1/template/', headers=self._HEADERS, params={'limit': limit, 'offset': skip})
         if not res.ok:
-            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            if res.status_code == 401:
+                raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            raise exceptions.AMcardsException(f'Something went wrong when fetching templates. AMcards Status Code: {res.status_code}, AMcards Body: {res.text}.')
 
         templates_json = res.json().get('objects', [])
         return [Template._from_json(template_json) for template_json in templates_json]
 
     def template(self, id: str | int) -> Template:
         """Fetches client's AMcards template with a specified id.
 
@@ -197,15 +203,17 @@
         :rtype: List[:py:class:`Template <amcards.models.Template>`]
 
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
         res = requests.get(url=f'{DOMAIN}/.api/v1/quicksendtemplate/', headers=self._HEADERS, params={'limit': limit, 'offset': skip})
         if not res.ok:
-            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            if res.status_code == 401:
+                raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            raise exceptions.AMcardsException(f'Something went wrong when fetching quicksends. AMcards Status Code: {res.status_code}, AMcards Body: {res.text}.')
 
         templates_json = res.json().get('objects', [])
         return [Template._from_json(template_json) for template_json in templates_json]
 
     def quicksend(self, id: str | int) -> Template:
         """Fetches client's AMcards quicksend template with a specified id.
 
@@ -237,15 +245,17 @@
         :rtype: List[:py:class:`Campaign <amcards.models.Campaign>`]
 
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
         res = requests.get(url=f'{DOMAIN}/.api/v1/campaign/', headers=self._HEADERS, params={'limit': limit, 'offset': skip})
         if not res.ok:
-            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            if res.status_code == 401:
+                raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            raise exceptions.AMcardsException(f'Something went wrong when fetching campaigns. AMcards Status Code: {res.status_code}, AMcards Body: {res.text}.')
 
         campaigns_json = res.json().get('objects', [])
         return [Campaign._from_json(campaign_json) for campaign_json in campaigns_json]
 
     def campaign(self, id: str | int) -> Campaign:
         """Fetches client's AMcards drip campaign with a specified id.
 
@@ -285,15 +295,17 @@
         params = {
             'limit': limit,
             'offset': skip,
         } | (filters or {})
 
         res = requests.get(url=f'{DOMAIN}/.api/v1/card/', headers=self._HEADERS, params=params)
         if not res.ok:
-            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            if res.status_code == 401:
+                raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            raise exceptions.AMcardsException(f'Something went wrong when fetching cards. AMcards Status Code: {res.status_code}, AMcards Body: {res.text}.')
 
         cards_json = res.json().get('objects', [])
         return [Card._from_json(card_json) for card_json in cards_json]
 
     def card(self, id: str | int) -> Card:
         """Fetches client's AMcards card with a specified id.
 
@@ -330,15 +342,17 @@
         """
         params = {
             'limit': 1,
         } | (filters or {})
 
         res = requests.get(url=f'{DOMAIN}/.api/v1/card/', headers=self._HEADERS, params=params)
         if not res.ok:
-            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            if res.status_code == 401:
+                raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+            raise exceptions.AMcardsException(f'Something went wrong when fetching card count. AMcards Status Code: {res.status_code}, AMcards Body: {res.text}.')
 
         return res.json()['meta']['total_count']
 
     def mailing(self, id: str | int) -> Mailing:
         """Fetches client's AMcards mailing with a specified id.
 
         :param str or int id: Unique id for the :py:class:`mailing <amcards.models.Mailing>` you are fetching.
```

### Comparing `python_amcards-1.3.2/amcards/exceptions.py` & `python_amcards-1.3.3/amcards/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.2/amcards/models.py` & `python_amcards-1.3.3/amcards/models.py`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.2/python_amcards.egg-info/PKG-INFO` & `python_amcards-1.3.3/python_amcards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.3.2
+Version: 1.3.3
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `python_amcards-1.3.2/setup.py` & `python_amcards-1.3.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def README():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='python-amcards',
-    version='1.3.2',
+    version='1.3.3',
     description='A wrapper for the AMcards API.',
     long_description=README(),
     long_description_content_type='text/x-rst',
     author='Simone Sestili',
     author_email='simone.sestili@amcards.com',
     url='https://github.com/simonesestili/python-amcards',
     packages=['amcards'],
```

