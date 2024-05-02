# Comparing `tmp/fmtutil-1.0.3.tar.gz` & `tmp/fmtutil-1.0.4.tar.gz`

## Comparing `fmtutil-1.0.3.tar` & `fmtutil-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__about__.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__main__.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__type.py
--rw-r--r--   0        0        0    36848 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__version.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/cli.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/exceptions.py
--rw-r--r--   0        0        0   133534 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/formatter.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/utils.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.3/LICENSE
--rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.3/README.md
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 fmtutil-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 fmtutil-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__about__.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__main__.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__type.py
+-rw-r--r--   0        0        0    36743 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/__version.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/cli.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/exceptions.py
+-rw-r--r--   0        0        0   133878 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/formatter.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 fmtutil-1.0.4/fmtutil/utils.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.4/LICENSE
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.4/README.md
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 fmtutil-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 fmtutil-1.0.4/PKG-INFO
```

### Comparing `fmtutil-1.0.3/fmtutil/__init__.py` & `fmtutil-1.0.4/fmtutil/__init__.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.3/fmtutil/__type.py` & `fmtutil-1.0.4/fmtutil/__type.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.3/fmtutil/__version.py` & `fmtutil-1.0.4/fmtutil/__version.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from functools import wraps
 from re import Pattern
 from typing import (
     Any,
     Callable,
     ClassVar,
     NoReturn,
-    Optional,
     SupportsInt,
     Union,
     cast,
     get_args,
 )
 
 from typing_extensions import TypeAlias
@@ -361,15 +360,15 @@
     @comparison
     def __ge__(self, other: Comparable) -> bool:
         return self.compare(other) >= 0
 
     def __getitem__(
         self,
         index: Union[int, slice],
-    ) -> Union[int, Optional[str], tuple[Union[int, str], ...]]:
+    ) -> Union[int, str | None, tuple[Union[int, str], ...]]:
         """If the part requested is undefined, or a part of the range requested
         is undefined, it will throw an index error.
 
         Negative indices are not supported.
 
         :param index: a positive integer indicating the offset or a ``slice``
             object.
@@ -566,15 +565,15 @@
         else:
             match = cls.regex.match(version)
         if match is None:
             raise ValueError(f"{version} is not valid {cls.__name__} string")
 
         return cls(**match.groupdict())
 
-    def replace(self, **parts: Union[int, Optional[str]]) -> BaseVersion:
+    def replace(self, **parts: Union[int, str | None]) -> BaseVersion:
         """Replace one or more parts of a version and return a new instance.
 
         :param parts: the parts to be updated. Valid keys are:
             ``major``, ``minor``, ``patch``, ``pre``, or ``build``
 
         :raises TypeError: if ``parts`` contain invalid keys
 
@@ -582,15 +581,15 @@
         """
         version = self.to_dict()
         version.update(parts)
         try:
             return self.__class__(**version)
         except TypeError as err:
             unknown = set(parts) - set(self.to_dict())
-            error = (
+            error: str = (
                 f"replace() got {len(unknown)} unexpected keyword "
                 f"argument(s): {', '.join(unknown)}"
             )
             raise TypeError(error) from err
 
     @classmethod
     def is_valid(cls, version: str) -> bool:
@@ -622,15 +621,15 @@
         if (0 == self.major == other.major) and (self[:3] != other[:3]):
             return False
 
         return (self.major == other.major) and (other.minor >= self.minor)
 
     @staticmethod
     def _extract_letter(
-        letter: Optional[str],
+        letter: str | None,
         force_raise: bool = False,
     ) -> tuple[str, int]:
         """Extract letter to standard word.
 
         :param letter: A letter string that want to extract with prefix pattern.
         :param force_raise: A flag for forcing raise error if an input letter
             does not match with standard prefix.
@@ -713,29 +712,29 @@
 
     def __init__(
         self,
         epoch: SupportsInt = 0,
         major: SupportsInt = 0,
         minor: SupportsInt = 0,
         patch: SupportsInt = 0,
-        pre: Optional[Union[String, int]] = None,
-        post: Optional[Union[String, int]] = None,
-        dev: Optional[Union[String, int]] = None,
-        local: Optional[String] = None,
+        pre: String | int | None = None,
+        post: String | int | None = None,
+        dev: String | int | None = None,
+        local: String | None = None,
     ):
         super().__init__(major, minor, patch)
         if (ep := int(epoch or "0")) < 0:
             raise ValueError(
                 f"{epoch!r} is negative. A epoch version can only be positive."
             )
 
         self.epoch: int = ep
-        self.pre: Optional[str] = None if pre is None else str(pre)
-        self.post: Optional[str] = None if post is None else str(post)
-        self.dev: Optional[str] = None if dev is None else str(dev)
+        self.pre: str | None = None if pre is None else str(pre)
+        self.post: str | None = None if post is None else str(post)
+        self.dev: str | None = None if dev is None else str(dev)
         self.local = None if local is None else str(local)
 
     def __extract_tuple(self):
         release: tuple[int, ...] = necessary_release(self.to_tuple()[1:4])
         if self.pre is None and self.post is None and self.dev is not None:
             pre = NegInf
         elif self.pre is None:
@@ -753,39 +752,39 @@
                 (i, "") if isinstance(i, int) else (NegInf, i)
                 for i in self.__extract_local(self.local)
             )
         return self.epoch, release, pre, post, dev, local
 
     @staticmethod
     def __extract_local(
-        local: Optional[str],
-    ) -> Optional[tuple[Union[str, int], ...]]:
+        local: str | None,
+    ) -> tuple[Union[str, int], ...] | None:
         if local is not None:
             return tuple(
                 part.lower() if not part.isdigit() else int(part)
                 for part in re.compile(r"[._-]").split(local)
             )
         return None
 
     @property
-    def v_pre(self) -> Optional[int]:
+    def v_pre(self) -> int | None:
         """Return the version number of pre part if it was set."""
         return self._extract_letter(self.pre)[1] if self.pre else None
 
     @property
-    def v_post(self) -> Optional[int]:
+    def v_post(self) -> int | None:
         """Return the version number of post part if it was set."""
         return self._extract_letter(self.post)[1] if self.post else None
 
     @property
-    def v_dev(self) -> Optional[int]:
+    def v_dev(self) -> int | None:
         """Return the version number of dev part if it was set."""
         return self._extract_letter(self.dev)[1] if self.dev else None
 
-    def bump_pre(self, token: Optional[str] = "rc") -> VersionPackage:
+    def bump_pre(self, token: str | None = "rc") -> VersionPackage:
         """Raise the pre part of the packaging version, return a new object.
 
         :rtype: VersionPackage
         :return: A new object with the raised pre part.
         """
         cls = type(self)
         if self.pre is not None:
@@ -980,22 +979,22 @@
     )
 
     def __init__(
         self,
         major: SupportsInt,
         minor: SupportsInt = 0,
         patch: SupportsInt = 0,
-        pre: Optional[Union[String, int]] = None,
-        build: Optional[Union[String, int]] = None,
+        pre: String | int | None = None,
+        build: String | int | None = None,
     ):
         super().__init__(major, minor, patch)
-        self.pre: Optional[str] = None if pre is None else str(pre)
-        self.build: Optional[str] = None if build is None else str(build)
+        self.pre: str | None = None if pre is None else str(pre)
+        self.build: str | None = None if build is None else str(build)
 
-    def bump_pre(self, token: Optional[str] = "rc") -> VersionSemver:
+    def bump_pre(self, token: str | None = "rc") -> VersionSemver:
         """Raise the pre part of the version, return a new object but leave
         self untouched.
 
         :param token: defaults to ``'rc'``
         :return: new :class:`Version` object with the raised pre part.
             The original object is not modified.
         """
@@ -1007,15 +1006,15 @@
             pre = "rc.0"
         else:
             pre = str(token) + ".0"
 
         pre = increment(pre)
         return self.__class__(self.major, self.minor, self.patch, pre)
 
-    def bump_build(self, token: Optional[str] = "build") -> VersionSemver:
+    def bump_build(self, token: str | None = "build") -> VersionSemver:
         """Raise the build part of the version, return a new object but leave
         self untouched.
 
         :param token: defaults to ``'build'``
         :return: new :class:`Version` object with the raised build part.
             The original object is not modified.
         """
```

### Comparing `fmtutil-1.0.3/fmtutil/cli.py` & `fmtutil-1.0.4/fmtutil/cli.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.3/fmtutil/exceptions.py` & `fmtutil-1.0.4/fmtutil/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
 """
-Define Errors Object for formatter
+Define Errors Object for formatter that will use instead built-in exception
+classes without NotImplementedError only.
 """
 from __future__ import annotations
 
-from typing import Union
-
 
 class BaseError(Exception):
     """Base Error Object that use for catch any errors statement of
     all step in this package.
     """
 
 
@@ -36,22 +35,22 @@
         >>> FormatterArgumentError(
         ...     argument='demo',
         ...     message='does not support',
         ... )
         FormatterArgumentError("with 'demo', does not support")
 
     :param argument: An argument of this error that raise to client
-    :type argument: Union[str, tuple]
+    :type argument: str | tuple
     :param message: A string message of this error
     :type message: str
     """
 
     def __init__(
         self,
-        argument: Union[str, tuple[str, ...]],
+        argument: str | tuple[str, ...],
         message: str,
     ) -> None:
         """Main Initialization that merge the argument and message input values
         with specific content message together like
 
             `__class__` with `argument`, `message`
         """
@@ -72,8 +71,8 @@
 
 
 class FormatterGroupValueError(FormatterValueError):
     """Error raise for value does not valid"""
 
 
 class FormatterGroupArgumentError(FormatterArgumentError):
-    """Error raise for a wrong configuration argument."""
+    """Error raise for a wrong configuration argument"""
```

### Comparing `fmtutil-1.0.3/fmtutil/formatter.py` & `fmtutil-1.0.4/fmtutil/formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 from functools import lru_cache, partial, total_ordering, wraps
 from itertools import tee, zip_longest
 from typing import (
     Any,
     Callable,
+    ClassVar,
     NoReturn,
-    Optional,
     TypedDict,
     Union,
     final,  # docs: https://github.com/python/mypy/issues/9953
 )
 
 from dateutil.relativedelta import relativedelta
 from typing_extensions import TypeAlias
@@ -54,14 +54,15 @@
     caller,
     can_float,
     can_int,
     convert_fmt_str,
     default,
     itself,
     remove_pad,
+    scache,
 )
 
 FormatterType = type["Formatter"]
 FormatterGroupType = type["FormatterGroup"]
 ConstantType = type["Constant"]
 
 PriorityCallable: TypeAlias = Union[
@@ -72,15 +73,15 @@
 FormatterCallable: TypeAlias = Union[Callable[[], Any], partial[Any]]
 
 
 class PriorityValue(TypedDict):
     """Type Dictionary for value of mapping of ``cls.priorities``"""
 
     value: PriorityCallable
-    level: Optional[Union[int, TupleInt]]
+    level: int | TupleInt | None
 
 
 @final
 class CRegexValue(TypedDict):
     """Type Dictionary for value of mapping of ``cls.formatter``"""
 
     value: Union[FormatterCallable, str]
@@ -116,15 +117,15 @@
             A list of boolean that have index equal the level attribute.
         * count: int
             A counting number of True value in the slot.
         * value: int
             A sum of weighted value from a True value in any slot position.
 
     Methods:
-        * update: [Optional[Union[int, TupleInt]]] -> SlotLevel
+        * update: int | TupleInt | None -> SlotLevel
             Self that was updated level
         * checker: [Union[int, TupleInt]] -> bool
             A True if all values in ``self.slot`` that match with index numbers
             are True.
 
     Static-methods:
         * make_tuple: [Union[int, TupleInt]] -> TupleInt
@@ -176,26 +177,26 @@
         :return: A sum of weighted value from a True value in any slot
             position.
         """
         return sum(index * int(i) for index, i in enumerate(self.slot, start=1))
 
     def update(
         self,
-        numbers: Optional[Union[int, TupleInt]] = None,
+        numbers: int | TupleInt | None = None,
         strict: bool = True,
     ) -> SlotLevel:
         """Update boolean value in ``self.slot`` from False to True.
 
         :param numbers: updated numbers of this SlotLevel object.
         :type numbers: Union[int, TupleInt]
         :param strict: a strict flag for raise error when pass out of
             range numbers.
         :type strict: bool(=True)
 
-        :raises ValueError: if updated number does not exist in range.
+        :raises FormatterValueError: if updated number does not exist in range.
 
         :rtype: SlotLevel
         :return: Self that was updated level
         """
         _numbers: Union[int, TupleInt] = numbers or (0,)
         for num in self.make_tuple(_numbers):
             if num == 0:
@@ -208,15 +209,15 @@
                     f"number for update the slot level object does not "
                     f"in range of 0 and {self.level}."
                 )
         return self
 
     def checker(
         self,
-        numbers: Union[int, TupleInt],
+        numbers: int | TupleInt,
     ) -> bool:
         """Return True if boolean value in ``self.slot`` is all True.
 
         :param numbers: An index number values that want to check in slot.
         :type numbers: Union[int, TupleInt]
 
         :rtype: bool
@@ -230,15 +231,15 @@
                 if (0 <= (_n := (n - 1)) <= (self.level - 1))
                 else False
             )
             for n in filter(lambda x: x != 0, _numbers)
         )
 
     @staticmethod
-    def make_tuple(value: Union[int, TupleInt]) -> TupleInt:
+    def make_tuple(value: int | TupleInt) -> TupleInt:
         """Return tuple of integer value that was created from input value
         parameter if it is not tuple.
 
         :param value: a tuple of integers or any integer
         :type value: Union[int, TupleInt]
 
         :rtype: TupleInt
@@ -250,19 +251,19 @@
 @dataclass(frozen=True)
 class PriorityData:
     """Priority Data class.
 
     .. dataclass attributes::
 
         - value: PriorityCallable
-        - level: Optional[Union[int, TupleInt]]
+        - level: int | TupleInt | None
     """
 
     value: PriorityCallable = field(default=itself, repr=False)
-    level: Optional[Union[int, TupleInt]] = field(default=(0,))
+    level: int | TupleInt | None = field(default=(0,))
 
 
 class BaseFormatter(ABC):
     """Base-class Formatter object that implement `__slots__` attribute for any
     instance classes.
 
     .. metaclass attributes::
@@ -277,15 +278,15 @@
 class Formatter(BaseFormatter):
     """Formatter object for inherit to any formatter subclass that define
     format and parse method. The base class will implement necessary
     properties and method for subclass that should implement or enhance such
     as `the cls.formatter()` method or the `cls.priorities` property.
 
     :param formats: A mapping value of priority attribute data.
-    :type formats: Optional[Dict[str, Any]](=None)
+    :type formats: dict[str, Any] | None(=None)
     :param set_strict_mode: A flag to allow checking duplicate attribute value.
     :type set_strict_mode: bool(=False)
     :param set_std_value: A flag to allow for set standard value form string,
         `self.class-name.lower()` if it True.
     :type set_std_value: bool(=True)
 
     .. class attributes::
@@ -322,15 +323,15 @@
         * priorities: ReturnPrioritiesType
             A priorities value that define by property of this formatter object.
 
     .. methods::
         * _setter_std_value: [bool] -> NoReturn
             Setting standard value that have an argument name be the class name
             with lower case if input flag is True.
-        * values: [Optional[Any]] -> DictStr
+        * values: Any | None -> DictStr
             A dict of format string, and it's string value that was passed an
             input value to `cls.formatter` method.
         * format: [str] -> str
             A string value that was formatted from format string pattern.
         * validate: [] -> bool
             A Validate method that will call after setup all attributes in
             initialize layer.
@@ -339,53 +340,58 @@
             and a format string pattern is valid with ``self.value``.
         * to_const: [] -> ConstantType
             A Constant object that create from constant of ``self.values`` and
             has class name with ``f'{self.__class__.__name__}Const'`` with
             ``self.values()``.
 
     .. static-methods::
-        * __validate_format: [Optional[Dict[str, Any]]] -> Dict[str, Any]
+        * __validate_format: Dict[str, Any] | None -> Dict[str, Any]
             A formats value that validate with duplicate format string values.
-        * formatter: [Optional[Any]] -> ReturnFormattersType
+        * formatter: Any | None -> ReturnFormattersType
             A formatter value that define by property of this formatter object.
         * prepare_value: [Any] -> Any
             A prepared value with defined logic.
 
     .. seealso::
 
         This class is abstract class for any formatter class. It will raise
     `NotImplementedError` when the necessary attributes and methods does not
     implement from subclass.
     """
 
     # This value must reassign from child class
-    base_fmt: str = ""
+    base_fmt: ClassVar[str] = ""
 
     # This value must reassign from child class
-    base_level: int = 1
+    base_level: ClassVar[int] = 1
 
     class Config:
         """A Configuration object that use for group and keep any config for
         this sub-formatter object.
         """
 
-        base_config_value: Optional[Any] = None
+        base_config_value: ClassVar[Any | None] = None
 
     def __init_subclass__(
         cls: FormatterType,
         /,
-        level: Optional[int] = None,
+        level: int | None = None,
+        fmt: str | None = None,
         **kwargs: Any,
     ) -> NoReturn:
-        """Subclass Initialize method.
+        """Subclass Initialize method that will declare class variables if it
+        set from class creation or direct override with that variables.
 
-        :param level
-        :type level: int (default=1)
+        :param level: The max level that this formatter class will limit.
+        :type level: int | None(=1)
+        :param fmt: The default format string value that use on the parsing.
+        :type fmt: str | None(=None)
         """
-        cls.base_level = level or cls.base_level
+        cls.base_level: int = level or cls.base_level
+        cls.base_fmt: str = fmt or cls.base_fmt
         super().__init_subclass__(**kwargs)
 
         if not cls.base_fmt:
             raise NotImplementedError(
                 "Please implement base_fmt class property for this "
                 "sub-formatter class."
             )
@@ -419,34 +425,34 @@
         fmts, values = zip(*fmt_filter)
         return cls.parse(value="_".join(values), fmt="_".join(fmts))
 
     @classmethod
     def parse(
         cls,
         value: String,
-        fmt: Optional[str] = None,
+        fmt: str | None = None,
         *,
         strict: bool = False,
     ) -> Formatter:
         """Parse bytes or string value with its format to this formatter object.
         This method generates the value for itself data that can be formatted
         to another format string values.
 
         :param value: A bytes or string value that match with fmt.
         :type value: String
         :param fmt: a format value will use `cls.base_fmt` if it does not pass
             from input argument.
-        :type fmt: Optional[str](=None)
+        :type fmt: str | None(=None)
         :param strict: A flag strict validate that pass to ``set_strict_mode``.
         :type strict: bool(=False)
 
         :raises NotImplementedError: if fmt value parameter does not pass form
             input, or `cls.base_fmt` does not implement.
-        :raises ValueError: if value does not match with regular expression
-            format string.
+        :raises FormatterValueError: if value does not match with regular
+            expression format string.
 
         :rtype: Formatter
         :return: An instance of formatter that parse from a bytes or string
             value by a format string or base format string if it None.
         """
         _fmt: str = fmt or cls.base_fmt
         _value: str = bytes2str(value)
@@ -466,44 +472,47 @@
         )
 
     @classmethod
     def gen_format(
         cls,
         fmt: str,
         *,
-        prefix: Optional[str] = None,
-        suffix: Optional[str] = None,
+        prefix: str | None = None,
+        suffix: str | None = None,
         alias: bool = True,
     ) -> str:
         """Generate format string value that combine from any matching of
         format name with format regular expression value that able to search.
 
         :param fmt: a format string value pass from input argument.
         :type fmt: str
         :param prefix: a prefix string value that will add to alias format
             string value.
-        :type prefix: Optional[str]
+        :type prefix: str | None(=None)
         :param suffix: a suffix string value that will add to alias format
             string value.
-        :type suffix: Optional[str]
+        :type suffix: str | None(=None)
         :param alias: an alias boolean flag that will pass alias name if it
             true to the format string value.
         :type alias: bool
 
         :rtype: str
         :return: A format string value that was changed to the regular
             expression string value for comply with the `re` module to any
             string value.
         """
         _cache: dict[str, int] = defaultdict(int)
         _prefix: str = prefix or ""
         _suffix: str = suffix or ""
         regexes = cls.regex()
-        for fmt_match in re.finditer(r"(%[-+!*]?[A-Za-z])", fmt):
+        for fmt_match in re.finditer(r"(%?%[-+!*]?[A-Za-z])", fmt):
             fmt_str: str = fmt_match.group()
+            if fmt_str.startswith("%%"):
+                fmt = fmt.replace(fmt_str, fmt_str[1:], 1)
+                continue
             if fmt_str not in regexes:
                 raise FormatterArgumentError(
                     "fmt",
                     (
                         f"The format string, {fmt_str!r}, does not exists in "
                         f"``cls.regex``."
                     ),
@@ -514,15 +523,18 @@
                 r"\(\?P<(?P<alias>\w+)>(?P<fmt>(?:(?!\(\?P<\w+>).)*)\)",
                 regex,
             ):
                 _sr_re: str = fmt_inside.group("alias")
                 regex = re.sub(
                     rf"\(\?P<{_sr_re}>",
                     (
-                        f"(?P<{_prefix}{_sr_re}__{_cache[_sr_re]}{_suffix}>"
+                        (
+                            f"(?P<{_prefix}{_sr_re}{scache(_cache[_sr_re])}"
+                            f"{_suffix}>"
+                        )
                         if alias
                         else "("
                     ),
                     regex,
                     count=1,
                 )
                 _cache[_sr_re] += 1
@@ -583,15 +595,15 @@
                             f"format cregex string that contain {cs} regex "
                             f"does not found."
                         ),
                     )
             results[f] = cr.replace("[ESCAPE]", "%%")
         return results
 
-    def values(self, value: Optional[Any] = None) -> DictStr:
+    def values(self, value: Any | None = None) -> DictStr:
         """Return a dict of format string, and it's string value that was passed
         an input value to `cls.formatter` method.
 
         :rtype: DictStr
         :return: A dict of format string, and it's string value that was passed
             an input value to `cls.formatter` method.
 
@@ -632,15 +644,15 @@
                     f"the format: {_fmt_str!r} does not support for "
                     f"{self.__class__.__name__!r}"
                 ) from err
         return fmt.replace("[ESCAPE]", "%")
 
     def __init__(
         self,
-        formats: Optional[dict[str, Any]] = None,
+        formats: dict[str, Any] | None = None,
         *,
         set_strict_mode: bool = False,
         set_std_value: bool = True,
     ) -> None:
         """Main initialization get the format mapping from input argument
         and generate the necessary attributes for define the value of this
         base formatter object.
@@ -807,22 +819,22 @@
             raise FormatterValueError(
                 f"Parsing value does not valid with {error}."
             )
         return not sl
 
     @staticmethod
     def __validate_format(
-        formats: Optional[dict[str, Any]] = None,
+        formats: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         """Return a formats value that validate with duplicate format string
         values, and it will raise error if any duplication format name do not
         all equal.
 
         :param formats:
-        :type formats: Optional[Dict[str, Any]]
+        :type formats: dict[str, Any] | None(=None)
 
         :rtype: Dict[str, Any]
         :return: A formats value that validate with duplicate format string
             values.
         """
         results: dict[str, Any] = {}
         _formats: dict[str, Any] = formats or {}
@@ -851,20 +863,20 @@
         raise NotImplementedError(
             "Please implement ``priorities`` property for this sub-formatter "
             "class"
         )
 
     @staticmethod
     @abstractmethod
-    def formatter(value: Optional[Any] = None) -> ReturnFormattersType:
+    def formatter(value: Any | None = None) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object.
 
         :param value: An any value that want to generate with formatter.
-        :type value: Optional[Any](=None)
+        :type value: Any | None(=None)
 
         :rtype: ReturnFormattersType
         :return: a formatter value that define by property of this formatter
             object.
         """
         raise NotImplementedError(
             "Please implement ``formatter`` static method for this "
@@ -928,21 +940,19 @@
         except (TypeError, FormatterValueError):
             return NotImplemented
 
     def __format__(self, format_spec) -> str:
         return self.format(format_spec)
 
 
-class Serial(Formatter):
+class Serial(Formatter, fmt="%n"):
     """Serial formatter object that parse and format any serial (positive
     integer) value.
     """
 
-    base_fmt: str = "%n"
-
     class Config(Formatter.Config):
         serial_max_padding: int = 3
         serial_max_binary: int = 8
 
     __slots__ = (
         "number",
         "serial",
@@ -999,27 +1009,27 @@
                 "value": default("0"),
                 "level": 0,
             },
         }
 
     @staticmethod
     def formatter(
-        serial: Optional[Union[int, str, float]] = None,
+        serial: int | str | float | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %n  : Normal serial number
             %p  : Padding serial number
             %b  : Binary number
             %c  : Normal with comma separate number
             %u  : Normal with underscore separate number
 
         :param serial: A serial value that pass to generate all format.
-        :type serial: Optional[Union[int, str, float]](=None)
+        :type serial: int | str | float | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             serial formatter object.
         """
         _value: int = Serial.prepare_value(serial)
         return {
@@ -1046,22 +1056,22 @@
             "%u": {
                 "value": partial(itself, f"{_value:_}"),
                 "regex": r"(?P<number_underscore>\d{1,3}(?:_\d{3})*)",
             },
         }
 
     @staticmethod
-    def prepare_value(value: Optional[Union[int, str, float]]) -> int:
+    def prepare_value(value: int | str | float | None) -> int:
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object. Return 0 if an
         input value does not pass.
 
         :param value: A value that want to prepare before passing to this
             serial formatter.
-        :type value: Optional[Union[int, str, float]]
+        :type value: int | str | float | None
 
         :raises FormatterValueError: If an input value does not able cast to
             integer, or it's value less than 0.
 
         :rtype: int
         :return: A prepared positive integer value.
         """
@@ -1140,19 +1150,17 @@
     "3": "Wednesday",
     "4": "Tuesday",
     "5": "Friday",
     "6": "Saturday",
 }
 
 
-class Datetime(Formatter, level=10):
+class Datetime(Formatter, level=10, fmt="%Y-%m-%d %H:%M:%S.%f"):
     """Datetime formatter object that parse and format any datetime value."""
 
-    base_fmt: str = "%Y-%m-%d %H:%M:%S.%f"
-
     __slots__ = (
         "year",
         "month",
         "week",
         "weeks",
         "day",
         "hour",
@@ -1400,15 +1408,15 @@
                 "value": default("000000"),
                 "level": 0,
             },
         }
 
     @staticmethod
     def formatter(
-        dt: Optional[Union[str, datetime, date]] = None,
+        dt: str | datetime | date | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %n  : Normal format with `%Y%m%d_%H%M%S`
         **  %G  : ISO 8601 year
         **  %C  : Century
@@ -1446,15 +1454,15 @@
         **  %V  : ISO 8601 week-number (01-53)
             %p  : Locale’s AM or PM.
             %f  : Microsecond as a decimal number, zero-padded on the left.
         **  %x  : Local version of date (%Y/%m/%d)
         **  %X  : Local version of time (%H:%M:%S)
 
         :param dt: A datetime value that pass to generate all format.
-        :type dt: Optional[Union[str, datetime, date]](=None)
+        :type dt: str | datetime | date | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             datetime formatter object.
         """
         _dt: datetime = Datetime.prepare_value(dt)
         return {
@@ -1583,22 +1591,22 @@
             "%f": {
                 "value": partial(_dt.strftime, "%f"),
                 "regex": r"(?P<microsecond_pad>\d{6})",
             },
         }
 
     @staticmethod
-    def prepare_value(value: Optional[Union[str, datetime, date]]) -> datetime:
+    def prepare_value(value: str | datetime | date | None) -> datetime:
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object. Return
         ``datetime.now()`` if an input value does not pass.
 
         :param value: A value that want to prepare before passing to this
             datetime formatter.
-        :type value: Optional[Union[str, datetime, date]]
+        :type value: str | datetime | date | None
 
         :raises FormatterValueError: If an input value does be
             ``datetime.datetime`` or ``datetime.date``.
 
         :rtype: datetime
         :return: A prepared datetime value.
         """
@@ -1779,15 +1787,15 @@
             return self.value - other.value
         return NotImplemented
 
     def __rsub__(self, other: Any) -> Any:
         return NotImplemented
 
 
-class Version(Formatter, level=4):
+class Version(Formatter, level=4, fmt="%m_%n_%c"):
     """Version formatter object that parse and format any version
     (``packaging.version.Version``) value.
 
     .. patterns::
 
         Version segments reference from ``packaging.version``:
         - epoch             1!1.0.0
@@ -1820,16 +1828,14 @@
         - The standard of versioning will align with the PEP0440
         (https://peps.python.org/pep-0440/)
 
         - Enhance the version object from the packaging library
         (https://packaging.pypa.io/en/latest/version.html)
     """
 
-    base_fmt: str = "%m_%n_%c"
-
     __slots__ = (
         "version",
         "epoch",
         "major",
         "minor",
         "micro",
         "pre",
@@ -1953,15 +1959,15 @@
                 "value": lambda x: x,
                 "level": 0,
             },
         }
 
     @staticmethod
     def formatter(
-        version: Optional[Union[str, VerPackage]] = None,
+        version: str | VerPackage | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %f  : full version format with `%m_%n_%c`
             %-f : full version format with `%m-%n-%c`
         **  %r  : release version format `%m.%n.%c`
@@ -1973,15 +1979,15 @@
             %p  : post release
             %-p : post release number
             %d  : dev release
             %l  : local release
             %-l : local release number
 
         :param version: A version value that pass to generate all format.
-        :type version: Optional[Union[str, __version.VersionPackage]](=None)
+        :type version: str | __version.VerPackage | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             version formatter object.
         """
         _version: VerPackage = Version.prepare_value(version)
         return {
@@ -2047,24 +2053,24 @@
                 "value": partial(itself, f"+{_version.local}"),
                 "regex": r"(?P<local_str>[a-z0-9]+(?:[-_\.][a-z0-9]+)*)",
             },
         }
 
     @staticmethod
     def prepare_value(
-        value: Optional[Union[str, VerPackage]],
+        value: str | VerPackage | None,
     ) -> VerPackage:
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object. Return
         ``__version.VersionPackage.parse("0.0.1")`` if an input value does not
         pass.
 
         :param value: A value that want to prepare before passing to this
             version formatter.
-        :type value: Optional[Union[str, __version.VersionPackage]]
+        :type value: str |  __version.VersionPackage | None
 
         :raises FormatterValueError: If an input value does be
             ``__version.VersionPackage``
 
         :rtype: __version.VersionPackage
         :return: A prepared version value.
         """
@@ -2154,25 +2160,23 @@
     def __sub__(self, other: Any):  # type: ignore # no cov
         return NotImplemented
 
     def __rsub__(self, other: Any):  # type: ignore # no cov
         return NotImplemented
 
 
-class Naming(Formatter, level=5):
+class Naming(Formatter, level=5, fmt="%n"):
     """Naming formatter object that parse and format any name value.
 
     .. note::
 
         A name value that parsing to this class should not contain any
     special characters, this will keep only.
     """
 
-    base_fmt: str = "%n"
-
     __slots__ = (
         "naming",
         "strings",
         "flats",
         "shorts",
         "vowels",
     )
@@ -2395,15 +2399,15 @@
                 ),
                 "level": 0,
             },
         }
 
     @staticmethod
     def formatter(
-        nm: Optional[Union[str, list[str]]] = None,
+        nm: str | list[str] | None = None,
     ) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %n  : Normal name format
             %N  : Normal name upper case format
             %-N : Normal name title case format
@@ -2427,15 +2431,15 @@
             %v  : normal name removed vowel
             %V  : normal name removed vowel with upper case
 
         .. refs::
             * https://gist.github.com/SuppieRK/a6fb471cf600271230c8c7e532bdae4b
 
         :param nm: A naming value that pass to generate all format.
-        :type nm: Optional[Union[str, List[str]]](=None)
+        :type nm: str | list[str] | None(=None)
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             naming formatter object.
         """
         _value: list[str] = Naming.prepare_value(nm)
         return {
@@ -2576,22 +2580,22 @@
                     re.sub, r"[AEIOU]", "", "".join(_value).upper()
                 ),
                 "regex": r"(?P<vowels_upper>[B-DF-HJ-NP-TV-Z]+)",
             },
         }
 
     @staticmethod
-    def prepare_value(value: Optional[Union[str, list[str]]]) -> list[str]:
+    def prepare_value(value: str | list[str] | None) -> list[str]:
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object. Return
         List of empty string if an input value does not pass.
 
         :param value: A value that want to prepare before passing to this
             naming formatter.
-        :type value: Optional[Union[str, List[str]]]
+        :type value: str | list[str] | None
 
         :raises FormatterValueError: If an input value does be list of str.
 
         :rtype: List[str]
         :return: A prepared naming value.
         """
         if value is None:
@@ -2725,25 +2729,25 @@
             else ""
         )
 
     @staticmethod
     def __join_with(
         by: str,
         values: list[str],
-        func: Optional[Callable[[str], str]] = None,
+        func: Callable[[str], str] | None = None,
     ) -> str:
         """Return a string value that join with any separate string after
         prepare with an input function if it set.
 
         :param by: A seperator string that want to join.
         :type by: str
         :param values: A list of word that want to join with.
         :type values: List[str]
         :param func: A function that want to prepare before join.
-        :type func: Optional[Callable[[str], str]](=None)
+        :type func: Callable[[str], str] | None(=None)
 
         :rtype: str
         :return: A string value that join with any separate string after
             prepare with an input function if it set.
         """
         return by.join(map(func, values)) if func else by.join(values)
 
@@ -2794,25 +2798,23 @@
     "PB",
     "EB",
     "ZB",
     "YB",
 )
 
 
-class Storage(Formatter):
+class Storage(Formatter, fmt="%b"):
     """Storage formatter object that parse and format any storage value.
 
     .. note::
 
         A storage value will use ``decimal.Decimal`` package for wrap up
     standard value for this Storage formatter object.
     """
 
-    base_fmt: str = "%b"
-
     class Config(Formatter.Config):
         storage_rounding: int = 0
 
     __slots__ = (
         "bit",
         "byte",
         "storage",
@@ -2890,15 +2892,15 @@
             "byte_default": {
                 "value": self.__default_from_bit,
                 "level": 0,
             },
         }
 
     @staticmethod
-    def formatter(storage: Optional[int] = None) -> ReturnFormattersType:
+    def formatter(storage: int | None = None) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object. Generate formatter that support mapping formatter,
 
             %b  : Bit format
             %B  : Byte format
             %K  : Kilo-Byte format
             %M  : Mega-Byte format
@@ -2906,15 +2908,15 @@
             %T  : Tera-Byte format
             %P  : Peta-Byte format
             %E  : Exa-Byte format
             %Z  : Zetta-Byte format
             %Y  : Yotta-Byte format
 
         :param storage: A storage value that pass to generate all format.
-        :type storage: Optional[int]
+        :type storage: int | None
 
         :rtype: ReturnFormattersType
         :return: A generated mapping values of all format string pattern of this
             storage formatter object.
         """
         size: Decimal = Storage.prepare_value(storage)
         return {
@@ -2958,23 +2960,23 @@
                 "value": partial(Storage.bit2byte, size, "YB"),
                 "regex": r"(?P<byte_yotta>[0-9]*YB)",
             },
         }
 
     @staticmethod
     def prepare_value(
-        value: Union[int, float, Decimal, str, None],
+        value: int | float | Decimal | str | None,
     ) -> Decimal:
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object. Return 0 if an
         input value does not pass.
 
         :param value: A value that want to prepare before passing to this
             storage formatter.
-        :type value: Optional[int, float, Decimal, str]
+        :type value: int | float | Decimal | str | None
 
         :raises FormatterValueError: If an input value does not able cast to
             integer, or it's value less than 0.
 
         :rtype: decimal.Decimal
         :return: A prepared positive decimal value.
         """
@@ -3040,40 +3042,40 @@
         return Storage.round_up(Decimal(value.replace(order, "")) * p)
 
 
 ConstantComparator: TypeAlias = Callable[["Constant", "Constant"], bool]
 
 
 def const_comparison(operator: ConstantComparator) -> ConstantComparator:
+    """Decorator function for compare operators in the Constant class."""
+
     @wraps(operator)
     def wrapper(self: Constant, other) -> bool:
         if not issubclass(other.__class__, Constant):
             return NotImplemented
         return operator(self, other)
 
     return wrapper
 
 
-class Constant(Formatter):
+class Constant(Formatter, fmt="%%"):
     """Constant object for create Constant class in the constructor function.
 
     :param formats: A mapping value of priority attribute data.
-    :type formats: Optional[Dict[str, Any]](=None)
+    :type formats: Dict[str, Any] | None(=None)
     :param set_strict_mode: A flag to allow checking duplicate attribute value.
     :type set_strict_mode: bool(=False)
 
     .. seealso::
 
         This class does not implement abstract properties because it does not
     any senses to compare a constant instance such as ``__add__``, or
     ``__sub__`` properties.
     """
 
-    base_fmt: str = "%%"
-
     __slots__: tuple[str, ...] = ("_constant",)
 
     @classmethod
     def from_value(cls, value: Any) -> NoReturn:
         """Passer the value to this formatter that will pass this value to
         ``cls.formatter`` method and map with the base format string value
         before parse by ``cls.parse``.
@@ -3089,26 +3091,26 @@
             "class initialization."
         )
 
     @classmethod
     def parse(
         cls,
         value: String,
-        fmt: Optional[str] = None,
+        fmt: str | None = None,
         *,
         strict: bool = False,
     ) -> Formatter:
         """Parse bytes or string value with its format to this formatter object.
         This method generates the value for itself data that can be formatted
         to another format string values.
 
         :param value: A bytes or string value that match with fmt.
         :type value: String
         :param fmt: a format value.
-        :type fmt: Optional[str](=None)
+        :type fmt: str | None(=None)
         :param strict: A flag strict validate that pass to ``set_strict_mode``.
         :type strict: bool(=False)
 
         :raises NotImplementedError: If an input fmt value does not pass.
 
         :rtype: Formatter
         :return: An instance of formatter that parse from a bytes or string
@@ -3119,15 +3121,15 @@
                 "The Constant class does not support for default format string "
                 "when parsing with this unknown format value."
             )
         return super().parse(value, fmt, strict=strict)
 
     def __init__(
         self,
-        formats: Optional[dict[str, Any]] = None,
+        formats: dict[str, Any] | None = None,
         *,
         set_strict_mode: bool = False,
     ) -> None:
         """Main initialization get the format mapping from input argument
         and generate the necessary attributes for define the value of this
         base formatter object. This process will set the standard value after
         set ``self._constant`` value.
@@ -3182,20 +3184,20 @@
         """
         raise NotImplementedError(
             "Please implement ``priorities`` property for this sub-constant "
             "formatter class"
         )
 
     @staticmethod
-    def formatter(value: Optional[str] = None) -> ReturnFormattersType:
+    def formatter(value: str | None = None) -> ReturnFormattersType:
         """Return a formatter value that define by property of this formatter
         object.
 
         :param value: An any value that want to generate with formatter.
-        :type value: Optional[str](=None)
+        :type value: str | None(=None)
 
         :rtype: ReturnFormattersType
         :return: a formatter value that define by property of this formatter
             object.
         """
         raise NotImplementedError(
             "Please implement ``formatter`` staticmethod for this sub-constant "
@@ -3240,38 +3242,38 @@
         return self < other
 
 
 def dict2const(
     fmt: DictStr,
     name: str,
     *,
-    base_fmt: Optional[str] = None,
+    base_fmt: str | None = None,
 ) -> ConstantType:
     """Constant function constructor that receive the dict of format string
     value and constant value.
 
     :param fmt: A mapping of format string and value of its format that want
         to make constant object.
     :type fmt: DictStr
     :param name: A custom class name that want to rename.
     :type name: str
     :param base_fmt: A base format string value.
-    :type base_fmt: Optional[str](=None)
+    :type base_fmt: str | None(=None)
 
     :rtype: ConstantType
     :return: A constant object that construct from an input fmt and name values.
     """
     _base_fmt: str = base_fmt or "".join(fmt.keys())
 
     class CustomConstant(Constant):
         """Dynamic Custom Constant object that will change the class name to an
         input name from constructor function.
         """
 
-        base_fmt: str = _base_fmt
+        base_fmt: ClassVar[str] = _base_fmt
 
         __qualname__ = name
 
         __slots__: tuple[str, ...] = (
             name.lower(),
             "_constant",
             *(convert_fmt_str(f) for f in fmt),
@@ -3282,22 +3284,22 @@
                 f"<{self.__class__.__name__}"
                 f".parse('{self.string}', "
                 f"{'|'.join(self.__search_fmt(c) for c in self._constant)!r})>"
             )
 
         @staticmethod
         def formatter(  # type: ignore[override]
-            v: Optional[str] = None,
+            v: str | None = None,
         ) -> ReturnFormattersType:
             """Return a formatter value that define by property of this
             formatter object. Generate formatter that support mapping formatter
             with an input dict in fmt value.
 
             :param v: A constant value that pass to generate all format.
-            :type v: Optional[int](=None)
+            :type v: str | None(=None)
 
             :rtype: ReturnFormattersType
             :return: A generated mapping values of all format string pattern of
                 this constant formatter object.
             """
             # It does not use an input value.
             _ = CustomConstant.prepare_value(v)
@@ -3323,15 +3325,15 @@
             :returns: A properties of the constant formatter object.
             """
             return {
                 convert_fmt_str(f): {"value": lambda x: x, "level": 1}
                 for f in fmt
             }
 
-        def values(self, value: Optional[Any] = None) -> DictStr:
+        def values(self, value: Any | None = None) -> DictStr:
             """Return the constant values"""
             _ = self.prepare_value(value)
             return fmt
 
         def __search_fmt(self, value: str) -> str:
             """Return the first format that equal to an input string value.
 
@@ -3344,41 +3346,41 @@
             return [k for k, v in iter(self.values().items()) if v == value][0]
 
     CustomConstant.__name__ = name
     return CustomConstant
 
 
 def make_const(
-    name: Optional[str] = None,
-    formatter: Optional[Union[DictStr, Formatter]] = None,
+    name: str | None = None,
+    formatter: DictStr | Formatter | None = None,
     *,
-    fmt: Optional[FormatterType] = None,
-    value: Optional[Any] = None,
+    fmt: FormatterType | None = None,
+    value: Any | None = None,
 ) -> ConstantType:
     """Helper constant constructor function that will prepare all input values
     before call ``dict2const`` constructor function.
 
     :param name: A custom class name that want to rename.
-    :type name: Optional[str](=None)
+    :type name: str | None(=None)
     :param formatter: ...
-    :type formatter: Optional[Union[DictStr, Formatter]]
+    :type formatter: DictStr | Formatter | None
     :param fmt: A formatter object.
-    :type fmt: Optional[FormatterType](=None)
+    :type fmt: FormatterType | None(=None)
     :param value: A value that want to passer to an input fmt value.
-    :type value: Optional[Any](=None)
+    :type value: Any | None(=None)
 
     :raises FormatterArgumentError: If an input formatter was passed together
         with an input fmt value.
     :raises FormatterArgumentError: If an input name does not set for construct
         a constant object.
 
     :rtype: ConstantType
     :return: A constant object that construct from an input fmt and name values.
     """
-    base_fmt: Optional[str] = None
+    base_fmt: str | None = None
     _fmt: DictStr
     if formatter is None:
         if fmt is None or not inspect.isclass(fmt):
             raise FormatterArgumentError(
                 "formatter",
                 "The Constant constructor function must pass formatter nor fmt "
                 "arguments.",
@@ -3473,15 +3475,15 @@
 class FormatterGroup:
     """Group of Formatters with dynamic group naming like 'timestamp' for
     Datetime, 'name' for Naming. This class will use for ``make_group``
     constructor function because of different and complicate group of formatter
     instances.
 
     :param formats: A mapping value of priority attribute data.
-    :type formats: Optional[dict](=None)
+    :type formats: FormatsGroupType
     :param ignore_construct: A flag for ignore pass an input formats value to
         validate and construct function.
     :type ignore_construct: bool(=False)
 
     :raises FormatterGroupValueError: If any group naming from an input formats
         does not exist in ``cls.base_groups`` value.
 
@@ -3515,15 +3517,15 @@
             A Formatter instance.
         * format: [str] -> str
             A string value that was formatted and filled by an input format
             string pattern.
         * adjust: [Dict[str, Any]] -> FormatterGroup
             Adjust any formatter instance in ``self.groups`` of this formatter
             group.
-        * to_const: [Optional[List[str]]] -> FormatterGroupType
+        * to_const: list[str] | None -> FormatterGroupType
             A FormatterGroup object that create from constant of ``self.groups``
             values.
 
     .. seealso::
 
         This class is an abstract class for any formatter group that override
     the ``cls.base_groups`` value with mapping for group naming and Formatter
@@ -3620,17 +3622,17 @@
         :rtype: FormatterGroup
         :return: An instance of formatter group that parse from a bytes or
             string value by a format string.
         """
         _value: str = bytes2str(value)
         parser_rs: ReturnParseType = cls.__parse(_value, fmt)
         rs: dict[str, DictStr] = defaultdict(dict)
-        for group in parser_rs:
-            group_origin: str = group.split("__")[0]
-            rs[group_origin] |= parser_rs[group]["props"]
+        for g in parser_rs:
+            group_origin: str = g.split("__")[0]
+            rs[group_origin] |= parser_rs[g]["props"]
         return cls(formats=rs)
 
     @classmethod
     def __parse(
         cls,
         value: str,
         fmt: str,
@@ -3661,17 +3663,17 @@
         _search_dict: DictStr = _search.groupdict()
         rs: ReturnParseType = {}
         for name in iter(_fmt_getter.copy()):
             rs[name] = {
                 "fmt": _fmt_getter[name]["fmt"],
                 "value": _search_dict.pop(name),
                 "props": {
-                    k.replace(name, "", 1): _search_dict.pop(k)
+                    k.replace(f"{name}___", "", 1): _search_dict.pop(k)
                     for k in filter(
-                        lambda x: x.startswith(name),
+                        lambda x: x.startswith(f"{name}___"),
                         _search_dict.copy(),
                     )
                 },
             }
         return rs
 
     @classmethod
@@ -3699,19 +3701,19 @@
             ):
                 # Format Dict Example:
                 # {'name': '{timestamp:%Y_%m_%d}', 'format': '%Y_%m_%d'}
                 fmt_dict: DictStr = fmt_match.groupdict()
                 fmt_str: str
                 if not (fmt_str := fmt_dict["format"]):
                     fmt_str = formatter.base_fmt
-                group_index: str = f"{group}__{_index}"
+                group_index: str = f"{group}{scache(_index)}"
                 fmt_re = formatter.gen_format(
                     fmt_str,
-                    prefix=group_index,
-                    suffix=f"{_index}",
+                    prefix=f"{group_index}___",
+                    suffix=scache(_index),
                 )
                 fmt = fmt.replace(
                     fmt_dict["found"],
                     f"(?P<{group_index}>{fmt_re})",
                     1,
                 )
                 fmt_getter[group_index] = {"fmt": fmt_str}
@@ -3877,15 +3879,15 @@
             k: (fmt + values[k]) if k in values else fmt
             for k, fmt in self.groups.items()
         }
         return self.__class__(formats=_groups)
 
     def to_const(
         self,
-        included: Optional[list[str]] = None,
+        included: list[str] | None = None,
     ) -> FormatterGroupType:  # no cov
         """Convert this formatter group instance to constant group object.
 
         :rtype: FormatterGroupType
         :return: A FormatterGroup object that create from constant of
             ``self.groups`` values.
         """
@@ -3909,27 +3911,27 @@
 def make_group(group: BaseGroupsType) -> FormatterGroupType:
     """Making Formatter Group constructor function that return a FormatterGroup
     class from an input group value.
 
     :param group: A dict of group naming and Formatter class.
     :type group: BaseGroupsType
 
-    :raises ValueError: If any value in an input group does not be subclassed of
-        Formatter instance.
+    :raises FormatterGroupValueError: If any value in an input group does not
+        be subclassed of Formatter instance.
     :raises FormatterGroupArgumentError: If any value in an input group does not
         be objected that mean this value is any instance.
 
     :rtype: FormatterGroupType
     :return: A FormatterGroup class that construct from an input group value.
     """
     # Validate argument group that should contain ``FormatterType``
     for _ in group.values():
         try:
             if not issubclass(_, Formatter):
-                raise ValueError(
+                raise FormatterGroupValueError(
                     f"Make group constructor function want group with type, "
                     f"Dict[str, FormatterType], not {_.__name__!r}."
                 )
         except TypeError as err:
             raise FormatterGroupArgumentError(
                 "group",
                 (
```

### Comparing `fmtutil-1.0.3/fmtutil/utils.py` & `fmtutil-1.0.4/fmtutil/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import re
 from collections.abc import Iterable
 from decimal import Decimal
 from typing import (
     Any,
     Callable,
-    Union,
     get_args,
 )
 
 from .__type import String
 
 FMT_STR_MAP: dict[str, str] = {
     "-": "minus",
@@ -44,56 +43,54 @@
     "V": "victor",
     "W": "whiskey",
     "X": "xray",
     "Y": "yankee",
     "Z": "zulu",
 }
 
-concat: Callable[[Union[list[str], Iterable[str]]], str] = "".join
+concat: Callable[[list[str] | Iterable[str]], str] = "".join
 
 
 def itself(x: Any = None) -> Any:
     """Return itself value"""
     return x
 
 
 def default(value: Any) -> Callable[[], Any]:
     """Return wrapper function of value"""
     return lambda: value
 
 
-def caller(func: Union[Callable[[], Any], Any]) -> Any:
+def caller(func: Callable[[], Any] | Any) -> Any:
     """Call function if it was callable
 
     Examples:
-
-    >>> some_func = lambda: 100
-    >>> caller(some_func)
-    100
+        >>> some_func = lambda: 100
+        >>> caller(some_func)
+        100
     """
     return func() if callable(func) else func
 
 
 def convert_fmt_str(fmt: str) -> str:
     """Convert format string to format string name
 
     Examples:
-
-    >>> convert_fmt_str('%a')
-    'alpha'
-    >>> convert_fmt_str('%!b')
-    'bravo_exclamation'
-    >>> convert_fmt_str('%S')
-    'sierra_upper'
-    >>> convert_fmt_str('%-N')
-    'november_upper_minus'
-    >>> convert_fmt_str('G')
-    'G'
-    >>> convert_fmt_str('%H')
-    'hotel_upper'
+        >>> convert_fmt_str('%a')
+        'alpha'
+        >>> convert_fmt_str('%!b')
+        'bravo_exclamation'
+        >>> convert_fmt_str('%S')
+        'sierra_upper'
+        >>> convert_fmt_str('%-N')
+        'november_upper_minus'
+        >>> convert_fmt_str('G')
+        'G'
+        >>> convert_fmt_str('%H')
+        'hotel_upper'
     """
     _fmt_re: str = fmt
     if search := re.search(r"^%(?P<prefix>[-+!*]?)(?P<format>[a-zA-Z])$", fmt):
         search_dict = search.groupdict()
         _fmt: str
         if (_fmt := search_dict["format"]).isupper():
             _fmt_re = f"{FMT_STR_OTAN_MAP[_fmt]}upper"
@@ -106,71 +103,72 @@
     return _fmt_re
 
 
 def can_int(value: Any) -> bool:
     """Check value that able cast to integer.
 
     Example:
-
-    >>> can_int('0.0')
-    True
-    >>> can_int('-1.0')
-    True
+        >>> can_int('0.0')
+        True
+        >>> can_int('-1.0')
+        True
     """
     try:
         return float(str(value)).is_integer()
     except (TypeError, ValueError):
         return False
 
 
 def can_float(value: Any) -> bool:
     """Check value that able cast to float.
 
     Example:
-
-    >>> can_float('0.01')
-    True
-    >>> can_float('0.1a')
-    False
+        >>> can_float('0.01')
+        True
+        >>> can_float('0.1a')
+        False
     """
     if value is None:
         return False
     try:
         float(value)
         return True
     except ValueError:
         return False
 
 
 def remove_pad(value: str) -> str:
     """Remove zero padding of string
 
     Examples:
-
-    >>> remove_pad('000')
-    '0'
-    >>> remove_pad('0123')
-    '123'
+        >>> remove_pad('000')
+        '0'
+        >>> remove_pad('0123')
+        '123'
     """
     return _last_char if (_last_char := value[-1]) == "0" else value.lstrip("0")
 
 
 def bytes2str(value: String) -> str:
     """Convert byte to string
 
     Example:
-
-    >>> bytes2str(b'foo')
-    'foo'
-    >>> bytes2str('foo')
-    'foo'
+        >>> bytes2str(b'foo')
+        'foo'
+        >>> bytes2str('foo')
+        'foo'
     """
     if isinstance(value, bytes):
         value = str(value, "utf-8", "strict")
     elif not isinstance(value, get_args(String)):
         raise TypeError(f"not expecting type '{type(value)}'")
     return value
 
 
 def float2decimal(value: float, precision: int = 15) -> Decimal:
     """Convert float to decimal with default precision value."""
     return Decimal(value).quantize(Decimal(10) ** -precision)
+
+
+def scache(cache_num: int) -> str:
+    """Return cache suffix string"""
+    return f"__{cache_num}" if cache_num > 0 else ""
```

### Comparing `fmtutil-1.0.3/.gitignore` & `fmtutil-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.3/LICENSE` & `fmtutil-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.3/README.md` & `fmtutil-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.3/pyproject.toml` & `fmtutil-1.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -49,58 +49,59 @@
 perf = [
     "memory-profiler==0.61.0",
 ]
 
 [project.scripts]
 fmtutil = "fmtutil.__main__:main"
 
-[tool.shelf.git]
-commit_prefix_force_fix = true
-
 [tool.shelf.version]
 version = "./fmtutil/__about__.py"
 changelog = "./docs/en/docs/CHANGELOG.md"
 
+[tool.shelf.git]
+commit_prefix_force_fix = true
+
+[tool.hatch.version]
+scheme = "standard"
+source = "code"
+path = "fmtutil/__about__.py"
+
+[tool.hatch.build.targets.sdist]
+exclude = [
+    "/.github",
+    "/docs",
+    "/tests",
+    "/.pre-commit-config.yaml",
+    "/fmtutil/__assets.py",
+]
+
+[tool.hatch.build.targets.wheel]
+packages = ["fmtutil"]
+
 [tool.coverage.run]
 branch = true
 concurrency = ["thread", "multiprocessing"]
 parallel = true
 context = '${CONTEXT}'
 source = [
     "fmtutil",
 ]
 omit = [
     "tests/perfs/",
     "scripts/",
     "fmtutil/__about__.py",
+    "fmtutil/__assets.py",
     "fmtutil/__main__.py",
     "fmtutil/__type.py",
     "fmtutil/__version.py",
     "fmtutil/cli.py",
     "fmtutil/utils.py",
-    "fmtutil/migrate/",
 ]
 relative_files = true
 
-[tool.hatch.version]
-scheme = "standard"
-source = "code"
-path = "fmtutil/__about__.py"
-
-[tool.hatch.build.targets.sdist]
-exclude = [
-    "/.github",
-    "/docs",
-    "/tests",
-    "/.pre-commit-config.yaml",
-]
-
-[tool.hatch.build.targets.wheel]
-packages = ["fmtutil"]
-
 [tool.coverage.report]
 exclude_lines = [
     "no cov",
     "if TYPE_CHECKING:",
     "raise NotImplementedError",
 ]
 
@@ -143,30 +144,32 @@
         | venv
     )/
 )
 """
 
 [tool.ruff]
 line-length = 80
-lint.select = [
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".git",
+    ".mypy_cache",
+    ".ruff_cache",
+    "venv",
+]
+
+[tool.ruff.lint]
+select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
-lint.ignore = [
+ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".git",
-    ".mypy_cache",
-    ".ruff_cache",
-    "venv",
-]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `fmtutil-1.0.3/PKG-INFO` & `fmtutil-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fmtutil
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Utility Formatter Objects
 Project-URL: Homepage, https://github.com/korawica/fmtutil/
 Project-URL: Source Code, https://github.com/korawica/fmtutil/
 Author-email: korawica <korawich.anu@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: formatter,utility
```

