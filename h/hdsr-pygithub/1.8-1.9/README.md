# Comparing `tmp/hdsr_pygithub-1.8.tar.gz` & `tmp/hdsr_pygithub-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_pygithub-1.8.tar", last modified: Wed Mar  1 09:48:23 2023, max compression
+gzip compressed data, was "dist\hdsr_pygithub-1.9.tar", last modified: Tue Mar  7 14:10:41 2023, max compression
```

## Comparing `hdsr_pygithub-1.8.tar` & `hdsr_pygithub-1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 09:48:21.000000 hdsr_pygithub-1.8/
--rw-rw-rw-   0        0        0     1086 2021-11-10 10:47:16.000000 hdsr_pygithub-1.8/LICENSE
--rw-rw-rw-   0        0        0     9534 2023-03-01 09:48:22.000000 hdsr_pygithub-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8682 2023-03-01 09:47:10.000000 hdsr_pygithub-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 09:48:21.000000 hdsr_pygithub-1.8/hdsr_pygithub/
--rw-rw-rw-   0        0        0      142 2022-01-05 15:55:52.000000 hdsr_pygithub-1.8/hdsr_pygithub/__init__.py
--rw-rw-rw-   0        0        0      918 2022-06-22 09:29:12.000000 hdsr_pygithub-1.8/hdsr_pygithub/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-01 09:48:21.000000 hdsr_pygithub-1.8/hdsr_pygithub/downloader/
--rw-rw-rw-   0        0        0        0 2022-01-05 15:55:52.000000 hdsr_pygithub-1.8/hdsr_pygithub/downloader/__init__.py
--rw-rw-rw-   0        0        0    14819 2023-03-01 09:47:10.000000 hdsr_pygithub-1.8/hdsr_pygithub/downloader/base.py
--rw-rw-rw-   0        0        0     6474 2022-06-22 09:29:12.000000 hdsr_pygithub-1.8/hdsr_pygithub/downloader/dir.py
--rw-rw-rw-   0        0        0     2561 2022-06-22 09:29:12.000000 hdsr_pygithub-1.8/hdsr_pygithub/downloader/file.py
--rw-rw-rw-   0        0        0      555 2022-01-05 15:55:52.000000 hdsr_pygithub-1.8/hdsr_pygithub/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-01 09:48:21.000000 hdsr_pygithub-1.8/hdsr_pygithub/tests/
--rw-rw-rw-   0        0        0        0 2021-11-11 12:35:47.000000 hdsr_pygithub-1.8/hdsr_pygithub/tests/__init__.py
--rw-rw-rw-   0        0        0     8237 2023-03-01 09:47:10.000000 hdsr_pygithub-1.8/hdsr_pygithub/tests/test_dir_downloader.py
--rw-rw-rw-   0        0        0     3850 2023-03-01 09:47:10.000000 hdsr_pygithub-1.8/hdsr_pygithub/tests/test_file_downloader.py
--rw-rw-rw-   0        0        0     1382 2023-03-01 09:47:10.000000 hdsr_pygithub-1.8/hdsr_pygithub/tests/test_general.py
--rw-rw-rw-   0        0        0      603 2022-07-14 12:17:42.000000 hdsr_pygithub-1.8/hdsr_pygithub/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-01 09:48:21.000000 hdsr_pygithub-1.8/hdsr_pygithub.egg-info/
--rw-rw-rw-   0        0        0     9534 2023-03-01 09:48:19.000000 hdsr_pygithub-1.8/hdsr_pygithub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-03-01 09:48:19.000000 hdsr_pygithub-1.8/hdsr_pygithub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 09:48:19.000000 hdsr_pygithub-1.8/hdsr_pygithub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-01 09:48:19.000000 hdsr_pygithub-1.8/hdsr_pygithub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       66 2023-03-01 09:48:19.000000 hdsr_pygithub-1.8/hdsr_pygithub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-01 09:48:19.000000 hdsr_pygithub-1.8/hdsr_pygithub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2021-11-11 09:44:52.000000 hdsr_pygithub-1.8/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-03-01 09:48:22.000000 hdsr_pygithub-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-03-01 09:47:10.000000 hdsr_pygithub-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-07 14:10:40.000000 hdsr_pygithub-1.9/
+-rw-rw-rw-   0        0        0     1086 2021-11-10 10:47:16.000000 hdsr_pygithub-1.9/LICENSE
+-rw-rw-rw-   0        0        0     9761 2023-03-07 14:10:41.000000 hdsr_pygithub-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8909 2023-03-07 14:09:40.000000 hdsr_pygithub-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-07 14:10:40.000000 hdsr_pygithub-1.9/hdsr_pygithub/
+-rw-rw-rw-   0        0        0      142 2022-01-05 15:55:52.000000 hdsr_pygithub-1.9/hdsr_pygithub/__init__.py
+-rw-rw-rw-   0        0        0      398 2023-03-07 11:39:38.000000 hdsr_pygithub-1.9/hdsr_pygithub/constants.py
+drwxrwxrwx   0        0        0        0 2023-03-07 14:10:40.000000 hdsr_pygithub-1.9/hdsr_pygithub/downloader/
+-rw-rw-rw-   0        0        0        0 2022-01-05 15:55:52.000000 hdsr_pygithub-1.9/hdsr_pygithub/downloader/__init__.py
+-rw-rw-rw-   0        0        0    15973 2023-03-07 11:56:22.000000 hdsr_pygithub-1.9/hdsr_pygithub/downloader/base.py
+-rw-rw-rw-   0        0        0     6474 2022-06-22 09:29:12.000000 hdsr_pygithub-1.9/hdsr_pygithub/downloader/dir.py
+-rw-rw-rw-   0        0        0     2561 2022-06-22 09:29:12.000000 hdsr_pygithub-1.9/hdsr_pygithub/downloader/file.py
+-rw-rw-rw-   0        0        0      555 2022-01-05 15:55:52.000000 hdsr_pygithub-1.9/hdsr_pygithub/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-03-07 14:10:40.000000 hdsr_pygithub-1.9/hdsr_pygithub/tests/
+-rw-rw-rw-   0        0        0        0 2021-11-11 12:35:47.000000 hdsr_pygithub-1.9/hdsr_pygithub/tests/__init__.py
+-rw-rw-rw-   0        0        0     8237 2023-03-01 09:47:10.000000 hdsr_pygithub-1.9/hdsr_pygithub/tests/test_dir_downloader.py
+-rw-rw-rw-   0        0        0     3850 2023-03-01 09:47:10.000000 hdsr_pygithub-1.9/hdsr_pygithub/tests/test_file_downloader.py
+-rw-rw-rw-   0        0        0     1382 2023-03-06 20:50:35.000000 hdsr_pygithub-1.9/hdsr_pygithub/tests/test_general.py
+-rw-rw-rw-   0        0        0      603 2022-07-14 12:17:42.000000 hdsr_pygithub-1.9/hdsr_pygithub/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-07 14:10:40.000000 hdsr_pygithub-1.9/hdsr_pygithub.egg-info/
+-rw-rw-rw-   0        0        0     9761 2023-03-07 14:10:38.000000 hdsr_pygithub-1.9/hdsr_pygithub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2023-03-07 14:10:38.000000 hdsr_pygithub-1.9/hdsr_pygithub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-07 14:10:38.000000 hdsr_pygithub-1.9/hdsr_pygithub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 14:10:38.000000 hdsr_pygithub-1.9/hdsr_pygithub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       66 2023-03-07 14:10:38.000000 hdsr_pygithub-1.9/hdsr_pygithub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-03-07 14:10:38.000000 hdsr_pygithub-1.9/hdsr_pygithub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2021-11-11 09:44:52.000000 hdsr_pygithub-1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-03-07 14:10:41.000000 hdsr_pygithub-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1606 2023-03-06 21:27:51.000000 hdsr_pygithub-1.9/setup.py
```

### Comparing `hdsr_pygithub-1.8/LICENSE` & `hdsr_pygithub-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/PKG-INFO` & `hdsr_pygithub-1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,142 @@
 Metadata-Version: 2.1
 Name: hdsr_pygithub
-Version: 1.8
+Version: 1.9
 Summary: An interface for interacting with hdsr github repos
 Home-page: https://github.com/hdsr-mid/hdsr_pygithub
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_pygithub/archive/v1.8.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_pygithub/archive/v1.9.tar.gz
 Keywords: interface,interaction,github,files,hdsr
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[HdsrMidReadOnly]: https://github.com/HdsrMidReadOnly
-[change personal access token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
-[authorisation page]: https://github.com/orgs/hdsr-mid/people/HdsrMidReadOnly
+[token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
 [hdsr-mid]: [https://github.com/hdr-mid]
 [pypi]: https://pypi.org/project/hdsr_pygithub
 [mit]: https://github.com/hdsr-mid/hdsr_pygithub/blob/main/LICENSE.txt
 
 ### Context
 * Created: November 2021
 * Author: Renier Kramer, renier.kramer@hdsr.nl
 * Python version: >3.5
 
+
 ### Description
-A python project that enables interaction with the GitHub API v3 to e.g. read/download files from the 
-github organisation [hdsr-mid]. This project uses the github account [HdsrMidReadOnly], that has read-only access 
-to some of the [hdsr-mid] repos. This organisation requires 2FA, so authentication - via github api - is only 
-possible with a personal access token. For this account the following yields:
-- A personal access token has been created which is required for the Github API
-- The token has no expiration date
-- To [change personal access token] for account HdsrMidReadOnly 
-    - login github.com with account HdsrMidReadOnly
-        - email: hdsrmidgithub@gmail.com
-        - password: please contact renier.kramer@hdsr.nl
-    - go to settings >> developer settings >> personal access token >> generate new token
--  To change authorization for account HdsrMidReadOnly
-   - get admin rights for [hdsr-mid]
-   - go to [authorisation page]
-
-Usually, 3 ways exists to log in with GitHub API:
-- Github(login_or_token=<user>, password=<pass>)
-- Github(login_or_token=<personal_access_token>)
-- Github(base_url="https://{hostname}/api/v3", login_or_token=<personal_access_token>)
-
-However, the first is not possible for github organisation 'hdsr-mid' since 13 sep 2021 as it requires
-two-factor authentication for everyone in the hdsr-mid organisation: login trough github api is now only possible
-with token (options 1 and 2). In this project we use option 2.
+A python project that enables interaction with the GitHub API v3 to e.g. read/download dirs/files from the 
+github organisation [hdsr-mid]. Often downloading is not required as files can be loaded in 
+memory, see 'Usage 1' below. To interact with private repos you need to authenticate via a personal github 
+access token (see 'Token' below).
+
+### Token
+A token (a long hash) has to be created once (and updated when it expires). You can [do this yourself][token]. In short:
+1. Login github.com with your account (user + password)
+2. Ensure you have at least read-permission for hdsr-mid repo(s) you want to interact. If not, please contact 
+   renier.kramer@hdsr.nl
+3. Go to settings >> developer settings >> personal access token >> generate new token. We recommend setting an expiry 
+   date of max 1 year (for safety reasons).
+4. You can use this token in two ways:
+   1. Create a file on your personal HDSR drive: 'G:/secrets.env' and add 1 line: GITHUB_PERSONAL_ACCESS_TOKEN=blabla
+   2. Use it hardcode in you code, see 'Usage 1: simple'. In this case, be careful sharing your code. 
+   
+#### Why use a token?
+This project is build on another pypi project 'PyGithub'. That project provides three ways for authentication exists 
+to log in with GitHub API:
+1. Github(login_or_token=<user>, password=<pass>)
+2. Github(login_or_token=<personal_access_token>)
+3. Github(base_url="https://{hostname}/api/v3", login_or_token=<personal_access_token>)
+   
+However, option 1 is not possible for github organisation 'hdsr-mid' since 13 sep 2021 as it requires 2FA for 
+everyone in the hdsr-mid organisation: login trough github api is now only possible with a token (options 1 and 2). 
+In this project we use option 2.
 
-### Usage (simple)
+### Usage 1: simple (little arguments and hard-coded personal_access_token)
 ```
 pip install hdsr-pygithub
 from hdsr_pygithub import GithubFileDownloader
 from pathlib import Path
 
 github_downloader = GithubFileDownloader(
-    repo_name="startenddate",                                               # any hdsr-mid repo for which account HdsrMidReadOnly has access (see README.md)
+    repo_name="startenddate",                                               # ensure your github account has read-permission for this repo
     target_file=Path("data/output/results/mwm_peilschalen_short.csv"),      # this file must exist in the master branch
+    personal_access_token=<your_personal_access_token>                      # see topic 'Token' 4.2 above
 )
 
 # download files to disk
 download_directory = github_downloader.download_files(download_directory=<a_dir>)
 downloaded_filepath = download_directory / "data/output/results/mwm_peilschalen_short.csv"
 assert downloaded_filepath.exists()
 
 # or read file in memory using e.g. pandas
 import pandas as pd
 url = github_downloader.get_download_url()
 # in case filetype is a .csv (other filetypes see: https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html):
 dataframe_file = pd.read_csv(filepath_or_buffer=url)
 ```
 
-### Usage (sophisticated)
+### Usage 2: sophisticated (more arguments and personal_access_token in .env file)
 ```
+# Ensure you followed steps 1, 2, 3, and 4a of topic 'Token' above
 pip install hdsr-pygithub
 from hdsr_pygithub import GithubDirDownloader
 from datetime import datetime
 from pathlib import Path
 
 github_downloader = GithubDirDownloader(
-    repo_name="startenddate",                                               # any hdsr-mid repo for which account HdsrMidReadOnly has access (see README.md)
+    repo_name="startenddate",                                               # ensure your github account has read-permission for this repo
     branch_name="main",                                                     # defaults to 'main' if not specified                                                                        
     target_dir=Path("data/output/results/"),                                # this dir must exist in the branch specified above
     allowed_period_no_updates=datetime.timedelta(weeks=10),                 # defaults to 1 year if not specified 
-    personal_access_token=<personal_access_token>,                          # you can use your own github account's token
     repo_organisation='hdsr-mid',                                           # defaults to 'hdsr-mid'
 )
 
 # download complete github directory (recursive) to disk
 download_directory = github_downloader.download_files(download_directory=<a_dir>)
 assert download_directory.is_dir()
 
 # or download complete github directory (recursive) to disk to your Temp directory (C:/Users/<user>/AppData/Local/Temp/..)
 download_directory = github_downloader.download_files(use_tmp_dir=True)
 assert download_directory.is_dir()
 ```
 
+
 ### License 
 [MIT][mit]
 
 ### Releases
 [PyPi][pypi]
 
 ### Contributions
 All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
 Issues are posted on: https://github.com/hdsr-mid/hdsr_pygithub/issues
 
-### Test coverage (release v1.8)
+### Test coverage (release v1.9)
 ```
------------ coverage: platform win32, python 3.9.7-final-0 -----------
+---------- coverage: platform win32, python 3.11.0-final-0 -----------
 Name                               Stmts   Miss  Cover
 ------------------------------------------------------
 hdsr_pygithub\__init__.py              2      0   100%
-hdsr_pygithub\constants.py             5      0   100%
-hdsr_pygithub\downloader\base.py     207     30    86%
+hdsr_pygithub\constants.py             7      0   100%
+hdsr_pygithub\downloader\base.py     227     33    85%
 hdsr_pygithub\downloader\dir.py       88      0   100%
 hdsr_pygithub\downloader\file.py      34      0   100%
 hdsr_pygithub\exceptions.py           15      1    93%
 setup.py                              10     10     0%
 ------------------------------------------------------
-TOTAL                                361     41    89%
+TOTAL                                383     44    89%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_pygithub-1.8/README.md` & `hdsr_pygithub-1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,120 @@
-[HdsrMidReadOnly]: https://github.com/HdsrMidReadOnly
-[change personal access token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
-[authorisation page]: https://github.com/orgs/hdsr-mid/people/HdsrMidReadOnly
+[token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
 [hdsr-mid]: [https://github.com/hdr-mid]
 [pypi]: https://pypi.org/project/hdsr_pygithub
 [mit]: https://github.com/hdsr-mid/hdsr_pygithub/blob/main/LICENSE.txt
 
 ### Context
 * Created: November 2021
 * Author: Renier Kramer, renier.kramer@hdsr.nl
 * Python version: >3.5
 
+
 ### Description
-A python project that enables interaction with the GitHub API v3 to e.g. read/download files from the 
-github organisation [hdsr-mid]. This project uses the github account [HdsrMidReadOnly], that has read-only access 
-to some of the [hdsr-mid] repos. This organisation requires 2FA, so authentication - via github api - is only 
-possible with a personal access token. For this account the following yields:
-- A personal access token has been created which is required for the Github API
-- The token has no expiration date
-- To [change personal access token] for account HdsrMidReadOnly 
-    - login github.com with account HdsrMidReadOnly
-        - email: hdsrmidgithub@gmail.com
-        - password: please contact renier.kramer@hdsr.nl
-    - go to settings >> developer settings >> personal access token >> generate new token
--  To change authorization for account HdsrMidReadOnly
-   - get admin rights for [hdsr-mid]
-   - go to [authorisation page]
-
-Usually, 3 ways exists to log in with GitHub API:
-- Github(login_or_token=<user>, password=<pass>)
-- Github(login_or_token=<personal_access_token>)
-- Github(base_url="https://{hostname}/api/v3", login_or_token=<personal_access_token>)
-
-However, the first is not possible for github organisation 'hdsr-mid' since 13 sep 2021 as it requires
-two-factor authentication for everyone in the hdsr-mid organisation: login trough github api is now only possible
-with token (options 1 and 2). In this project we use option 2.
+A python project that enables interaction with the GitHub API v3 to e.g. read/download dirs/files from the 
+github organisation [hdsr-mid]. Often downloading is not required as files can be loaded in 
+memory, see 'Usage 1' below. To interact with private repos you need to authenticate via a personal github 
+access token (see 'Token' below).
+
+### Token
+A token (a long hash) has to be created once (and updated when it expires). You can [do this yourself][token]. In short:
+1. Login github.com with your account (user + password)
+2. Ensure you have at least read-permission for hdsr-mid repo(s) you want to interact. If not, please contact 
+   renier.kramer@hdsr.nl
+3. Go to settings >> developer settings >> personal access token >> generate new token. We recommend setting an expiry 
+   date of max 1 year (for safety reasons).
+4. You can use this token in two ways:
+   1. Create a file on your personal HDSR drive: 'G:/secrets.env' and add 1 line: GITHUB_PERSONAL_ACCESS_TOKEN=blabla
+   2. Use it hardcode in you code, see 'Usage 1: simple'. In this case, be careful sharing your code. 
+   
+#### Why use a token?
+This project is build on another pypi project 'PyGithub'. That project provides three ways for authentication exists 
+to log in with GitHub API:
+1. Github(login_or_token=<user>, password=<pass>)
+2. Github(login_or_token=<personal_access_token>)
+3. Github(base_url="https://{hostname}/api/v3", login_or_token=<personal_access_token>)
+   
+However, option 1 is not possible for github organisation 'hdsr-mid' since 13 sep 2021 as it requires 2FA for 
+everyone in the hdsr-mid organisation: login trough github api is now only possible with a token (options 1 and 2). 
+In this project we use option 2.
 
-### Usage (simple)
+### Usage 1: simple (little arguments and hard-coded personal_access_token)
 ```
 pip install hdsr-pygithub
 from hdsr_pygithub import GithubFileDownloader
 from pathlib import Path
 
 github_downloader = GithubFileDownloader(
-    repo_name="startenddate",                                               # any hdsr-mid repo for which account HdsrMidReadOnly has access (see README.md)
+    repo_name="startenddate",                                               # ensure your github account has read-permission for this repo
     target_file=Path("data/output/results/mwm_peilschalen_short.csv"),      # this file must exist in the master branch
+    personal_access_token=<your_personal_access_token>                      # see topic 'Token' 4.2 above
 )
 
 # download files to disk
 download_directory = github_downloader.download_files(download_directory=<a_dir>)
 downloaded_filepath = download_directory / "data/output/results/mwm_peilschalen_short.csv"
 assert downloaded_filepath.exists()
 
 # or read file in memory using e.g. pandas
 import pandas as pd
 url = github_downloader.get_download_url()
 # in case filetype is a .csv (other filetypes see: https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html):
 dataframe_file = pd.read_csv(filepath_or_buffer=url)
 ```
 
-### Usage (sophisticated)
+### Usage 2: sophisticated (more arguments and personal_access_token in .env file)
 ```
+# Ensure you followed steps 1, 2, 3, and 4a of topic 'Token' above
 pip install hdsr-pygithub
 from hdsr_pygithub import GithubDirDownloader
 from datetime import datetime
 from pathlib import Path
 
 github_downloader = GithubDirDownloader(
-    repo_name="startenddate",                                               # any hdsr-mid repo for which account HdsrMidReadOnly has access (see README.md)
+    repo_name="startenddate",                                               # ensure your github account has read-permission for this repo
     branch_name="main",                                                     # defaults to 'main' if not specified                                                                        
     target_dir=Path("data/output/results/"),                                # this dir must exist in the branch specified above
     allowed_period_no_updates=datetime.timedelta(weeks=10),                 # defaults to 1 year if not specified 
-    personal_access_token=<personal_access_token>,                          # you can use your own github account's token
     repo_organisation='hdsr-mid',                                           # defaults to 'hdsr-mid'
 )
 
 # download complete github directory (recursive) to disk
 download_directory = github_downloader.download_files(download_directory=<a_dir>)
 assert download_directory.is_dir()
 
 # or download complete github directory (recursive) to disk to your Temp directory (C:/Users/<user>/AppData/Local/Temp/..)
 download_directory = github_downloader.download_files(use_tmp_dir=True)
 assert download_directory.is_dir()
 ```
 
+
 ### License 
 [MIT][mit]
 
 ### Releases
 [PyPi][pypi]
 
 ### Contributions
 All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
 Issues are posted on: https://github.com/hdsr-mid/hdsr_pygithub/issues
 
-### Test coverage (release v1.8)
+### Test coverage (release v1.9)
 ```
------------ coverage: platform win32, python 3.9.7-final-0 -----------
+---------- coverage: platform win32, python 3.11.0-final-0 -----------
 Name                               Stmts   Miss  Cover
 ------------------------------------------------------
 hdsr_pygithub\__init__.py              2      0   100%
-hdsr_pygithub\constants.py             5      0   100%
-hdsr_pygithub\downloader\base.py     207     30    86%
+hdsr_pygithub\constants.py             7      0   100%
+hdsr_pygithub\downloader\base.py     227     33    85%
 hdsr_pygithub\downloader\dir.py       88      0   100%
 hdsr_pygithub\downloader\file.py      34      0   100%
 hdsr_pygithub\exceptions.py           15      1    93%
 setup.py                              10     10     0%
 ------------------------------------------------------
-TOTAL                                361     41    89%
+TOTAL                                383     44    89%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/downloader/base.py` & `hdsr_pygithub-1.9/hdsr_pygithub/downloader/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC
 from abc import abstractmethod
 from dateutil.parser import parse
+from dotenv import load_dotenv
 from github import Github
 from github.Branch import Branch
 from github.ContentFile import ContentFile
 from github.GithubException import GithubException
 from github.PaginatedList import PaginatedList
 from github.Repository import Repository
 from hdsr_pygithub import constants
@@ -13,55 +14,79 @@
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import base64
 import datetime
 import logging
+import os
 import tempfile
 
 
 logger = logging.getLogger(__name__)
 
 
 _1mb = 1000000
 
 
 class GithubDownloaderBase(ABC):
     def __init__(
         self,
         repo_name: str,
-        personal_access_token: str = constants.GITHUB_HDSR_READ_ONLY_ACCOUNT_ACCESS_TOKEN,
         repo_organisation: str = constants.DEFAULT_GITHUB_ORGANISATION,
         branch_name: str = None,
+        personal_access_token: str = None,
         allowed_period_no_updates: datetime.timedelta = datetime.timedelta(weeks=52),
     ) -> None:
         self.repo_name = repo_name
         self.branch_name = branch_name if branch_name else "main"
         self.allowed_period_no_updates = allowed_period_no_updates
-        self.personal_access_token = personal_access_token
         self.repo_organisation = repo_organisation
+        self._personal_access_token = personal_access_token
+        logger.info(f"loading personal_access_token from .env = {not bool(personal_access_token)}")
+        #
         self.content_dict = {}
         self._github_instance = None
         self._repo_instance = None
         self._content_file = None
         self._branch_commits = None
+        #
         self.validate_base_constructor()
 
+    @property
+    def personal_access_token(self) -> str:
+        if self._personal_access_token is not None:
+            return self._personal_access_token
+        try:
+            token_path = constants.SECRETS_ENV_PATH
+            logger.info(f"retrieving your github personal access token from {token_path}")
+            assert token_path.is_file(), f"could not find {token_path}"
+            load_dotenv(dotenv_path=token_path.as_posix())
+            token = os.environ.get(constants.TOKEN_KEY, None)
+            assert token, f"file {token_path} exists, but it must contain a row: {constants.TOKEN_KEY}=blablabla"
+            assert (
+                isinstance(token, str) and len(token) > 20
+            ), f"{constants.TOKEN_KEY} must a string of at least 20 chars"
+            self._personal_access_token = token
+        except Exception as err:
+            msg = (
+                f"could not get {constants.TOKEN_KEY} from {constants.SECRETS_ENV_PATH}. err={err}. Please read "
+                f"topic 'Token' on https://pypi.org/project/hdsr-pygithub/"
+            )
+            raise AssertionError(msg)
+        return self._personal_access_token
+
     def validate_base_constructor(self) -> None:
-        assert (
-            isinstance(self.personal_access_token, str) and self.personal_access_token
-        ), f"github personal access token must be str {self.personal_access_token}"
+        assert self.personal_access_token
         assert isinstance(self.allowed_period_no_updates, datetime.timedelta), (
             f"allowed_period_no_updates must be a datetime.timedelta " f"{self.allowed_period_no_updates}"
         )
         assert isinstance(self.repo_name, str) and self.repo_name, f"repo_name must be str {self.repo_name}"
         if self.repo_organisation:
             assert isinstance(self.repo_organisation, str), f"repo_organisation must be a str {self.repo_organisation}"
-
         available_branches = [branch.name for branch in self.repo_instance.get_branches()]
         if self.branch_name not in available_branches:
             raise exceptions.GithubBranchNotFound(msg=f"branch '{self.branch_name}' not found in {available_branches}")
 
     @property
     def github_instance(self) -> Github:
         if self._github_instance is not None:
```

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/downloader/dir.py` & `hdsr_pygithub-1.9/hdsr_pygithub/downloader/dir.py`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/downloader/file.py` & `hdsr_pygithub-1.9/hdsr_pygithub/downloader/file.py`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/exceptions.py` & `hdsr_pygithub-1.9/hdsr_pygithub/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/tests/test_dir_downloader.py` & `hdsr_pygithub-1.9/hdsr_pygithub/tests/test_dir_downloader.py`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/tests/test_file_downloader.py` & `hdsr_pygithub-1.9/hdsr_pygithub/tests/test_file_downloader.py`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/tests/test_general.py` & `hdsr_pygithub-1.9/hdsr_pygithub/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub/tests/utils.py` & `hdsr_pygithub-1.9/hdsr_pygithub/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub.egg-info/PKG-INFO` & `hdsr_pygithub-1.9/hdsr_pygithub.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,142 @@
 Metadata-Version: 2.1
 Name: hdsr-pygithub
-Version: 1.8
+Version: 1.9
 Summary: An interface for interacting with hdsr github repos
 Home-page: https://github.com/hdsr-mid/hdsr_pygithub
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_pygithub/archive/v1.8.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_pygithub/archive/v1.9.tar.gz
 Keywords: interface,interaction,github,files,hdsr
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[HdsrMidReadOnly]: https://github.com/HdsrMidReadOnly
-[change personal access token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
-[authorisation page]: https://github.com/orgs/hdsr-mid/people/HdsrMidReadOnly
+[token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
 [hdsr-mid]: [https://github.com/hdr-mid]
 [pypi]: https://pypi.org/project/hdsr_pygithub
 [mit]: https://github.com/hdsr-mid/hdsr_pygithub/blob/main/LICENSE.txt
 
 ### Context
 * Created: November 2021
 * Author: Renier Kramer, renier.kramer@hdsr.nl
 * Python version: >3.5
 
+
 ### Description
-A python project that enables interaction with the GitHub API v3 to e.g. read/download files from the 
-github organisation [hdsr-mid]. This project uses the github account [HdsrMidReadOnly], that has read-only access 
-to some of the [hdsr-mid] repos. This organisation requires 2FA, so authentication - via github api - is only 
-possible with a personal access token. For this account the following yields:
-- A personal access token has been created which is required for the Github API
-- The token has no expiration date
-- To [change personal access token] for account HdsrMidReadOnly 
-    - login github.com with account HdsrMidReadOnly
-        - email: hdsrmidgithub@gmail.com
-        - password: please contact renier.kramer@hdsr.nl
-    - go to settings >> developer settings >> personal access token >> generate new token
--  To change authorization for account HdsrMidReadOnly
-   - get admin rights for [hdsr-mid]
-   - go to [authorisation page]
-
-Usually, 3 ways exists to log in with GitHub API:
-- Github(login_or_token=<user>, password=<pass>)
-- Github(login_or_token=<personal_access_token>)
-- Github(base_url="https://{hostname}/api/v3", login_or_token=<personal_access_token>)
-
-However, the first is not possible for github organisation 'hdsr-mid' since 13 sep 2021 as it requires
-two-factor authentication for everyone in the hdsr-mid organisation: login trough github api is now only possible
-with token (options 1 and 2). In this project we use option 2.
+A python project that enables interaction with the GitHub API v3 to e.g. read/download dirs/files from the 
+github organisation [hdsr-mid]. Often downloading is not required as files can be loaded in 
+memory, see 'Usage 1' below. To interact with private repos you need to authenticate via a personal github 
+access token (see 'Token' below).
+
+### Token
+A token (a long hash) has to be created once (and updated when it expires). You can [do this yourself][token]. In short:
+1. Login github.com with your account (user + password)
+2. Ensure you have at least read-permission for hdsr-mid repo(s) you want to interact. If not, please contact 
+   renier.kramer@hdsr.nl
+3. Go to settings >> developer settings >> personal access token >> generate new token. We recommend setting an expiry 
+   date of max 1 year (for safety reasons).
+4. You can use this token in two ways:
+   1. Create a file on your personal HDSR drive: 'G:/secrets.env' and add 1 line: GITHUB_PERSONAL_ACCESS_TOKEN=blabla
+   2. Use it hardcode in you code, see 'Usage 1: simple'. In this case, be careful sharing your code. 
+   
+#### Why use a token?
+This project is build on another pypi project 'PyGithub'. That project provides three ways for authentication exists 
+to log in with GitHub API:
+1. Github(login_or_token=<user>, password=<pass>)
+2. Github(login_or_token=<personal_access_token>)
+3. Github(base_url="https://{hostname}/api/v3", login_or_token=<personal_access_token>)
+   
+However, option 1 is not possible for github organisation 'hdsr-mid' since 13 sep 2021 as it requires 2FA for 
+everyone in the hdsr-mid organisation: login trough github api is now only possible with a token (options 1 and 2). 
+In this project we use option 2.
 
-### Usage (simple)
+### Usage 1: simple (little arguments and hard-coded personal_access_token)
 ```
 pip install hdsr-pygithub
 from hdsr_pygithub import GithubFileDownloader
 from pathlib import Path
 
 github_downloader = GithubFileDownloader(
-    repo_name="startenddate",                                               # any hdsr-mid repo for which account HdsrMidReadOnly has access (see README.md)
+    repo_name="startenddate",                                               # ensure your github account has read-permission for this repo
     target_file=Path("data/output/results/mwm_peilschalen_short.csv"),      # this file must exist in the master branch
+    personal_access_token=<your_personal_access_token>                      # see topic 'Token' 4.2 above
 )
 
 # download files to disk
 download_directory = github_downloader.download_files(download_directory=<a_dir>)
 downloaded_filepath = download_directory / "data/output/results/mwm_peilschalen_short.csv"
 assert downloaded_filepath.exists()
 
 # or read file in memory using e.g. pandas
 import pandas as pd
 url = github_downloader.get_download_url()
 # in case filetype is a .csv (other filetypes see: https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html):
 dataframe_file = pd.read_csv(filepath_or_buffer=url)
 ```
 
-### Usage (sophisticated)
+### Usage 2: sophisticated (more arguments and personal_access_token in .env file)
 ```
+# Ensure you followed steps 1, 2, 3, and 4a of topic 'Token' above
 pip install hdsr-pygithub
 from hdsr_pygithub import GithubDirDownloader
 from datetime import datetime
 from pathlib import Path
 
 github_downloader = GithubDirDownloader(
-    repo_name="startenddate",                                               # any hdsr-mid repo for which account HdsrMidReadOnly has access (see README.md)
+    repo_name="startenddate",                                               # ensure your github account has read-permission for this repo
     branch_name="main",                                                     # defaults to 'main' if not specified                                                                        
     target_dir=Path("data/output/results/"),                                # this dir must exist in the branch specified above
     allowed_period_no_updates=datetime.timedelta(weeks=10),                 # defaults to 1 year if not specified 
-    personal_access_token=<personal_access_token>,                          # you can use your own github account's token
     repo_organisation='hdsr-mid',                                           # defaults to 'hdsr-mid'
 )
 
 # download complete github directory (recursive) to disk
 download_directory = github_downloader.download_files(download_directory=<a_dir>)
 assert download_directory.is_dir()
 
 # or download complete github directory (recursive) to disk to your Temp directory (C:/Users/<user>/AppData/Local/Temp/..)
 download_directory = github_downloader.download_files(use_tmp_dir=True)
 assert download_directory.is_dir()
 ```
 
+
 ### License 
 [MIT][mit]
 
 ### Releases
 [PyPi][pypi]
 
 ### Contributions
 All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
 Issues are posted on: https://github.com/hdsr-mid/hdsr_pygithub/issues
 
-### Test coverage (release v1.8)
+### Test coverage (release v1.9)
 ```
------------ coverage: platform win32, python 3.9.7-final-0 -----------
+---------- coverage: platform win32, python 3.11.0-final-0 -----------
 Name                               Stmts   Miss  Cover
 ------------------------------------------------------
 hdsr_pygithub\__init__.py              2      0   100%
-hdsr_pygithub\constants.py             5      0   100%
-hdsr_pygithub\downloader\base.py     207     30    86%
+hdsr_pygithub\constants.py             7      0   100%
+hdsr_pygithub\downloader\base.py     227     33    85%
 hdsr_pygithub\downloader\dir.py       88      0   100%
 hdsr_pygithub\downloader\file.py      34      0   100%
 hdsr_pygithub\exceptions.py           15      1    93%
 setup.py                              10     10     0%
 ------------------------------------------------------
-TOTAL                                361     41    89%
+TOTAL                                383     44    89%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_pygithub-1.8/hdsr_pygithub.egg-info/SOURCES.txt` & `hdsr_pygithub-1.9/hdsr_pygithub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/pyproject.toml` & `hdsr_pygithub-1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_pygithub-1.8/setup.py` & `hdsr_pygithub-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.8"
+version = "1.9"
 
 install_requires = [
     "pathlib",
     "typing",
     "PyGithub",
     "python-dateutil",
 ]
```

