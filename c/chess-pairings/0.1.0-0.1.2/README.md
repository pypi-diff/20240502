# Comparing `tmp/chess_pairings-0.1.0.tar.gz` & `tmp/chess_pairings-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_pairings-0.1.0.tar", last modified: Mon Apr 29 10:03:52 2024, max compression
+gzip compressed data, was "chess_pairings-0.1.2.tar", last modified: Thu May  2 17:56:03 2024, max compression
```

## Comparing `chess_pairings-0.1.0.tar` & `chess_pairings-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 10:03:52.558382 chess_pairings-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      534 2024-04-29 10:03:52.558382 chess_pairings-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-04-29 08:07:46.000000 chess_pairings-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      544 2024-04-29 10:03:15.000000 chess_pairings-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-29 10:03:52.558382 chess_pairings-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 10:03:52.548382 chess_pairings-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 10:03:52.558382 chess_pairings-0.1.0/src/chess_pairings/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-04-29 08:12:54.000000 chess_pairings-0.1.0/src/chess_pairings/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      327 2024-04-29 09:58:00.000000 chess_pairings-0.1.0/src/chess_pairings/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 10:03:52.558382 chess_pairings-0.1.0/src/chess_pairings/chess_results/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-29 08:48:02.000000 chess_pairings-0.1.0/src/chess_pairings/chess_results/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      531 2024-04-29 09:57:54.000000 chess_pairings-0.1.0/src/chess_pairings/chess_results/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2347 2024-04-29 09:51:37.000000 chess_pairings-0.1.0/src/chess_pairings/chess_results/_donwload.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      357 2024-04-29 09:52:31.000000 chess_pairings-0.1.0/src/chess_pairings/chess_results/errors.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      274 2024-04-29 10:02:35.000000 chess_pairings-0.1.0/src/chess_pairings/chess_results/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3972 2024-04-29 10:02:34.000000 chess_pairings-0.1.0/src/chess_pairings/chess_results/parsing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      712 2024-04-29 09:53:41.000000 chess_pairings-0.1.0/src/chess_pairings/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 10:03:52.558382 chess_pairings-0.1.0/src/chess_pairings.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      534 2024-04-29 10:03:52.000000 chess_pairings-0.1.0/src/chess_pairings.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      589 2024-04-29 10:03:52.000000 chess_pairings-0.1.0/src/chess_pairings.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-29 10:03:52.000000 chess_pairings-0.1.0/src/chess_pairings.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       49 2024-04-29 10:03:52.000000 chess_pairings-0.1.0/src/chess_pairings.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-29 10:03:52.000000 chess_pairings-0.1.0/src/chess_pairings.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 17:56:03.434073 chess_pairings-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-02 17:56:03.434073 chess_pairings-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-02 17:55:59.000000 chess_pairings-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 17:56:03.434073 chess_pairings-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 17:56:03.424073 chess_pairings-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 17:56:03.424073 chess_pairings-0.1.2/src/chess_pairings/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      327 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 17:56:03.434073 chess_pairings-0.1.2/src/chess_pairings/chess_results/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/chess_results/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      531 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/chess_results/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2347 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/chess_results/_donwload.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      357 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/chess_results/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      274 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/chess_results/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4007 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/chess_results/parsing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      715 2024-05-02 17:54:54.000000 chess_pairings-0.1.2/src/chess_pairings/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 17:56:03.434073 chess_pairings-0.1.2/src/chess_pairings.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-02 17:56:03.000000 chess_pairings-0.1.2/src/chess_pairings.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      589 2024-05-02 17:56:03.000000 chess_pairings-0.1.2/src/chess_pairings.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-02 17:56:03.000000 chess_pairings-0.1.2/src/chess_pairings.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       49 2024-05-02 17:56:03.000000 chess_pairings-0.1.2/src/chess_pairings.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-05-02 17:56:03.000000 chess_pairings-0.1.2/src/chess_pairings.egg-info/top_level.txt
```

### Comparing `chess_pairings-0.1.0/PKG-INFO` & `chess_pairings-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chess-pairings
-Version: 0.1.0
+Version: 0.1.2
 Summary: Tools for storing and fetching chess tournament pairings
 Author-email: Marcel Claramunt <marcel@moveread.com>
-Project-URL: repo, https://github.com/moveread/REPO.git
+Project-URL: repo, https://github.com/moveread/chess.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Provides-Extra: chess-results
 Requires-Dist: beautifulsoup4; extra == "chess-results"
 Requires-Dist: aiohttp; extra == "chess-results"
```

### Comparing `chess_pairings-0.1.0/pyproject.toml` & `chess_pairings-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-pairings"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Tools for storing and fetching chess tournament pairings"
 dependencies = [
   "pydantic"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
-repo = "https://github.com/moveread/REPO.git"
+repo = "https://github.com/moveread/chess.git"
 
 [project.optional-dependencies]
 chess-results = ["beautifulsoup4", "aiohttp"]
```

### Comparing `chess_pairings-0.1.0/src/chess_pairings/chess_results/__init__.pyi` & `chess_pairings-0.1.2/src/chess_pairings/chess_results/__init__.pyi`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.0/src/chess_pairings/chess_results/_donwload.py` & `chess_pairings-0.1.2/src/chess_pairings/chess_results/_donwload.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.0/src/chess_pairings/chess_results/parsing.py` & `chess_pairings-0.1.2/src/chess_pairings/chess_results/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,20 +83,21 @@
       ...
 
 def safe_int(s) -> int | None:
   return E.safe(lambda: int(s)).get_or(None)
 
 def parse_row(row: Row) -> Pairing:
   if row.black_no == '':
-    return Unpaired(player=row.white, reason=row.black)
+    return Unpaired(player=row.white, reason=row.black, tag='unpaired')
   else:
     return Paired(
       result=parse_result(row.result), white=row.white, black=row.black,
       white_no=safe_int(row.white_no), white_elo=safe_int(row.white_elo),
       black_no=safe_int(row.black_no), black_elo=safe_int(row.black_elo),
+      tag='paired'
     )
   
 def parse_rounds(soup: BeautifulSoup) -> Either[ParsingError, list[list[Pairing]]]:
   try:
     rounds: dict[int, list[Pairing]] = {}
     columns = parse_columns(soup).unsafe()
     headings = soup.find_all(string=re.compile("^Round ."))
```

### Comparing `chess_pairings-0.1.0/src/chess_pairings/types.py` & `chess_pairings-0.1.2/src/chess_pairings/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     white: str
     black: str
     white_no: int | None = None
     white_elo: int | None = None
     black_no: int | None = None
     black_elo: int | None = None
     result: Result | None = None
-    paired: bool = True
-    
+    tag: Literal['paired']
+
 class Unpaired(BaseModel):
     player: str
     reason: str
-    paired: bool = False
+    tag: Literal['unpaired']
     
 Pairing: TypeAlias = Paired | Unpaired
 RoundPairings: TypeAlias = Sequence[Pairing]
 GroupPairings: TypeAlias = Sequence[RoundPairings]
 TournamentPairings: TypeAlias = Mapping[str, GroupPairings]
 """Group -> Round -> Board -> Pairing"""
```

### Comparing `chess_pairings-0.1.0/src/chess_pairings.egg-info/PKG-INFO` & `chess_pairings-0.1.2/src/chess_pairings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chess-pairings
-Version: 0.1.0
+Version: 0.1.2
 Summary: Tools for storing and fetching chess tournament pairings
 Author-email: Marcel Claramunt <marcel@moveread.com>
-Project-URL: repo, https://github.com/moveread/REPO.git
+Project-URL: repo, https://github.com/moveread/chess.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Provides-Extra: chess-results
 Requires-Dist: beautifulsoup4; extra == "chess-results"
 Requires-Dist: aiohttp; extra == "chess-results"
```

### Comparing `chess_pairings-0.1.0/src/chess_pairings.egg-info/SOURCES.txt` & `chess_pairings-0.1.2/src/chess_pairings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

