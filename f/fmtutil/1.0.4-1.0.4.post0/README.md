# Comparing `tmp/fmtutil-1.0.4.tar.gz` & `tmp/fmtutil-1.0.4.post0.tar.gz`

## Comparing `fmtutil-1.0.4.tar` & `fmtutil-1.0.4.post0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__about__.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__main__.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__type.py
--rw-r--r--   0        0        0    36743 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__version.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/cli.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/exceptions.py
--rw-r--r--   0        0        0   133878 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/formatter.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/utils.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.4/LICENSE
--rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.4/README.md
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 fmtutil-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 fmtutil-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/__about__.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/__main__.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/__type.py
+-rw-r--r--   0        0        0    36743 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/__version.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/cli.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/exceptions.py
+-rw-r--r--   0        0        0   136785 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/formatter.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/fmtutil/utils.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/LICENSE
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/README.md
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/pyproject.toml
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 fmtutil-1.0.4.post0/PKG-INFO
```

### Comparing `fmtutil-1.0.4/fmtutil/__init__.py` & `fmtutil-1.0.4.post0/fmtutil/__init__.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/fmtutil/__type.py` & `fmtutil-1.0.4.post0/fmtutil/__type.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/fmtutil/__version.py` & `fmtutil-1.0.4.post0/fmtutil/__version.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/fmtutil/cli.py` & `fmtutil-1.0.4.post0/fmtutil/cli.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/fmtutil/exceptions.py` & `fmtutil-1.0.4.post0/fmtutil/exceptions.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/fmtutil/formatter.py` & `fmtutil-1.0.4.post0/fmtutil/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1007,16 +1007,17 @@
             },
             "number_default": {
                 "value": default("0"),
                 "level": 0,
             },
         }
 
-    @staticmethod
+    @classmethod
     def formatter(
+        cls,
         serial: int | str | float | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %n  : Normal serial number
             %p  : Padding serial number
@@ -1027,30 +1028,30 @@
         :param serial: A serial value that pass to generate all format.
         :type serial: int | str | float | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             serial formatter object.
         """
-        _value: int = Serial.prepare_value(serial)
+        _value: int = cls.prepare_value(serial)
         return {
             "%n": {
                 # "value": lambda: str(_value),
                 "value": partial(itself, str(_value)),
                 "regex": r"(?P<number>[0-9]*)",
             },
             "%p": {
-                "value": partial(Serial.to_padding, str(_value)),
+                "value": partial(cls.to_padding, str(_value)),
                 "regex": (
                     r"(?P<number_pad>"
-                    rf"[0-9]{{{str(Serial.Config.serial_max_padding)}}})"
+                    rf"[0-9]{{{str(cls.Config.serial_max_padding)}}})"
                 ),
             },
             "%b": {
-                "value": partial(Serial.to_binary, str(_value)),
+                "value": partial(cls.to_binary, str(_value)),
                 "regex": r"(?P<number_binary>[0-1]*)",
             },
             "%c": {
                 "value": partial(itself, f"{_value:,}"),
                 "regex": r"(?P<number_comma>\d{1,3}(?:,\d{3})*)",
             },
             "%u": {
@@ -1079,44 +1080,42 @@
             return 0
         if not can_int(value) or ((prepare := int(float(value))) < 0):
             raise FormatterValueError(
                 f"Serial formatter does not support for value, {value!r}."
             )
         return prepare
 
-    @staticmethod
-    def to_padding(value: str) -> str:
+    @classmethod
+    def to_padding(cls, value: str) -> str:
         """Return a padding string value with zero by setting config
         ``Serial.Config.serial_max_padding`` value.
 
         :param value: A string value that want to pad with zero.
         :type value: str
 
         :rtype: str
         :return: A padding string value with zero by setting config
             ``Serial.Config.serial_max_padding`` value.
         """
-        return (
-            value.rjust(Serial.Config.serial_max_padding, "0") if value else ""
-        )
+        return value.rjust(cls.Config.serial_max_padding, "0") if value else ""
 
-    @staticmethod
-    def to_binary(value: str) -> str:
+    @classmethod
+    def to_binary(cls, value: str) -> str:
         """Return a binary number string value with limit of max zero padding
         by setting config ``Serial.Config.serial_max_binary`` value.
 
         :param value: A string value that want to convert to binary.
         :type value: str
 
         :rtype: str
         :return: A binary number string value with limit of max zero padding
             by setting config ``Serial.Config.serial_max_binary`` value.
         """
         return (
-            f"{int(value):0{str(Serial.Config.serial_max_binary)}b}"
+            f"{int(value):0{str(cls.Config.serial_max_binary)}b}"
             if value
             else ""
         )
 
 
 MONTHS: DictStr = {
     "Jan": "01",
@@ -1406,16 +1405,17 @@
             },
             "microsecond_default": {
                 "value": default("000000"),
                 "level": 0,
             },
         }
 
-    @staticmethod
+    @classmethod
     def formatter(
+        cls,
         dt: str | datetime | date | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %n  : Normal format with `%Y%m%d_%H%M%S`
         **  %G  : ISO 8601 year
@@ -1460,38 +1460,38 @@
         :param dt: A datetime value that pass to generate all format.
         :type dt: str | datetime | date | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             datetime formatter object.
         """
-        _dt: datetime = Datetime.prepare_value(dt)
+        _dt: datetime = cls.prepare_value(dt)
         return {
             "%n": {
                 "value": partial(_dt.strftime, "%Y%m%d_%H%M%S"),
                 "cregex": "%Y%m%d_%H%M%S",
             },
             "%Y": {
                 "value": partial(_dt.strftime, "%Y"),
                 "regex": r"(?P<year>\d{4})",
             },
             "%y": {
                 "value": partial(_dt.strftime, "%y"),
                 "regex": r"(?P<year_cut_pad>\d{2})",
             },
             "%-y": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%y"),
+                "value": partial(cls.remove_pad_dt, _dt, "%y"),
                 "regex": r"(?P<year_cut>\d{1,2})",
             },
             "%m": {
                 "value": partial(_dt.strftime, "%m"),
                 "regex": r"(?P<month_pad>01|02|03|04|05|06|07|08|09|10|11|12)",
             },
             "%-m": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%m"),
+                "value": partial(cls.remove_pad_dt, _dt, "%m"),
                 "regex": r"(?P<month>1|2|3|4|5|6|7|8|9|10|11|12)",
             },
             "%b": {
                 "value": partial(_dt.strftime, "%b"),
                 "regex": (
                     r"(?P<month_short>"
                     r"Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)"
@@ -1526,58 +1526,58 @@
                 "regex": r"(?P<week_mon>[1-7])",
             },
             "%d": {
                 "value": partial(_dt.strftime, "%d"),
                 "regex": r"(?P<day_pad>[0-3][0-9])",
             },
             "%-d": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%d"),
+                "value": partial(cls.remove_pad_dt, _dt, "%d"),
                 "regex": r"(?P<day>\d{1,2})",
             },
             "%H": {
                 "value": partial(_dt.strftime, "%H"),
                 "regex": r"(?P<hour_pad>[0-2][0-9])",
             },
             "%-H": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%H"),
+                "value": partial(cls.remove_pad_dt, _dt, "%H"),
                 "regex": r"(?P<hour>\d{2})",
             },
             "%I": {
                 "value": partial(_dt.strftime, "%I"),
                 "regex": (
                     r"(?P<hour_12_pad>"
                     r"00|01|02|03|04|05|06|07|08|09|10|11|12)"
                 ),
             },
             "%-I": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%I"),
+                "value": partial(cls.remove_pad_dt, _dt, "%I"),
                 "regex": r"(?P<hour_12>0|1|2|3|4|5|6|7|8|9|10|11|12)",
             },
             "%M": {
                 "value": partial(_dt.strftime, "%M"),
                 "regex": r"(?P<minute_pad>[0-6][0-9])",
             },
             "%-M": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%M"),
+                "value": partial(cls.remove_pad_dt, _dt, "%M"),
                 "regex": r"(?P<minute>\d{1,2})",
             },
             "%S": {
                 "value": partial(_dt.strftime, "%S"),
                 "regex": r"(?P<second_pad>[0-6][0-9])",
             },
             "%-S": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%S"),
+                "value": partial(cls.remove_pad_dt, _dt, "%S"),
                 "regex": r"(?P<second>\d{1,2})",
             },
             "%j": {
                 "value": partial(_dt.strftime, "%j"),
                 "regex": r"(?P<day_year_pad>[0-3][0-9][0-9])",
             },
             "%-j": {
-                "value": partial(Datetime.remove_pad_dt, _dt, "%j"),
+                "value": partial(cls.remove_pad_dt, _dt, "%j"),
                 "regex": r"(?P<day_year>\d{1,3})",
             },
             "%U": {
                 "value": partial(_dt.strftime, "%U"),
                 "regex": r"(?P<weeks_year_sun_pad>[0-5][0-9])",
             },
             "%W": {
@@ -1957,16 +1957,17 @@
             },
             "local_str": {
                 "value": lambda x: x,
                 "level": 0,
             },
         }
 
-    @staticmethod
+    @classmethod
     def formatter(
+        cls,
         version: str | VerPackage | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %f  : full version format with `%m_%n_%c`
             %-f : full version format with `%m-%n-%c`
@@ -1985,15 +1986,15 @@
         :param version: A version value that pass to generate all format.
         :type version: str | __version.VerPackage | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             version formatter object.
         """
-        _version: VerPackage = Version.prepare_value(version)
+        _version: VerPackage = cls.prepare_value(version)
         return {
             "%f": {
                 "value": partial(
                     itself,
                     f"{_version.major}_{_version.minor}_{_version.patch}",
                 ),
                 "cregex": "%m_%n_%c",
@@ -2397,16 +2398,17 @@
                 "value": self.__default(
                     lambda x: re.sub(r"[aeiou]", "", "".join(x))
                 ),
                 "level": 0,
             },
         }
 
-    @staticmethod
+    @classmethod
     def formatter(
+        cls,
         nm: str | list[str] | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %n  : Normal name format
             %N  : Normal name upper case format
@@ -2437,138 +2439,138 @@
         :param nm: A naming value that pass to generate all format.
         :type nm: str | list[str] | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             naming formatter object.
         """
-        _value: list[str] = Naming.prepare_value(nm)
+        _value: list[str] = cls.prepare_value(nm)
         return {
             "%n": {
-                "value": partial(Naming.__join_with, " ", _value),
+                "value": partial(cls.__join_with, " ", _value),
                 "cregex": "%l",
             },
             "%N": {
                 "value": partial(
-                    Naming.__join_with, " ", _value, lambda x: x.upper()
+                    cls.__join_with, " ", _value, lambda x: x.upper()
                 ),
                 "cregex": "%u",
             },
             "%-N": {
                 "value": partial(
-                    Naming.__join_with, " ", _value, lambda x: x.capitalize()
+                    cls.__join_with, " ", _value, lambda x: x.capitalize()
                 ),
                 "cregex": "%t",
             },
             "%u": {
                 "value": partial(
-                    Naming.__join_with, " ", _value, lambda x: x.upper()
+                    cls.__join_with, " ", _value, lambda x: x.upper()
                 ),
                 "regex": r"(?P<strings_upper>[A-Z0-9]+(?:\s[A-Z0-9]+)*)",
             },
             "%l": {
-                "value": partial(Naming.__join_with, " ", _value),
+                "value": partial(cls.__join_with, " ", _value),
                 "regex": r"(?P<strings>[a-z0-9]+(?:\s[a-z0-9]+)*)",
             },
             "%t": {
                 "value": partial(
-                    Naming.__join_with, " ", _value, lambda x: x.capitalize()
+                    cls.__join_with, " ", _value, lambda x: x.capitalize()
                 ),
                 "regex": (
                     r"(?P<strings_title>[A-Z][a-z0-9]+(?:\s[A-Z]+[a-z0-9]*)*)"
                 ),
             },
             "%a": {
                 "value": partial(
-                    Naming.__join_with,
+                    cls.__join_with,
                     "",
                     _value,
                     lambda x: (x[0] if x else ""),
                 ),
                 "regex": r"(?P<shorts>[a-z0-9]+)",
             },
             "%A": {
                 "value": partial(
-                    Naming.__join_with,
+                    cls.__join_with,
                     "",
                     _value,
                     lambda x: (x[0].upper() if x else ""),
                 ),
                 "regex": r"(?P<shorts_upper>[A-Z0-9]+)",
             },
             "%c": {
-                "value": partial(Naming.camel_case, "_".join(_value)),
+                "value": partial(cls.camel_case, "_".join(_value)),
                 "regex": (
                     r"(?P<strings_camel>[a-z]+"
                     r"((\d)|([A-Z0-9][a-z0-9]+))*([A-Z])?)"
                     # r"(?P<strings_camel>[a-z]+(?:[A-Z0-9]+[a-z0-9]+[A-Za-z0-9]*)*)"
                 ),
             },
             "%-c": {
-                "value": partial(Naming.pascal_case, "_".join(_value)),
+                "value": partial(cls.pascal_case, "_".join(_value)),
                 "cregex": "%p",
             },
             "%p": {
-                "value": partial(Naming.pascal_case, "_".join(_value)),
+                "value": partial(cls.pascal_case, "_".join(_value)),
                 "regex": (
                     r"(?P<strings_pascal>[A-Z]"
                     r"([A-Z0-9]*[a-z][a-z0-9]*[A-Z]|"
                     r"[a-z0-9]*[A-Z][A-Z0-9]*[a-z])["
                     r"A-Za-z0-9]*)"
                     # r"(?P<strings_pascal>(?:[A-Z][a-z0-9]+)(?:[A-Z]+[a-z0-9]*)*)"
                 ),
             },
             "%k": {
-                "value": partial(Naming.__join_with, "-", _value),
+                "value": partial(cls.__join_with, "-", _value),
                 "regex": r"(?P<strings_kebab>[a-z0-9]+(?:-[a-z0-9]+)*)",
             },
             "%K": {
                 "value": partial(
-                    Naming.__join_with, "-", _value, lambda x: x.upper()
+                    cls.__join_with, "-", _value, lambda x: x.upper()
                 ),
                 "regex": r"(?P<strings_kebab_upper>[A-Z0-9]+(?:-[A-Z0-9]+)*)",
             },
             "%-K": {
                 "value": partial(
-                    Naming.__join_with, "-", _value, lambda x: x.capitalize()
+                    cls.__join_with, "-", _value, lambda x: x.capitalize()
                 ),
                 "cregex": "%T",
             },
             "%f": {
-                "value": partial(Naming.__join_with, "", _value),
+                "value": partial(cls.__join_with, "", _value),
                 "regex": r"(?P<flats>[a-z0-9]+)",
             },
             "%F": {
                 "value": partial(
-                    Naming.__join_with, "", _value, lambda x: x.upper()
+                    cls.__join_with, "", _value, lambda x: x.upper()
                 ),
                 "regex": r"(?P<flats_upper>[A-Z0-9]+)",
             },
             "%s": {
-                "value": partial(Naming.__join_with, "_", _value),
+                "value": partial(cls.__join_with, "_", _value),
                 "regex": r"(?P<strings_snake>[a-z0-9]+(?:_[a-z0-9]+)*)",
             },
             "%S": {
                 "value": partial(
-                    Naming.__join_with, "_", _value, lambda x: x.upper()
+                    cls.__join_with, "_", _value, lambda x: x.upper()
                 ),
                 "regex": r"(?P<strings_snake_upper>[A-Z0-9]+(?:_[A-Z0-9]+)*)",
             },
             "%-S": {
                 "value": partial(
-                    Naming.__join_with, "_", _value, lambda x: x.capitalize()
+                    cls.__join_with, "_", _value, lambda x: x.capitalize()
                 ),
                 "regex": (
                     r"(?P<strings_snake_title>"
                     r"[A-Z][a-z0-9]+(?:_[A-Z]+[a-z0-9]*)*)"
                 ),
             },
             "%T": {
                 "value": partial(
-                    Naming.__join_with, "-", _value, lambda x: x.capitalize()
+                    cls.__join_with, "-", _value, lambda x: x.capitalize()
                 ),
                 "regex": (
                     r"(?P<strings_train>"
                     r"[A-Z][a-z0-9]+(?:-[A-Z]+[a-z0-9]*)*)"
                 ),
             },
             "%v": {
@@ -2579,16 +2581,16 @@
                 "value": partial(
                     re.sub, r"[AEIOU]", "", "".join(_value).upper()
                 ),
                 "regex": r"(?P<vowels_upper>[B-DF-HJ-NP-TV-Z]+)",
             },
         }
 
-    @staticmethod
-    def prepare_value(value: str | list[str] | None) -> list[str]:
+    @classmethod
+    def prepare_value(cls, value: str | list[str] | None) -> list[str]:
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object. Return
         List of empty string if an input value does not pass.
 
         :param value: A value that want to prepare before passing to this
             naming formatter.
         :type value: str | list[str] | None
@@ -2597,15 +2599,15 @@
 
         :rtype: List[str]
         :return: A prepared naming value.
         """
         if value is None:
             return [""]
         if isinstance(value, str):
-            return Naming.__remove_special_char(value)
+            return cls.__remove_special_char(value)
         elif not isinstance(value, list) or any(
             not isinstance(v, str) for v in value
         ):
             raise FormatterValueError(
                 f"Naming formatter does not support for value, {value!r}."
             )
         return [re.sub(r"[^\-.\w\s]+", "", v) for v in value]
@@ -2707,28 +2709,28 @@
 
         :rtype: str
         :return: A string value with pascal case that reference by
             `inflection`.
         """
         return re.sub(r"(?:^|_)(.)", lambda m: m.group(1).upper(), snake_case)
 
-    @staticmethod
-    def camel_case(snake_case: str) -> str:
+    @classmethod
+    def camel_case(cls, snake_case: str) -> str:
         """Return a string value with camel case with lower case first
         letter.
 
         :param snake_case: A word with the snake case string.
         :type snake_case: str
 
         :rtype: str
         :return: A string value with camel case with lower case first
             letter.
         """
         return (
-            (snake_case[0].lower() + Naming.pascal_case(snake_case)[1:])
+            (snake_case[0].lower() + cls.pascal_case(snake_case)[1:])
             if snake_case
             else ""
         )
 
     @staticmethod
     def __join_with(
         by: str,
@@ -2798,14 +2800,22 @@
     "PB",
     "EB",
     "ZB",
     "YB",
 )
 
 
+@final
+class StorageSearchOrder(TypedDict):
+    """Type Dictionary for value of mapping of ``cls.search_order``"""
+
+    value: str
+    order: str
+
+
 class Storage(Formatter, fmt="%b"):
     """Storage formatter object that parse and format any storage value.
 
     .. note::
 
         A storage value will use ``decimal.Decimal`` package for wrap up
     standard value for this Storage formatter object.
@@ -2826,14 +2836,34 @@
         return Decimal(self.string)
 
     @property
     def string(self) -> str:
         """Return a bit string value."""
         return str(self.bit)  # type: ignore[no-any-return]
 
+    def validate(self) -> bool:
+        """Validate method that validate all Storage attributes in initialize
+        layer.
+
+        :raises FormatterValueError: If one of these rules was failed,
+            * attribute ``self.week`` does not equal with value.
+            * attribute ``self.locale`` does not equal with value.
+
+        :rtype: bool
+        :return: True if all validation rules was passed.
+        """
+        if (b := self.byte2bit(self.byte)) != self.bit:
+            raise FormatterValueError(
+                f"Byte that was parsed does not equal with bit, receive {b} bit"
+                f"(byte to bit) but get "
+                f"{self.bit:.{self.Config.storage_rounding:02d}f} bit from "
+                f"parsing."
+            )
+        return True
+
     @property
     def priorities(self) -> ReturnPrioritiesType:
         """Return a priorities value that define by property of this formatter
         object.
 
         Level Priority:
             [
@@ -2958,16 +2988,17 @@
             },
             "%Y": {
                 "value": partial(Storage.bit2byte, size, "YB"),
                 "regex": r"(?P<byte_yotta>[0-9]*YB)",
             },
         }
 
-    @staticmethod
+    @classmethod
     def prepare_value(
+        cls,
         value: int | float | Decimal | str | None,
     ) -> Decimal:
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object. Return 0 if an
         input value does not pass.
 
         :param value: A value that want to prepare before passing to this
@@ -2983,67 +3014,142 @@
         if value is None:
             return Decimal("0")
         if not can_float(value) or (Decimal(value) < 0):
             raise FormatterValueError(
                 f"Storage formatter does not support for value, {value!r}."
             )
         # Wrap the value to string after pass to decimal value.
-        return Decimal(str(value))
+        return cls.round_up(Decimal(str(value)))
 
-    @staticmethod
-    def round_up(value: Decimal) -> Decimal:
+    @classmethod
+    def round_up(cls, value: Decimal) -> Decimal:
         """Return a rounded value that use ``cls.Config.storage_rounding``.
 
         :param value: A decimal value that want to round up.
         :type value: decimal.Decimal
 
         :rtype: decimal.Decimal
         :return: A rounded value that use ``cls.Config.storage_rounding``.
         """
-        return round(value, Storage.Config.storage_rounding)
+        return round(value, cls.Config.storage_rounding)
 
     def __default_from_byte(self) -> Decimal:
         """Return default value that calculate from the byte value."""
-        return self.round_up(Decimal(self.byte or "0") * 8)
+        return Decimal(self.byte or "0") * 8
 
     def __default_from_bit(self) -> Decimal:
         """Return default value that calculate from the bit value."""
-        return self.round_up(Decimal(self.bit or "0") / 8)
+        return Decimal(self.bit or "0") / 8
 
-    @staticmethod
-    def bit2byte(value: Decimal, order: str) -> str:
+    @classmethod
+    def bit2byte(
+        cls,
+        value: Decimal,
+        order: str,
+        *,
+        suffix: bool = True,
+    ) -> str:
         """Convert the bit value to byte value with string type that depend on
         an input order value.
 
         :param value: A decimal value that want to convert to the byte string.
         :type value: str
         :param order: The order value that want to power with 1024.
         :type order: str
+        :param suffix: A suffix flag that will add order string to return value
+        :type suffix: bool
+
+        Examples:
+
+            >>> Storage.bit2byte('150', 'B')
+            19B
+            >>> Storage.bit2byte('150', 'B', suffix=False)
+            19
 
         :rtype: str
-        :return: The bit value to byte value with string type that depend on
-            an input order value.
+        :return: The bit to byte value with string type that depend on an input
+            order value.
         """
         p: Decimal = Decimal(math.pow(1024, SIZE.index(order)))
-        return f"{(Storage.round_up((value / 8) / p))}{order}"
+        return f"{(cls.round_up((value / 8) / p))}{order if suffix else ''}"
 
-    @staticmethod
-    def str2byte(value: str, order: str) -> Decimal:
+    @classmethod
+    def search_order(cls, value: str) -> StorageSearchOrder:
+        """Searching order suffix
+
+        :rtype: StorageSearchOrder
+        """
+        _decimal: str = (
+            rf"(?:\.\d{{0,{st_round}}})?"
+            if (st_round := cls.Config.storage_rounding) > 0
+            else ""
+        )
+        return (
+            s.groupdict()
+            if (
+                s := re.search(
+                    rf"(?P<value>\d+{_decimal})(?P<order>[KMGTPEZY]?B)?",
+                    value,
+                )
+            )
+            else {"value": value, "order": "B"}
+        )
+
+    @classmethod
+    def str2byte(cls, value: str, order: str | None = None) -> Decimal:
         """Convert to byte value that depend on an input order value.
 
         :param value: A string value that want to convert to the byte value.
         :type value: str
         :param order: The order value that want to power with 1024.
-        :type order: str
+        :type order: str | None(=None)
+
+        Examples:
+
+            >>> Storage.str2byte('12MB', 'MB')
 
         :rtype: decimal.Decimal
         :return: A converted byte value that depend on an input order value.
         """
+        if order is None:
+            searching: StorageSearchOrder = cls.search_order(value)
+            value = searching["value"]
+            order = searching["order"]
         p: Decimal = Decimal(math.pow(1024, SIZE.index(order)))
-        return Storage.round_up(Decimal(value.replace(order, "")) * p)
+        return cls.round_up(Decimal(value.replace(order, "")) * p)
+
+    @classmethod
+    def byte2bit(cls, value: str | Decimal, order: str = "B") -> Decimal:
+        """Convert the byte value to bit value with string type that depend on
+        an input order value or default with `B`.
+
+        :param value: A decimal value that want to convert to the byte string.
+        :type value: str
+        :param order: The order value that want to power with 1024.
+        :type order: str(=B)
+
+        Examples:
+
+            >>> Storage.byte2bit(19.000)
+            152.000
+
+        :rtype: decimal.Decimal
+        :return: The byte to bit value with string type that depend on an input
+            order value.
+        """
+        p: Decimal = Decimal(math.pow(1024, SIZE.index(order)))
+        return cls.round_up(
+            (
+                Decimal(value.replace(order, ""))
+                if isinstance(value, str)
+                else value
+            )
+            * p
+            * 8
+        )
 
 
 ConstantComparator: TypeAlias = Callable[["Constant", "Constant"], bool]
 
 
 def const_comparison(operator: ConstantComparator) -> ConstantComparator:
     """Decorator function for compare operators in the Constant class."""
@@ -3610,29 +3716,27 @@
         fmt: str,
     ) -> FormatterGroup:
         """Parse bytes or string value with its format to this formatter object.
         This method generates the value for itself data that can be formatted
         to another format string values.
 
         :param value: A bytes or string value that match with fmt.
-        :type value: str
+        :type value: String
         :param fmt: a format string value that must have the formatter group
             pattern like `{group-name:fmt-str}`.
         :type fmt: str
 
         :rtype: FormatterGroup
         :return: An instance of formatter group that parse from a bytes or
             string value by a format string.
         """
-        _value: str = bytes2str(value)
-        parser_rs: ReturnParseType = cls.__parse(_value, fmt)
+        parser_rs: ReturnParseType = cls.__parse(bytes2str(value), fmt)
         rs: dict[str, DictStr] = defaultdict(dict)
         for g in parser_rs:
-            group_origin: str = g.split("__")[0]
-            rs[group_origin] |= parser_rs[g]["props"]
+            rs[g.split("__")[0]] |= parser_rs[g]["props"]
         return cls(formats=rs)
 
     @classmethod
     def __parse(
         cls,
         value: str,
         fmt: str,
```

### Comparing `fmtutil-1.0.4/fmtutil/utils.py` & `fmtutil-1.0.4.post0/fmtutil/utils.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/.gitignore` & `fmtutil-1.0.4.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/LICENSE` & `fmtutil-1.0.4.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/README.md` & `fmtutil-1.0.4.post0/README.md`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/pyproject.toml` & `fmtutil-1.0.4.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.4/PKG-INFO` & `fmtutil-1.0.4.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fmtutil
-Version: 1.0.4
+Version: 1.0.4.post0
 Summary: The Utility Formatter Objects
 Project-URL: Homepage, https://github.com/korawica/fmtutil/
 Project-URL: Source Code, https://github.com/korawica/fmtutil/
 Author-email: korawica <korawich.anu@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: formatter,utility
```

