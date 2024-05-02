# Comparing `tmp/PerplexiPy-1.0.4-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11711 bytes, number of entries: 10
+Zip file size: 12240 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     9253 b- defN 24-Apr-22 04:33 perplexipy/__init__.py
--rw-r--r--  2.0 unx     9490 b- defN 24-Apr-26 04:59 perplexipy/codex.py
+-rw-r--r--  2.0 unx    13193 b- defN 24-May-02 18:08 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6833 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-26 05:03 PerplexiPy-1.0.4.dist-info/RECORD
-10 files, 29022 bytes uncompressed, 10319 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6968 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      814 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/RECORD
+10 files, 32861 bytes uncompressed, 10848 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.4.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.4.dist-info/METADATA
+Filename: PerplexiPy-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.4.dist-info/WHEEL
+Filename: PerplexiPy-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.4.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.4.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.4.dist-info/RECORD
+Filename: PerplexiPy-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/codex.py

```diff
@@ -47,42 +47,157 @@
 
 QUERY_DETAILED = 'Give me a concise coding example and include URL references in reply this prompt: '
 """
 @private
 """
 
 
+def _die(msg: str, exitCode: int = 99):
+    if exitCode == 1:
+        msgColor = 'white'
+    else:
+        msgColor = 'bright_yellow'
+    click.secho(msg+'\n', fg = msgColor)
+    sys.exit(exitCode)
+
+
 # *** globals ***
 
-_client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
+try:
+    _client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
+except:
+    _die('PERPLEXITY_API_KEY undefined in the environment or .env file', 2)
+
 _client.model = DEFAULT_MODEL_NAME
 _queryCodeStyle = True
 
 
 # *** classes and objects ***
 
 class CodexREPL:
 
     def __init__(self):
         self._client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
         self._client.model = DEFAULT_MODEL_NAME
         self._queryCodeStyle = True
 
 
+    def core(self, userQuery: str) -> str:
+        """
+        Send a user query to the model for processing.
+
+        Arguments
+        ---------
+            userQuery
+        A string with the user query, most often a programming question.
+
+        Returns
+        -------
+        The result of the query, or `None` if the query was empty.
+        """
+        result = None
+        if userQuery:
+            if not self._client:
+                self._client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
+                self._client.model = DEFAULT_MODEL_NAME
+            result = self._client.query(userQuery)
+
+        return result
+
+
+    def activeModel(self, modelID: int = 0) -> str:
+        if modelID:
+            try:
+                ref = modelID-1
+                model = list(self._client.models.keys())[ref]
+                self._client.model = model
+            except:
+                click.secho('Invalid model ID = %s' % modelID, bg = 'red', fg = 'white')
+        click.secho('Active model: %s\n' % self._client.model, fg = 'green', bold = True)
+        return self._client.model
+
+
+
+    def _displayModels(self) -> list:
+        """
+        Display the list of models supported by the API.
+
+        Returns
+        =======
+        A list of strings, each corresponding to a model name.
+        """
+        _activeModel()
+        print('Available models:\n')
+        n = 1
+        for model in self._client.models.keys():
+            print('%2d - %s' % (n, model))
+            n += 1
+        print()
+
+        return list(self._client.models.keys())
+
+
+    def editingMode(self, session: PromptSession, mode = None) -> PromptSession:
+        if mode:
+            mode = mode.lower()
+            newEditingMode = EditingMode.EMACS if mode == 'emacs' else EditingMode.VI
+            session = PromptSession(editing_mode = newEditingMode)
+
+        editingMode = str(session.editing_mode).replace('EditingMode.', '').lower()
+        click.secho('Editing mode = %s' % editingMode, fg = 'bright_blue')
+
+        return session
+
+    def _queryStyle(self, newStyle: str = None) -> bool:
+        if newStyle:
+            self._queryCodeStyle = newStyle != 'human'
+        click.secho('Coding query style = %s' % self._queryCodeStyle, fg = 'bright_blue')
+        return self._queryCodeStyle
+
+    def _makeQuery(self, userQuery: str) -> str:
+        if self._queryCodeStyle:
+            userQuery = QUERY_DETAILED+userQuery
+
+        return codex.core(userQuery)
+
+
+    def _saveConfigTo(self, config: dict, fileName: str = CONFIG_FILE_NAME, pathName = CONFIG_PATH):
+        if not os.path.exists(pathName):
+            os.makedirs(pathName)
+        with open(fileName, 'w') as outputFile:
+            yaml.dump(config, outputFile)
+
+
+    def _loadConfigFrom(self, fileName: str = CONFIG_FILE_NAME, pathName = CONFIG_PATH) -> dict:
+        if os.path.exists(fileName):
+            with open(fileName, 'r') as inputFile:
+                config = yaml.safe_load(inputFile)
+        else:
+            # TODO:  turn this into a self-contained object; maybe a named
+            #        tuple?
+            config = {
+                'activeModel': DEFAULT_MODEL_NAME,
+                'editingMode': 'vi',
+                'queryCodeStyle': _queryCodeStyle,
+            }
+            _saveConfigTo(config, fileName, pathName)
+        return config
+
+
+    def _displayConfigInfo(self):
+        click.secho('Config file: %s' % CONFIG_FILE_NAME)
+        click.secho(str(_loadConfigFrom())+'\n')
+
+
     def run(self):
         pass
 
 
 # *** implementation ***
 
-def _die(msg: str, exitCode: int = 99):
-    click.echo(msg)
-    sys.exit(99)
-
-
 def _helpUser() -> str:
     return "Syntax: codex repl | 'your coding question here in single quotes'\n"
 
 
 def codexCore(userQuery: str) -> str:
     """
     Send a user query to the model for processing.
@@ -233,15 +348,14 @@
             'queryCodeStyle': _queryCodeStyle,
         }
         _saveConfigTo(config, fileName, pathName)
     return config
 
 
 def _displayConfigInfo():
-    pass
     click.secho('Config file: %s' % CONFIG_FILE_NAME)
     click.secho(str(_loadConfigFrom())+'\n')
 
 
 # TODO: Refactor REPL - https://github.com/CIME-Software/perplexipy/issues/46
 def _runREPL() -> str:
     """
```

## Comparing `PerplexiPy-1.0.4.dist-info/LICENSE.txt` & `PerplexiPy-1.0.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.4.dist-info/METADATA` & `PerplexiPy-1.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.4
+Version: 1.0.5
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.4 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.5 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
 
 
@@ -94,14 +94,17 @@
 ============
 ```bash
 pip install perplexipy
 ```
 
 Package information:  https://pypi.org/project/perplexipy
 
+PerplexiPy requires an API key issued by Perplexity.  You may set PERPLEXITY_API_KEY
+as an environment variable or use a `.env` file.
+
 
 API key
 =======
 Access to the Perplexity API requires a paid subscription and an API key.
 
 Use of `.env` is recommended for storing the private key.  There is an automatic
 constant `PERPLEXITY_API_KEY` that gets initialized to the value of a `.env` key
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.4 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.5 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.4 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.5 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
@@ -40,45 +40,46 @@
 software.github.io/perplexipy/perplexipy.html - The _P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b
 tutorial notebook The `man` page can be generated from the source distribution
 using this command: ```bash make manpage ``` The output will reside in: `./
 manpages/perplexipy.3`. The `man` page isn't included in the Python package
 wheel because there's no accepted standard installation that's cross-compatible
 among all supported operating systems and distributions. Installation
 ============ ```bash pip install perplexipy ``` Package information: https://
-pypi.org/project/perplexipy API key ======= Access to the Perplexity API
-requires a paid subscription and an API key. Use of `.env` is recommended for
-storing the private key. There is an automatic constant `PERPLEXITY_API_KEY`
-that gets initialized to the value of a `.env` key of the same name via the
-`dotenv` API. Otherwise, `PERPLEXITY_API_KEY` may be handled like any other
-secret by the implementing team. This module provides no other tools or
-services for handling the API key. This key is used only during
-`PerplexityClient` instantiation: ```python import os key = os.environ
-['PERPLEXITY_API_KEY'] client = PerplexityClient(key = key) print(client.query
-('Brief answer: greet the world in Swedish.')) ``` Usage ===== See the
-_P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b notebook for a richer example of the API's
-capabilities. In general: ```python client = PerplexityClient() result =
-client.query('Show me how to declare a list in Python') # result is a string
-results = client.queryBatch('Show me different ways of declaring a Python
-list') for result in results: print(result) # results is a tuple of one or more
-results results = client.queryStreamable('Tell me why lists are important in
-programming') for result in results: print(result) # results is a long stream
-of data, served over time. models = client.models # lists all models supported
-by Perplexity AI print('Model names:') for model in models.keys(): print(' -
-%s' % model) try: client.model = 'bogus-LLM-7b' except PerplexityClientError as
-e: print(e) client.model = models.keys()[0] # OK ``` Async usage ===========
-Not supported at this time. Interactive usage ================= PerplexiPy
-ships with the Codex Playground, an interactive REPL console. To run it:
-```bash # In a virtualenv: pip install -U perplexipy export
-PERPLEXITY_API_KEY="your-key-goes-here" codex repl ``` Full description of
-Codex Playground and other use cases like streaming API and CLI argument
-passing in the [Codex README](https://github.com/CIME-Software/perplexipy/blob/
-master/codex-README.md). License ======= The **PerplexiPy** package,
-documentation and examples are licensed under the [BSD-3 open source license]
-(https://github.com/CIME-Software/perplexipy/blob/master/LICENSE.txt). See also
-======== - **codex** - a PerplexiPy command line code explainer - API
+pypi.org/project/perplexipy PerplexiPy requires an API key issued by
+Perplexity. You may set PERPLEXITY_API_KEY as an environment variable or use a
+`.env` file. API key ======= Access to the Perplexity API requires a paid
+subscription and an API key. Use of `.env` is recommended for storing the
+private key. There is an automatic constant `PERPLEXITY_API_KEY` that gets
+initialized to the value of a `.env` key of the same name via the `dotenv` API.
+Otherwise, `PERPLEXITY_API_KEY` may be handled like any other secret by the
+implementing team. This module provides no other tools or services for handling
+the API key. This key is used only during `PerplexityClient` instantiation:
+```python import os key = os.environ['PERPLEXITY_API_KEY'] client =
+PerplexityClient(key = key) print(client.query('Brief answer: greet the world
+in Swedish.')) ``` Usage ===== See the _P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b notebook for a
+richer example of the API's capabilities. In general: ```python client =
+PerplexityClient() result = client.query('Show me how to declare a list in
+Python') # result is a string results = client.queryBatch('Show me different
+ways of declaring a Python list') for result in results: print(result) #
+results is a tuple of one or more results results = client.queryStreamable
+('Tell me why lists are important in programming') for result in results: print
+(result) # results is a long stream of data, served over time. models =
+client.models # lists all models supported by Perplexity AI print('Model names:
+') for model in models.keys(): print(' - %s' % model) try: client.model =
+'bogus-LLM-7b' except PerplexityClientError as e: print(e) client.model =
+models.keys()[0] # OK ``` Async usage =========== Not supported at this time.
+Interactive usage ================= PerplexiPy ships with the Codex Playground,
+an interactive REPL console. To run it: ```bash # In a virtualenv: pip install
+-U perplexipy export PERPLEXITY_API_KEY="your-key-goes-here" codex repl ```
+Full description of Codex Playground and other use cases like streaming API and
+CLI argument passing in the [Codex README](https://github.com/CIME-Software/
+perplexipy/blob/master/codex-README.md). License ======= The **PerplexiPy**
+package, documentation and examples are licensed under the [BSD-3 open source
+license](https://github.com/CIME-Software/perplexipy/blob/master/LICENSE.txt).
+See also ======== - **codex** - a PerplexiPy command line code explainer - API
 documentation: https://cime-software.github.io/perplexipy - _P_e_r_p_l_e_x_i_t_y_ _A_I -
 m0toko: a Sopel bot plug-in that uses PerplexiPy for providing AI-enhanced
 chatbot functionality: https://github.com/pr3d4t0r/m0toko - PyPI: _o_p_e_n_a_i
 Caveats ======= The code should work with Python 3.7 or later, but it was only
 tested with Python 3.9.16 and later. Download the package and install it from
 source if support for an earlier Python version is required. Bugs ==== Feature
 requests and bug reports: https://github.com/CIME-Software/perplexipy/issues
```

