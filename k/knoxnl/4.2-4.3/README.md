# Comparing `tmp/knoxnl-4.2.tar.gz` & `tmp/knoxnl-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knoxnl-4.2.tar", last modified: Tue Apr 23 20:48:19 2024, max compression
+gzip compressed data, was "knoxnl-4.3.tar", last modified: Wed May  1 22:07:14 2024, max compression
```

## Comparing `knoxnl-4.2.tar` & `knoxnl-4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 20:48:19.374326 knoxnl-4.2/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-12 20:07:00.000000 knoxnl-4.2/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    17171 2024-04-23 20:48:19.361412 knoxnl-4.2/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    16780 2024-04-23 20:46:05.000000 knoxnl-4.2/README.md
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 20:48:19.078777 knoxnl-4.2/knoxnl/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-23 20:45:59.000000 knoxnl-4.2/knoxnl/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    43489 2024-04-23 20:47:58.000000 knoxnl-4.2/knoxnl/knoxnl.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 20:48:19.345332 knoxnl-4.2/knoxnl.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    17171 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      273 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       46 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-03-15 11:47:02.000000 knoxnl-4.2/knoxnl.egg-info/not-zip-safe
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       44 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        7 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/top_level.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-23 20:48:19.376408 knoxnl-4.2/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2347 2024-04-04 20:24:25.000000 knoxnl-4.2/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-01 22:07:14.014052 knoxnl-4.3/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-12 20:07:00.000000 knoxnl-4.3/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    19058 2024-05-01 22:07:14.003862 knoxnl-4.3/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    18636 2024-05-01 17:17:52.000000 knoxnl-4.3/README.md
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-01 22:07:13.572540 knoxnl-4.3/knoxnl/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-05-01 17:17:56.000000 knoxnl-4.3/knoxnl/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    55612 2024-05-01 22:06:26.000000 knoxnl-4.3/knoxnl/knoxnl.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-01 22:07:13.986807 knoxnl-4.3/knoxnl.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    19058 2024-05-01 22:07:12.000000 knoxnl-4.3/knoxnl.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      273 2024-05-01 22:07:13.000000 knoxnl-4.3/knoxnl.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-01 22:07:12.000000 knoxnl-4.3/knoxnl.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       46 2024-05-01 22:07:12.000000 knoxnl-4.3/knoxnl.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-03-15 11:47:02.000000 knoxnl-4.3/knoxnl.egg-info/not-zip-safe
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       60 2024-05-01 22:07:13.000000 knoxnl-4.3/knoxnl.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        7 2024-05-01 22:07:13.000000 knoxnl-4.3/knoxnl.egg-info/top_level.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-01 22:07:14.024739 knoxnl-4.3/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2365 2024-05-01 17:17:54.000000 knoxnl-4.3/setup.py
```

### Comparing `knoxnl-4.2/LICENSE` & `knoxnl-4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `knoxnl-4.2/PKG-INFO` & `knoxnl-4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: knoxnl
-Version: 4.2
+Version: 4.3
 Summary: A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)
 Home-page: https://github.com/xnl-h4ck3r/knoxnl
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: termcolor
 Requires-Dist: pyaml
 Requires-Dist: urlparse3
+Requires-Dist: python-dateutil
 
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.2
+## About - v4.3
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
+**DISCLAIMER: We are not responsible for any use, and especially misuse, of this tool or the KNOXSS API**
+
 ## Installation
 
 **NOTE: If you already have a `config.yml` file, it will not be overwritten. The file `config.yml.NEW` will be created in the same directory. If you need the new config, remove `config.yml` and rename `config.yml.NEW` back to `config.yml`.**
 
 `knoxnl` supports **Python 3**.
 
 Install `knoxnl` in default (global) python environment.
@@ -37,48 +40,57 @@
 ```bash
 pip install git+https://github.com/xnl-h4ck3r/knoxnl.git -v
 ```
 
 You can upgrade with
 
 ```bash
+knoxnl -up
+```
+
+OR
+
+```bash
 pip install --upgrade knoxnl
 ```
 
 ### pipx
 
 Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
 
 ```bash
 pipx install git+https://github.com/xnl-h4ck3r/knoxnl.git
 ```
 
 ## Usage
 
-| Arg  | Long Arg                 | Description                                                                                                                                                                                                                                                |
-| ---- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| -i   | --input                  | Input to send to KNOXSS API: a single URL, or file of URLs. **NOTE: If you pass a URL, put it in quotes otherwise the shell can interpret `&` characters as instruction to run a background task.**                                                        |
-| -o   | --output                 | The file to save the successful XSS and payloads to. If the file already exist it will just be appended to unless option `-ow` is passed.                                                                                                                  |
-| -ow  | --output-overwrite       | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                                    |
-| -oa  | --output-all             | Write all results to the output file, not just successful one's.                                                                                                                                                                                           |
-| -X   | --http-method            | Which HTTP method to use, values `GET`, `POST` or `BOTH` (default: `GET`). If `BOTH` is chosen, then a `GET` call will be made, followed by a `POST`.                                                                                                      |
-| -pd  | --post-data              | If a POST request is made, this is the POST data passed. It must be in the format `'param1=value&param2=value&param3=value'`. If this isn't passed and query string parameters are used, then these will be used as POST data if POST Method is requested. |
-| -H   | --headers                | Add custom headers to pass with HTTP requests. Pass in the format `'Header1:value1;\|Header2:value2'` (e.g. separate different headers with a pipe \| character).                                                                                          |
-| -A   | --api-key                | The KNOXSS API Key to use. This will be used instead of the value in `config.yml`                                                                                                                                                                          |
-| -afb | --advanced-filter-bypass | If the advanced filter bypass should be used on the KNOXSS API.                                                                                                                                                                                            |
-| -s   | --success-only           | Only show successful XSS payloads in the CLI output.                                                                                                                                                                                                       |
-| -p   | --processes              | Basic multithreading is done when getting requests for a file of URLs. This argument determines the number of processes (one per URL to check) are run per minute (default: 3). This is due to the rate limit of the KNOXSS API.                           |
-| -t   | --timeout                | How many seconds to wait for the KNOXSS API to respond before giving up (default: 600). If set to 0, then timeout will be used.                                                                                                                            |
-| -bp  | --burp-piper             | Use if **knoxnl** is called from the Burp Piper extension, so that a request in **Burp Suite** proxy can be tested. See the [Using in Burp Suite Proxy](#using-in-burp-suite-proxy) section below.                                                         |
-| -r   | --retries                | The number of times to retry when having issues connecting to the KNOXSS API (default: 3)                                                                                                                                                                  |
-| -ri  | --retry-interval         | How many seconds to wait before retrying when having issues connecting to the KNOXSS API (default: 30)                                                                                                                                                     |
-| -rb  | --retry-backoff          | The backoff factor used when retrying when having issues connecting to the KNOXSS API (default: 1.5). For example, with defaults, first time will wait for 30 seconds, 2nd time will be 45 (30 x 1.5) seconds, etc.                                        |
-| -v   | --verbose                | Verbose output                                                                                                                                                                                                                                             |
-|      | --version                | Show current version number.                                                                                                                                                                                                                               |
-| -h   | --help                   | show the help message and exit                                                                                                                                                                                                                             |
+| Arg  | Long Arg                 | Description                                                                                                                                                                                                                                                                  |
+| ---- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| -i   | --input                  | Input to send to KNOXSS API: a single URL, or file of URLs. **NOTE: If you pass a URL, put it in quotes otherwise the shell can interpret `&` characters as instruction to run a background task.**                                                                          |
+| -o   | --output                 | The file to save the successful XSS and payloads to. If the file already exist it will just be appended to unless option `-ow` is passed. If the full path doesn't exist, then any necessary directories will be created.                                                    |
+| -ow  | --output-overwrite       | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                                                      |
+| -oa  | --output-all             | Write all results to the output file, not just successful one's.                                                                                                                                                                                                             |
+| -X   | --http-method            | Which HTTP method to use, values `GET`, `POST` or `BOTH` (default: `GET`). If `BOTH` is chosen, then a `GET` call will be made, followed by a `POST`.                                                                                                                        |
+| -pd  | --post-data              | If a POST request is made, this is the POST data passed. It must be in the format `'param1=value&param2=value&param3=value'`. If this isn't passed and query string parameters are used, then these will be used as POST data if POST Method is requested.                   |
+| -H   | --headers                | Add custom headers to pass with HTTP requests. Pass in the format `'Header1:value1;\|Header2:value2'` (e.g. separate different headers with a pipe \| character).                                                                                                            |
+| -A   | --api-key                | The KNOXSS API Key to use. This will be used instead of the value in `config.yml`                                                                                                                                                                                            |
+| -afb | --advanced-filter-bypass | If the advanced filter bypass should be used on the KNOXSS API.                                                                                                                                                                                                              |
+| -s   | --success-only           | Only show successful XSS payloads in the CLI output.                                                                                                                                                                                                                         |
+| -p   | --processes              | Basic multithreading is done when getting requests for a file of URLs. This argument determines the number of processes (one per URL to check) are run per minute (default: 3). This is due to the rate limit of the KNOXSS API.                                             |
+| -t   | --timeout                | How many seconds to wait for the KNOXSS API to respond before giving up (default: 600). If set to 0, then timeout will be used.                                                                                                                                              |
+| -bp  | --burp-piper             | Use if **knoxnl** is called from the Burp Piper extension, so that a request in **Burp Suite** proxy can be tested. See the [Using in Burp Suite Proxy](#using-in-burp-suite-proxy) section below.                                                                           |
+| -r   | --retries                | The number of times to retry when having issues connecting to the KNOXSS API (default: 3)                                                                                                                                                                                    |
+| -ri  | --retry-interval         | How many seconds to wait before retrying when having issues connecting to the KNOXSS API (default: 30)                                                                                                                                                                       |
+| -rb  | --retry-backoff          | The backoff factor used when retrying when having issues connecting to the KNOXSS API (default: 1.5). For example, with defaults, first time will wait for 30 seconds, 2nd time will be 45 (30 x 1.5) seconds, etc.                                                          |
+| -pur | --pause-until-reset      | If the API Limit reset time is known and the API limit is reached, wait the required time until the limit is reset and continue again. The reset time is only known if knoxnl has run for request number 1 previously. The API rate limit is reset 24 hours after request 1. |
+| -sb  | --skip-blocked           | The number of 403 Forbidden responses from a target (for a given HTTP method + scheme + (sub)domain) before skipping. This is useful if you know the target has a WAF. The default is zero, which means no blocking is done.                                                 |
+| -up  | --update                 | Update knoxnl to the latest version.                                                                                                                                                                                                                                         |
+| -v   | --verbose                | Verbose output                                                                                                                                                                                                                                                               |
+|      | --version                | Show current version number.                                                                                                                                                                                                                                                 |
+| -h   | --help                   | show the help message and exit                                                                                                                                                                                                                                               |
 
 ## config.yml
 
 The `config.yml` file (in the global location based on the OS, e.g. `~/.config/knoxnl/config.yml`) has the keys which can be updated to suit your needs:
 
 - `API_URL` - This can be set to the KNOXSS API endpoint, if and when it is changed
 - `API_KEY` - Your KNOXSS API key that you will have generated on https://knoxss.me/
@@ -86,21 +98,21 @@
 
 ## Important Notes from KNOXSS API Guidelines
 
 - Unlike other APIs that just retrieve data from a database, KNOXSS API returns the results like the web interface, actually performing a comprehensive vulnerability scan for XSS. Since scan results are not stored by our system, they need to be generated on the fly taking several JavaScript-evaluated live tests to return them. So it's natural the data returned takes much more time to get delivered since there's a long process involved at server side.
 - The API standard rate limit is 5000 requests over a 24 hours period. That means an average of **2.3 requests per minute** so please try to keep this pace **to not overload the system**. Due to this rate limit, if the input is a file or URLs, then only a batch (determined by argument `-p`/`--processes`) will be run per minute.
 - **Generating or Regenerating your API Key** - The API key is in your profile. If you have never generated it you need to hit the button at least once to generate it and save. Any time you need a new API key for security reasons, you can simply hit the button and regenerate it.
 - **Flash Mode Mark - [XSS]** - Provide the `[XSS]` mark in any place of the target's data values to enable Flash Mode which enables KNOXSS to perform a single quick XSS Polyglot based test.
-- At the time of writing this, the daily limit of KNOXSS API calls is **5000**. If you are testing a large file of URLs,it is advisable that you use the `-o` / `--output` option to specify a file where output will be written. If you do reach the API limit with a 24 hour period, this is reset at about 17:00 GMT.
-- If you pass an input file and the API limit is reached, or the Service is Unavailable, part way through the input, all unchecked URLs will be output to an file in the same location, and with the same name as the input file, but with a `.YYYYMMDD_HHMMSS.todo` suffix. You can then rename this file and use this as input at another time.
-- By default, only successful results are written to the output file.
-- Passing argument `-oa` / `--output-all` will write **ALL** results to the output file, not just successful one's.
 
-## Important Notes fof knoxnl
+## Important Notes for knoxnl
 
+- At the time of writing this, the daily limit of KNOXSS API calls is **5000**. If you are testing a large file of URLs, it is advisable that you use the `-o` / `--output` option to specify a file where output will be written. If you do reach the API limit, it resets 24 hours after the first API call was made. If you are processing a file of URLs, you can use the `-pur`/`--pause-until-reset` to wait until the reset happens and then continue (this is only possible if the first request was run by `knoxnl` so it could save the response timestamp).
+- If you pass an input file and the API limit is reached, or the Service is Unavailable, part way through the input, all unchecked URLs will be output to an file in the same location, and with the same name as the input file, but with a `.YYYYMMDD_HHMMSS.todo` suffix. You can then rename this file and use this as input at another time. The `.todo` file will be created in the current directory unless a path is specified in the `-o`/`--output` directory, and then the `.todo` file will be created in the same directory.
+- By default, only successful results are written to the output file.
+- Passing argument `-oa` / `--output-all` will write **ALL** results to the output file, not just successful one's.
 - The KNOXSS API has a rate limit of no more than 5 URLs processed per minute. If the rate limit is exceeded then you might end up getting blocked by their WAF, and you will not get the results you want. This rate limit is taken into account when passing a file of URLs as input. However, if you keep running for a single URL more than this per minute you wil run into problems. Please respect the rules of their API.
 - The KNOXSS only deals with POST requests with basic post data in the format `'param1=value&param2=value&param3=value'`.
 - If the `-pd`/`--post-data` argument is not passed and a POST request is made, it will use the query string from the URL as post data if it has one.
 - If a file is passed as input and POST method is required, then the post data parameters need to be provided as a query string for the URL in the file, e.g. `https://example.com?postParam1=value&postParam2-value`. If you use the `-pd`/`--post-data` with an input file then ALL URLs will use that post data.
 - These are required based on the way the KNOXSS API works.
 
 ## Examples
```

### Comparing `knoxnl-4.2/README.md` & `knoxnl-4.3/knoxnl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,32 @@
+Metadata-Version: 2.1
+Name: knoxnl
+Version: 4.3
+Summary: A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)
+Home-page: https://github.com/xnl-h4ck3r/knoxnl
+Author: @xnl-h4ck3r
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: argparse
+Requires-Dist: requests
+Requires-Dist: termcolor
+Requires-Dist: pyaml
+Requires-Dist: urlparse3
+Requires-Dist: python-dateutil
+
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.2
+## About - v4.3
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
+**DISCLAIMER: We are not responsible for any use, and especially misuse, of this tool or the KNOXSS API**
+
 ## Installation
 
 **NOTE: If you already have a `config.yml` file, it will not be overwritten. The file `config.yml.NEW` will be created in the same directory. If you need the new config, remove `config.yml` and rename `config.yml.NEW` back to `config.yml`.**
 
 `knoxnl` supports **Python 3**.
 
 Install `knoxnl` in default (global) python environment.
@@ -23,48 +40,57 @@
 ```bash
 pip install git+https://github.com/xnl-h4ck3r/knoxnl.git -v
 ```
 
 You can upgrade with
 
 ```bash
+knoxnl -up
+```
+
+OR
+
+```bash
 pip install --upgrade knoxnl
 ```
 
 ### pipx
 
 Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
 
 ```bash
 pipx install git+https://github.com/xnl-h4ck3r/knoxnl.git
 ```
 
 ## Usage
 
-| Arg  | Long Arg                 | Description                                                                                                                                                                                                                                                |
-| ---- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| -i   | --input                  | Input to send to KNOXSS API: a single URL, or file of URLs. **NOTE: If you pass a URL, put it in quotes otherwise the shell can interpret `&` characters as instruction to run a background task.**                                                        |
-| -o   | --output                 | The file to save the successful XSS and payloads to. If the file already exist it will just be appended to unless option `-ow` is passed.                                                                                                                  |
-| -ow  | --output-overwrite       | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                                    |
-| -oa  | --output-all             | Write all results to the output file, not just successful one's.                                                                                                                                                                                           |
-| -X   | --http-method            | Which HTTP method to use, values `GET`, `POST` or `BOTH` (default: `GET`). If `BOTH` is chosen, then a `GET` call will be made, followed by a `POST`.                                                                                                      |
-| -pd  | --post-data              | If a POST request is made, this is the POST data passed. It must be in the format `'param1=value&param2=value&param3=value'`. If this isn't passed and query string parameters are used, then these will be used as POST data if POST Method is requested. |
-| -H   | --headers                | Add custom headers to pass with HTTP requests. Pass in the format `'Header1:value1;\|Header2:value2'` (e.g. separate different headers with a pipe \| character).                                                                                          |
-| -A   | --api-key                | The KNOXSS API Key to use. This will be used instead of the value in `config.yml`                                                                                                                                                                          |
-| -afb | --advanced-filter-bypass | If the advanced filter bypass should be used on the KNOXSS API.                                                                                                                                                                                            |
-| -s   | --success-only           | Only show successful XSS payloads in the CLI output.                                                                                                                                                                                                       |
-| -p   | --processes              | Basic multithreading is done when getting requests for a file of URLs. This argument determines the number of processes (one per URL to check) are run per minute (default: 3). This is due to the rate limit of the KNOXSS API.                           |
-| -t   | --timeout                | How many seconds to wait for the KNOXSS API to respond before giving up (default: 600). If set to 0, then timeout will be used.                                                                                                                            |
-| -bp  | --burp-piper             | Use if **knoxnl** is called from the Burp Piper extension, so that a request in **Burp Suite** proxy can be tested. See the [Using in Burp Suite Proxy](#using-in-burp-suite-proxy) section below.                                                         |
-| -r   | --retries                | The number of times to retry when having issues connecting to the KNOXSS API (default: 3)                                                                                                                                                                  |
-| -ri  | --retry-interval         | How many seconds to wait before retrying when having issues connecting to the KNOXSS API (default: 30)                                                                                                                                                     |
-| -rb  | --retry-backoff          | The backoff factor used when retrying when having issues connecting to the KNOXSS API (default: 1.5). For example, with defaults, first time will wait for 30 seconds, 2nd time will be 45 (30 x 1.5) seconds, etc.                                        |
-| -v   | --verbose                | Verbose output                                                                                                                                                                                                                                             |
-|      | --version                | Show current version number.                                                                                                                                                                                                                               |
-| -h   | --help                   | show the help message and exit                                                                                                                                                                                                                             |
+| Arg  | Long Arg                 | Description                                                                                                                                                                                                                                                                  |
+| ---- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| -i   | --input                  | Input to send to KNOXSS API: a single URL, or file of URLs. **NOTE: If you pass a URL, put it in quotes otherwise the shell can interpret `&` characters as instruction to run a background task.**                                                                          |
+| -o   | --output                 | The file to save the successful XSS and payloads to. If the file already exist it will just be appended to unless option `-ow` is passed. If the full path doesn't exist, then any necessary directories will be created.                                                    |
+| -ow  | --output-overwrite       | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                                                      |
+| -oa  | --output-all             | Write all results to the output file, not just successful one's.                                                                                                                                                                                                             |
+| -X   | --http-method            | Which HTTP method to use, values `GET`, `POST` or `BOTH` (default: `GET`). If `BOTH` is chosen, then a `GET` call will be made, followed by a `POST`.                                                                                                                        |
+| -pd  | --post-data              | If a POST request is made, this is the POST data passed. It must be in the format `'param1=value&param2=value&param3=value'`. If this isn't passed and query string parameters are used, then these will be used as POST data if POST Method is requested.                   |
+| -H   | --headers                | Add custom headers to pass with HTTP requests. Pass in the format `'Header1:value1;\|Header2:value2'` (e.g. separate different headers with a pipe \| character).                                                                                                            |
+| -A   | --api-key                | The KNOXSS API Key to use. This will be used instead of the value in `config.yml`                                                                                                                                                                                            |
+| -afb | --advanced-filter-bypass | If the advanced filter bypass should be used on the KNOXSS API.                                                                                                                                                                                                              |
+| -s   | --success-only           | Only show successful XSS payloads in the CLI output.                                                                                                                                                                                                                         |
+| -p   | --processes              | Basic multithreading is done when getting requests for a file of URLs. This argument determines the number of processes (one per URL to check) are run per minute (default: 3). This is due to the rate limit of the KNOXSS API.                                             |
+| -t   | --timeout                | How many seconds to wait for the KNOXSS API to respond before giving up (default: 600). If set to 0, then timeout will be used.                                                                                                                                              |
+| -bp  | --burp-piper             | Use if **knoxnl** is called from the Burp Piper extension, so that a request in **Burp Suite** proxy can be tested. See the [Using in Burp Suite Proxy](#using-in-burp-suite-proxy) section below.                                                                           |
+| -r   | --retries                | The number of times to retry when having issues connecting to the KNOXSS API (default: 3)                                                                                                                                                                                    |
+| -ri  | --retry-interval         | How many seconds to wait before retrying when having issues connecting to the KNOXSS API (default: 30)                                                                                                                                                                       |
+| -rb  | --retry-backoff          | The backoff factor used when retrying when having issues connecting to the KNOXSS API (default: 1.5). For example, with defaults, first time will wait for 30 seconds, 2nd time will be 45 (30 x 1.5) seconds, etc.                                                          |
+| -pur | --pause-until-reset      | If the API Limit reset time is known and the API limit is reached, wait the required time until the limit is reset and continue again. The reset time is only known if knoxnl has run for request number 1 previously. The API rate limit is reset 24 hours after request 1. |
+| -sb  | --skip-blocked           | The number of 403 Forbidden responses from a target (for a given HTTP method + scheme + (sub)domain) before skipping. This is useful if you know the target has a WAF. The default is zero, which means no blocking is done.                                                 |
+| -up  | --update                 | Update knoxnl to the latest version.                                                                                                                                                                                                                                         |
+| -v   | --verbose                | Verbose output                                                                                                                                                                                                                                                               |
+|      | --version                | Show current version number.                                                                                                                                                                                                                                                 |
+| -h   | --help                   | show the help message and exit                                                                                                                                                                                                                                               |
 
 ## config.yml
 
 The `config.yml` file (in the global location based on the OS, e.g. `~/.config/knoxnl/config.yml`) has the keys which can be updated to suit your needs:
 
 - `API_URL` - This can be set to the KNOXSS API endpoint, if and when it is changed
 - `API_KEY` - Your KNOXSS API key that you will have generated on https://knoxss.me/
@@ -72,21 +98,21 @@
 
 ## Important Notes from KNOXSS API Guidelines
 
 - Unlike other APIs that just retrieve data from a database, KNOXSS API returns the results like the web interface, actually performing a comprehensive vulnerability scan for XSS. Since scan results are not stored by our system, they need to be generated on the fly taking several JavaScript-evaluated live tests to return them. So it's natural the data returned takes much more time to get delivered since there's a long process involved at server side.
 - The API standard rate limit is 5000 requests over a 24 hours period. That means an average of **2.3 requests per minute** so please try to keep this pace **to not overload the system**. Due to this rate limit, if the input is a file or URLs, then only a batch (determined by argument `-p`/`--processes`) will be run per minute.
 - **Generating or Regenerating your API Key** - The API key is in your profile. If you have never generated it you need to hit the button at least once to generate it and save. Any time you need a new API key for security reasons, you can simply hit the button and regenerate it.
 - **Flash Mode Mark - [XSS]** - Provide the `[XSS]` mark in any place of the target's data values to enable Flash Mode which enables KNOXSS to perform a single quick XSS Polyglot based test.
-- At the time of writing this, the daily limit of KNOXSS API calls is **5000**. If you are testing a large file of URLs,it is advisable that you use the `-o` / `--output` option to specify a file where output will be written. If you do reach the API limit with a 24 hour period, this is reset at about 17:00 GMT.
-- If you pass an input file and the API limit is reached, or the Service is Unavailable, part way through the input, all unchecked URLs will be output to an file in the same location, and with the same name as the input file, but with a `.YYYYMMDD_HHMMSS.todo` suffix. You can then rename this file and use this as input at another time.
-- By default, only successful results are written to the output file.
-- Passing argument `-oa` / `--output-all` will write **ALL** results to the output file, not just successful one's.
 
-## Important Notes fof knoxnl
+## Important Notes for knoxnl
 
+- At the time of writing this, the daily limit of KNOXSS API calls is **5000**. If you are testing a large file of URLs, it is advisable that you use the `-o` / `--output` option to specify a file where output will be written. If you do reach the API limit, it resets 24 hours after the first API call was made. If you are processing a file of URLs, you can use the `-pur`/`--pause-until-reset` to wait until the reset happens and then continue (this is only possible if the first request was run by `knoxnl` so it could save the response timestamp).
+- If you pass an input file and the API limit is reached, or the Service is Unavailable, part way through the input, all unchecked URLs will be output to an file in the same location, and with the same name as the input file, but with a `.YYYYMMDD_HHMMSS.todo` suffix. You can then rename this file and use this as input at another time. The `.todo` file will be created in the current directory unless a path is specified in the `-o`/`--output` directory, and then the `.todo` file will be created in the same directory.
+- By default, only successful results are written to the output file.
+- Passing argument `-oa` / `--output-all` will write **ALL** results to the output file, not just successful one's.
 - The KNOXSS API has a rate limit of no more than 5 URLs processed per minute. If the rate limit is exceeded then you might end up getting blocked by their WAF, and you will not get the results you want. This rate limit is taken into account when passing a file of URLs as input. However, if you keep running for a single URL more than this per minute you wil run into problems. Please respect the rules of their API.
 - The KNOXSS only deals with POST requests with basic post data in the format `'param1=value&param2=value&param3=value'`.
 - If the `-pd`/`--post-data` argument is not passed and a POST request is made, it will use the query string from the URL as post data if it has one.
 - If a file is passed as input and POST method is required, then the post data parameters need to be provided as a query string for the URL in the file, e.g. `https://example.com?postParam1=value&postParam2-value`. If you use the `-pd`/`--post-data` with an input file then ALL URLs will use that post data.
 - These are required based on the way the KNOXSS API works.
 
 ## Examples
```

### Comparing `knoxnl-4.2/knoxnl/knoxnl.py` & `knoxnl-4.3/knoxnl/knoxnl.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,38 +17,48 @@
 import os
 import sys
 from pathlib import Path
 try:
     from . import __version__
 except:
     pass
-from datetime import datetime
+from datetime import datetime, timedelta
 from requests.adapters import HTTPAdapter, Retry
 import re
 import time
 from urllib.parse import urlparse
+from dateutil import tz
+import subprocess
 
 # Global variables
 stopProgram = False
 latestApiCalls = "Unknown"
 urlPassed = True
 rateLimitExceeded = False
 needToStop = False
 needToRetry = False
 dontDisplay = False
 successCount = 0
+safeCount = 0
+errorCount = 0
+requestCount = 0
+skipCount = 0
 outFile = None
 fileIsOpen = False
 todoFileName = ''
 currentCount = {}
 configPath = ''
 inputValues = set()
-blockedDomains = set()
+blockedDomains = {}
 HTTP_ADAPTER = None
 retryAttempt = 0
+apiResetPath = ''
+timeAPIReset = None
+forbiddenResponseCount = 0
+latestVersion = ''
 
 pauseEvent = mp.Event()
 
 DEFAULT_API_URL = 'https://api.knoxss.pro'
 
 # The default timeout for KNOXSS API to respond in seconds
 DEFAULT_TIMEOUT = 600
@@ -71,23 +81,22 @@
 class knoxss:
     Code = ''
     XSS = ''
     PoC = ''
     Calls = ''
     Error = ''
     POSTData = ''
+    Timestamp = ''
 
 def showVersion():
+    global latestVersion
     try:
-        
-        try:
-            resp = requests.get('https://raw.githubusercontent.com/xnl-h4ck3r/knoxnl/main/knoxnl/__init__.py',timeout=3)
-        except:
+        if latestVersion == '':
             print('Current knoxnl version '+__version__+' (unable to check if latest)')
-        if __version__ == resp.text.split('=')[1].replace('"',''):
+        elif __version__ == latestVersion:
             print('Current knoxnl version '+__version__+' ('+colored('latest','green')+')\n')
         else:
             print('Current knoxnl version '+__version__+' ('+colored('outdated','red')+')\n')
     except:
         pass
     
 def showBanner():
@@ -95,26 +104,32 @@
     print(" _           "+colored("_ ___    ","red")+colored("__","yellow")+colored("      _","cyan"))
     print("| | ___ __   "+colored("V","red")+"_"+colored(r"V\ \  ","red")+colored("/ /","yellow")+colored("_ __","green")+colored(" | | ","cyan"))
     print(r"| |/ / '_ \ / _ \ "[:-1]+colored(r"\ \ "[:-1],"red")+colored("/ /","yellow")+colored(r"| '_ \ "[:-1],"green")+colored("| | ","cyan"))
     print("|   <| | | | (_) "+colored("/ /","red")+colored(r"\ \ "[:-1],"yellow")+colored("| | | |","green")+colored(" | ","cyan"))
     print(r"|_|\_\_| |_|\___"+colored("/_/  ","red")+colored(r"\_\ "[:-1],"yellow")+colored("_| |_|","green")+colored("_| ","cyan"))
     print(colored("                 by @Xnl-h4ck3r ","magenta"))
     print()
+    print(colored('DISCLAIMER: We are not responsible for any use, and especially misuse, of this tool or the KNOXSS API','yellow'))
+    print()
     showVersion()
 
 # Functions used when printing messages dependant on verbose options
 def verbose():
     return args.verbose
 
 def showBlocked():
     global blockedDomains
     try:
-        # If there were any domains that might be blocking KNOXSS, let the user know
-        if len(blockedDomains) > 0:
-            print(colored('The following domains seem to be blocking KNOXSS and might be worth excluding for now:','yellow'),colored(', '.join(blockedDomains),'white'))
+        # Accumulate domains with a count more than the specified limit into a list
+        domainsBlockedLimit = [domain for domain, count in blockedDomains.items() if count > args.skip_blocked-1]
+        if domainsBlockedLimit:
+            # Join the domains into a comma-separated string
+            domainList = ', '.join(domainsBlockedLimit)
+        
+            print(colored('The following domains seem to be blocking KNOXSS and might be worth excluding for now:','yellow'),colored(domainList,'white'))
     except:
         pass
     
 # Handle the user pressing Ctrl-C and programatic interupts
 def handler(signal_received, frame):
     """
     This function is called if Ctrl-C is called by the user
@@ -136,27 +151,28 @@
                     print(colored('All unchecked URLs have been written to','cyan'),colored(todoFileName+'\n', 'white'))
                 except Exception as e:
                     print(colored('Error saving file ','cyan'),colored(todoFileName+'\n', 'white'),colored(':'+str(e),'red'))
         except:
             pass
         
         # If there were any domains that might be blocking KNOXSS, let the user know
-        showBlocked()
+        if args.skip_blocked > 0:
+            showBlocked()
         
         # Try to close the output file before ending
         try:
             outFile.close()
         except:
             pass
         quit()
             
 # Show the chosen options and config settings
 def showOptions():
 
-    global urlPassed, fileIsOpen, API_URL
+    global urlPassed, fileIsOpen, API_URL, timeAPIReset
             
     try:
         print(colored('Selected config and settings:', 'cyan'))
         
         print(colored('Config file path:', 'magenta'), configPath)
         print(colored('KNOXSS API Url:', 'magenta'), API_URL)
         print(colored('KNOXSS API Key:', 'magenta'), API_KEY)    
@@ -199,15 +215,25 @@
         print(colored('-afb: ' + str(args.advanced_filter_bypass), 'magenta'), 'Whether the Advanced Filter Bypass option is passed to KNOXSS API.')
         print(colored('-t: ' + str(args.timeout), 'magenta'), 'The number of seconds to wait for KNOXSS API to respond.')
         
         print(colored('-r: ' + str(args.retries), 'magenta'), 'The number of times to retry when having issues connecting to the KNOXSS API.')
         if args.retries > 0:
             print(colored('-ri: ' + str(args.retry_interval), 'magenta'), 'How many seconds to wait before retrying when having issues connecting to the KNOXSS API.')
             print(colored('-rb: ' + str(args.retry_backoff), 'magenta'), 'The backoff factor used when retrying when having issues connecting to the KNOXSS API.')
-            
+        
+        if args.skip_blocked > 0:
+            print(colored('-sb: ' + str(args.skip_blocked), 'magenta'), 'The number of 403 Forbidden responses from a target (for a given HTTP method + scheme + (sub)domain) before skipping.')
+        
+        if timeAPIReset is not None:
+            print(colored('KNOXSS API Limit Reset Time:', 'magenta'), str(timeAPIReset.strftime("%Y-%m-%d %H:%M")))  
+            if args.pause_until_reset:
+                print(colored('-pur: True', 'magenta'), 'If the API limit is reached, the program will pause and then continue again when it has been reset.')
+        else:
+            if args.pause_until_reset:
+                print(colored('-pur: True', 'magenta'), 'NOT POSSIBLE: Unfortunately the API reset time is currently unknown, so the program cannot be paused and continue when the API limit is reached.')
         print()
 
     except Exception as e:
         print(colored('ERROR showOptions: ' + str(e), 'red'))
 
 # If an API key wasn't supplied, or was invalid, then point the user to https://knoxss.me
 def needApiKey():
@@ -215,15 +241,15 @@
     try:
         print(colored('Haven\'t got an API key? Why not head over to https://knoxss.me and subscribe?\nDon\'t forget to generate and SAVE your API key before using it here! 🤘\n', 'green')) 
     except:
         print(colored('Haven\'t got an API key? Why not head over to https://knoxss.me and subscribe?\nDon\'t forget to generate and SAVE your API key before using it here!\n', 'green')) 
               
 def getConfig():
     # Try to get the values from the config file, otherwise use the defaults
-    global API_URL, API_KEY, DISCORD_WEBHOOK, configPath, HTTP_ADAPTER
+    global API_URL, API_KEY, DISCORD_WEBHOOK, configPath, HTTP_ADAPTER, apiResetPath
     try:
         
         # Put config in global location based on the OS.
         configPath = (
             Path(os.path.join(os.getenv('APPDATA', ''), 'knoxnl')) if os.name == 'nt'
             else Path(os.path.join(os.path.expanduser("~"), ".config", "knoxnl")) if os.name == 'posix'
             else Path(os.path.join(os.path.expanduser("~"), "Library", "Application Support", "knoxnl")) if os.name == 'darwin'
@@ -240,19 +266,23 @@
                 respect_retry_after_header=False
             )
             HTTP_ADAPTER = HTTPAdapter(max_retries=retry)
         except Exception as e:
             print(colored('ERROR getConfig 2: ' + str(e), 'red'))
         
         configPath.absolute
+        # Set config file path and apireset file path
         if configPath == '':
+            apiResetPath = '.apireset'
             configPath = 'config.yml'
         else:
+            apiResetPath = Path(configPath / '.apireset')
             configPath = Path(configPath / 'config.yml')
         config = yaml.safe_load(open(configPath))
+        
         try:
             API_URL = config.get('API_URL')
         except Exception as e:
             print(colored('Unable to read "API_URL" from config.yml; defaults set', 'red'))
             API_KEY = DEFAULT_API_URL
         try:
             API_KEY = config.get('API_KEY')
@@ -290,15 +320,15 @@
                 print(colored('Unable to read config.yml; using default API URL and passed API Key', 'cyan'))
             DISCORD_WEBHOOK = args.discord_webhook    
         except Exception as e:
             print(colored('ERROR getConfig 1: ' + str(e), 'red'))
             
 # Call the KNOXSS API
 def knoxssApi(targetUrl, headers, method, knoxssResponse):
-    global latestApiCalls, rateLimitExceeded, needToStop, dontDisplay, HTTP_ADAPTER, inputValues, needToRetry
+    global latestApiCalls, rateLimitExceeded, needToStop, dontDisplay, HTTP_ADAPTER, inputValues, needToRetry, requestCount
     try:
         apiHeaders = {'X-API-KEY' : API_KEY, 
                      'Content-Type' : 'application/x-www-form-urlencoded',
                      'User-Agent' : 'knoXnl tool by @xnl-h4ck3r'
                      }
         
         # Replace any & in the URL with encoded value so we can add other data using &
@@ -309,15 +339,15 @@
     
         # If processing a POST
         if method == 'POST' and args.http_method in ('POST','BOTH'):
             postData = ''
             
             # If the --post-data argument was passed, use those values
             if args.post_data != '':
-                postData = args.post_data.replace('&', '%26')
+                postData = args.post_data.replace('&', '%26').replace('+', '%2B')
                 # If the target has query string parameters, remove them
                 if '?' in targetUrl:
                     targetData = targetData.split('?')[0]
                     
             else: # post-data not passed
                 # If the target has parameters, i.e. ? then replace it with &post=, otherwise add &post= to the end
                 if '?' in targetUrl:
@@ -343,17 +373,24 @@
 
         # Make a request to the KNOXSS API
         try:
             tryAgain = True
             while tryAgain:
                 tryAgain = False
                 try:
-                    session = requests.Session()
-                    session.mount('https://', HTTP_ADAPTER)
+                    try:
+                        session = requests.Session()
+                        session.mount('https://', HTTP_ADAPTER)
+                    except Exception as e:
+                        print(colored(':( There was a problem setting up a network session: ' + str(e), 'red'))
+                        knoxssResponse.Error = 'Some kind of network error occurred before calling KNOXSS'
+                        return
+                    
                     # If a session timeout of 0 is passed, don't provide a timeout value.
+                    requestCount = requestCount + 1
                     if args.timeout == 0:
                         resp = session.post(
                             url=API_URL,
                             headers=apiHeaders,
                             data=data.encode('utf-8')
                         )
                     else:
@@ -394,15 +431,15 @@
                     
                     # Try to get the JSON response
                     try:
                         jsonResponse = json.loads(fullResponse)
                         if jsonResponse == '':
                             knoxssResponse.Error = fullResponse
                         else:
-                            knoxssResponse.Error = 'none'
+                            knoxssResponse.Error = 'No JSON response found'
                             
                         # If the error has "try again", and we haven't already tried before, set to True to try one more time
                         if 'expiration time reset' in fullResponse.lower():
                             if tryAgain:
                                 tryAgain = False
                             else:
                                 tryAgain = True
@@ -414,22 +451,25 @@
                                 knoxssResponse.Calls = 'Unknown'
                             knoxssResponse.Error = str(jsonResponse['Error'])
                             
                             # If service unavailable flag to stop
                             if knoxssResponse.Error == 'service unavailable':
                                 needToRetry = True
                             # If the API rate limit is exceeded, flag to stop
-                            elif knoxssResponse.Error == 'API rate limit exceeded.':
+                            elif latestApiCalls == '22/5000': #knoxssResponse.Error == 'API rate limit exceeded.':
                                 rateLimitExceeded = True
-                                needToStop = True
                                 knoxssResponse.Calls = 'API rate limit exceeded!'
+                                # Flag to stop if we aren't going to wait until the API limit is reset
+                                if not (timeAPIReset is not None and args.pause_until_reset):
+                                    needToStop = True
                             else: # remove the URL from the int input set
                                 inputValues.discard(targetUrl)
                                 
                             knoxssResponse.POSTData = str(jsonResponse['POST Data'])
+                            knoxssResponse.Timestamp = str(jsonResponse['Timestamp'])
                         
                     except Exception as e:
                         knoxssResponse.Calls = 'Unknown'
                         if fullResponse is None:
                             fullResponse = ''
                             knoxssResponse.Error = 'Empty response from API'
 
@@ -462,14 +502,27 @@
         except Exception as e:
             knoxssResponse.Error = 'FAIL'
             print(colored(':( There was a problem calling KNOXSS API: ' + str(e), 'red'))
             
     except Exception as e:
         print(colored('ERROR knoxss 1:  ' + str(e), 'red'))
 
+def checkForAlteredParams(url):
+    # Show a warning if it looks like the user has tampered with the parameter values before sending to knoxnl. Some indications of this are using FUZZ and also Gxss.
+    # Show a warning if any XSS payloads appear to be included in the URL already
+    try:
+        if '=FUZZ' in url or '=Gxss' in url:
+            print(colored('WARNING: It appears the URL may have been manually changed by yourself (or another tool) first. KNOXSS might not work as expected without the default values of parameters (some parameters might be value sensitive). Just pass original URLs to knoxnl.', 'yellow'))
+        regexCheck = r'<[A-Z]+|alert([^\}]*)|javascript:'
+        regexCheckCompiled = re.compile(regexCheck, re.IGNORECASE)
+        if regexCheckCompiled.search(url):
+            print(colored('WARNING: It appears the URL may already include some XSS payload. If that\'s correct, KNOXSS won\'t work as expected since it\'s not meant to receive XSS payloads, but to provide them.', 'yellow'))
+    except Exception as e:
+        print(colored('ERROR checkForAlteredParams 1:  ' + str(e), 'red'))
+        
 def processInput():
     global urlPassed, latestApiCalls, stopProgram, inputValues, todoFileName
     try:
         latestApiCalls = 'Unknown'
 
         # if the Burp Piper Extension argument was passed, assume the input is passed by stdin 
         if args.burp_piper:
@@ -531,14 +584,17 @@
         inputArg = args.input
         if urlPassed:
             print(colored('Calling KNOXSS API...\n', 'cyan'))
             # Check if input has scheme. If not, then add https://
             if '://' not in inputArg:
                 print(colored('WARNING: Input "'+inputArg+'" should include a scheme. Using https by default...', 'yellow'))
                 inputArg = 'https://'+inputArg
+            # Check for non default values of parameters
+            checkForAlteredParams(inputArg)
+
             processUrl(inputArg)
         else: # It's a file of URLs
             try:
                 # Open file and put all values in input set
                 with open(inputArg, 'r') as inputFile:
                     lines = inputFile.readlines()          
                 for line in lines:
@@ -574,100 +630,162 @@
             result = requests.post(DISCORD_WEBHOOK, json=data)
             if 300 <= result.status_code < 200:
                 print(colored('WARNING: Failed to send notification to Discord - ' + result.json(), 'yellow'))
         except Exception as e:
             print(colored('WARNING: Failed to send notification to Discord - ' + str(e), 'yellow'))
     except Exception as e:
         print(colored('ERROR discordNotify 1: ' + str(e), 'red'))
+
+def getAPILimitReset():
+    global apiResetPath, timeAPIReset
+    try:
+        # If the .apireset file exists then get the API reset time
+        if os.path.exists(apiResetPath):
+            # Read the timestamp from the file
+            with open(apiResetPath, 'r') as file:
+                timeAPIReset = datetime.strptime(file.read().strip(), '%Y-%m-%d %H:%M')
+    
+        # If the timestamp is more than 24 hours ago, then delete the file and set the timeAPIReset back to None
+        if timeAPIReset is not None and (datetime.now() - timeAPIReset) > timedelta(hours=24):
+            timeAPIReset = None
+            # If the .apireset file already exists then delete it
+            if os.path.exists(apiResetPath):
+                os.remove(apiResetPath)
+
+    except Exception as e:
+        print(colored('ERROR getAPILimitReset 1: ' + str(e), 'red'))
+        
+def setAPILimitReset(timestamp):
+    global apiResetPath, latestApiCalls, timeAPIReset
+    try:
+        # Convert the timestamp to the local timezone and add 24 hours and 5 minutes
+        timestamp = datetime.strptime(timestamp, '%a, %d %b %Y %H:%M:%S %z')
+        localTimezone = tz.tzlocal()
+        localTimestamp = timestamp.astimezone(localTimezone)
+        timeAPIReset = localTimestamp + timedelta(hours=24, minutes=5)
+
+        # If the .apireset file already exists then delete it
+        if os.path.exists(apiResetPath):
+            os.remove(apiResetPath)
+            
+        # Write the new API limit reset time to the .apireset file, and set the global variable
+        with open(apiResetPath, 'w') as file:
+            file.write(timeAPIReset.strftime('%Y-%m-%d %H:%M'))
+        
+    except Exception as e:
+        print(colored('ERROR setAPILimitReset 1: ' + str(e), 'red'))
         
 def processOutput(target, method, knoxssResponse):
-    global latestApiCalls, successCount, outFile, currentCount, rateLimitExceeded, urlPassed, needToStop, dontDisplay, blockedDomains, needToRetry
+    global latestApiCalls, successCount, outFile, currentCount, rateLimitExceeded, urlPassed, needToStop, dontDisplay, blockedDomains, needToRetry, forbiddenResponseCount, errorCount, safeCount, requestCount, skipCount
     try:
         if knoxssResponse.Error != 'FAIL':
                 
             if knoxssResponse.Error != 'none':
                 if not args.success_only:
                     knoxssResponseError = knoxssResponse.Error
                     # If there is a 403, it maybe because the users IP is blocked on the KNOXSS firewall
                     if knoxssResponse.Code == "403":
                        knoxssResponseError = '403 Forbidden - Check http://knoxss.me manually and if you are blocked, contact Twitter/X @KN0X55 or brutelogic@null.net'
                        needToStop = True
                     # If there is "InvalidChunkLength" in the error returned, it means the KNOXSS API returned an empty response
-                    if 'InvalidChunkLength' in knoxssResponseError:
+                    elif 'InvalidChunkLength' in knoxssResponseError:
                         knoxssResponseError = 'The API Timed Out'
                         needToRetry = True
-                    # If the error has "can\'t test it (forbidden)" it means the target is blocking KNOXSS IP address
-                    if 'can\'t test it (forbidden)' in knoxssResponseError:
-                        knoxssResponseError = 'Target is blocking KNOXSS IP'
-                        try:
-                            parsedTarget = urlparse(target)
-                            domain = parsedTarget.scheme + '://' + parsedTarget.netloc
-                            blockedDomains.add(domain)
-                        except:
-                            pass
-                    
+                    # If the error has "can\'t test it (forbidden)" it means the a 403 was returned by the target
+                    elif 'can\'t test it (forbidden)' in knoxssResponseError:
+                        knoxssResponseError = 'Target returned a "403 Forbidden". There could be WAF in place.'
+                        # If requested to skip blocked domains after a limit, then save them
+                        if args.skip_blocked > 0:
+                            try:
+                                parsedTarget = urlparse(target)
+                                domain = '(' + method + ') ' + str(parsedTarget.scheme + '://' + parsedTarget.netloc)
+                                pauseEvent.set()
+                                blockedDomains[domain] = blockedDomains.get(domain, 0) + 1
+                                pauseEvent.clear()
+                            except:
+                                pass
+                        
                     # If method is POST, remove the query string from the target and show the post data in [ ] 
                     if method == 'POST':
                         try:
                             querystring = target.split('?')[1]
                         except:
                             querystring = ''
                         target = target.split('?')[0]
                         if args.post_data:
                             target = target + ' ['+args.post_data+']'
                         else:
                             if querystring != '':
                                 target = target + ' [' + querystring + ']'                            
                     
                     if not dontDisplay:        
-                        xssText = '[ ERR! ] - (' + method + ')  ' + target + '  KNOXSS ERR: ' + knoxssResponseError
-                        if urlPassed or rateLimitExceeded:
+                        xssText = '[ ERR! ] - (' + method + ') ' + target + '  KNOXSS ERR: ' + knoxssResponseError
+                        errorCount = errorCount + 1
+                        if urlPassed:
                             print(colored(xssText, 'red'))
                         else:
                             print(colored(xssText, 'red'), colored('['+latestApiCalls+']','white'))
                         if args.output_all and fileIsOpen:
                             outFile.write(xssText + '\n')
             else:
+                # If it is a new reset time then replace the .apireset file
+                if knoxssResponse.Timestamp != '' and latestApiCalls.startswith('1/'):
+                    setAPILimitReset(knoxssResponse.Timestamp)
+                    
                 if knoxssResponse.XSS == 'true':
-                    xssText = '[ XSS! ] - (' + method + ')  ' + knoxssResponse.PoC
+                    xssText = '[ XSS! ] - (' + method + ') ' + knoxssResponse.PoC
                     if urlPassed:
                         print(colored(xssText, 'green'))
                     else:
                         print(colored(xssText, 'green'), colored('['+latestApiCalls+']','white'))
                     successCount = successCount + 1
                     # Send a notification to discord if a webook was provided
                     if DISCORD_WEBHOOK != '':
                         discordNotify(target,knoxssResponse.PoC)
                     # Write the successful XSS details to file
                     if fileIsOpen:
                         outFile.write(xssText + '\n')
                 else:
                     if not args.success_only:
-                        xssText = '[ SAFE ] - (' + method + ')  ' + target
+                        xssText = '[ SAFE ] - (' + method + ') ' + target
+                        safeCount = safeCount + 1
                         if urlPassed:
                             print(colored(xssText, 'yellow'))
                         else:
                             print(colored(xssText, 'yellow'), colored('['+latestApiCalls+']','white'))
                         if args.output_all and fileIsOpen:
                             outFile.write(xssText + '\n') 
                     
     except Exception as e:
         print(colored('ERROR showOutput 1: ' + str(e), 'red'))
 
 # Process one URL        
 def processUrl(target):
     
-    global stopProgram, latestApiCalls, urlPassed, needToStop, needToRetry, retryAttempt
+    global stopProgram, latestApiCalls, urlPassed, needToStop, needToRetry, retryAttempt, rateLimitExceeded, timeAPIReset, skipCount, apiResetPath
     try:    
         # If the event is set, pause for a while until its unset again
         while pauseEvent.is_set() and not stopProgram and not needToStop:
             time.sleep(1)
-            
+        
         if not stopProgram and not needToStop:
-                
+            
+            # If the API Limit was exceeded, and we want to wait until the limit is reset pause all processes until that time
+            if rateLimitExceeded and timeAPIReset is not None and args.pause_until_reset:
+                # Set the event to pause all processes
+                pauseEvent.set()
+                print(colored(f'WAITING UNTIL {str(timeAPIReset.strftime("%Y-%m-%d %H:%M"))} WHEN THEN API LIMIT HAS BEEN RESET...','yellow'))
+                time_difference = (timeAPIReset - datetime.now()).total_seconds()
+                timeAPIReset = None
+                os.remove(apiResetPath)
+                time.sleep(time_difference)
+                print(colored('API LIMIT HAS BEEN RESET. RESUMING...','yellow'))
+                # Reset the event for to unpause all processes
+                pauseEvent.clear()
+                    
             # If we need to try again because of an KNOXSS error, then delay
             if needToRetry and args.retries > 0:
                 if retryAttempt < args.retries:
                     # Set the event to pause all processes
                     pauseEvent.set()
                     needToRetry = False
                     if retryAttempt == 0:
@@ -689,46 +807,84 @@
             # Check if target has scheme. If not, then add https://
             if '://' not in target:
                 print(colored('WARNING: Input "'+target+'" should include a scheme. Using https by default...', 'yellow'))
                 target = 'https://'+target
             
             # If the domain has already been flagged as blocked, then skip it and remove from the input values so not written to the .todo file
             parsedTarget = urlparse(target)
-            domain = parsedTarget.scheme + '://' + parsedTarget.netloc
-            if domain in blockedDomains:
-                print(colored('[ SKIP ] - ' + domain + ' has already been flagged as blocked, so skipping ' + target, 'yellow', attrs=['dark']))
-                inputValues.discard(target)
-            else:
-                headers = args.headers.strip()
-                knoxssResponse=knoxss()        
-
-                if args.http_method in ('GET','BOTH'): 
-                    method = 'GET'
+ 
+            headers = args.headers.strip()
+            knoxssResponse=knoxss()        
+
+            if args.http_method in ('GET','BOTH'): 
+                method = 'GET'
+                domain = '(' + method + ') ' + str(parsedTarget.scheme + '://' + parsedTarget.netloc)
+                
+                # If skipping blocked domains was requested, check if the domain is in blockedDomains, if not, add it with count 0
+                if args.skip_blocked > 0:
+                    while pauseEvent.is_set():
+                        time.sleep(1)
+                    pauseEvent.set()
+                    if domain not in blockedDomains:
+                        blockedDomains[domain] = 0
+                    pauseEvent.clear()
+                
+                # If skipping blocked domains was requested and the domain has been blocked more than the requested number of times, then skip, otherwise process  
+                if args.skip_blocked > 0 and blockedDomains[domain] > args.skip_blocked-1:
+                    print(colored('[ SKIP ] - ' + domain + ' has already been flagged as blocked, so skipping ' + target, 'yellow', attrs=['dark']))
+                    skipCount = skipCount + 1
+                    inputValues.discard(target)
+                else:
                     knoxssApi(target, headers, method, knoxssResponse)
                     processOutput(target, method, knoxssResponse)
-            
-                if args.http_method in ('POST','BOTH'): 
-                    method = 'POST'
+        
+            if args.http_method in ('POST','BOTH'): 
+                method = 'POST'
+                domain = '(' + method + ') ' + str(parsedTarget.scheme + '://' + parsedTarget.netloc)
+                
+                # If skipping blocked domains was requested, check if the domain is in blockedDomains, if not, add it with count 0
+                if args.skip_blocked > 0:
+                    while pauseEvent.is_set():
+                        time.sleep(1)
+                    pauseEvent.set()
+                    if domain not in blockedDomains:
+                        blockedDomains[domain] = 0
+                    pauseEvent.clear()
+                
+                # If skipping blocked domains was requested and the domain has been blocked more than the requested number of times, then skip, otherwise process  
+                if args.skip_blocked > 0 and blockedDomains[domain] > args.skip_blocked-1:
+                    print(colored('[ SKIP ] - ' + domain + ' has already been flagged as blocked, so skipping ' + target, 'yellow', attrs=['dark']))
+                    skipCount = skipCount + 1
+                    inputValues.discard(target)
+                else:
                     knoxssApi(target, headers, method, knoxssResponse)
                     processOutput(target, method, knoxssResponse)
 
     except Exception as e:
         pauseEvent.clear()
         print(colored('ERROR processUrl 1: ' + str(e), 'red'))   
 
 # Validate the -p argument 
 def processes_type(x):
     x = int(x) 
     if x < 1 or x > 5:
         raise argparse.ArgumentTypeError('The number of processes must be between 1 and 5')     
     return x
-                                
+
+def updateProgram():
+    try:
+        # Execute pip install --upgrade knoxnl
+        subprocess.run(['pip', 'install', '--upgrade', 'knoxnl'], check=True)
+        print(colored(f'knoxnl successfully updated {__version__} -> {latestVersion} (latest) 🤘', 'green'))
+    except subprocess.CalledProcessError as e:
+        print(colored(f'Unable to update knoxnl to version {latestVersion}: {str(e)}', 'red'))
+                                       
 # Run knoXnl
 def main():
-    global args, latestApiCalls, urlPassed, successCount, fileIsOpen, outFile, needToStop, todoFileName, blockedDomains
+    global args, latestApiCalls, urlPassed, successCount, fileIsOpen, outFile, needToStop, todoFileName, blockedDomains, latestVersion, safeCount, errorCount, requestCount, skipCount
     
     # Tell Python to run the handler() function when SIGINT is received
     signal(SIGINT, handler)
 
     # Parse command line arguments
     parser = argparse.ArgumentParser(
         description='knoXnl - by @Xnl-h4ck3r: A wrapper around the KNOXSS API by Brute Logic (requires an API key)'    
@@ -847,37 +1003,85 @@
     parser.add_argument(
         '-rb',
         '--retry-backoff',
         help='The backoff factor used when retrying when having issues connecting to the KNOXSS API (default: '+str(DEFAULT_RETRY_BACKOFF_FACTOR)+')',
         default=DEFAULT_RETRY_BACKOFF_FACTOR,
         type=float,
     )
+    parser.add_argument(
+        '-pur',
+        '--pause-until-reset',
+        action='store_true',
+        help='If the API Limit reset time is known and the API limit is reached, wait the required time until the limit is reset and continue again. The reset time is only known if knoxnl has run for request number 1 previously. The API rate limit is reset 24 hours after request 1.',
+    )
+    parser.add_argument(
+        '-sb',
+        '--skip-blocked',
+        help='The number of 403 Forbidden responses from a target (for a given HTTP method + scheme + (sub)domain) before skipping. This is useful if you know the target has a WAF. The default is zero, which means no blocking is done.',
+        default=0,
+        type=int,
+    )
+    parser.add_argument(
+        '-up',
+        '--update',
+        action='store_true',
+        help='Update knoxnl to the latest version.',
+    )
     parser.add_argument('-v', '--verbose', action='store_true', help="Verbose output")
     parser.add_argument('--version', action='store_true', help="Show version number")
     args = parser.parse_args()
 
     # If --version was passed, display version and exit
     if args.version:
         print(colored('knoxnl - v' + __version__,'cyan'))
         sys.exit()
-        
+
+    # Get the latest version
+    try:
+        resp = requests.get('https://raw.githubusercontent.com/xnl-h4ck3r/knoxnl/main/knoxnl/__init__.py',timeout=3)
+        latestVersion = resp.text.split('=')[1].replace('"','')
+    except:
+        pass
+                        
+    showBanner()
+
+    # If --update was passed, update to the latest version
+    if args.update:
+        try:
+            if latestVersion == '':
+                print(colored('Unable to check the latest version. Check your internet connection.', 'red'))
+            elif __version__ != latestVersion:
+                updateProgram()
+                sys.exit()
+        except Exception as e:
+            print(colored(f'ERROR: Unable to update - {str(e)}','red'))
+             
     # If no input was given, raise an error
     if sys.stdin.isatty():
         if args.input is None:
             print(colored('You need to provide an input with -i argument or through <stdin>.', 'red'))
             sys.exit()
             
-    showBanner()
-
     # Get the config settings from the config.yml file
     getConfig()
+    
+    # Get the API reset time from the .apireset file
+    getAPILimitReset()
 
     # If -o (--output) argument was passed then open the output file
     if args.output != "":
         try:
+            # If the filename has any "/" in it, remove the contents after the last one to just get the path and create the directories if necessary
+            try:
+                output_path = os.path.abspath(os.path.expanduser(args.output))
+                output_dir = os.path.dirname(output_path)
+                if not os.path.exists(output_dir):
+                    os.makedirs(output_dir)
+            except Exception as e:
+                pass
             # If argument -ow was passed and the file exists, overwrite it, otherwise append to it
             if args.output_overwrite:
                 outFile = open(os.path.expanduser(args.output), "w")
             else:
                 outFile = open(os.path.expanduser(args.output), "a")
             fileIsOpen = True
         except Exception as e:
@@ -898,17 +1102,24 @@
                 with open(todoFileName, 'w') as file:
                     for inp in inputValues:
                         file.write(inp+'\n')
                 print(colored('Had to stop due to errors. All unchecked URLs have been written to','cyan'),colored(todoFileName+'\n', 'white'))
             except Exception as e:
                 print(colored('Was unable to write .todo file: '+str(e),'red'))
         
-        showBlocked()
-            
-        # Report if any successful XSS was found this time
+        if args.skip_blocked > 0:
+            showBlocked()
+        
+        # Report number of Safe, Error and Skipped results
+        if args.skip_blocked > 0:
+            print(colored(f'Requests made to KNOXSS API: {str(requestCount)} (XSS!: {str(successCount)}, SAFE: {str(safeCount)}, ERR!: {str(errorCount)}, SKIP: {str(skipCount)})','cyan'))
+        else:
+             print(colored(f'Requests made to KNOXSS API: {str(requestCount)} (XSS!: {str(successCount)}, SAFE: {str(safeCount)}, ERR!: {str(errorCount)})','cyan'))
+             
+        # Report if any successful XSS was found this time. 
         # If the console can't display 🤘 then an error will be raised to try without
         try:
             if successCount > 0:
                 print(colored('🤘 '+str(successCount)+' successful XSS found! 🤘\n','green'))
             else:
                 print(colored('No successful XSS found... better luck next time! 🤘\n','cyan'))
         except:
```

### Comparing `knoxnl-4.2/knoxnl.egg-info/PKG-INFO` & `knoxnl-4.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-Metadata-Version: 2.1
-Name: knoxnl
-Version: 4.2
-Summary: A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)
-Home-page: https://github.com/xnl-h4ck3r/knoxnl
-Author: @xnl-h4ck3r
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argparse
-Requires-Dist: requests
-Requires-Dist: termcolor
-Requires-Dist: pyaml
-Requires-Dist: urlparse3
-
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.2
+## About - v4.3
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
+**DISCLAIMER: We are not responsible for any use, and especially misuse, of this tool or the KNOXSS API**
+
 ## Installation
 
 **NOTE: If you already have a `config.yml` file, it will not be overwritten. The file `config.yml.NEW` will be created in the same directory. If you need the new config, remove `config.yml` and rename `config.yml.NEW` back to `config.yml`.**
 
 `knoxnl` supports **Python 3**.
 
 Install `knoxnl` in default (global) python environment.
@@ -37,48 +25,57 @@
 ```bash
 pip install git+https://github.com/xnl-h4ck3r/knoxnl.git -v
 ```
 
 You can upgrade with
 
 ```bash
+knoxnl -up
+```
+
+OR
+
+```bash
 pip install --upgrade knoxnl
 ```
 
 ### pipx
 
 Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
 
 ```bash
 pipx install git+https://github.com/xnl-h4ck3r/knoxnl.git
 ```
 
 ## Usage
 
-| Arg  | Long Arg                 | Description                                                                                                                                                                                                                                                |
-| ---- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| -i   | --input                  | Input to send to KNOXSS API: a single URL, or file of URLs. **NOTE: If you pass a URL, put it in quotes otherwise the shell can interpret `&` characters as instruction to run a background task.**                                                        |
-| -o   | --output                 | The file to save the successful XSS and payloads to. If the file already exist it will just be appended to unless option `-ow` is passed.                                                                                                                  |
-| -ow  | --output-overwrite       | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                                    |
-| -oa  | --output-all             | Write all results to the output file, not just successful one's.                                                                                                                                                                                           |
-| -X   | --http-method            | Which HTTP method to use, values `GET`, `POST` or `BOTH` (default: `GET`). If `BOTH` is chosen, then a `GET` call will be made, followed by a `POST`.                                                                                                      |
-| -pd  | --post-data              | If a POST request is made, this is the POST data passed. It must be in the format `'param1=value&param2=value&param3=value'`. If this isn't passed and query string parameters are used, then these will be used as POST data if POST Method is requested. |
-| -H   | --headers                | Add custom headers to pass with HTTP requests. Pass in the format `'Header1:value1;\|Header2:value2'` (e.g. separate different headers with a pipe \| character).                                                                                          |
-| -A   | --api-key                | The KNOXSS API Key to use. This will be used instead of the value in `config.yml`                                                                                                                                                                          |
-| -afb | --advanced-filter-bypass | If the advanced filter bypass should be used on the KNOXSS API.                                                                                                                                                                                            |
-| -s   | --success-only           | Only show successful XSS payloads in the CLI output.                                                                                                                                                                                                       |
-| -p   | --processes              | Basic multithreading is done when getting requests for a file of URLs. This argument determines the number of processes (one per URL to check) are run per minute (default: 3). This is due to the rate limit of the KNOXSS API.                           |
-| -t   | --timeout                | How many seconds to wait for the KNOXSS API to respond before giving up (default: 600). If set to 0, then timeout will be used.                                                                                                                            |
-| -bp  | --burp-piper             | Use if **knoxnl** is called from the Burp Piper extension, so that a request in **Burp Suite** proxy can be tested. See the [Using in Burp Suite Proxy](#using-in-burp-suite-proxy) section below.                                                         |
-| -r   | --retries                | The number of times to retry when having issues connecting to the KNOXSS API (default: 3)                                                                                                                                                                  |
-| -ri  | --retry-interval         | How many seconds to wait before retrying when having issues connecting to the KNOXSS API (default: 30)                                                                                                                                                     |
-| -rb  | --retry-backoff          | The backoff factor used when retrying when having issues connecting to the KNOXSS API (default: 1.5). For example, with defaults, first time will wait for 30 seconds, 2nd time will be 45 (30 x 1.5) seconds, etc.                                        |
-| -v   | --verbose                | Verbose output                                                                                                                                                                                                                                             |
-|      | --version                | Show current version number.                                                                                                                                                                                                                               |
-| -h   | --help                   | show the help message and exit                                                                                                                                                                                                                             |
+| Arg  | Long Arg                 | Description                                                                                                                                                                                                                                                                  |
+| ---- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| -i   | --input                  | Input to send to KNOXSS API: a single URL, or file of URLs. **NOTE: If you pass a URL, put it in quotes otherwise the shell can interpret `&` characters as instruction to run a background task.**                                                                          |
+| -o   | --output                 | The file to save the successful XSS and payloads to. If the file already exist it will just be appended to unless option `-ow` is passed. If the full path doesn't exist, then any necessary directories will be created.                                                    |
+| -ow  | --output-overwrite       | If the output file already exists, it will be overwritten instead of being appended to.                                                                                                                                                                                      |
+| -oa  | --output-all             | Write all results to the output file, not just successful one's.                                                                                                                                                                                                             |
+| -X   | --http-method            | Which HTTP method to use, values `GET`, `POST` or `BOTH` (default: `GET`). If `BOTH` is chosen, then a `GET` call will be made, followed by a `POST`.                                                                                                                        |
+| -pd  | --post-data              | If a POST request is made, this is the POST data passed. It must be in the format `'param1=value&param2=value&param3=value'`. If this isn't passed and query string parameters are used, then these will be used as POST data if POST Method is requested.                   |
+| -H   | --headers                | Add custom headers to pass with HTTP requests. Pass in the format `'Header1:value1;\|Header2:value2'` (e.g. separate different headers with a pipe \| character).                                                                                                            |
+| -A   | --api-key                | The KNOXSS API Key to use. This will be used instead of the value in `config.yml`                                                                                                                                                                                            |
+| -afb | --advanced-filter-bypass | If the advanced filter bypass should be used on the KNOXSS API.                                                                                                                                                                                                              |
+| -s   | --success-only           | Only show successful XSS payloads in the CLI output.                                                                                                                                                                                                                         |
+| -p   | --processes              | Basic multithreading is done when getting requests for a file of URLs. This argument determines the number of processes (one per URL to check) are run per minute (default: 3). This is due to the rate limit of the KNOXSS API.                                             |
+| -t   | --timeout                | How many seconds to wait for the KNOXSS API to respond before giving up (default: 600). If set to 0, then timeout will be used.                                                                                                                                              |
+| -bp  | --burp-piper             | Use if **knoxnl** is called from the Burp Piper extension, so that a request in **Burp Suite** proxy can be tested. See the [Using in Burp Suite Proxy](#using-in-burp-suite-proxy) section below.                                                                           |
+| -r   | --retries                | The number of times to retry when having issues connecting to the KNOXSS API (default: 3)                                                                                                                                                                                    |
+| -ri  | --retry-interval         | How many seconds to wait before retrying when having issues connecting to the KNOXSS API (default: 30)                                                                                                                                                                       |
+| -rb  | --retry-backoff          | The backoff factor used when retrying when having issues connecting to the KNOXSS API (default: 1.5). For example, with defaults, first time will wait for 30 seconds, 2nd time will be 45 (30 x 1.5) seconds, etc.                                                          |
+| -pur | --pause-until-reset      | If the API Limit reset time is known and the API limit is reached, wait the required time until the limit is reset and continue again. The reset time is only known if knoxnl has run for request number 1 previously. The API rate limit is reset 24 hours after request 1. |
+| -sb  | --skip-blocked           | The number of 403 Forbidden responses from a target (for a given HTTP method + scheme + (sub)domain) before skipping. This is useful if you know the target has a WAF. The default is zero, which means no blocking is done.                                                 |
+| -up  | --update                 | Update knoxnl to the latest version.                                                                                                                                                                                                                                         |
+| -v   | --verbose                | Verbose output                                                                                                                                                                                                                                                               |
+|      | --version                | Show current version number.                                                                                                                                                                                                                                                 |
+| -h   | --help                   | show the help message and exit                                                                                                                                                                                                                                               |
 
 ## config.yml
 
 The `config.yml` file (in the global location based on the OS, e.g. `~/.config/knoxnl/config.yml`) has the keys which can be updated to suit your needs:
 
 - `API_URL` - This can be set to the KNOXSS API endpoint, if and when it is changed
 - `API_KEY` - Your KNOXSS API key that you will have generated on https://knoxss.me/
@@ -86,21 +83,21 @@
 
 ## Important Notes from KNOXSS API Guidelines
 
 - Unlike other APIs that just retrieve data from a database, KNOXSS API returns the results like the web interface, actually performing a comprehensive vulnerability scan for XSS. Since scan results are not stored by our system, they need to be generated on the fly taking several JavaScript-evaluated live tests to return them. So it's natural the data returned takes much more time to get delivered since there's a long process involved at server side.
 - The API standard rate limit is 5000 requests over a 24 hours period. That means an average of **2.3 requests per minute** so please try to keep this pace **to not overload the system**. Due to this rate limit, if the input is a file or URLs, then only a batch (determined by argument `-p`/`--processes`) will be run per minute.
 - **Generating or Regenerating your API Key** - The API key is in your profile. If you have never generated it you need to hit the button at least once to generate it and save. Any time you need a new API key for security reasons, you can simply hit the button and regenerate it.
 - **Flash Mode Mark - [XSS]** - Provide the `[XSS]` mark in any place of the target's data values to enable Flash Mode which enables KNOXSS to perform a single quick XSS Polyglot based test.
-- At the time of writing this, the daily limit of KNOXSS API calls is **5000**. If you are testing a large file of URLs,it is advisable that you use the `-o` / `--output` option to specify a file where output will be written. If you do reach the API limit with a 24 hour period, this is reset at about 17:00 GMT.
-- If you pass an input file and the API limit is reached, or the Service is Unavailable, part way through the input, all unchecked URLs will be output to an file in the same location, and with the same name as the input file, but with a `.YYYYMMDD_HHMMSS.todo` suffix. You can then rename this file and use this as input at another time.
-- By default, only successful results are written to the output file.
-- Passing argument `-oa` / `--output-all` will write **ALL** results to the output file, not just successful one's.
 
-## Important Notes fof knoxnl
+## Important Notes for knoxnl
 
+- At the time of writing this, the daily limit of KNOXSS API calls is **5000**. If you are testing a large file of URLs, it is advisable that you use the `-o` / `--output` option to specify a file where output will be written. If you do reach the API limit, it resets 24 hours after the first API call was made. If you are processing a file of URLs, you can use the `-pur`/`--pause-until-reset` to wait until the reset happens and then continue (this is only possible if the first request was run by `knoxnl` so it could save the response timestamp).
+- If you pass an input file and the API limit is reached, or the Service is Unavailable, part way through the input, all unchecked URLs will be output to an file in the same location, and with the same name as the input file, but with a `.YYYYMMDD_HHMMSS.todo` suffix. You can then rename this file and use this as input at another time. The `.todo` file will be created in the current directory unless a path is specified in the `-o`/`--output` directory, and then the `.todo` file will be created in the same directory.
+- By default, only successful results are written to the output file.
+- Passing argument `-oa` / `--output-all` will write **ALL** results to the output file, not just successful one's.
 - The KNOXSS API has a rate limit of no more than 5 URLs processed per minute. If the rate limit is exceeded then you might end up getting blocked by their WAF, and you will not get the results you want. This rate limit is taken into account when passing a file of URLs as input. However, if you keep running for a single URL more than this per minute you wil run into problems. Please respect the rules of their API.
 - The KNOXSS only deals with POST requests with basic post data in the format `'param1=value&param2=value&param3=value'`.
 - If the `-pd`/`--post-data` argument is not passed and a POST request is made, it will use the query string from the URL as post data if it has one.
 - If a file is passed as input and POST method is required, then the post data parameters need to be provided as a query string for the URL in the file, e.g. `https://example.com?postParam1=value&postParam2-value`. If you use the `-pd`/`--post-data` with an input file then ALL URLs will use that post data.
 - These are required based on the way the KNOXSS API works.
 
 ## Examples
```

### Comparing `knoxnl-4.2/setup.py` & `knoxnl-4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description="A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)",
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author="@xnl-h4ck3r",
     url="https://github.com/xnl-h4ck3r/knoxnl",
     py_modules=["knoxnl"],
     zip_safe=False,
-    install_requires=["argparse","requests","termcolor","pyaml","urlparse3"],
+    install_requires=["argparse","requests","termcolor","pyaml","urlparse3","python-dateutil"],
     entry_points={
         'console_scripts': [
             'knoxnl = knoxnl.knoxnl:main',
         ],
     },
 )
```

