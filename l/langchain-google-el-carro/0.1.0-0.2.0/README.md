# Comparing `tmp/langchain_google_el_carro-0.1.0-py3-none-any.whl.zip` & `tmp/langchain_google_el_carro-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 21106 bytes, number of entries: 11
--rw-r--r--  2.0 unx      894 b- defN 24-Feb-28 23:10 langchain_google_el_carro/__init__.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Feb-28 23:10 langchain_google_el_carro/chat_message_history.py
--rw-r--r--  2.0 unx     9028 b- defN 24-Feb-28 23:10 langchain_google_el_carro/engine.py
--rw-r--r--  2.0 unx    14268 b- defN 24-Feb-28 23:10 langchain_google_el_carro/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Feb-28 23:10 langchain_google_el_carro/py.typed
--rw-r--r--  2.0 unx      597 b- defN 24-Feb-28 23:10 langchain_google_el_carro/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Feb-28 23:12 langchain_google_el_carro-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    19637 b- defN 24-Feb-28 23:12 langchain_google_el_carro-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-28 23:12 langchain_google_el_carro-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 24-Feb-28 23:12 langchain_google_el_carro-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1042 b- defN 24-Feb-28 23:12 langchain_google_el_carro-0.1.0.dist-info/RECORD
-11 files, 60337 bytes uncompressed, 19298 bytes compressed:  68.0%
+Zip file size: 21308 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      894 b- defN 24-May-01 23:40 langchain_google_el_carro/__init__.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-01 23:40 langchain_google_el_carro/chat_message_history.py
+-rw-r--r--  2.0 unx     9028 b- defN 24-May-01 23:40 langchain_google_el_carro/engine.py
+-rw-r--r--  2.0 unx    14268 b- defN 24-May-01 23:40 langchain_google_el_carro/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-01 23:40 langchain_google_el_carro/py.typed
+-rw-r--r--  2.0 unx      597 b- defN 24-May-01 23:40 langchain_google_el_carro/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-01 23:42 langchain_google_el_carro-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    21183 b- defN 24-May-01 23:42 langchain_google_el_carro-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 23:42 langchain_google_el_carro-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 24-May-01 23:42 langchain_google_el_carro-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1042 b- defN 24-May-01 23:42 langchain_google_el_carro-0.2.0.dist-info/RECORD
+11 files, 61883 bytes uncompressed, 19500 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: langchain_google_el_carro/py.typed
 Comment: 
 
 Filename: langchain_google_el_carro/version.py
 Comment: 
 
-Filename: langchain_google_el_carro-0.1.0.dist-info/LICENSE
+Filename: langchain_google_el_carro-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_el_carro-0.1.0.dist-info/METADATA
+Filename: langchain_google_el_carro-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_el_carro-0.1.0.dist-info/WHEEL
+Filename: langchain_google_el_carro-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_el_carro-0.1.0.dist-info/top_level.txt
+Filename: langchain_google_el_carro-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_el_carro-0.1.0.dist-info/RECORD
+Filename: langchain_google_el_carro-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_el_carro/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## Comparing `langchain_google_el_carro-0.1.0.dist-info/LICENSE` & `langchain_google_el_carro-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_el_carro-0.1.0.dist-info/METADATA` & `langchain_google_el_carro-0.2.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-el-carro
-Version: 0.1.0
+Version: 0.2.0
 Summary: LangChain integrations for Google El Carro Oracle
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,177 +205,221 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/googleapis/langchain-google-el-carro-python
 Project-URL: Repository, https://github.com/googleapis/langchain-google-el-carro-python.git
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-el-carro-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-el-carro-python/blob/main/CHANGELOG.md
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
 Requires-Dist: SQLAlchemy <3.0.0,>=2.0.25
 Requires-Dist: oracledb <3.0.0,>=2.0.1
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
 Provides-Extra: test
 Requires-Dist: langchain <1.0.0,>=0.1.8 ; extra == 'test'
 Requires-Dist: pytest >=7.4.4 ; extra == 'test'
-Requires-Dist: black[jupyter] ==23.12.0 ; extra == 'test'
+Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
-Requires-Dist: mypy ==1.7.1 ; extra == 'test'
+Requires-Dist: mypy ==1.9.0 ; extra == 'test'
 
-# El Carro for Oracle Databases for Langchain
+El Carro for Oracle Databases for LangChain
+==================================================
 
-This package contains the [LangChain][langchain] integrations for
-the [Google El Carro Oracle Operator](https://github.com/GoogleCloudPlatform/elcarro-oracle-operator).
+|preview| |pypi| |versions|
 
-> **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the
-> Google Cloud Terms of Service. Please note that pre-GA products and features
-> might have limited support, and changes to pre-GA products and features might
-> not be compatible with other pre-GA versions. For more information, see
-> the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
-
-* [Documentation](https://github.com/googleapis/langchain-google-el-carro-python/tree/main/docs/)
-
-## Known Limitations
-
-* The library supports El Carro Operator for Oracle 18c and higher versions.
-* By default the library
-  uses [thin mode](https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html)
-  for Oracle connectivity,
-  to use thick mode please follow the
-  corresponding [section](#oracle-thick-mode-connectivity).
-* To use VARCHAR2 datatype of size more than 4000 please
-  change the
-  parameter [MAX_STRING_SIZE](https://docs.oracle.com/en/database/oracle/oracle-database/19/refrn/MAX_STRING_SIZE.html#GUID-D424D23B-0933-425F-BC69-9C0E6724693C)
+- `Client Library Documentation`_
+- `Product Documentation`_
+
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
+.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-el-carro.svg  
+   :target: https://pypi.org/project/langchain-google-el-carro/
+.. |versions| image:: https://img.shields.io/pypi/pyversions/langchain-google-el-carro.svg
+   :target: https://pypi.org/project/langchain-google-el-carro/
+.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/langchain-google-el-carro/latest
+.. _Product Documentation: https://github.com/GoogleCloudPlatform/elcarro-oracle-operator
+
+Known Limitations
+-----------------
+
+- The library supports El Carro Operator for Oracle 18c and higher versions.
+
+- By default the library uses `thin mode.`_ for Oracle connectivity,
+  to use thick mode please follow the corresponding `section.`_.
+
+- To use VARCHAR2 datatype of size more than 4000 please change the parameter `MAX_STRING_SIZE.`_
   in the Oracle instance.
 
-## Getting Started
+.. _thin mode.: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html
+.. _section.: #oracle-thick-mode-connectivity
+.. _MAX_STRING_SIZE.: https://docs.oracle.com/en/database/oracle/oracle-database/19/refrn/MAX_STRING_SIZE.html#GUID-D424D23B-0933-425F-BC69-9C0E6724693C
+
+Quick Start
+-----------
 
-### Create an El Carro Operator Oracle Instance and a Database (PDB)
+Create an El Carro Operator Oracle Instance and a Database (PDB)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 In order to use this library, you first need to have an El Carro Operator
-software running
-with an Instance (CDB) and a Database (PDB).
+software running with an Instance (CDB) and a Database (PDB).
 
 Please follow the steps for El Carro Oracle Operator to provision a new database
 and create a PDB:
 
-* [El Carro Oracle 18c XE quickstart](https://github.com/GoogleCloudPlatform/elcarro-oracle-operator/blob/main/docs/content/quickstart-18c-xe.md)
-* [El Carro Oracle 19c EE quickstart](https://github.com/GoogleCloudPlatform/elcarro-oracle-operator/blob/main/docs/content/quickstart-19c-ee.md)
+- `El Carro Oracle 18c XE quickstart`_
+- `El Carro Oracle 19c EE quickstart`_
 
-### Installation
+.. _El Carro Oracle 18c XE quickstart: https://github.com/GoogleCloudPlatform/elcarro-oracle-operator/blob/main/docs/content/quickstart-18c-xe.md
+.. _El Carro Oracle 19c EE quickstart: https://github.com/GoogleCloudPlatform/elcarro-oracle-operator/blob/main/docs/content/quickstart-19c-ee.md
 
-Install this library in a [`virtualenv`][venv] using pip. [`virtualenv`][venv]
-is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
-
-With [`virtualenv`][venv], it's possible to install this library without needing
-system
-install permissions, and without clashing with the installed system
+
+Installation
+~~~~~~~~~~~~
+
+Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. The basic problem it addresses is
+one of dependencies and versions, and indirectly permissions.
+
+With `virtualenv`_, it’s
+possible to install this library without needing system install
+permissions, and without clashing with the installed system
 dependencies.
 
-```bash
-pip install virtualenv
-virtualenv <your-env>
-source <your-env>/bin/activate
-<your-env>/bin/pip install langchain-google-el-carro-python
-```
-
-## Document Loader Usage
-
-Use
-a [document loader](https://python.langchain.com/docs/modules/data_connection/document_loaders/)
-to load data as LangChain `Document`s.
-
-```python
-from langchain_google_el_carro import ElCarroEngine
-from langchain_google_el_carro.loader import \
-    ElCarroLoader, ElCarroDocumentSaver
-
-elcarro_engine = ElCarroEngine.from_instance(
-    "Your El Carro endpoint hostname", # e.g. 127.0.0.1
-    "Your El Carro endpoint port", # e.g. 3307
-    "Your PDB name",  # e.g. PDB1
-    "Your DB user",
-    "Your DB password",
-)
-loader = ElCarroLoader(
-    elcarro_engine,
-    table_name="my-table-name"
-)
-docs = loader.lazy_load()
-```
-
-See the
-full [Document Loader](https://github.com/googleapis/langchain-google-el-carro-python/tree/main/docs/doc_loader.md)
-tutorial.
-
-## Chat Message History Usage
-
-Use [ChatMessageHistory](https://python.langchain.com/docs/modules/memory/chat_messages/)
-to store messages and provide conversation history to LLMs.
-
-```python
-from langchain_google_el_carro import ElCarroEngine
-from langchain_google_el_carro.chat_message_history import \
-    ElCarroChatMessageHistory
-
-elcarro_engine = ElCarroEngine.from_instance(
-    "Your El Carro endpoint hostname", # e.g. 127.0.0.1
-    "Your El Carro endpoint port", # e.g. 3307
-    "Your PDB name",  # e.g. PDB1
-    "Your DB user",
-    "Your DB password",
-)
-history = ElCarroChatMessageHistory(
-    elcarro_engine=elcarro_engine, 
-    table_name="my-message-store",
-    session_id="my-session_id"
-)
-```
-
-See the
-full [Chat Message History](https://github.com/googleapis/langchain-google-el-carro-python/tree/main/docs/chat_message_history.md)
-tutorial.
-
-### Oracle Thick Mode Connectivity
-
-Thick mode connectivity requires you to install the Oracle Client libraries and
-pass `thick_mode=True` to `ElCarroEngine`. Follow these
-sections of the `oracledb` installation guide
-
-* [Oracle Instant Client Zip Files](https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html#oracle-instant-client-zip-files)
-* [Oracle Instant Client RPMs](https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html#oracle-instant-client-rpms)
-
-Example for Linux x64, glibc 2.14+:
-
-```bash
-wget https://download.oracle.com/otn_software/linux/instantclient/2113000/instantclient-basic-linux.x64-21.13.0.0.0dbru.zip -O /tmp/drv.zip
-rm -fr /tmp/instantclient_21_13/; unzip /tmp/drv.zip -d /tmp
-export LD_LIBRARY_PATH=/tmp/instantclient_21_13/:$LD_LIBRARY_PATH
-```
+.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Python >= 3.8
+
+Mac/Linux
+^^^^^^^^^
+
+.. code-block:: console
+
+   pip install virtualenv
+   virtualenv <your-env>
+   source <your-env>/bin/activate
+   <your-env>/bin/pip install langchain-google-el-carro
+
+Windows
+^^^^^^^
+
+.. code-block:: console
+
+    pip install virtualenv
+    virtualenv <your-env>
+    <your-env>\Scripts\activate
+    <your-env>\Scripts\pip.exe install langchain-google-el-carro
+
+
+Document Loader Usage
+~~~~~~~~~~~~~~~~~~~~~
+
+Use a document loader to load data as LangChain ``Document``\ s.
+
+.. code-block:: python
+
+    from langchain_google_el_carro import ElCarroEngine
+    from langchain_google_el_carro.loader import \
+        ElCarroLoader, ElCarroDocumentSaver
 
-## Contributing
+    elcarro_engine = ElCarroEngine.from_instance(
+        "Your El Carro endpoint hostname", # e.g. 127.0.0.1
+        "Your El Carro endpoint port", # e.g. 3307
+        "Your PDB name",  # e.g. PDB1
+        "Your DB user",
+        "Your DB password",
+    )
+    loader = ElCarroLoader(
+        elcarro_engine,
+        table_name="my-table-name"
+    )
+    docs = loader.lazy_load()
+
+See the full `Document Loader`_ tutorial.
+
+.. _`Document Loader`: https://github.com/googleapis/langchain-google-el-carro-python/blob/main/docs/document_loader.ipynb
+
+Chat Message History Usage
+--------------------------
+
+Use ``ChatMessageHistory`` to store messages and provide conversation
+history to LLMs.
+
+.. code:: python
+
+    from langchain_google_el_carro import ElCarroEngine
+    from langchain_google_el_carro.chat_message_history import \
+        ElCarroChatMessageHistory
+
+    elcarro_engine = ElCarroEngine.from_instance(
+        "Your El Carro endpoint hostname", # e.g. 127.0.0.1
+        "Your El Carro endpoint port", # e.g. 3307
+        "Your PDB name",  # e.g. PDB1
+        "Your DB user",
+        "Your DB password",
+    )
+    history = ElCarroChatMessageHistory(
+        elcarro_engine=elcarro_engine, 
+        table_name="my-message-store",
+        session_id="my-session_id"
+    )
+
+See the full `Chat Message History`_ tutorial.
+
+.. _`Chat Message History`: https://github.com/googleapis/langchain-google-el-carro-python/blob/main/docs/chat_message_history.ipynb
+
+
+Oracle Thick Mode Connectivity
+------------------------------
+
+Thick mode connectivity requires you to install the Oracle Client libraries and pass ``thick_mode=True`` to ``ElCarroEngine``. Follow these sections of the `oracledb` installation guide:
+
+- `Oracle Instant Client Zip Files`_
+- `Oracle Instant Client RPMs`_
+
+Example for Linux x64, glibc 2.14+::
+
+    wget https://download.oracle.com/otn_software/linux/instantclient/2113000/instantclient-basic-linux.x64-21.13.0.0.0dbru.zip -O /tmp/drv.zip
+    rm -fr /tmp/instantclient_21_13/; unzip /tmp/drv.zip -d /tmp
+    export LD_LIBRARY_PATH=/tmp/instantclient_21_13/:$LD_LIBRARY_PATH
+
+.. _Oracle Instant Client Zip Files: https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html#oracle-instant-client-zip-files
+.. _Oracle Instant Client RPMs: https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html#oracle-instant-client-rpms
+
+
+Contributions
+~~~~~~~~~~~~~
 
 Contributions to this library are always welcome and highly encouraged.
 
-See [CONTRIBUTING](CONTRIBUTING.md) for more information how to get started.
+See `CONTRIBUTING`_ for more information how to get started.
 
-Please note that this project is released with a Contributor Code of Conduct. By
-participating in
-this project you agree to abide by its terms.
-See [Code of Conduct](CODE_OF_CONDUCT.md) for more
+Please note that this project is released with a Contributor Code of Conduct. By participating in
+this project you agree to abide by its terms. See `Code of Conduct`_ for more
 information.
 
-## License
+.. _`CONTRIBUTING`: https://github.com/googleapis/langchain-google-el-carro-python/blob/main/CONTRIBUTING.md
+.. _`Code of Conduct`: https://github.com/googleapis/langchain-google-el-carro-python/blob/main/CODE_OF_CONDUCT.md
 
-Apache 2.0 - See [LICENSE](LICENSE) for more information.
+License
+-------
 
-## Disclaimer
+Apache 2.0 - See
+`LICENSE <https://github.com/googleapis/langchain-google-el-carro-python/tree/main/LICENSE>`_
+for more information.
 
-This is not an officially supported Google product.
+Disclaimer
+----------
 
-[venv]: https://virtualenv.pypa.io/en/latest/
-
-[langchain]: https://github.com/langchain-ai/langchain
+This is not an officially supported Google product.
```

## Comparing `langchain_google_el_carro-0.1.0.dist-info/RECORD` & `langchain_google_el_carro-0.2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 langchain_google_el_carro/__init__.py,sha256=E15__p65j8dKLE18xdlFUgriJqhbgqtEb6ZFEoPa8OU,894
 langchain_google_el_carro/chat_message_history.py,sha256=PBpqLcfe4Qh6kY3-HCKa3zk0ZnoZU7DdbV-FCzZz5pM,3395
 langchain_google_el_carro/engine.py,sha256=ACpaWysJ-8cUOWnhs-S27UbBsHgUlzzewfm4OH28i20,9028
 langchain_google_el_carro/loader.py,sha256=IuPNH1K4AUPga2b8zsb_g5oLFcnhvZ0r4TP4jXB71RQ,14268
 langchain_google_el_carro/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_el_carro/version.py,sha256=RuXdOB4FN_GOqGKFzaNfTuwuWOqyoQLC1DkG2RBXgGw,597
-langchain_google_el_carro-0.1.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_el_carro-0.1.0.dist-info/METADATA,sha256=j8bg7R8jEsCec-f5F93TNHG1fbk1GwBoVqD75nA_2cM,19637
-langchain_google_el_carro-0.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-langchain_google_el_carro-0.1.0.dist-info/top_level.txt,sha256=1zsJB-gefXATk3gsVVhFYqcixUFJBFESBaLTcdSE7oQ,26
-langchain_google_el_carro-0.1.0.dist-info/RECORD,,
+langchain_google_el_carro/version.py,sha256=c32tFkU7bcWMAeqBrDdHTYBzbZPaJPvhWqbKnyY_LxM,597
+langchain_google_el_carro-0.2.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_el_carro-0.2.0.dist-info/METADATA,sha256=RfthDaD2DzCtlnEH5dDOZb2kF8TKnKY6oEPn_0G5-c4,21183
+langchain_google_el_carro-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_el_carro-0.2.0.dist-info/top_level.txt,sha256=1zsJB-gefXATk3gsVVhFYqcixUFJBFESBaLTcdSE7oQ,26
+langchain_google_el_carro-0.2.0.dist-info/RECORD,,
```

