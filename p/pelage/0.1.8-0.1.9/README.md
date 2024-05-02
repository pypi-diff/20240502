# Comparing `tmp/pelage-0.1.8.tar.gz` & `tmp/pelage-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelage-0.1.8.tar", max compression
+gzip compressed data, was "pelage-0.1.9.tar", max compression
```

## Comparing `pelage-0.1.8.tar` & `pelage-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2024-03-07 21:02:52.572635 pelage-0.1.8/LICENSE
--rw-r--r--   0        0        0     4727 2024-04-04 16:22:53.886116 pelage-0.1.8/README.md
--rw-r--r--   0        0        0       42 2024-03-09 07:40:35.887285 pelage-0.1.8/pelage/__init__.py
--rw-r--r--   0        0        0    43450 2024-04-03 18:00:15.892560 pelage-0.1.8/pelage/checks.py
--rw-r--r--   0        0        0        0 2024-03-07 20:43:38.400138 pelage-0.1.8/pelage/data/.keep
--rw-r--r--   0        0        0      774 2024-03-22 06:43:08.899733 pelage-0.1.8/pelage/utils.py
--rw-r--r--   0        0        0      684 2024-04-04 16:24:31.855310 pelage-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 pelage-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-07 21:02:52.572635 pelage-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4727 2024-04-28 08:56:04.252709 pelage-0.1.9/README.md
+-rw-r--r--   0        0        0       42 2024-03-09 07:40:35.887285 pelage-0.1.9/pelage/__init__.py
+-rw-r--r--   0        0        0    47181 2024-04-28 08:41:31.984535 pelage-0.1.9/pelage/checks.py
+-rw-r--r--   0        0        0        0 2024-03-07 20:43:38.400138 pelage-0.1.9/pelage/data/.keep
+-rw-r--r--   0        0        0      774 2024-03-22 06:43:08.899733 pelage-0.1.9/pelage/utils.py
+-rw-r--r--   0        0        0      684 2024-04-28 08:55:12.150517 pelage-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 pelage-0.1.9/PKG-INFO
```

### Comparing `pelage-0.1.8/LICENSE` & `pelage-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pelage-0.1.8/README.md` & `pelage-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pelage-0.1.8/pelage/checks.py` & `pelage-0.1.9/pelage/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1049,29 +1049,59 @@
             msg = f"Some values were removed from col '{column}', for ex: {*set_diff,}"
             raise PolarsAssertError(supp_message=msg)
 
     return data
 
 
 def is_monotonic(
-    data: pl.DataFrame, column: str, decreasing: bool = False, strict: bool = True
+    data: pl.DataFrame,
+    column: str,
+    decreasing: bool = False,
+    strict: bool = True,
+    interval: Optional[Union[int, float, str]] = None,
+    group_by: Optional[PolarsOverClauseInput] = None,
 ) -> pl.DataFrame:
     """Verify that values in a column are consecutively increasing or decreasing
 
     Parameters
     ----------
     data : pl.DataFrame
         To check
     column : str
         Name of the column that should be monotonic.
     decreasing : bool, optional
         Should the column be decreasing, by default False
     strict : bool, optional
         The series must be stricly increasing or decreasing, no consecutive equal values
         are allowed, by default True
+    interval : Optional[Union[int, float, str, pl.Duration]], optional, by default None
+        For time-based column, the interval can be specified as a string as in the
+        function `dt.offset_by` or `pl.DataFrame().rolling`. It can also be specified
+        with the `pl.duration()` function directly in a more explicit manner.
+
+        When using a string, the interval is dictated by the following string language:
+            - 1ns (1 nanosecond)
+            - 1us (1 microsecond)
+            - 1ms (1 millisecond)
+            - 1s (1 second)
+            - 1m (1 minute)
+            - 1h (1 hour)
+            - 1d (1 calendar day)
+            - 1w (1 calendar week)
+            - 1mo (1 calendar month)
+            - 1q (1 calendar quarter)
+            - 1y (1 calendar year)
+            - 1i (1 index count)
+        By "calendar day", we mean the corresponding time on the next day (which may
+        not be 24 hours, due to daylight savings). Similarly for "calendar week",
+        "calendar month", "calendar quarter", and "calendar year".,
+
+    group_by : Optional[PolarsOverClauseInput], optional, by default None
+        When specified, the monotonic characteristics and intervals are estimated for
+        each group independently.
 
     Returns
     -------
     pl.DataFrame
         The original polars DataFrame when the check passes
 
 
@@ -1096,33 +1126,88 @@
     >>> bad = pl.DataFrame({"int": [1, 2, 1], "str": ["x", "y", "z"]})
     >>> bad.pipe(plg.is_monotonic, "int")
     Traceback (most recent call last):
     ...
     pelage.checks.PolarsAssertError: Details
     Error with the DataFrame passed to the check function:
     -->Column "int" expected to be monotonic but is not, try .sort("int")
-    """
+    >>> given = pl.DataFrame(
+    ...     [
+    ...         ("2020-01-01 01:42:00", "A"),
+    ...         ("2020-01-01 01:43:00", "A"),
+    ...         ("2020-01-01 01:44:00", "A"),
+    ...         ("2021-12-12 01:43:00", "B"),
+    ...         ("2021-12-12 01:44:00", "B"),
+    ...     ],
+    ...     schema=["dates", "group"],
+    ... ).with_columns(pl.col("dates").str.to_datetime())
+    >>> given.pipe(plg.is_monotonic, "dates", interval="1m", group_by="group")
+    shape: (5, 2)
+    ┌─────────────────────┬───────┐
+    │ dates               ┆ group │
+    │ ---                 ┆ ---   │
+    │ datetime[μs]        ┆ str   │
+    ╞═════════════════════╪═══════╡
+    │ 2020-01-01 01:42:00 ┆ A     │
+    │ 2020-01-01 01:43:00 ┆ A     │
+    │ 2020-01-01 01:44:00 ┆ A     │
+    │ 2021-12-12 01:43:00 ┆ B     │
+    │ 2021-12-12 01:44:00 ┆ B     │
+    └─────────────────────┴───────┘
+    >>> given.pipe(plg.is_monotonic, "dates", interval="3m", group_by="group")
+    Traceback (most recent call last):
+    ...
+    pelage.checks.PolarsAssertError: Details
+    Error with the DataFrame passed to the check function:
+    -->Intervals differ from the specified 3m interval. Unexpected: {datetime.timedelta(seconds=60)}
+    """  # noqa: E501
+    select_diff_expression = (
+        pl.col(column).diff()
+        if group_by is None
+        else pl.col(column).diff().over(group_by)
+    )
+
     # Cast necessary for dates and datetimes
-    diff_column = data.get_column(column).diff().cast(int)
+    diff_column = data.select(select_diff_expression).get_column(column)
+    diff_column_sign = diff_column.cast(int)
 
     if not decreasing and not strict:
-        comparisons = (diff_column >= 0).all()
+        comparisons = (diff_column_sign >= 0).all()
     if not decreasing and strict:
-        comparisons = (diff_column > 0).all()
+        comparisons = (diff_column_sign > 0).all()
     if decreasing and not strict:
-        comparisons = (diff_column <= 0).all()
+        comparisons = (diff_column_sign <= 0).all()
     if decreasing and strict:
-        comparisons = (diff_column < 0).all()
+        comparisons = (diff_column_sign < 0).all()
 
     if not comparisons:
         error_msg = (
             f'Column "{column}" expected to be monotonic but is not,'
             + f' try .sort("{column}")'
         )
         raise PolarsAssertError(supp_message=error_msg)
+
+    if interval is None:
+        return data
+
+    if diff_column.dtype == pl.Duration:
+        assert isinstance(interval, str)
+        dummy_time = pl.Series(["1970-01-01 00:00:00"]).str.to_datetime()
+        expected_timedelta = dummy_time.dt.offset_by(interval) - dummy_time
+        actual_timedelta = diff_column.drop_nulls().unique()
+        bad_intervals = set(actual_timedelta) - set(expected_timedelta)
+
+    else:
+        bad_intervals = (diff_column != interval).any()
+
+    if bad_intervals:
+        raise PolarsAssertError(
+            supp_message=f"Intervals differ from the specified {interval} interval."
+            + f" Unexpected: {bad_intervals}"
+        )
     return data
 
 
 def custom_check(data: pl.DataFrame, expresion: pl.Expr) -> pl.DataFrame:
     """Use custom Polars expression to check the DataFrame, based on `.filter()`.
     The expression when used through the dataframe method `.filter()` should return an
     empty dataframe.
```

### Comparing `pelage-0.1.8/pelage/utils.py` & `pelage-0.1.9/pelage/utils.py`

 * *Files identical despite different names*

### Comparing `pelage-0.1.8/pyproject.toml` & `pelage-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelage"
-version = "0.1.8"
+version = "0.1.9"
 description = "This package contains a collection of tests to improve your Polars data analysis superpowers"
 authors = ["Alix Tiran-Cappello <alix.tiran-cappello@laposte.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 3.13"
```

### Comparing `pelage-0.1.8/PKG-INFO` & `pelage-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelage
-Version: 0.1.8
+Version: 0.1.9
 Summary: This package contains a collection of tests to improve your Polars data analysis superpowers
 License: MIT
 Author: Alix Tiran-Cappello
 Author-email: alix.tiran-cappello@laposte.net
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

