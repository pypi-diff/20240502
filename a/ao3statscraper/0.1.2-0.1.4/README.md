# Comparing `tmp/ao3statscraper-0.1.2.tar.gz` & `tmp/ao3statscraper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ao3statscraper-0.1.2.tar", last modified: Sat Apr 27 23:33:36 2024, max compression
+gzip compressed data, was "ao3statscraper-0.1.4.tar", last modified: Thu May  2 13:09:12 2024, max compression
```

## Comparing `ao3statscraper-0.1.2.tar` & `ao3statscraper-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.314817 ao3statscraper-0.1.2/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.1.2/LICENSE
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48518 2024-04-27 23:33:36.314817 ao3statscraper-0.1.2/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     7140 2024-04-25 15:35:41.000000 ao3statscraper-0.1.2/README.md
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/ao3statscraper/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/__init__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-04-27 23:33:23.000000 ao3statscraper-0.1.2/ao3statscraper/__version__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2428 2024-04-24 23:01:50.000000 ao3statscraper-0.1.2/ao3statscraper/ao3requester.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6508 2024-04-24 22:59:18.000000 ao3statscraper-0.1.2/ao3statscraper/configuration.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/plotting.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/pw.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.1.2/ao3statscraper/scrape.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/ao3statscraper/scripts/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      177 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/__init__.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      905 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3_hits_to_kudos.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3234 2024-04-24 21:11:36.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3_purge_stats_data.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3660 2024-04-24 21:10:58.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3plot.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3661 2024-04-24 22:55:08.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3scrape.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/statsdata.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/utils.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/ao3statscraper.egg-info/
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48518 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      754 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/entry_points.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      109 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/requires.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/top_level.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1613 2024-04-27 23:33:23.000000 ao3statscraper-0.1.2/pyproject.toml
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-04-27 23:33:36.314817 ao3statscraper-0.1.2/setup.cfg
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/tests/
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/tests/test_passwords.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/tests/test_writing_data.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.1.4/LICENSE
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48957 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     7554 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/README.md
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/ao3statscraper/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/__init__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/__version__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2425 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/ao3requester.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8351 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/configuration.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/plotting.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/pw.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.1.4/ao3statscraper/scrape.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/ao3statscraper/scripts/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      177 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/__init__.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      905 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_hits_to_kudos.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3234 2024-04-24 21:11:36.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_purge_stats_data.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3660 2024-04-24 21:10:58.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3plot.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3961 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3scrape.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/statsdata.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/utils.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/ao3statscraper.egg-info/
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48957 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      754 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/entry_points.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      119 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/requires.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/top_level.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1630 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/pyproject.toml
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/setup.cfg
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/tests/
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/tests/test_passwords.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/tests/test_writing_data.py
```

### Comparing `ao3statscraper-0.1.2/LICENSE` & `ao3statscraper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/PKG-INFO` & `ao3statscraper-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.1.2
+Version: 0.1.4
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,16 +686,17 @@
 Classifier: Intended Audience :: End Users/Desktop
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: datetime
 Requires-Dist: lxml
 Requires-Dist: matplotlib>=3.6
-Requires-Dist: pycryptodome>=3.20
+Requires-Dist: packaging
 Requires-Dist: pandas>=2.2.0
+Requires-Dist: pycryptodome>=3.20
 Requires-Dist: pyjson
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: termcolor
 
 # AO3StatScraper
@@ -721,59 +722,64 @@
 
 ```
 py -m pip install ao3statscraper
 ```
 
 
 Alternately, the source code is available on
-[gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper).  On OSX and Linux,
-you can install a local version by cloning the repository using git:
+[gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper).
+you can install a local version by cloning the repository using git.
+On OSX and Linux, you can use:
 
 ```
-git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git
-cd AO3StatScraper  # go into the directory
-python3 -m pip install .
+git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git    # get you the git repository
+cd AO3StatScraper                                                 # go into the directory
+python3 -m pip install .                                          # install package
 ```
 
 
 
 ## User Guide
 
 ### Overview: How It Works
 
-`AO3StatScraper` simply downloads your AO3 stats page (pretty much the same as 
+`AO3StatScraper` simply downloads your AO3 stats page (pretty much the same as
 opening it in your browser and hitting `Save this page...`) and then extract the
 stats from that html content. To be able to access your stats, you need to log
 in to AO3, which is why `AO3StatScraper` will ask you for your username and
 password.
 
-Unless specified otherwise, by default `AO3StatScraper` (i.e. the script
-`ao3get`) will store your current stats as a snapshot. The data is written in
+
+By default `AO3StatScraper` (i.e. the script `ao3get`) will store your current
+stats as a snapshot. This includes both your total user statistics as well as
+your individual work statistics. The data is written in
 the csv (Comma Separated Values) format, so plenty of other software and
 packages should be able to read it in easily. Your total user statistics are
 stored in a separate file from your work statistics.
 
 
 
 ### Getting Started
 
 The main use case for `AO3StatScraper` is to fetch and display your current AO3
 statistics using scripts provided by `AO3StatScraper`. Currently, there are 4
 scripts:
 
-- `ao3get` : The main script to fetch your AO3 stats.
-- `ao3plot`: Plots the stats stored with `ao3get`
+- `ao3get` : The main script to fetch and display your AO3 stats.
+- `ao3plot`: Plots the stats stored with `ao3get`.
 - `ao3_hits_to_kudos`: List all your works in ascending order of their
   hits/kudos ratio
 - `ao3_purge`: Deletes saved stats such that there is a minumum time between the
   remaining ones
 
+The scripts are discussed in more detail further below.
+
 
 **IMPORTANT**: Before you can run the other scripts, you first need to configure
-`AO3StatScraper`.  This is done by calling `ao3get`. It will launch the
+`AO3StatScraper`. This is done by calling `ao3get`. It will launch the
 configuration dialogue automatically if it hasn't been configured yet. You can
 always re-configure it by invoking `ao3get -c`.
 
 
 
 
 ### `ao3get`
@@ -794,26 +800,30 @@
 - `--config`: Run the configuration dialogue and exit.
 - `--remove-last`: Deletes the last snapshot `ao3get` stored and exits. May come
   in handy if you're nervously re-downloading your stats every minute.
 - `--no-write`: This flag modifies the behavious for `--all` and `--diff`
   running modes. While current stats are fetched from AO3, they won't be written
   into a snapshot.
 
+The list above does not cover all the available options. Please use
+`ao3get --help` to see all the available options.
 
 Using `ao3get` requires you to log in to your AO3 account. You can either type
 in your username and password each time you invoke it, or you can store it with
 `AO3StatScraper`, locked behind a master password. There are no restrictions on
 how sophisticated your master password needs to be, so if you can't be
-inconvenienced, you can even leave it empty.
+inconvenienced, you can even leave it empty. Alternately, you can opt out of
+using a master password at all, although this is not encouraged. But it would
+allow you to e.g. set up an automated way to fetch your stats at regular times.
 
 
 ### `ao3plot`
 
 `ao3plot` will display some simple graphs based on the stored snapshots. It
-never stores snapshots itself, you will need to do that using `ao3get`. 
+never stores snapshots itself, you will need to do that using `ao3get`.
 
 By default, `ao3plot` will ask you to select which work you would like to see
 graphs of stats for. You can also select to plot your total user statistics.
 
 Alternately, you can skip that dialogue by using the following flags:
 
 - `-u`: Show total user statistics.
@@ -833,17 +843,17 @@
 This script just reads in the last stored snapshot and prints out all your works
 in ascending order of their hits/kudos ratio.
 
 
 
 ### `ao3_purge`
 
-In case you find yourself in a situation where you feel you have stored way too 
-many snapshots, `ao3_purge` offers you the option to delete stats snapshots such 
-that there is some minimal time between them. By default, this frequency is set 
+In case you find yourself in a situation where you feel you have stored way too
+many snapshots, `ao3_purge` offers you the option to delete stats snapshots such
+that there is some minimal time between them. By default, this frequency is set
 to 12h. You can provide the frequency you like using the `--frequency` flag.
 
 
 
 
 ## Examples
 
@@ -888,17 +898,14 @@
 
 # Roadmap and Contributing
 
 Help and contributions to maintain and extend this tool are very welcome!
 
 Some ideas what might be added in the future include
 - Writing/reading of file formats other than csv.
-- Option to make the script automatizable so users can make it fetch their stats
-  regularly. The problem here is that it would need to circumvent typing in a
-  password.
 - Maybe add a GUI for CLI-averse users. This tool was always intended to be a
   command line tool on my end. Having never programmed a GUI in my life, I don't
   intend to start now. However, if anybody is willing to pack this up in a nice
   simple portable GUI, you are very welcome and encouraged to do so! I'll gladly
   add it to the repository.
 
 I'm using unix exclusively, so there may be issues on other operating systems.
```

### Comparing `ao3statscraper-0.1.2/README.md` & `ao3statscraper-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,59 +21,64 @@
 
 ```
 py -m pip install ao3statscraper
 ```
 
 
 Alternately, the source code is available on
-[gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper).  On OSX and Linux,
-you can install a local version by cloning the repository using git:
+[gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper).
+you can install a local version by cloning the repository using git.
+On OSX and Linux, you can use:
 
 ```
-git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git
-cd AO3StatScraper  # go into the directory
-python3 -m pip install .
+git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git    # get you the git repository
+cd AO3StatScraper                                                 # go into the directory
+python3 -m pip install .                                          # install package
 ```
 
 
 
 ## User Guide
 
 ### Overview: How It Works
 
-`AO3StatScraper` simply downloads your AO3 stats page (pretty much the same as 
+`AO3StatScraper` simply downloads your AO3 stats page (pretty much the same as
 opening it in your browser and hitting `Save this page...`) and then extract the
 stats from that html content. To be able to access your stats, you need to log
 in to AO3, which is why `AO3StatScraper` will ask you for your username and
 password.
 
-Unless specified otherwise, by default `AO3StatScraper` (i.e. the script
-`ao3get`) will store your current stats as a snapshot. The data is written in
+
+By default `AO3StatScraper` (i.e. the script `ao3get`) will store your current
+stats as a snapshot. This includes both your total user statistics as well as
+your individual work statistics. The data is written in
 the csv (Comma Separated Values) format, so plenty of other software and
 packages should be able to read it in easily. Your total user statistics are
 stored in a separate file from your work statistics.
 
 
 
 ### Getting Started
 
 The main use case for `AO3StatScraper` is to fetch and display your current AO3
 statistics using scripts provided by `AO3StatScraper`. Currently, there are 4
 scripts:
 
-- `ao3get` : The main script to fetch your AO3 stats.
-- `ao3plot`: Plots the stats stored with `ao3get`
+- `ao3get` : The main script to fetch and display your AO3 stats.
+- `ao3plot`: Plots the stats stored with `ao3get`.
 - `ao3_hits_to_kudos`: List all your works in ascending order of their
   hits/kudos ratio
 - `ao3_purge`: Deletes saved stats such that there is a minumum time between the
   remaining ones
 
+The scripts are discussed in more detail further below.
+
 
 **IMPORTANT**: Before you can run the other scripts, you first need to configure
-`AO3StatScraper`.  This is done by calling `ao3get`. It will launch the
+`AO3StatScraper`. This is done by calling `ao3get`. It will launch the
 configuration dialogue automatically if it hasn't been configured yet. You can
 always re-configure it by invoking `ao3get -c`.
 
 
 
 
 ### `ao3get`
@@ -94,26 +99,30 @@
 - `--config`: Run the configuration dialogue and exit.
 - `--remove-last`: Deletes the last snapshot `ao3get` stored and exits. May come
   in handy if you're nervously re-downloading your stats every minute.
 - `--no-write`: This flag modifies the behavious for `--all` and `--diff`
   running modes. While current stats are fetched from AO3, they won't be written
   into a snapshot.
 
+The list above does not cover all the available options. Please use
+`ao3get --help` to see all the available options.
 
 Using `ao3get` requires you to log in to your AO3 account. You can either type
 in your username and password each time you invoke it, or you can store it with
 `AO3StatScraper`, locked behind a master password. There are no restrictions on
 how sophisticated your master password needs to be, so if you can't be
-inconvenienced, you can even leave it empty.
+inconvenienced, you can even leave it empty. Alternately, you can opt out of
+using a master password at all, although this is not encouraged. But it would
+allow you to e.g. set up an automated way to fetch your stats at regular times.
 
 
 ### `ao3plot`
 
 `ao3plot` will display some simple graphs based on the stored snapshots. It
-never stores snapshots itself, you will need to do that using `ao3get`. 
+never stores snapshots itself, you will need to do that using `ao3get`.
 
 By default, `ao3plot` will ask you to select which work you would like to see
 graphs of stats for. You can also select to plot your total user statistics.
 
 Alternately, you can skip that dialogue by using the following flags:
 
 - `-u`: Show total user statistics.
@@ -133,17 +142,17 @@
 This script just reads in the last stored snapshot and prints out all your works
 in ascending order of their hits/kudos ratio.
 
 
 
 ### `ao3_purge`
 
-In case you find yourself in a situation where you feel you have stored way too 
-many snapshots, `ao3_purge` offers you the option to delete stats snapshots such 
-that there is some minimal time between them. By default, this frequency is set 
+In case you find yourself in a situation where you feel you have stored way too
+many snapshots, `ao3_purge` offers you the option to delete stats snapshots such
+that there is some minimal time between them. By default, this frequency is set
 to 12h. You can provide the frequency you like using the `--frequency` flag.
 
 
 
 
 ## Examples
 
@@ -188,17 +197,14 @@
 
 # Roadmap and Contributing
 
 Help and contributions to maintain and extend this tool are very welcome!
 
 Some ideas what might be added in the future include
 - Writing/reading of file formats other than csv.
-- Option to make the script automatizable so users can make it fetch their stats
-  regularly. The problem here is that it would need to circumvent typing in a
-  password.
 - Maybe add a GUI for CLI-averse users. This tool was always intended to be a
   command line tool on my end. Having never programmed a GUI in my life, I don't
   intend to start now. However, if anybody is willing to pack this up in a nice
   simple portable GUI, you are very welcome and encouraged to do so! I'll gladly
   add it to the repository.
 
 I'm using unix exclusively, so there may be issues on other operating systems.
```

### Comparing `ao3statscraper-0.1.2/ao3statscraper/__init__.py` & `ao3statscraper-0.1.4/ao3statscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/ao3requester.py` & `ao3statscraper-0.1.4/ao3statscraper/ao3requester.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 
 
 class Requester:
     """Requester object
 
-       Mostly lifted from https://github.com/ArmindoFlores/ao3_api
+    Mostly lifted from https://github.com/ArmindoFlores/ao3_api
     """
 
     def __init__(self, rqtw=-1, timew=60):
         """Limits the request rate to prevent HTTP 429 (rate limiting) responses.
         12 request per minute seems to be the limit.
 
         Args:
```

### Comparing `ao3statscraper-0.1.2/ao3statscraper/configuration.py` & `ao3statscraper-0.1.4/ao3statscraper/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,38 +2,48 @@
 
 
 import os
 import platform
 import yaml
 import pathlib
 from getpass import getpass
+from packaging.version import Version
+import datetime
+
 
 from .utils import clear_terminal
 from .pw import get_credentials, read_secrets, store_secrets
+from .__version__ import __version__ as ao3SSversion
+
+
+min_compatible_version = Version("0.1.4")
 
 
 class PlottingConfig(object):
     """
     Configuration for the plotting script.
     """
 
     def __init__(self):
         self.prettify = True
         return
 
 
 class Config(object):
-    store_login = None
     username = "Your AO3 Username"
     password = "Don't type your password in plain text"
 
+    store_login = None
+    use_master_pw = None
+
     ao3dir = None
     datadir = None
     conffile = None
     pklfile = None
+    timestamp = None
 
     plotting = None
 
     def __init__(self, reset_conffile=False):
         """
         Initialize configuration.
         If `reset_conffile` is True, then write a new config file from scratch
@@ -108,14 +118,17 @@
         return
 
     def setup_config_file(self):
         """
         Set up permanent configuration and dump them in the configure file.
         """
 
+        t = datetime.datetime.now()
+        self.timestamp = f"{t.year:04d}-{t.month:02d}-{t.day:02d}-{t.hour:02d}-{t.minute:02d}-{t.second:02d}"
+
         clear_terminal()
         print("Welcome to the configuration setup for the AO3 Stat Scraper.")
         print(
             f"After this setup, a configuration file will be written in `{self.conffile}`"
         )
         print("You can freely modify it on your own without calling this dialogue.")
         print(
@@ -142,26 +155,38 @@
                 print("Too many attempts. Exiting.")
                 quit()
 
         store_login = True
         if store_login_str.startswith(("n", "N")):
             store_login = False
 
+        use_master = True
+        master_pwd = self.timestamp
+
         if store_login:
-            # Grab master password.
             clear_terminal()
-            master_pwd = getpass(
-                "Enter a master password (not your AO3 login password):\n"
-            )
-            clear_terminal()
-            master_pwd2 = getpass("Enter the password again:\n")
-
-            if master_pwd != master_pwd2:
-                print("Error: Passwords do not match.")
-                quit()
+            print("You can store your AO3 login encrypted using a master password.")
+            print("This is strongly recommended.")
+            use_master_str = input("Do you want to set up a master password? [Y/n]\n")
+
+            if use_master_str.startswith(("n", "N")):
+                use_master = False
+
+            if use_master:
+                # Get master password.
+                clear_terminal()
+                master_pwd = getpass(
+                    "Enter a master password (not your AO3 login password):\n"
+                )
+                clear_terminal()
+                master_pwd2 = getpass("Enter the password again:\n")
+
+                if master_pwd != master_pwd2:
+                    print("Error: Passwords do not match.")
+                    quit()
 
             # Grab AO3 credentials.
             username, password = get_credentials()
             # And store them.
             self.set_credentials(username, password)
             store_secrets(master_pwd, username, password, self.pklfile)
 
@@ -172,57 +197,85 @@
             os.mkdir(datadir)
         except FileExistsError:
             pass
 
         # Store the config
         self.datadir = datadir
         self.store_login = store_login
+        self.use_master_pw = use_master
 
         # Now write the config file.
         confdict = {}
         global_conf = {
             "data_directory": self.datadir,
             "store_login": self.store_login,
+            "version": ao3SSversion,
+            "config_time": self.timestamp,
+            "use_master_pw": self.use_master_pw,
         }
 
         confdict = {
             "Globals": global_conf,
         }
 
         ymlfp = open(self.conffile, "w")
         yaml.dump(confdict, ymlfp)
         ymlfp.close()
 
         return
 
     def _read_config_file(self):
+        """
+        Read in contents of the config file.
+        """
         ymlfp = open(self.conffile, "r")
         confdata = yaml.load(ymlfp, Loader=yaml.Loader)
         ymlfp.close()
 
+        refresh_config = False
+        # Catch versions too old to even keep track of config version
+        try:
+            self.store_login = confdata["Globals"]["version"]
+        except KeyError:
+            refresh_config = True
+
+        if Version(ao3SSversion) > min_compatible_version:
+            refresh_config = True
+
+        if refresh_config:
+            print(
+                "ERROR: Your config file is set up for an older version of AO3StatScraper."
+            )
+            print("Please re-configure it using `ao3get -c`")
+            quit(1)
+
         try:
             self.datadir = confdata["Globals"]["data_directory"]
             self.store_login = confdata["Globals"]["store_login"]
+            self.timestamp = confdata["Globals"]["config_time"]
+            self.use_master_pw = confdata["Globals"]["use_master_pw"]
         except KeyError:
             print("ERROR: Some fields are missing from your config file.")
             print("It might be out of date.")
-            print("Re-generate it using `ao3get -c`")
+            print("Re-configure it using `ao3get -c`")
             quit(1)
 
         return
 
     def prep_scrape(self):
         """
         Ensure everything is set for a scrape.
         """
 
         if self.store_login:
-            master_pwd = getpass(
-                "Enter master password (not your AO3 login password):\n"
-            )
+            master_pwd = self.timestamp
+            if self.use_master_pw:
+                master_pwd = getpass(
+                    "Enter master password (not your AO3 login password):\n"
+                )
             username, password = read_secrets(master_pwd, self.pklfile, retry=True)
         else:
             username, password = get_credentials()
 
         self.set_credentials(username, password)
 
         return
```

### Comparing `ao3statscraper-0.1.2/ao3statscraper/plotting.py` & `ao3statscraper-0.1.4/ao3statscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/pw.py` & `ao3statscraper-0.1.4/ao3statscraper/pw.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/scrape.py` & `ao3statscraper-0.1.4/ao3statscraper/scrape.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/scripts/ao3_hits_to_kudos.py` & `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_hits_to_kudos.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/scripts/ao3_purge_stats_data.py` & `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_purge_stats_data.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/scripts/ao3plot.py` & `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3plot.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/scripts/ao3scrape.py` & `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3scrape.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,28 +60,40 @@
         "-n",
         "--no-write",
         action="store_true",
         default=False,
         dest="no_write",
         help="Don't write new stats snapshots after displaying them.",
     )
+    parser.add_argument(
+        "-s",
+        "--show-dir",
+        action="store_true",
+        default=False,
+        dest="showdir",
+        help="Print out directory where data is stored and exit.",
+    )
 
     args = parser.parse_args()
 
     return args
 
 
 def ao3scrape():
     from ..configuration import Config
     from ..statsdata import WorkStatsData, TotStatsData
     from ..scrape import UserSession
 
     args = _parse_scrape_args()
     conf = Config(reset_conffile=args.run_config)
 
+    if args.showdir:
+        print(f"Data directory is '{conf.datadir}'")
+        quit()
+
     if args.remove_last:
         tsfile = TotStatsData.get_latest_dump_filename(conf)
         wsfile = WorkStatsData.get_latest_dump_filename(conf)
 
         print(f"This will remove files {tsfile} and {wsfile}.")
         answer = input("Continue? [y/N] ")
         if answer.startswith(("y", "Y")):
```

### Comparing `ao3statscraper-0.1.2/ao3statscraper/statsdata.py` & `ao3statscraper-0.1.4/ao3statscraper/statsdata.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper/utils.py` & `ao3statscraper-0.1.4/ao3statscraper/utils.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/ao3statscraper.egg-info/PKG-INFO` & `ao3statscraper-0.1.4/ao3statscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.1.2
+Version: 0.1.4
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,16 +686,17 @@
 Classifier: Intended Audience :: End Users/Desktop
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: datetime
 Requires-Dist: lxml
 Requires-Dist: matplotlib>=3.6
-Requires-Dist: pycryptodome>=3.20
+Requires-Dist: packaging
 Requires-Dist: pandas>=2.2.0
+Requires-Dist: pycryptodome>=3.20
 Requires-Dist: pyjson
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: termcolor
 
 # AO3StatScraper
@@ -721,59 +722,64 @@
 
 ```
 py -m pip install ao3statscraper
 ```
 
 
 Alternately, the source code is available on
-[gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper).  On OSX and Linux,
-you can install a local version by cloning the repository using git:
+[gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper).
+you can install a local version by cloning the repository using git.
+On OSX and Linux, you can use:
 
 ```
-git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git
-cd AO3StatScraper  # go into the directory
-python3 -m pip install .
+git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git    # get you the git repository
+cd AO3StatScraper                                                 # go into the directory
+python3 -m pip install .                                          # install package
 ```
 
 
 
 ## User Guide
 
 ### Overview: How It Works
 
-`AO3StatScraper` simply downloads your AO3 stats page (pretty much the same as 
+`AO3StatScraper` simply downloads your AO3 stats page (pretty much the same as
 opening it in your browser and hitting `Save this page...`) and then extract the
 stats from that html content. To be able to access your stats, you need to log
 in to AO3, which is why `AO3StatScraper` will ask you for your username and
 password.
 
-Unless specified otherwise, by default `AO3StatScraper` (i.e. the script
-`ao3get`) will store your current stats as a snapshot. The data is written in
+
+By default `AO3StatScraper` (i.e. the script `ao3get`) will store your current
+stats as a snapshot. This includes both your total user statistics as well as
+your individual work statistics. The data is written in
 the csv (Comma Separated Values) format, so plenty of other software and
 packages should be able to read it in easily. Your total user statistics are
 stored in a separate file from your work statistics.
 
 
 
 ### Getting Started
 
 The main use case for `AO3StatScraper` is to fetch and display your current AO3
 statistics using scripts provided by `AO3StatScraper`. Currently, there are 4
 scripts:
 
-- `ao3get` : The main script to fetch your AO3 stats.
-- `ao3plot`: Plots the stats stored with `ao3get`
+- `ao3get` : The main script to fetch and display your AO3 stats.
+- `ao3plot`: Plots the stats stored with `ao3get`.
 - `ao3_hits_to_kudos`: List all your works in ascending order of their
   hits/kudos ratio
 - `ao3_purge`: Deletes saved stats such that there is a minumum time between the
   remaining ones
 
+The scripts are discussed in more detail further below.
+
 
 **IMPORTANT**: Before you can run the other scripts, you first need to configure
-`AO3StatScraper`.  This is done by calling `ao3get`. It will launch the
+`AO3StatScraper`. This is done by calling `ao3get`. It will launch the
 configuration dialogue automatically if it hasn't been configured yet. You can
 always re-configure it by invoking `ao3get -c`.
 
 
 
 
 ### `ao3get`
@@ -794,26 +800,30 @@
 - `--config`: Run the configuration dialogue and exit.
 - `--remove-last`: Deletes the last snapshot `ao3get` stored and exits. May come
   in handy if you're nervously re-downloading your stats every minute.
 - `--no-write`: This flag modifies the behavious for `--all` and `--diff`
   running modes. While current stats are fetched from AO3, they won't be written
   into a snapshot.
 
+The list above does not cover all the available options. Please use
+`ao3get --help` to see all the available options.
 
 Using `ao3get` requires you to log in to your AO3 account. You can either type
 in your username and password each time you invoke it, or you can store it with
 `AO3StatScraper`, locked behind a master password. There are no restrictions on
 how sophisticated your master password needs to be, so if you can't be
-inconvenienced, you can even leave it empty.
+inconvenienced, you can even leave it empty. Alternately, you can opt out of
+using a master password at all, although this is not encouraged. But it would
+allow you to e.g. set up an automated way to fetch your stats at regular times.
 
 
 ### `ao3plot`
 
 `ao3plot` will display some simple graphs based on the stored snapshots. It
-never stores snapshots itself, you will need to do that using `ao3get`. 
+never stores snapshots itself, you will need to do that using `ao3get`.
 
 By default, `ao3plot` will ask you to select which work you would like to see
 graphs of stats for. You can also select to plot your total user statistics.
 
 Alternately, you can skip that dialogue by using the following flags:
 
 - `-u`: Show total user statistics.
@@ -833,17 +843,17 @@
 This script just reads in the last stored snapshot and prints out all your works
 in ascending order of their hits/kudos ratio.
 
 
 
 ### `ao3_purge`
 
-In case you find yourself in a situation where you feel you have stored way too 
-many snapshots, `ao3_purge` offers you the option to delete stats snapshots such 
-that there is some minimal time between them. By default, this frequency is set 
+In case you find yourself in a situation where you feel you have stored way too
+many snapshots, `ao3_purge` offers you the option to delete stats snapshots such
+that there is some minimal time between them. By default, this frequency is set
 to 12h. You can provide the frequency you like using the `--frequency` flag.
 
 
 
 
 ## Examples
 
@@ -888,17 +898,14 @@
 
 # Roadmap and Contributing
 
 Help and contributions to maintain and extend this tool are very welcome!
 
 Some ideas what might be added in the future include
 - Writing/reading of file formats other than csv.
-- Option to make the script automatizable so users can make it fetch their stats
-  regularly. The problem here is that it would need to circumvent typing in a
-  password.
 - Maybe add a GUI for CLI-averse users. This tool was always intended to be a
   command line tool on my end. Having never programmed a GUI in my life, I don't
   intend to start now. However, if anybody is willing to pack this up in a nice
   simple portable GUI, you are very welcome and encouraged to do so! I'll gladly
   add it to the repository.
 
 I'm using unix exclusively, so there may be issues on other operating systems.
```

### Comparing `ao3statscraper-0.1.2/ao3statscraper.egg-info/SOURCES.txt` & `ao3statscraper-0.1.4/ao3statscraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/pyproject.toml` & `ao3statscraper-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = ["ao3statscraper", "ao3statscraper.scripts"]
 
 
 [project]
 name = "ao3statscraper"
 description="Scrape stats from your AO3 stats page."
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.4"
 authors= [
     { name = "Lars Ikarion", email="lars.ikarion@gmail.com"},
     ]
 license = { file = "LICENSE" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -23,16 +23,17 @@
 ]
 keywords = [ "AO3", "web", "stats", "matplotlib" ]
 dependencies=[ 
     "bs4",
     "datetime",
     "lxml",
     "matplotlib>=3.6", 
-    "pycryptodome>=3.20",
+    "packaging",
     "pandas>=2.2.0",
+    "pycryptodome>=3.20",
     "pyjson",
     "pyyaml",
     "requests",
     "tabulate",
     "termcolor",
     ]
 
@@ -44,15 +45,15 @@
 ao3get= "ao3statscraper.scripts:ao3scrape"
 
 
 [project.urls]
 "Homepage" = "https://gitlab.com/athenaslilowl1/AO3StatScraper"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ao3statscraper-0.1.2/tests/test_passwords.py` & `ao3statscraper-0.1.4/tests/test_passwords.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.2/tests/test_writing_data.py` & `ao3statscraper-0.1.4/tests/test_writing_data.py`

 * *Files identical despite different names*

