# Comparing `tmp/langchain_google_bigtable-0.2.0-py3-none-any.whl.zip` & `tmp/langchain_google_bigtable-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18237 bytes, number of entries: 11
--rw-r--r--  2.0 unx      957 b- defN 24-Mar-27 17:51 langchain_google_bigtable/__init__.py
--rw-r--r--  2.0 unx     4069 b- defN 24-Mar-27 17:51 langchain_google_bigtable/chat_message_history.py
--rw-r--r--  2.0 unx     1490 b- defN 24-Mar-27 17:51 langchain_google_bigtable/common.py
--rw-r--r--  2.0 unx    17224 b- defN 24-Mar-27 17:51 langchain_google_bigtable/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-27 17:51 langchain_google_bigtable/py.typed
--rw-r--r--  2.0 unx      597 b- defN 24-Mar-27 17:51 langchain_google_bigtable/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Mar-27 17:53 langchain_google_bigtable-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    17705 b- defN 24-Mar-27 17:53 langchain_google_bigtable-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 17:53 langchain_google_bigtable-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 24-Mar-27 17:53 langchain_google_bigtable-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1042 b- defN 24-Mar-27 17:53 langchain_google_bigtable-0.2.0.dist-info/RECORD
-11 files, 54560 bytes uncompressed, 16429 bytes compressed:  69.9%
+Zip file size: 18362 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      957 b- defN 24-May-01 23:07 langchain_google_bigtable/__init__.py
+-rw-r--r--  2.0 unx     4069 b- defN 24-May-01 23:07 langchain_google_bigtable/chat_message_history.py
+-rw-r--r--  2.0 unx     1490 b- defN 24-May-01 23:07 langchain_google_bigtable/common.py
+-rw-r--r--  2.0 unx    17224 b- defN 24-May-01 23:07 langchain_google_bigtable/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-01 23:07 langchain_google_bigtable/py.typed
+-rw-r--r--  2.0 unx      597 b- defN 24-May-01 23:07 langchain_google_bigtable/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-01 23:09 langchain_google_bigtable-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18752 b- defN 24-May-01 23:09 langchain_google_bigtable-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 23:09 langchain_google_bigtable-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 24-May-01 23:09 langchain_google_bigtable-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1042 b- defN 24-May-01 23:09 langchain_google_bigtable-0.2.1.dist-info/RECORD
+11 files, 55607 bytes uncompressed, 16554 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: langchain_google_bigtable/py.typed
 Comment: 
 
 Filename: langchain_google_bigtable/version.py
 Comment: 
 
-Filename: langchain_google_bigtable-0.2.0.dist-info/LICENSE
+Filename: langchain_google_bigtable-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_bigtable-0.2.0.dist-info/METADATA
+Filename: langchain_google_bigtable-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_bigtable-0.2.0.dist-info/WHEEL
+Filename: langchain_google_bigtable-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_bigtable-0.2.0.dist-info/top_level.txt
+Filename: langchain_google_bigtable-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_bigtable-0.2.0.dist-info/RECORD
+Filename: langchain_google_bigtable-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_bigtable/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

## Comparing `langchain_google_bigtable-0.2.0.dist-info/LICENSE` & `langchain_google_bigtable-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_bigtable-0.2.0.dist-info/METADATA` & `langchain_google_bigtable-0.2.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-bigtable
-Version: 0.2.0
+Version: 0.2.1
 Summary: LangChain integrations for Google Cloud Bigtable
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,119 +206,166 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/googleapis/langchain-google-bigtable-python
 Project-URL: Repository, https://github.com/googleapis/langchain-google-bigtable-python.git
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-bigtable-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-bigtable-python/blob/main/CHANGELOG.md
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: langchain-core <1.0.0,>=0.1.1
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
 Requires-Dist: google-cloud-bigtable <3.0.0,>=2.22.0
 Provides-Extra: test
 Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
 Requires-Dist: mypy ==1.9.0 ; extra == 'test'
 Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
 
-# Cloud Bigtable for LangChain
+Bigtable for LangChain
+======================
 
-This package contains the [LangChain][langchain] integrations for Cloud Bigtable.
+|preview| |pypi| |versions|
 
-> **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
+- `Client Library Documentation`_
+- `Product Documentation`_
 
-* [Documentation][docs]
-* [API Reference]()
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://cloud.google.com/products#product-launch-stages
+.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-bigtable.svg
+   :target: https://pypi.org/project/langchain-google-bigtable/
+.. |versions| image:: https://img.shields.io/pypi/pyversions/langchain-google-bigtable.svg
+   :target: https://pypi.org/project/langchain-google-bigtable/
+.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/langchain-google-bigtable/latest
+.. _Product Documentation: https://cloud.google.com/bigtable
 
-## Getting Started
+Quick Start
+-----------
 
-In order to use this library, you first need to go through the following steps:
+In order to use this library, you first need to go through the following
+steps:
 
-1. [Select or create a Cloud Platform project.][project]
-2. [Enable billing for your project.][billing]
-3. [Enable the Google Cloud Bigtable API.][api]
-4. [Setup Authentication.][auth]
+1. `Select or create a Cloud Platform project.`_
+2. `Enable billing for your project.`_
+3. `Enable the Google Cloud Bigtable API.`_
+4. `Setup Authentication.`_
 
-### Installation
+.. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
+.. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
+.. _Enable the Google Cloud Bigtable API.: https://console.cloud.google.com/flows/enableapi?apiid=bigtable.googleapis.com
+.. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
-Install this library in a [`virtualenv`][venv] using pip. [`virtualenv`][venv] is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Installation
+~~~~~~~~~~~~
 
-With [`virtualenv`][venv], it's possible to install this library without needing system
-install permissions, and without clashing with the installed system
-dependencies.
+Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. The basic problem it addresses is
+one of dependencies and versions, and indirectly permissions.
 
-```bash
-pip install virtualenv
-virtualenv <your-env>
-source <your-env>/bin/activate
-<your-env>/bin/pip install langchain-google-bigtable
-```
+With `virtualenv`_, it’s possible to install this library without needing system install permissions, and without clashing with the installed system dependencies.
 
-## Document Loader Usage
+.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
-Use a document loader to load data as LangChain `Document`s.
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
 
-```python
-from langchain_google_bigtable import BigtableLoader
+Python >= 3.8
 
+Mac/Linux
+^^^^^^^^^
 
-loader = BigtableLoader(
-    instance_id="my-instance",
-    table_name="my-table-name"
-)
-docs = loader.lazy_load()
-```
+.. code-block:: console
 
-See the full [Document Loader][loader] tutorial.
+   pip install virtualenv
+   virtualenv <your-env>
+   source <your-env>/bin/activate
+   <your-env>/bin/pip install langchain-google-bigtable
 
-## Chat Message History Usage
+Windows
+^^^^^^^
 
-Use `ChatMessageHistory` to store messages and provide conversation history to LLMs.
+.. code-block:: console
 
-```python
-from langchain_google_bigtable import BigtableChatMessageHistory
+   pip install virtualenv
+   virtualenv <your-env>
+   <your-env>\Scripts\activate
+   <your-env>\Scripts\pip.exe install langchain-google-bigtable
 
 
-history = BigtableChatMessageHistory(
-    instance_id="my-instance",
-    table_name="my-message-store",
-    session_id="my-session_id"
-)
-```
+Document Loader Usage
+~~~~~~~~~~~~~~~~~~~~~
 
-See the full [Chat Message History][history] tutorial.
+Use a document loader to load data as LangChain ``Document``\ s.
 
-## Contributing
+.. code-block:: python
+
+    from langchain_google_bigtable import BigtableLoader
+
+
+    loader = BigtableLoader(
+        instance_id="my-instance",
+        table_id="my-table-name"
+    )
+    docs = loader.lazy_load()
+
+See the full `Document Loader`_ tutorial.
+
+.. _`Document Loader`: https://github.com/googleapis/langchain-google-bigtable-python/blob/main/docs/document_loader.ipynb
+
+Chat Message History Usage
+--------------------------
+
+Use ``ChatMessageHistory`` to store messages and provide conversation
+history to LLMs.
+
+.. code:: python
+
+    from langchain_google_bigtable import BigtableChatMessageHistory
+
+
+    history = BigtableChatMessageHistory(
+        instance_id="my-instance",
+        table_id="my-message-store",
+        session_id="my-session_id"
+    )
+
+See the full `Chat Message History`_ tutorial.
+
+.. _`Chat Message History`: https://github.com/googleapis/langchain-google-bigtable-python/blob/main/docs/chat_message_history.ipynb
+
+Contributions
+~~~~~~~~~~~~~
 
 Contributions to this library are always welcome and highly encouraged.
 
-See [CONTRIBUTING][contributing] for more information how to get started.
+See `CONTRIBUTING`_ for more information how to get started.
 
 Please note that this project is released with a Contributor Code of Conduct. By participating in
-this project you agree to abide by its terms. See [Code of Conduct][coc] for more
+this project you agree to abide by its terms. See `Code of Conduct`_ for more
 information.
 
-## License
+.. _`CONTRIBUTING`: https://github.com/googleapis/langchain-google-bigtable-python/blob/main/CONTRIBUTING.md
+.. _`Code of Conduct`: https://github.com/googleapis/langchain-google-bigtable-python/blob/main/CODE_OF_CONDUCT.md
+
+
+License
+-------
 
-Apache 2.0 - See [LICENSE][license] for more information.
+Apache 2.0 - See
+`LICENSE <https://github.com/googleapis/langchain-google-bigtable-python/blob/main/LICENSE>`_
+for more information.
 
-## Disclaimer
+Disclaimer
+----------
 
 This is not an officially supported Google product.
 
-[project]: https://console.cloud.google.com/project
-[billing]: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-[api]: https://console.cloud.google.com/flows/enableapi?apiid=bigtable.googleapis.com
-[auth]: https://googleapis.dev/python/google-api-core/latest/auth.html
-[venv]: https://virtualenv.pypa.io/en/latest/
-[loader]: https://github.com/googleapis/langchain-google-bigtable-python/tree/main/docs/document_loader.ipynb
-[history]: https://github.com/googleapis/langchain-google-bigtable-python/tree/main/docs/chat_message_history.ipynb
-[langchain]: https://github.com/langchain-ai/langchain
-[docs]: https://github.com/googleapis/langchain-google-bigtable-python/tree/main/docs
-[license]: https://github.com/googleapis/langchain-google-bigtable-python/tree/main/LICENSE
-[contributing]: https://github.com/googleapis/langchain-google-bigtable-python/tree/main/CONTRIBUTING.md
-[coc]: https://github.com/googleapis/langchain-google-bigtable-python/tree/main/CODE_OF_CONDUCT.md
```

## Comparing `langchain_google_bigtable-0.2.0.dist-info/RECORD` & `langchain_google_bigtable-0.2.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 langchain_google_bigtable/__init__.py,sha256=qOswVwxGIVGPjwg0yjFj9vHZlJFD8ctfCE4oNz1w4tE,957
 langchain_google_bigtable/chat_message_history.py,sha256=j6ELZ07MwS00vV0Y8_37R80wdafMs49m-8Qj78Ld1f4,4069
 langchain_google_bigtable/common.py,sha256=LOISb6-5vFsa9m-CtCcX2njT6bbfNBy3gvp6P3B5_aU,1490
 langchain_google_bigtable/loader.py,sha256=6hCnEVBWbe1oVB0o8-f63H4bXv1B59Dd6id5u3yZJJQ,17224
 langchain_google_bigtable/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_bigtable/version.py,sha256=c32tFkU7bcWMAeqBrDdHTYBzbZPaJPvhWqbKnyY_LxM,597
-langchain_google_bigtable-0.2.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_bigtable-0.2.0.dist-info/METADATA,sha256=GyffH0Pg3ML3GBHGeG5WZKpr5xXc81yCPjBONX2Uqd8,17705
-langchain_google_bigtable-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_bigtable-0.2.0.dist-info/top_level.txt,sha256=cv5qmT-dg-qrQwjaRZNj4VBb--Y8KSWwzLc2Xohe87k,26
-langchain_google_bigtable-0.2.0.dist-info/RECORD,,
+langchain_google_bigtable/version.py,sha256=lal6j0-2qdxqYCLjy1FcTVeiboHQADADWfCBuVKcU3k,597
+langchain_google_bigtable-0.2.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_bigtable-0.2.1.dist-info/METADATA,sha256=UjtYMeD-T9UlOluIx7tWP79BjT-gmEge_YnPIxnk2f8,18752
+langchain_google_bigtable-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_bigtable-0.2.1.dist-info/top_level.txt,sha256=cv5qmT-dg-qrQwjaRZNj4VBb--Y8KSWwzLc2Xohe87k,26
+langchain_google_bigtable-0.2.1.dist-info/RECORD,,
```

