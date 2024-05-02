# Comparing `tmp/pwebarc-wrrarms-0.8.1.tar.gz` & `tmp/pwebarc-wrrarms-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwebarc-wrrarms-0.8.1.tar", last modified: Tue Mar 12 14:20:01 2024, max compression
+gzip compressed data, was "pwebarc-wrrarms-0.9.0.tar", last modified: Fri Mar 22 15:27:39 2024, max compression
```

## Comparing `pwebarc-wrrarms-0.8.1.tar` & `pwebarc-wrrarms-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-12 14:20:01.465525 pwebarc-wrrarms-0.8.1/
--rw-------   0 oxij      (1000) oxij      (1000)    40603 2024-03-12 14:20:01.465525 pwebarc-wrrarms-0.8.1/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)    39402 2024-03-12 09:45:43.000000 pwebarc-wrrarms-0.8.1/README.md
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-12 14:20:01.461525 pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/
--rw-------   0 oxij      (1000) oxij      (1000)    40603 2024-03-12 14:20:01.000000 pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)      410 2024-03-12 14:20:01.000000 pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/SOURCES.txt
--rw-------   0 oxij      (1000) oxij      (1000)        1 2024-03-12 14:20:01.000000 pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/dependency_links.txt
--rw-------   0 oxij      (1000) oxij      (1000)       50 2024-03-12 14:20:01.000000 pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/entry_points.txt
--rw-------   0 oxij      (1000) oxij      (1000)       21 2024-03-12 14:20:01.000000 pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/requires.txt
--rw-------   0 oxij      (1000) oxij      (1000)        8 2024-03-12 14:20:01.000000 pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/top_level.txt
--rw-------   0 oxij      (1000) oxij      (1000)     1438 2024-03-12 09:45:43.000000 pwebarc-wrrarms-0.8.1/pyproject.toml
--rw-------   0 oxij      (1000) oxij      (1000)       38 2024-03-12 14:20:01.465525 pwebarc-wrrarms-0.8.1/setup.cfg
--rw-------   0 oxij      (1000) oxij      (1000)       60 2023-11-22 20:16:29.000000 pwebarc-wrrarms-0.8.1/setup.py
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-12 14:20:01.464525 pwebarc-wrrarms-0.8.1/wrrarms/
--rw-------   0 oxij      (1000) oxij      (1000)      732 2024-03-08 17:27:59.000000 pwebarc-wrrarms-0.8.1/wrrarms/__init__.py
--rw-------   0 oxij      (1000) oxij      (1000)    60325 2024-03-12 09:45:43.000000 pwebarc-wrrarms-0.8.1/wrrarms/__main__.py
--rw-------   0 oxij      (1000) oxij      (1000)    13129 2024-03-12 09:45:43.000000 pwebarc-wrrarms-0.8.1/wrrarms/io.py
--rw-------   0 oxij      (1000) oxij      (1000)     9083 2024-03-11 09:03:23.000000 pwebarc-wrrarms-0.8.1/wrrarms/linst.py
--rw-------   0 oxij      (1000) oxij      (1000)     4451 2024-03-11 09:04:18.000000 pwebarc-wrrarms-0.8.1/wrrarms/mitmproxy.py
--rw-------   0 oxij      (1000) oxij      (1000)    13639 2024-03-11 09:03:23.000000 pwebarc-wrrarms-0.8.1/wrrarms/output.py
--rw-------   0 oxij      (1000) oxij      (1000)     2482 2024-03-11 09:03:23.000000 pwebarc-wrrarms-0.8.1/wrrarms/type.py
--rw-------   0 oxij      (1000) oxij      (1000)    23457 2024-03-12 06:45:17.000000 pwebarc-wrrarms-0.8.1/wrrarms/wrr.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-22 15:27:39.088163 pwebarc-wrrarms-0.9.0/
+-rw-r--r--   0 oxij      (1000) oxij      (1000)    40780 2024-03-22 15:27:39.088163 pwebarc-wrrarms-0.9.0/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)    39513 2024-03-22 15:23:00.000000 pwebarc-wrrarms-0.9.0/README.md
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-22 15:27:39.088163 pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/
+-rw-r--r--   0 oxij      (1000) oxij      (1000)    40780 2024-03-22 15:27:39.000000 pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)      410 2024-03-22 15:27:39.000000 pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/SOURCES.txt
+-rw-------   0 oxij      (1000) oxij      (1000)        1 2024-03-22 15:27:39.000000 pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/dependency_links.txt
+-rw-------   0 oxij      (1000) oxij      (1000)       50 2024-03-22 15:27:39.000000 pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/entry_points.txt
+-rw-------   0 oxij      (1000) oxij      (1000)       21 2024-03-22 15:27:39.000000 pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/requires.txt
+-rw-------   0 oxij      (1000) oxij      (1000)        8 2024-03-22 15:27:39.000000 pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/top_level.txt
+-rw-------   0 oxij      (1000) oxij      (1000)     1438 2024-03-22 15:23:00.000000 pwebarc-wrrarms-0.9.0/pyproject.toml
+-rw-------   0 oxij      (1000) oxij      (1000)       38 2024-03-22 15:27:39.088163 pwebarc-wrrarms-0.9.0/setup.cfg
+-rw-------   0 oxij      (1000) oxij      (1000)       60 2023-11-22 20:16:29.000000 pwebarc-wrrarms-0.9.0/setup.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-22 15:27:39.087162 pwebarc-wrrarms-0.9.0/wrrarms/
+-rw-------   0 oxij      (1000) oxij      (1000)      732 2024-03-08 17:27:59.000000 pwebarc-wrrarms-0.9.0/wrrarms/__init__.py
+-rw-------   0 oxij      (1000) oxij      (1000)    60036 2024-03-22 15:23:00.000000 pwebarc-wrrarms-0.9.0/wrrarms/__main__.py
+-rw-------   0 oxij      (1000) oxij      (1000)    13129 2024-03-22 15:15:52.000000 pwebarc-wrrarms-0.9.0/wrrarms/io.py
+-rw-------   0 oxij      (1000) oxij      (1000)     9117 2024-03-22 15:23:00.000000 pwebarc-wrrarms-0.9.0/wrrarms/linst.py
+-rw-------   0 oxij      (1000) oxij      (1000)     4451 2024-03-11 09:04:18.000000 pwebarc-wrrarms-0.9.0/wrrarms/mitmproxy.py
+-rw-------   0 oxij      (1000) oxij      (1000)    13573 2024-03-22 15:23:00.000000 pwebarc-wrrarms-0.9.0/wrrarms/output.py
+-rw-------   0 oxij      (1000) oxij      (1000)     2490 2024-03-22 15:23:00.000000 pwebarc-wrrarms-0.9.0/wrrarms/type.py
+-rw-------   0 oxij      (1000) oxij      (1000)    24676 2024-03-22 15:23:00.000000 pwebarc-wrrarms-0.9.0/wrrarms/wrr.py
```

### Comparing `pwebarc-wrrarms-0.8.1/PKG-INFO` & `pwebarc-wrrarms-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwebarc-wrrarms
-Version: 0.8.1
+Version: 0.9.0
 Summary: A tool for displaying and manipulating Web Request+Response (WRR) files of Private Passive Web Archive (pwebarc) project
 Author-email: Jan Malakhovski <oxij@oxij.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://oxij.org/software/pwebarc/
 Project-URL: GitHub, https://github.com/Own-Data-Privateer/pwebarc
 Project-URL: Support Development, https://oxij.org/#support
 Keywords: HTTP,HTTPS,archive,wayback machine,download
@@ -19,14 +19,17 @@
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: kisstdlib
+Requires-Dist: cbor2
+Requires-Dist: idna
 
 # What?
 
 `wrrarms` (`pwebarc-wrrarms`) is a tool for displaying and manipulating [Personal Private Passive Web Archive (pwebarc)](https://github.com/Own-Data-Privateer/pwebarc/) (also [there](https://oxij.org/software/pwebarc/)) Web Request+Response (WRR) files produced by [pWebArc browser extension](https://github.com/Own-Data-Privateer/pwebarc/tree/master/extension/) (also [there](https://oxij.org/software/pwebarc/tree/master/extension/)).
 
 # Quickstart
 
@@ -198,16 +201,16 @@
       - `sha256`: compute `hex(sha256(value.encode("utf-8"))`
       - `==`: apply `== arg`, `arg` is cast to the same type as the current value
       - `!=`: apply `!= arg`, similarly
       - `<`: apply `< arg`, similarly
       - `<=`: apply `<= arg`, similarly
       - `>`: apply `> arg`, similarly
       - `>=`: apply `>= arg`, similarly
-      - `prefix`: take first `arg` characters
-      - `suffix`: take last `arg` characters
+      - `prefix`: take first `arg` characters or list elements
+      - `suffix`: take last `arg` characters or list elements
       - `abbrev`: leave the current value as if if its length is less or equal than `arg` characters, otherwise take first `arg/2` followed by last `arg/2` characters
       - `abbrev_each`: `abbrev arg` each element in a value `list`
       - `replace`: replace all occurences of the first argument in the current value with the second argument, casts arguments to the same type as the current value
       - `pp_to_path`: encode `path_parts` `list` into a POSIX path, quoting as little as needed
       - `qsl_urlencode`: encode parsed `query` `list` into a URL's query component `str`
       - `qsl_to_path`: encode `query` `list` into a POSIX path, quoting as little as needed
     - reqres fields, these work the same way as constants above, i.e. they replace current value of `None` with field's value, if reqres is missing the field in question, which could happen for `response*` fields, the result is `None`:
@@ -257,35 +260,39 @@
       - `fhour`: similar to `shour`, but for `ftime`; int
       - `fminute`: similar to `sminute`, but for `ftime`; int
       - `fsecond`: similar to `ssecond`, but for `ftime`; int
       - `status`: `"NR"` if there was no response, `str(response.code) + "C"` if response was complete, `str(response.code) + "N"` otherwise; str
       - `method`: aliast for `request.method`; str
       - `raw_url`: aliast for `request.url`; str
       - `net_url`: `raw_url` with Punycode UTS46 IDNA encoded hostname, unsafe characters quoted, and without the fragment/hash part; this is the URL that actually gets sent to the server; str
+      - `pretty_url`: `raw_url`, but using `hostname`, `mq_path`, and `mq_nquery`; str
       - `scheme`: scheme part of `raw_url`; e.g. `http`, `https`, etc; str
       - `raw_hostname`: hostname part of `raw_url` as it is recorded in the reqres; str
       - `net_hostname`: hostname part of `raw_url`, encoded as Punycode UTS46 IDNA; this is what actually gets sent to the server; ASCII str
-      - `hostname`: `net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; str
+      - `hostname`: `net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; UNICODE str
       - `rhostname`: `hostname` with the order of its parts reversed; e.g. `"www.example.org"` -> `"com.example.www"`; str
       - `port`: port part of `raw_url`; int or None
       - `netloc`: netloc part of `raw_url`; i.e., in the most general case, `<username>:<password>@<hostname>:<port>`; str
       - `raw_path`: raw path part of `raw_url` as it is recorded is the reqres; e.g. `"https://www.example.org"` -> `""`, `"https://www.example.org/"` -> `"/"`, `"https://www.example.org/index.html"` -> `"/index.html"`; str
       - `path_parts`: component-wise unquoted "/"-split `raw_path` with empty components removed and dots and double dots interpreted away; e.g. `"https://www.example.org"` -> `[]`, `"https://www.example.org/"` -> `[]`, `"https://www.example.org/index.html"` -> `["index.html"]` , `"https://www.example.org/skipped/.//../used/"` -> `["used"]; list[str]
+      - `mq_path`: `path_parts` turned back into a minimally-quoted string; str
       - `wget_parts`: `path + ["index.html"]` if `raw_path` ends in a slash, `path` otherwise; this is what `wget` does in `wget -mpk`; list[str]
       - `raw_query`: query part of `raw_url` (i.e. everything after the `?` character and before the `#` character) as it is recorded in the reqres; str
       - `query_parts`: parsed (and component-wise unquoted) `raw_query`; list[tuple[str, str]]
       - `query_ne_parts`: `query_parts` with empty query parameters removed; list[tuple[str, str]]
+      - `mq_query`: `query_parts` turned back into a minimally-quoted string; str
+      - `mq_nquery`: `query_ne_parts` turned back into a minimally-quoted string; str
       - `oqm`: optional query mark: `?` character if `query` is non-empty, an empty string otherwise; str
       - `fragment`: fragment (hash) part of the url; str
       - `ofm`: optional fragment mark: `#` character if `fragment` is non-empty, an empty string otherwise; str
     - a compound expression built by piping (`|`) the above, for example:
       - `net_url|sha256`
       - `net_url|sha256|prefix 4`
-      - `path_parts|pp_to_path`
-      - `query_parts|qsl_to_path|abbrev 128`
+      - `path_parts|prefix 3|pp_to_path`
+      - `query_parts|prefix 3|qsl_to_path|abbrev 128`
       - `response.complete`: this will print the value of `response.complete` or `None`, if there was no response
       - `response.complete|false`: this will print `response.complete` or `False`
       - `response.body|eb`: this will print `response.body` or an empty string, if there was no response
 
 - output:
   - `--not-terminated`
   : don't terminate output values with anything, just concatenate them (default)
@@ -304,15 +311,15 @@
   - `ARG`
   : additional arguments to give to the COMMAND
   - `PATH`
   : input WRR file paths to be mapped into new temporary files
 
 - options:
   - `-e EXPR, --expr EXPR`
-  : the expression to compute, can be specified multiple times, see `{__package__} get --expr` for more info; (default: `response.body|es`)
+  : the expression to compute, can be specified multiple times, see `wrrarms get --expr` for more info; (default: `response.body|es`)
   - `-n NUM, --num-args NUM`
   : number of `PATH`s (default: `1`)
 
 - output:
   - `--not-terminated`
   : don't terminate output values with anything, just concatenate them (default)
   - `-l, --lf-terminated`
@@ -441,38 +448,38 @@
   - `-q, --quiet`
   : don't log computed updates to stderr
   - `-t DESTINATION, --to DESTINATION`
   : destination directory, when unset each source `PATH` must be a directory which will be treated as its own `DESTINATION`
   - `-o FORMAT, --output FORMAT`
   : format describing generated output paths, an alias name or "format:" followed by a custom pythonic %-substitution string:
     - available aliases and corresponding %-substitutions:
-      - `default`: `%(syear)d/%(smonth)02d/%(sday)02d/%(shour)02d%(sminute)02d%(ssecond)02d%(stime_msq)03d_%(qtime_ms)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s_%(hostname)s.%(num)d.wrr` (default)
-      - `short`: `%(syear)d/%(smonth)02d/%(sday)02d/%(stime_ms)d_%(qtime_ms)s.%(num)d.wrr`
-      - `surl`: `%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s`
-      - `url`: `%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s`
-      - `surl_msn`: `%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `url_msn`: `%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shpq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hpq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shpq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hpq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shupq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hupq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shupq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hupq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `srhupq`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `rhupq`: `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `srhupq_msn`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `rhupq_msn`: `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shupnq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hupnq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shupnq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hupnq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `flat`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr`
-      - `flat_n`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr`
+      - `default`    : `%(syear)d/%(smonth)02d/%(sday)02d/%(shour)02d%(sminute)02d%(ssecond)02d%(stime_msq)03d_%(qtime_ms)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s_%(hostname)s.%(num)d.wrr` (default)
+      - `short`      : `%(syear)d/%(smonth)02d/%(sday)02d/%(stime_ms)d_%(qtime_ms)s.%(num)d.wrr`
+      - `surl`       : `%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s`
+      - `surl_msn`   : `%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `shupq`      : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `shupq_msn`  : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `shupnq`     : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `shupnq_msn` : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `srhupq`     : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `srhupq_msn` : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `srhupnq`    : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `srhupnq_msn`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `url`        : `%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s`
+      - `url_msn`    : `%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `hupq`       : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `hupq_msn`   : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `hupnq`      : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `hupnq_msn`  : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `rhupq`      : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `rhupq_msn`  : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `rhupnq`     : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `rhupnq_msn` : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `flat`       : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr`
+      - `flat_n`     : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr`
     - available substitutions:
       - `num`: number of times the resulting output path was encountered before; adding this parameter to your `--output` format will ensure all generated file names will be unique
       - all expressions of `wrrarms get --expr`, which see
   - `--stdin0`
   : read zero-terminated `PATH`s from stdin, these will be processed after `PATH`s specified as command-line arguments
 
 - error handling:
```

### Comparing `pwebarc-wrrarms-0.8.1/README.md` & `pwebarc-wrrarms-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -172,16 +172,16 @@
       - `sha256`: compute `hex(sha256(value.encode("utf-8"))`
       - `==`: apply `== arg`, `arg` is cast to the same type as the current value
       - `!=`: apply `!= arg`, similarly
       - `<`: apply `< arg`, similarly
       - `<=`: apply `<= arg`, similarly
       - `>`: apply `> arg`, similarly
       - `>=`: apply `>= arg`, similarly
-      - `prefix`: take first `arg` characters
-      - `suffix`: take last `arg` characters
+      - `prefix`: take first `arg` characters or list elements
+      - `suffix`: take last `arg` characters or list elements
       - `abbrev`: leave the current value as if if its length is less or equal than `arg` characters, otherwise take first `arg/2` followed by last `arg/2` characters
       - `abbrev_each`: `abbrev arg` each element in a value `list`
       - `replace`: replace all occurences of the first argument in the current value with the second argument, casts arguments to the same type as the current value
       - `pp_to_path`: encode `path_parts` `list` into a POSIX path, quoting as little as needed
       - `qsl_urlencode`: encode parsed `query` `list` into a URL's query component `str`
       - `qsl_to_path`: encode `query` `list` into a POSIX path, quoting as little as needed
     - reqres fields, these work the same way as constants above, i.e. they replace current value of `None` with field's value, if reqres is missing the field in question, which could happen for `response*` fields, the result is `None`:
@@ -231,35 +231,39 @@
       - `fhour`: similar to `shour`, but for `ftime`; int
       - `fminute`: similar to `sminute`, but for `ftime`; int
       - `fsecond`: similar to `ssecond`, but for `ftime`; int
       - `status`: `"NR"` if there was no response, `str(response.code) + "C"` if response was complete, `str(response.code) + "N"` otherwise; str
       - `method`: aliast for `request.method`; str
       - `raw_url`: aliast for `request.url`; str
       - `net_url`: `raw_url` with Punycode UTS46 IDNA encoded hostname, unsafe characters quoted, and without the fragment/hash part; this is the URL that actually gets sent to the server; str
+      - `pretty_url`: `raw_url`, but using `hostname`, `mq_path`, and `mq_nquery`; str
       - `scheme`: scheme part of `raw_url`; e.g. `http`, `https`, etc; str
       - `raw_hostname`: hostname part of `raw_url` as it is recorded in the reqres; str
       - `net_hostname`: hostname part of `raw_url`, encoded as Punycode UTS46 IDNA; this is what actually gets sent to the server; ASCII str
-      - `hostname`: `net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; str
+      - `hostname`: `net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; UNICODE str
       - `rhostname`: `hostname` with the order of its parts reversed; e.g. `"www.example.org"` -> `"com.example.www"`; str
       - `port`: port part of `raw_url`; int or None
       - `netloc`: netloc part of `raw_url`; i.e., in the most general case, `<username>:<password>@<hostname>:<port>`; str
       - `raw_path`: raw path part of `raw_url` as it is recorded is the reqres; e.g. `"https://www.example.org"` -> `""`, `"https://www.example.org/"` -> `"/"`, `"https://www.example.org/index.html"` -> `"/index.html"`; str
       - `path_parts`: component-wise unquoted "/"-split `raw_path` with empty components removed and dots and double dots interpreted away; e.g. `"https://www.example.org"` -> `[]`, `"https://www.example.org/"` -> `[]`, `"https://www.example.org/index.html"` -> `["index.html"]` , `"https://www.example.org/skipped/.//../used/"` -> `["used"]; list[str]
+      - `mq_path`: `path_parts` turned back into a minimally-quoted string; str
       - `wget_parts`: `path + ["index.html"]` if `raw_path` ends in a slash, `path` otherwise; this is what `wget` does in `wget -mpk`; list[str]
       - `raw_query`: query part of `raw_url` (i.e. everything after the `?` character and before the `#` character) as it is recorded in the reqres; str
       - `query_parts`: parsed (and component-wise unquoted) `raw_query`; list[tuple[str, str]]
       - `query_ne_parts`: `query_parts` with empty query parameters removed; list[tuple[str, str]]
+      - `mq_query`: `query_parts` turned back into a minimally-quoted string; str
+      - `mq_nquery`: `query_ne_parts` turned back into a minimally-quoted string; str
       - `oqm`: optional query mark: `?` character if `query` is non-empty, an empty string otherwise; str
       - `fragment`: fragment (hash) part of the url; str
       - `ofm`: optional fragment mark: `#` character if `fragment` is non-empty, an empty string otherwise; str
     - a compound expression built by piping (`|`) the above, for example:
       - `net_url|sha256`
       - `net_url|sha256|prefix 4`
-      - `path_parts|pp_to_path`
-      - `query_parts|qsl_to_path|abbrev 128`
+      - `path_parts|prefix 3|pp_to_path`
+      - `query_parts|prefix 3|qsl_to_path|abbrev 128`
       - `response.complete`: this will print the value of `response.complete` or `None`, if there was no response
       - `response.complete|false`: this will print `response.complete` or `False`
       - `response.body|eb`: this will print `response.body` or an empty string, if there was no response
 
 - output:
   - `--not-terminated`
   : don't terminate output values with anything, just concatenate them (default)
@@ -278,15 +282,15 @@
   - `ARG`
   : additional arguments to give to the COMMAND
   - `PATH`
   : input WRR file paths to be mapped into new temporary files
 
 - options:
   - `-e EXPR, --expr EXPR`
-  : the expression to compute, can be specified multiple times, see `{__package__} get --expr` for more info; (default: `response.body|es`)
+  : the expression to compute, can be specified multiple times, see `wrrarms get --expr` for more info; (default: `response.body|es`)
   - `-n NUM, --num-args NUM`
   : number of `PATH`s (default: `1`)
 
 - output:
   - `--not-terminated`
   : don't terminate output values with anything, just concatenate them (default)
   - `-l, --lf-terminated`
@@ -415,38 +419,38 @@
   - `-q, --quiet`
   : don't log computed updates to stderr
   - `-t DESTINATION, --to DESTINATION`
   : destination directory, when unset each source `PATH` must be a directory which will be treated as its own `DESTINATION`
   - `-o FORMAT, --output FORMAT`
   : format describing generated output paths, an alias name or "format:" followed by a custom pythonic %-substitution string:
     - available aliases and corresponding %-substitutions:
-      - `default`: `%(syear)d/%(smonth)02d/%(sday)02d/%(shour)02d%(sminute)02d%(ssecond)02d%(stime_msq)03d_%(qtime_ms)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s_%(hostname)s.%(num)d.wrr` (default)
-      - `short`: `%(syear)d/%(smonth)02d/%(sday)02d/%(stime_ms)d_%(qtime_ms)s.%(num)d.wrr`
-      - `surl`: `%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s`
-      - `url`: `%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s`
-      - `surl_msn`: `%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `url_msn`: `%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shpq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hpq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shpq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hpq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shupq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hupq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shupq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hupq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `srhupq`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `rhupq`: `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `srhupq_msn`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `rhupq_msn`: `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shupnq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hupnq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shupnq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hupnq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `flat`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr`
-      - `flat_n`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr`
+      - `default`    : `%(syear)d/%(smonth)02d/%(sday)02d/%(shour)02d%(sminute)02d%(ssecond)02d%(stime_msq)03d_%(qtime_ms)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s_%(hostname)s.%(num)d.wrr` (default)
+      - `short`      : `%(syear)d/%(smonth)02d/%(sday)02d/%(stime_ms)d_%(qtime_ms)s.%(num)d.wrr`
+      - `surl`       : `%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s`
+      - `surl_msn`   : `%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `shupq`      : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `shupq_msn`  : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `shupnq`     : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `shupnq_msn` : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `srhupq`     : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `srhupq_msn` : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `srhupnq`    : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `srhupnq_msn`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `url`        : `%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s`
+      - `url_msn`    : `%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `hupq`       : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `hupq_msn`   : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `hupnq`      : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `hupnq_msn`  : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `rhupq`      : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `rhupq_msn`  : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `rhupnq`     : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `rhupnq_msn` : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `flat`       : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr`
+      - `flat_n`     : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr`
     - available substitutions:
       - `num`: number of times the resulting output path was encountered before; adding this parameter to your `--output` format will ensure all generated file names will be unique
       - all expressions of `wrrarms get --expr`, which see
   - `--stdin0`
   : read zero-terminated `PATH`s from stdin, these will be processed after `PATH`s specified as command-line arguments
 
 - error handling:
```

### Comparing `pwebarc-wrrarms-0.8.1/pwebarc_wrrarms.egg-info/PKG-INFO` & `pwebarc-wrrarms-0.9.0/pwebarc_wrrarms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwebarc-wrrarms
-Version: 0.8.1
+Version: 0.9.0
 Summary: A tool for displaying and manipulating Web Request+Response (WRR) files of Private Passive Web Archive (pwebarc) project
 Author-email: Jan Malakhovski <oxij@oxij.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://oxij.org/software/pwebarc/
 Project-URL: GitHub, https://github.com/Own-Data-Privateer/pwebarc
 Project-URL: Support Development, https://oxij.org/#support
 Keywords: HTTP,HTTPS,archive,wayback machine,download
@@ -19,14 +19,17 @@
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: kisstdlib
+Requires-Dist: cbor2
+Requires-Dist: idna
 
 # What?
 
 `wrrarms` (`pwebarc-wrrarms`) is a tool for displaying and manipulating [Personal Private Passive Web Archive (pwebarc)](https://github.com/Own-Data-Privateer/pwebarc/) (also [there](https://oxij.org/software/pwebarc/)) Web Request+Response (WRR) files produced by [pWebArc browser extension](https://github.com/Own-Data-Privateer/pwebarc/tree/master/extension/) (also [there](https://oxij.org/software/pwebarc/tree/master/extension/)).
 
 # Quickstart
 
@@ -198,16 +201,16 @@
       - `sha256`: compute `hex(sha256(value.encode("utf-8"))`
       - `==`: apply `== arg`, `arg` is cast to the same type as the current value
       - `!=`: apply `!= arg`, similarly
       - `<`: apply `< arg`, similarly
       - `<=`: apply `<= arg`, similarly
       - `>`: apply `> arg`, similarly
       - `>=`: apply `>= arg`, similarly
-      - `prefix`: take first `arg` characters
-      - `suffix`: take last `arg` characters
+      - `prefix`: take first `arg` characters or list elements
+      - `suffix`: take last `arg` characters or list elements
       - `abbrev`: leave the current value as if if its length is less or equal than `arg` characters, otherwise take first `arg/2` followed by last `arg/2` characters
       - `abbrev_each`: `abbrev arg` each element in a value `list`
       - `replace`: replace all occurences of the first argument in the current value with the second argument, casts arguments to the same type as the current value
       - `pp_to_path`: encode `path_parts` `list` into a POSIX path, quoting as little as needed
       - `qsl_urlencode`: encode parsed `query` `list` into a URL's query component `str`
       - `qsl_to_path`: encode `query` `list` into a POSIX path, quoting as little as needed
     - reqres fields, these work the same way as constants above, i.e. they replace current value of `None` with field's value, if reqres is missing the field in question, which could happen for `response*` fields, the result is `None`:
@@ -257,35 +260,39 @@
       - `fhour`: similar to `shour`, but for `ftime`; int
       - `fminute`: similar to `sminute`, but for `ftime`; int
       - `fsecond`: similar to `ssecond`, but for `ftime`; int
       - `status`: `"NR"` if there was no response, `str(response.code) + "C"` if response was complete, `str(response.code) + "N"` otherwise; str
       - `method`: aliast for `request.method`; str
       - `raw_url`: aliast for `request.url`; str
       - `net_url`: `raw_url` with Punycode UTS46 IDNA encoded hostname, unsafe characters quoted, and without the fragment/hash part; this is the URL that actually gets sent to the server; str
+      - `pretty_url`: `raw_url`, but using `hostname`, `mq_path`, and `mq_nquery`; str
       - `scheme`: scheme part of `raw_url`; e.g. `http`, `https`, etc; str
       - `raw_hostname`: hostname part of `raw_url` as it is recorded in the reqres; str
       - `net_hostname`: hostname part of `raw_url`, encoded as Punycode UTS46 IDNA; this is what actually gets sent to the server; ASCII str
-      - `hostname`: `net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; str
+      - `hostname`: `net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; UNICODE str
       - `rhostname`: `hostname` with the order of its parts reversed; e.g. `"www.example.org"` -> `"com.example.www"`; str
       - `port`: port part of `raw_url`; int or None
       - `netloc`: netloc part of `raw_url`; i.e., in the most general case, `<username>:<password>@<hostname>:<port>`; str
       - `raw_path`: raw path part of `raw_url` as it is recorded is the reqres; e.g. `"https://www.example.org"` -> `""`, `"https://www.example.org/"` -> `"/"`, `"https://www.example.org/index.html"` -> `"/index.html"`; str
       - `path_parts`: component-wise unquoted "/"-split `raw_path` with empty components removed and dots and double dots interpreted away; e.g. `"https://www.example.org"` -> `[]`, `"https://www.example.org/"` -> `[]`, `"https://www.example.org/index.html"` -> `["index.html"]` , `"https://www.example.org/skipped/.//../used/"` -> `["used"]; list[str]
+      - `mq_path`: `path_parts` turned back into a minimally-quoted string; str
       - `wget_parts`: `path + ["index.html"]` if `raw_path` ends in a slash, `path` otherwise; this is what `wget` does in `wget -mpk`; list[str]
       - `raw_query`: query part of `raw_url` (i.e. everything after the `?` character and before the `#` character) as it is recorded in the reqres; str
       - `query_parts`: parsed (and component-wise unquoted) `raw_query`; list[tuple[str, str]]
       - `query_ne_parts`: `query_parts` with empty query parameters removed; list[tuple[str, str]]
+      - `mq_query`: `query_parts` turned back into a minimally-quoted string; str
+      - `mq_nquery`: `query_ne_parts` turned back into a minimally-quoted string; str
       - `oqm`: optional query mark: `?` character if `query` is non-empty, an empty string otherwise; str
       - `fragment`: fragment (hash) part of the url; str
       - `ofm`: optional fragment mark: `#` character if `fragment` is non-empty, an empty string otherwise; str
     - a compound expression built by piping (`|`) the above, for example:
       - `net_url|sha256`
       - `net_url|sha256|prefix 4`
-      - `path_parts|pp_to_path`
-      - `query_parts|qsl_to_path|abbrev 128`
+      - `path_parts|prefix 3|pp_to_path`
+      - `query_parts|prefix 3|qsl_to_path|abbrev 128`
       - `response.complete`: this will print the value of `response.complete` or `None`, if there was no response
       - `response.complete|false`: this will print `response.complete` or `False`
       - `response.body|eb`: this will print `response.body` or an empty string, if there was no response
 
 - output:
   - `--not-terminated`
   : don't terminate output values with anything, just concatenate them (default)
@@ -304,15 +311,15 @@
   - `ARG`
   : additional arguments to give to the COMMAND
   - `PATH`
   : input WRR file paths to be mapped into new temporary files
 
 - options:
   - `-e EXPR, --expr EXPR`
-  : the expression to compute, can be specified multiple times, see `{__package__} get --expr` for more info; (default: `response.body|es`)
+  : the expression to compute, can be specified multiple times, see `wrrarms get --expr` for more info; (default: `response.body|es`)
   - `-n NUM, --num-args NUM`
   : number of `PATH`s (default: `1`)
 
 - output:
   - `--not-terminated`
   : don't terminate output values with anything, just concatenate them (default)
   - `-l, --lf-terminated`
@@ -441,38 +448,38 @@
   - `-q, --quiet`
   : don't log computed updates to stderr
   - `-t DESTINATION, --to DESTINATION`
   : destination directory, when unset each source `PATH` must be a directory which will be treated as its own `DESTINATION`
   - `-o FORMAT, --output FORMAT`
   : format describing generated output paths, an alias name or "format:" followed by a custom pythonic %-substitution string:
     - available aliases and corresponding %-substitutions:
-      - `default`: `%(syear)d/%(smonth)02d/%(sday)02d/%(shour)02d%(sminute)02d%(ssecond)02d%(stime_msq)03d_%(qtime_ms)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s_%(hostname)s.%(num)d.wrr` (default)
-      - `short`: `%(syear)d/%(smonth)02d/%(sday)02d/%(stime_ms)d_%(qtime_ms)s.%(num)d.wrr`
-      - `surl`: `%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s`
-      - `url`: `%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s`
-      - `surl_msn`: `%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `url_msn`: `%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shpq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hpq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shpq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hpq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shupq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hupq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shupq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hupq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `srhupq`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `rhupq`: `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `srhupq_msn`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `rhupq_msn`: `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `shupnq`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `hupnq`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr`
-      - `shupnq_msn`: `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `hupnq_msn`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
-      - `flat`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr`
-      - `flat_n`: `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr`
+      - `default`    : `%(syear)d/%(smonth)02d/%(sday)02d/%(shour)02d%(sminute)02d%(ssecond)02d%(stime_msq)03d_%(qtime_ms)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s_%(hostname)s.%(num)d.wrr` (default)
+      - `short`      : `%(syear)d/%(smonth)02d/%(sday)02d/%(stime_ms)d_%(qtime_ms)s.%(num)d.wrr`
+      - `surl`       : `%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s`
+      - `surl_msn`   : `%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `shupq`      : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `shupq_msn`  : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `shupnq`     : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `shupnq_msn` : `%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `srhupq`     : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `srhupq_msn` : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `srhupnq`    : `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `srhupnq_msn`: `%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `url`        : `%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s`
+      - `url_msn`    : `%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `hupq`       : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `hupq_msn`   : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `hupnq`      : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `hupnq_msn`  : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `rhupq`      : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr`
+      - `rhupq_msn`  : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `rhupnq`     : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr`
+      - `rhupnq_msn` : `%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr`
+      - `flat`       : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr`
+      - `flat_n`     : `%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr`
     - available substitutions:
       - `num`: number of times the resulting output path was encountered before; adding this parameter to your `--output` format will ensure all generated file names will be unique
       - all expressions of `wrrarms get --expr`, which see
   - `--stdin0`
   : read zero-terminated `PATH`s from stdin, these will be processed after `PATH`s specified as command-line arguments
 
 - error handling:
```

### Comparing `pwebarc-wrrarms-0.8.1/pyproject.toml` & `pwebarc-wrrarms-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [tool.setuptools]
 packages = ["wrrarms"]
 [project]
 name = "pwebarc-wrrarms"
-version = "0.8.1"
+version = "0.9.0"
 authors = [{ name = "Jan Malakhovski", email = "oxij@oxij.org" }]
 description = "A tool for displaying and manipulating Web Request+Response (WRR) files of Private Passive Web Archive (pwebarc) project"
 readme = "README.md"
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
```

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/__init__.py` & `pwebarc-wrrarms-0.9.0/wrrarms/__init__.py`

 * *Files identical despite different names*

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/__main__.py` & `pwebarc-wrrarms-0.9.0/wrrarms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,26 +211,30 @@
         if not filters_allow(cargs, rrexpr): return
 
         wrr_pprint(stdout, rrexpr.reqres, abs_in_path, cargs.abridged)
         stdout.flush()
 
     map_wrr_paths(emit, cargs.paths, order_by=cargs.walk_fs, errors=cargs.errors)
 
+default_get_expr = "response.body|es"
 def cmd_get(cargs : _t.Any) -> None:
     if len(cargs.exprs) == 0:
-        cargs.exprs = ["response.body|es"]
+        cargs.exprs = [default_get_expr]
 
     abs_path = _os.path.abspath(_os.path.expanduser(cargs.path))
     rrexpr = wrr_loadf_expr(abs_path)
     for expr in cargs.exprs:
         data = get_bytes(expr, rrexpr)
         stdout.write_bytes(data)
         stdout.write_bytes(cargs.terminator)
 
 def cmd_run(cargs : _t.Any) -> None:
+    if len(cargs.exprs) == 0:
+        cargs.exprs = [default_get_expr]
+
     if cargs.num_args < 1:
         raise Failure(gettext("`run` sub-command requires at least one PATH"))
     elif cargs.num_args - 1 > len(cargs.args):
         raise Failure(gettext("not enough arguments to satisfy `--num-args`"))
 
     # move (num_args - 1) arguments from args to paths
     ntail = len(cargs.args) + 1 - cargs.num_args
@@ -301,50 +305,52 @@
     compile_filters(cargs)
     elaborate_paths(cargs)
     slurp_stdin0(cargs)
     handle_sorting(cargs)
 
     def emit(abs_in_path : str, rel_in_path : str, rrexpr : ReqresExpr) -> None:
         if not filters_allow(cargs, rrexpr): return
-        stdout.write_bytes(_os.fsencode(abs_in_path) + cargs.terminator)
+        stdout.write(abs_in_path)
+        stdout.write_bytes(cargs.terminator)
         stdout.flush()
 
     map_wrr_paths(emit, cargs.paths, order_by=cargs.walk_fs, errors=cargs.errors)
 
 output_aliases = {
     "default":  "%(syear)d/%(smonth)02d/%(sday)02d/%(shour)02d%(sminute)02d%(ssecond)02d%(stime_msq)03d_%(qtime_ms)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s_%(hostname)s.%(num)d.wrr",
     "short": "%(syear)d/%(smonth)02d/%(sday)02d/%(stime_ms)d_%(qtime_ms)s.%(num)d.wrr",
 
-    "surl":       "%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s",
-    "url":                   "%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s",
-    "surl_msn":   "%(scheme)s/%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr",
-    "url_msn":               "%(netloc)s/%(path_parts|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path)s_%(method)s_%(status)s.%(num)d.wrr",
-
-    "shpq":       "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr",
-    "hpq":                   "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr",
-    "shpq_msn":   "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
-    "hpq_msn":               "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
-
-    "shupq":      "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr",
-    "hupq":                  "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr",
-    "shupq_msn":  "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
-    "hupq_msn":              "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
-
-    "srhupq":     "%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr",
-    "rhupq":                 "%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 120)s.wrr",
-    "srhupq_msn": "%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
-    "rhupq_msn":             "%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
-
-    "shupnq":     "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr",
-    "hupnq":                 "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 120)s.wrr",
-    "shupnq_msn": "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
-    "hupnq_msn":             "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+    "surl":       "%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s",
+    "surl_msn":   "%(scheme)s/%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr",
+
+    "shupq":      "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr",
+    "shupq_msn":  "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+    "shupnq":     "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr",
+    "shupnq_msn": "%(scheme)s/%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+
+    "srhupq":     "%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr",
+    "srhupq_msn": "%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+    "srhupnq":    "%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr",
+    "srhupnq_msn":"%(scheme)s/%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+
+    "url":                   "%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s",
+    "url_msn":               "%(netloc)s/%(mq_path)s%(oqm)s%(mq_query)s_%(method)s_%(status)s.%(num)d.wrr",
+
+    "hupq":                  "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr",
+    "hupq_msn":              "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+    "hupnq":                 "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr",
+    "hupnq_msn":             "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+
+    "rhupq":                 "%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 120)s.wrr",
+    "rhupq_msn":             "%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_query|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
+    "rhupnq":                "%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 120)s.wrr",
+    "rhupnq_msn":            "%(rhostname)s/%(wget_parts|abbrev_each 120|pp_to_path)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(status)s.%(num)d.wrr",
 
-    "flat":                  "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr",
-    "flat_n":                "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(query_ne_parts|qsl_to_path|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr",
+    "flat":                  "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.wrr",
+    "flat_n":                "%(hostname)s/%(wget_parts|abbrev_each 120|pp_to_path|replace / __|abbrev 120)s%(oqm)s%(mq_nquery|abbrev 100)s_%(method)s_%(net_url|sha256|prefix 4)s_%(status)s.%(num)d.wrr",
 }
 
 not_allowed = gettext("; this is not allowed to prevent accidental data loss")
 variance_help = gettext("; your `--output` format fails to provide enough variance to solve this problem automatically (did your forget to place a `%%(num)d` substitution in there?)") + not_allowed
 
 def make_deferred_emit(cargs : _t.Any,
                        destination : _t.AnyStr,
@@ -530,15 +536,15 @@
     else:
         assert False
 
     @_dc.dataclass
     class OrganizeSource(_t.Generic[_t.AnyStr]):
         abs_path : _t.AnyStr
         stat_result : _os.stat_result
-        modified_ms : int | None
+        modified : Decimal | None
 
         def anystr(self) -> _t.AnyStr:
             return self.abs_path
 
     @_dc.dataclass
     class OrganizeIntent(DeferredIO[OrganizeSource[_t.AnyStr], _t.AnyStr]):
         source : OrganizeSource[_t.AnyStr]
@@ -626,33 +632,33 @@
                 if file_content_equals(in_source.abs_path, disk_data):
                     # same data on disk
                     return self.source, True
 
             if not allow_updates:
                 return self.source, False
 
-            prev_modified_ms = self.source.modified_ms
-            if prev_modified_ms is None:
+            prev_modified = self.source.modified
+            if prev_modified is None:
                 # mtime was not cached yet, get it
                 if disk_data is None:
-                    prev_modified_ms = wrr_loadf_expr(self.source.abs_path).stime_ms
+                    prev_modified = wrr_loadf_expr(self.source.abs_path).stime
                 else:
                     # reuse disk_data read above
                     bio = _t.cast(_io.BufferedReader, _io.BytesIO(disk_data))
-                    prev_modified_ms = wrr_load_expr(bio, self.source.abs_path).stime_ms
+                    prev_modified = wrr_load_expr(bio, self.source.abs_path).stime
                 # cache the result
-                self.source.modified_ms = prev_modified_ms
+                self.source.modified = prev_modified
 
             del disk_data
 
-            new_modified_ms = in_source.modified_ms
+            new_modified = in_source.modified
             # in_source should be completely loaded just before each emit call
-            assert new_modified_ms is not None
+            assert new_modified is not None
 
-            if prev_modified_ms < new_modified_ms:
+            if prev_modified < new_modified:
                 # update source
                 self.source = in_source
 
             return self.source, True
 
         def run(self, abs_out_path : _t.AnyStr, dsync : DeferredSync[_t.AnyStr] | None = None, dry_run : bool = False) \
                 -> OrganizeSource[_t.AnyStr] | None:
@@ -679,15 +685,15 @@
                 raise exc
 
             return self.source
 
     emit_one, finish = make_deferred_emit(cargs, destination, action, actioning, OrganizeIntent)
 
     def emit(abs_in_path : str, rel_in_path : str, in_stat : _os.stat_result, rrexpr : ReqresExpr) -> None:
-        emit_one(OrganizeSource(abs_in_path, in_stat, rrexpr.stime_ms), rrexpr)
+        emit_one(OrganizeSource(abs_in_path, in_stat, rrexpr.stime), rrexpr)
 
     return emit, finish
 
 def cmd_organize(cargs : _t.Any) -> None:
     compile_filters(cargs)
     elaborate_output(cargs)
     elaborate_paths(cargs)
@@ -960,40 +966,40 @@
     add_paths(cmd)
     cmd.set_defaults(func=cmd_pprint)
 
     # get
     cmd = subparsers.add_parser("get", help=_("print values produced by computing given expressions on a given WRR file"),
                                 description = _(f"""Compute output values by evaluating expressions `EXPR`s on a given reqres stored at `PATH`, then print them to stdout terminating each value as specified."""))
 
-    cmd.add_argument("-e", "--expr", dest="exprs", metavar="EXPR", action="append", type=str, default = [], help=_('an expression to compute; can be specified multiple times in which case computed outputs will be printed sequentially, see also "output" options below; (default: `response.body|es`); each EXPR describes a state-transformer (pipeline) which starts from value `None` and evaluates a script built from the following:') + "\n" + \
+    cmd.add_argument("-e", "--expr", dest="exprs", metavar="EXPR", action="append", type=str, default = [], help=_(f'an expression to compute; can be specified multiple times in which case computed outputs will be printed sequentially, see also "output" options below; (default: `{default_get_expr}`); each EXPR describes a state-transformer (pipeline) which starts from value `None` and evaluates a script built from the following:') + "\n" + \
                      "- " + _("constants and functions:") + "\n" + \
                      "".join([f"  - `{name}`: {_(value[0]).replace('%', '%%')}\n" for name, value in Reqres_atoms.items()]) + \
                      "- " + _("reqres fields, these work the same way as constants above, i.e. they replace current value of `None` with field's value, if reqres is missing the field in question, which could happen for `response*` fields, the result is `None`:") + "\n" + \
                      "".join([f"  - `{name}`: {_(value).replace('%', '%%')}\n" for name, value in Reqres_fields.items()]) + \
                      "- " + _("derived attributes:") + "\n" + \
                      "".join([f"  - `{name}`: {_(value).replace('%', '%%')}\n" for name, value in Reqres_derived_attrs.items()]) + \
                      "- " + _("a compound expression built by piping (`|`) the above, for example:") + """
   - `net_url|sha256`
   - `net_url|sha256|prefix 4`
-  - `path_parts|pp_to_path`
-  - `query_parts|qsl_to_path|abbrev 128`
+  - `path_parts|prefix 3|pp_to_path`
+  - `query_parts|prefix 3|qsl_to_path|abbrev 128`
   - `response.complete`: this will print the value of `response.complete` or `None`, if there was no response
   - `response.complete|false`: this will print `response.complete` or `False`
   - `response.body|eb`: this will print `response.body` or an empty string, if there was no response
 """)
     add_terminator(cmd)
 
     cmd.add_argument("path", metavar="PATH", type=str, help=_("input WRR file path"))
     cmd.set_defaults(func=cmd_get)
 
     # run
     cmd = subparsers.add_parser("run", help=_("spawn a process with generated temporary files produced by given expressions computed on given WRR files as arguments"),
                                 description = _("""Compute output values by evaluating expressions `EXPR`s for each of `NUM` reqres stored at `PATH`s, dump the results into into newly generated temporary files terminating each value as specified, spawn a given `COMMAND` with given arguments `ARG`s and the resulting temporary file paths appended as the last `NUM` arguments, wait for it to finish, delete the temporary files, exit with the return code of the spawned process."""))
 
-    cmd.add_argument("-e", "--expr", dest="exprs", metavar="EXPR", action="append", type=str, default=["response.body|es"], help=_("the expression to compute, can be specified multiple times, see `{__package__} get --expr` for more info; (default: `response.body|es`)"))
+    cmd.add_argument("-e", "--expr", dest="exprs", metavar="EXPR", action="append", type=str, default=[], help=_(f"the expression to compute, can be specified multiple times, see `{__package__} get --expr` for more info; (default: `{default_get_expr}`)"))
     add_terminator(cmd)
 
     cmd.add_argument("-n", "--num-args", metavar="NUM", type=int, default = 1, help=_("number of `PATH`s (default: `%(default)s`)"))
     cmd.add_argument("command", metavar="COMMAND", type=str, help=_("command to spawn"))
     cmd.add_argument("args", metavar="ARG", nargs="*", type=str, help=_("additional arguments to give to the COMMAND"))
     cmd.add_argument("paths", metavar="PATH", nargs="+", type=str, help=_("input WRR file paths to be mapped into new temporary files"))
     cmd.set_defaults(func=cmd_run)
@@ -1086,15 +1092,15 @@
 setting this to a value smaller than `--batch-number` will not improve memory consumption very much since batched IO actions also cache information about their own files
 """))
     agrp.add_argument("--lazy", action="store_true", help=_(f"sets `--cache-number` and `--batch-number` to positive infinity; most useful in combination with `--symlink --latest` in which case it will force `{__package__}` to compute the desired file system state first and then perform disk writes in a single batch"))
 
     cmd.add_argument("-t", "--to", dest="destination", metavar="DESTINATION", type=str, help=_("destination directory, when unset each source `PATH` must be a directory which will be treated as its own `DESTINATION`"))
     cmd.add_argument("-o", "--output", metavar="FORMAT", default="default", type=str, help=_("""format describing generated output paths, an alias name or "format:" followed by a custom pythonic %%-substitution string:""") + "\n" + \
                      "- " + _("available aliases and corresponding %%-substitutions:") + "\n" + \
-                     "".join([f"  - `{name}`: `{value.replace('%', '%%')}`" + (" (default)" if name == "default" else "") + "\n" for name, value in output_aliases.items()]) + \
+                     "".join([f"  - `{name}`{' ' * (11 - len(name))}: `{value.replace('%', '%%')}`" + (" (default)" if name == "default" else "") + "\n" for name, value in output_aliases.items()]) + \
                      "- " + _("available substitutions:") + "\n" + \
                      "  - `num`: " + _("number of times the resulting output path was encountered before; adding this parameter to your `--output` format will ensure all generated file names will be unique") + "\n" + \
                      "  - " + _(f"all expressions of `{__package__} get --expr`, which see"))
 
     add_paths(cmd, True)
     cmd.set_defaults(func=cmd_organize)
```

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/io.py` & `pwebarc-wrrarms-0.9.0/wrrarms/io.py`

 * *Files identical despite different names*

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/linst.py` & `pwebarc-wrrarms-0.9.0/wrrarms/linst.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,17 +201,17 @@
           linst_apply1(None, lambda v, arg: v < linst_cast_val(v, arg))),
     "<=": ("apply `<= arg`, similarly",
           linst_apply1(None, lambda v, arg: v <= linst_cast_val(v, arg))),
     ">": ("apply `> arg`, similarly",
           linst_apply1(None, lambda v, arg: v > linst_cast_val(v, arg))),
     ">=": ("apply `>= arg`, similarly",
           linst_apply1(None, lambda v, arg: v >= linst_cast_val(v, arg))),
-    "prefix": ("take first `arg` characters",
+    "prefix": ("take first `arg` characters or list elements",
           linst_apply1(int, lambda v, arg: v[:arg])),
-    "suffix": ("take last `arg` characters",
+    "suffix": ("take last `arg` characters or list elements",
           linst_apply1(int, lambda v, arg: v[len(v) - arg:])),
     "abbrev": ("leave the current value as if if its length is less or equal than `arg` characters, otherwise take first `arg/2` followed by last `arg/2` characters",
           linst_apply1(int, abbrev)),
     "abbrev_each": ("`abbrev arg` each element in a value `list`",
           linst_apply1(int, lambda v, arg: list(map(lambda e: abbrev(e, arg), v)))),
     "replace": ("replace all occurences of the first argument in the current value with the second argument, casts arguments to the same type as the current value",
           linst_apply2(str, str, lambda v, arg1, arg2: v.replace(linst_cast_val(v, arg1), linst_cast_val(v, arg2)))),
```

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/mitmproxy.py` & `pwebarc-wrrarms-0.9.0/wrrarms/mitmproxy.py`

 * *Files identical despite different names*

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/output.py` & `pwebarc-wrrarms-0.9.0/wrrarms/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import cbor2.decoder as _cbor2dec
-import cbor2.encoder as _cbor2enc
+import cbor2 as _cbor2
 import io as _io
 import json as _json
 import typing as _t
 
 from kisstdlib.exceptions import *
 from kisstdlib.io import *
 
@@ -117,15 +116,15 @@
                 jsdump = _json.dumps(js, ensure_ascii = False, indent = 2)
                 data = encode(jsdump)
                 final, raw = True, True
 
         if not final:
             try:
                 with _io.BytesIO(data) as fp:
-                    cb = _cbor2dec.CBORDecoder(fp).decode()
+                    cb = _cbor2.CBORDecoder(fp).decode()
                     if len(fp.read()) != 0:
                         # not all of the data was decoded
                         raise Exception("failed to parse")
                 cbordump = pyrepr_dumps(cb, width = 80)
             except Exception:
                 pass
             else:
@@ -205,27 +204,26 @@
     def finish(self) -> None:
         self.fobj.flush()
 
 class CBORStreamEncoder(StreamEncoder):
     def __init__(self, fobj : TIOWrappedWriter, abridged : bool) -> None:
         super().__init__(fobj, abridged)
 
-        encoders = _cbor2enc.default_encoders.copy()
+        encoders = _cbor2.default_encoders.copy()
         if abridged:
             encoders[bytes] = _t.cast(_t.Any, self.encode_cbor_abridged)
             encoders[str] = _t.cast(_t.Any, self.encode_cbor_abridged)
-        self.encoder = _cbor2enc.CBOREncoder(_io.BytesIO(), default = self.encode_cbor)
-        self.encoder._encoders = encoders
+        self.encoder = _cbor2.CBOREncoder(_io.BytesIO(), encoders = encoders, default = self.encode_cbor)
 
     @staticmethod
-    def encode_cbor(enc : _cbor2enc.CBOREncoder, obj : _t.Any) -> None:
+    def encode_cbor(enc : _cbor2.CBOREncoder, obj : _t.Any) -> None:
         enc.encode(plainify(obj))
 
     @staticmethod
-    def encode_cbor_abridged(enc : _cbor2enc.CBOREncoder, obj : _t.Any) -> None:
+    def encode_cbor_abridged(enc : _cbor2.CBOREncoder, obj : _t.Any) -> None:
         abridged, value = abridge_anystr(obj, 256, False)
         if isinstance(value, bytes):
             enc.encode_bytestring(value)
         elif isinstance(value, str):
             enc.encode_string(value)
         else:
             assert False
@@ -233,15 +231,15 @@
     def start(self) -> None:
         super().start()
         self.fobj.write_bytes(b"\x9f") # start indefinite-length array
 
     def emit(self, path : str, names : list[str], values : list[_t.Any]) -> None:
         try:
             self.encoder.encode(values)
-            self.fobj.write_bytes(self.encoder.fp.getvalue())
+            self.fobj.write_bytes(self.encoder.fp.getvalue()) # type: ignore
         finally:
             self.encoder.fp = _io.BytesIO()
 
     def finish(self) -> None:
         self.fobj.write_bytes(b"\xff") # break symbol
         super().finish()
```

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/type.py` & `pwebarc-wrrarms-0.9.0/wrrarms/type.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     minutes = value // 60000
     value = value % 60000
     seconds = value // 1000
     value = value % 1000
     return str(hours) + ":" + format(minutes, "02") + ":" + format(seconds, "02") + "." + format(value, "03")
 
 def fmt_epoch_interval(from_epoch : Epoch, to_epoch : Epoch) -> str:
-    return f"[{str(from_epoch)}]--[{str(to_epoch)}] => {fmt_epoch_diff(from_epoch, to_epoch)}"
+    return f"[{from_epoch.format()}]--[{to_epoch.format()}] => {fmt_epoch_diff(from_epoch, to_epoch)}"
 
 def rec_get(obj : _t.Any, field : list[str]) -> _t.Any:
     if len(field) == 0:
         return obj
 
     this, *rest = field
     if isinstance(obj, dict) and this in obj:
```

### Comparing `pwebarc-wrrarms-0.8.1/wrrarms/wrr.py` & `pwebarc-wrrarms-0.9.0/wrrarms/wrr.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import cbor2 as _cbor2
 import dataclasses as _dc
-import decimal as _dec
 import gzip as _gzip
 import hashlib as _hashlib
 import idna as _idna
 import io as _io
 import logging as _logging
 import os as _os
 import sys as _sys
 import time as _time
 import typing as _t
 import urllib.parse as _up
 
+from decimal import Decimal
+
 from kisstdlib.exceptions import *
 from kisstdlib.path import *
 
 from .type import *
 from .linst import *
 
 Headers = list[tuple[str, bytes]]
@@ -127,27 +128,31 @@
     "fsecond": "similar to `ssecond`, but for `ftime`; int",
 
     "status": '`"NR"` if there was no response, `str(response.code) + "C"` if response was complete, `str(response.code) + "N"` otherwise; str',
 
     "method": "aliast for `request.method`; str",
     "raw_url": "aliast for `request.url`; str",
     "net_url": "`raw_url` with Punycode UTS46 IDNA encoded hostname, unsafe characters quoted, and without the fragment/hash part; this is the URL that actually gets sent to the server; str",
+    "pretty_url": "`raw_url`, but using `hostname`, `mq_path`, and `mq_nquery`; str",
     "scheme": "scheme part of `raw_url`; e.g. `http`, `https`, etc; str",
     "raw_hostname": "hostname part of `raw_url` as it is recorded in the reqres; str",
     "net_hostname": "hostname part of `raw_url`, encoded as Punycode UTS46 IDNA; this is what actually gets sent to the server; ASCII str",
-    "hostname": "`net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; str",
+    "hostname": "`net_hostname` decoded back into UNICODE; this is the canonical hostname representation for which IDNA-encoding and decoding are bijective; UNICODE str",
     "rhostname": '`hostname` with the order of its parts reversed; e.g. `"www.example.org"` -> `"com.example.www"`; str',
     "port": 'port part of `raw_url`; int or None',
     "netloc": "netloc part of `raw_url`; i.e., in the most general case, `<username>:<password>@<hostname>:<port>`; str",
     "raw_path": 'raw path part of `raw_url` as it is recorded is the reqres; e.g. `"https://www.example.org"` -> `""`, `"https://www.example.org/"` -> `"/"`, `"https://www.example.org/index.html"` -> `"/index.html"`; str',
     "path_parts": 'component-wise unquoted "/"-split `raw_path` with empty components removed and dots and double dots interpreted away; e.g. `"https://www.example.org"` -> `[]`, `"https://www.example.org/"` -> `[]`, `"https://www.example.org/index.html"` -> `["index.html"]` , `"https://www.example.org/skipped/.//../used/"` -> `["used"]; list[str]',
+    "mq_path": "`path_parts` turned back into a minimally-quoted string; str",
     "wget_parts": '`path + ["index.html"]` if `raw_path` ends in a slash, `path` otherwise; this is what `wget` does in `wget -mpk`; list[str]',
     "raw_query": "query part of `raw_url` (i.e. everything after the `?` character and before the `#` character) as it is recorded in the reqres; str",
     "query_parts": "parsed (and component-wise unquoted) `raw_query`; list[tuple[str, str]]",
     "query_ne_parts": "`query_parts` with empty query parameters removed; list[tuple[str, str]]",
+    "mq_query": "`query_parts` turned back into a minimally-quoted string; str",
+    "mq_nquery": "`query_ne_parts` turned back into a minimally-quoted string; str",
     "oqm": "optional query mark: `?` character if `query` is non-empty, an empty string otherwise; str",
     "fragment": "fragment (hash) part of the url; str",
     "ofm": "optional fragment mark: `#` character if `fragment` is non-empty, an empty string otherwise; str",
 }
 
 _time_attrs = set(["time", "time_ms", "time_msq", "year", "month", "day", "hour", "minute", "second"])
 
@@ -264,16 +269,16 @@
             self.items["ftime_msq"] = ftime_ms % 1000
             self._fill_time("f", ftime)
         elif name in ["raw_url", "net_url",
                       "scheme",
                       "raw_hostname", "net_hostname", "hostname", "rhostname",
                       "port",
                       "netloc",
-                      "raw_path", "path_parts", "wget_parts",
-                      "oqm", "raw_query", "query_parts", "query_neparts",
+                      "raw_path",
+                      "oqm", "raw_query",
                       "ofm", "fragment"]:
             raw_url = reqres.request.url
             self.items["raw_url"] = raw_url
             purl = _up.urlsplit(raw_url)
 
             scheme = purl.scheme
             self.items["scheme"] = scheme
@@ -326,14 +331,25 @@
             self.items["netloc"] = netloc
 
             net_netloc = "".join([netauth, net_hostname, netport])
             net_url = _up.quote(f"{scheme}://{net_netloc}{raw_path}{oqm}{raw_query}", safe="%/:=&?~#+!$,;'@()*[]|")
             if raw_query == "" and raw_url.endswith("?"):
                 net_url += "?"
             self.items["net_url"] = net_url
+        elif name in ["path_parts", "wget_parts",
+                      "query_parts", "query_neparts",
+                      "mq_path", "mq_query", "mq_nquery",
+                      "pretty_url"]:
+            scheme = self.get_value("scheme")
+            netloc = self.items["netloc"]
+            raw_path = self.get_value("raw_path")
+            raw_query = self.items["raw_query"]
+            oqm = self.items["oqm"]
+            ofm = self.items["ofm"]
+            fragment = self.items["fragment"]
 
             path_parts_insecure = [_up.unquote(e) for e in raw_path.split("/") if e != ""]
 
             # remove dots and securely interpret double dots
             path_parts : list[str] = []
             for e in path_parts_insecure:
                 if e == ".":
@@ -345,15 +361,26 @@
                 path_parts.append(e)
 
             self.items["path_parts"] = path_parts
             self.items["wget_parts"] = path_parts + ["index.html"] if raw_path.endswith("/") else path_parts
 
             qsl = _up.parse_qsl(raw_query, keep_blank_values=True)
             self.items["query_parts"] = qsl
-            self.items["query_ne_parts"] = [e for e in qsl if e[1] != ""]
+            qsl_ne = [e for e in qsl if e[1] != ""]
+            self.items["query_ne_parts"] = qsl_ne
+
+            mq_path = pp_to_path(path_parts)
+            self.items["mq_path"] = mq_path
+            mq_query = qsl_to_path(qsl)
+            self.items["mq_nquery"] = mq_query
+            mq_nquery = qsl_to_path(qsl_ne)
+            self.items["mq_nquery"] = mq_nquery
+
+            pretty_url = f"{scheme}://{netloc}{mq_path}{oqm}{mq_nquery}{ofm}{fragment}"
+            self.items["pretty_url"] = pretty_url
         elif name == "" or name in Reqres_fields:
             if name == "":
                 field = []
             else:
                 field = name.split(".")
             # set to None if it does not exist
             try:
@@ -452,15 +479,15 @@
     raise TypeError("wrong type: want %s or %s, got %s", bytes, str, type(x))
 
 def _t_int(x : _t.Any) -> int:
     if isinstance(x, int): return x
     raise TypeError("wrong type: want %s, got %s", int, type(x))
 
 def _t_epoch(x : _t.Any) -> Epoch:
-    return Epoch(_dec.Decimal(_t_int(x)) / 1000)
+    return Epoch(Decimal(_t_int(x)) / 1000)
 
 def _f_epoch(x : Epoch) -> int:
     return int(x * 1000)
 
 def _t_headers(x : _t.Any) -> Headers:
     if Headers.__instancecheck__(x):
         return _t.cast(Headers, x)
```

