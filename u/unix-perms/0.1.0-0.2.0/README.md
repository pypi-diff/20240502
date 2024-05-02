# Comparing `tmp/unix_perms-0.1.0.tar.gz` & `tmp/unix_perms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unix_perms-0.1.0.tar", max compression
+gzip compressed data, was "unix_perms-0.2.0.tar", max compression
```

## Comparing `unix_perms-0.1.0.tar` & `unix_perms-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1087 2024-04-27 19:48:15.257972 unix_perms-0.1.0/LICENSE
--rw-r--r--   0        0        0      579 2024-04-27 21:30:34.965879 unix_perms-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      169 2024-04-27 19:48:56.504844 unix_perms-0.1.0/README.md
--rw-r--r--   0        0        0      697 2024-04-28 03:22:56.656843 unix_perms-0.1.0/unix_perms/__init__.py
--rw-r--r--   0        0        0      373 2024-04-28 03:22:56.343490 unix_perms-0.1.0/unix_perms/exceptions.py
--rw-r--r--   0        0        0      814 2024-04-28 03:22:56.667361 unix_perms-0.1.0/unix_perms/models.py
--rw-r--r--   0        0        0     6272 2024-04-28 03:22:56.671364 unix_perms-0.1.0/unix_perms/octals.py
--rw-r--r--   0        0        0     2679 2024-04-28 03:22:56.336360 unix_perms-0.1.0/unix_perms/permissions.py
--rw-r--r--   0        0        0    12350 2024-04-28 03:25:41.223163 unix_perms-0.1.0/unix_perms/types.py
--rw-r--r--   0        0        0      445 2024-04-28 03:22:56.705384 unix_perms-0.1.0/unix_perms/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 unix_perms-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-04-27 19:48:15.257972 unix_perms-0.2.0/LICENSE
+-rw-r--r--   0        0        0      578 2024-05-02 03:51:04.540285 unix_perms-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      169 2024-05-02 03:43:08.690947 unix_perms-0.2.0/README.md
+-rw-r--r--   0        0        0      698 2024-05-02 03:51:08.238864 unix_perms-0.2.0/unix_perms/__init__.py
+-rw-r--r--   0        0        0      373 2024-04-28 03:22:56.343490 unix_perms-0.2.0/unix_perms/exceptions.py
+-rw-r--r--   0        0        0      814 2024-04-28 03:22:56.667361 unix_perms-0.2.0/unix_perms/models.py
+-rw-r--r--   0        0        0     6281 2024-05-02 03:50:07.478447 unix_perms-0.2.0/unix_perms/octals.py
+-rw-r--r--   0        0        0     2679 2024-04-28 03:22:56.336360 unix_perms-0.2.0/unix_perms/permissions.py
+-rw-r--r--   0        0        0    12350 2024-05-02 03:47:57.916375 unix_perms-0.2.0/unix_perms/types.py
+-rw-r--r--   0        0        0      445 2024-04-28 03:22:56.705384 unix_perms-0.2.0/unix_perms/utils.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 unix_perms-0.2.0/PKG-INFO
```

### Comparing `unix_perms-0.1.0/LICENSE` & `unix_perms-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unix_perms-0.1.0/pyproject.toml` & `unix_perms-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "unix-perms"
-version = "0.1.0"
-description = "Manage and interpret Linux file permissions with a Python package that provides intuitive tools for creating, validating, and describing permission codes."
+version = "0.2.0"
+description = "Manage and interpret Unix file permissions with a Python package that provides intuitive tools for creating, validating, and describing permission modes."
 authors = ["galactixx"]
 readme = "README.md"
 license = "MIT LICENSE"
 keywords = [
     "unix",
     "permissions",
     "files"
```

### Comparing `unix_perms-0.1.0/unix_perms/__init__.py` & `unix_perms-0.2.0/unix_perms/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from unix_perms.exceptions import InvalidOctalError
 from unix_perms.octals import (OctalConfig, from_octal_digit_to_config,
-                               from_octal_to_permissions_code,
-                               is_permissions_code)
+                               from_octal_to_permissions_mode,
+                               is_permissions_mode)
 from unix_perms.permissions import OctalPermissions
-from unix_perms.types import (PermissionsByte, PermissionsCode,
-                              PermissionsConfig)
+from unix_perms.types import (PermissionsByte, PermissionsConfig,
+                              PermissionsMode)
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 __all__ = [
     'InvalidOctalError',
     'OctalPermissions',
     'from_octal_digit_to_config',
-    'from_octal_to_permissions_code',
-    'is_permissions_code',
+    'from_octal_to_permissions_mode',
+    'is_permissions_mode',
     'OctalConfig',
     'PermissionsByte',
-    'PermissionsCode',
+    'PermissionsMode',
     'PermissionsConfig'
-]
+]
```

### Comparing `unix_perms-0.1.0/unix_perms/models.py` & `unix_perms-0.2.0/unix_perms/models.py`

 * *Files identical despite different names*

### Comparing `unix_perms-0.1.0/unix_perms/octals.py` & `unix_perms-0.2.0/unix_perms/octals.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     octal_config = _get_octal_digit_config(octal_digit=octal_digit)
     return octal_config
 
 
 def _octal_validation(octal: str) -> str:
     """
-    Private function to validate and convert a string Unix permissions code to a three digit code.
+    Private function to validate and convert a string Unix permissions mode to a three digit mode.
     """
     octal_string_length: int = len(octal)
 
     if not 1 <= octal_string_length <= 3:
         raise InvalidOctalError(
             'invalid octal representation length, must have a length ranging from 0 to 3'
         )
@@ -82,39 +82,39 @@
             'invalid digits in octal representation, digits must range from 0 to 7'
         )
 
     octal_int_string_repr: str = octal.zfill(3)
     return octal_int_string_repr
 
 
-def _to_octal_str_repr_conversion(octal: int) -> str:
+def _from_decimal_to_permissions_mode(octal: int) -> str:
     """
     Private function to convert a decimal representation of an octal
-    to a three digit string Unix permissions code.
+    to a three digit string Unix permissions mode.
     """
     octal_string: str = format(octal, 'o')
     octal_int_string_repr: str = _octal_validation(octal=octal_string)
     return octal_int_string_repr
 
 
-def from_octal_to_permissions_code(octal: Union[str, int]) -> str:
+def from_octal_to_permissions_mode(octal: Union[str, int]) -> str:
     """
-    Creates a Unix permissions code from an octal representation.
+    Creates a Unix permissions mode from an octal representation.
 
     This function accepts either a string or an integer as input. If the argument is
     a string, the value must be either in the format of an octal literal (e.g., '0o777')
-    or as a Unix permissions code (e.g., '777'). If the value is an integer, it must be a
+    or as a Unix permissions mode (e.g., '777'). If the value is an integer, it must be a
     decimal representation of an octal as an octal literal (e.g., 0o777) or directly as an
     integer (e.g., 511).
 
     Args:
         octal (str | int): An octal representation as a string or integer.
 
     Returns:
-        str: A string representation of a Unix permissions code.
+        str: A string representation of a Unix permissions mode.
     """
     if not isinstance(octal, (str, int)):
         raise TypeError(
             f"{type(octal)} is not a valid 'octal' type, must be of type ('str', 'int')"
         )
 
     if isinstance(octal, str):
@@ -127,36 +127,36 @@
 
         try:
             octal_as_int = int(octal, int_base)
         except ValueError:
             raise InvalidOctalError(message)
         else:
             octal_as_str = str(octal_as_int)
-            permissions_code: str = _octal_validation(octal=octal_as_str)
-            return permissions_code
+            permissions_mode: str = _octal_validation(octal=octal_as_str)
+            return permissions_mode
     else:
-        permissions_code: str = _to_octal_str_repr_conversion(octal=octal)
-        return permissions_code
+        permissions_mode: str = _from_decimal_to_permissions_mode(octal=octal)
+        return permissions_mode
 
 
-def is_permissions_code(octal: str) -> bool:
+def is_permissions_mode(octal: str) -> bool:
     """
-    A boolean function which determines if an octal representation is a valid Unix permissions code.
+    A boolean function which determines if an octal representation is a valid Unix permissions mode.
 
     This function accepts either a string or an integer as input. If the argument is
     a string, the value must be either in the format of an octal literal (e.g., '0o777')
-    or as a Unix permissions code (e.g., '777'). If the value is an integer, it must be a
+    or as a Unix permissions mode (e.g., '777'). If the value is an integer, it must be a
     decimal representation of an octal as an octal literal (e.g., 0o777) or directly as an
     integer (e.g., 511).
 
     Args:
         octal (str | int): An octal representation as a string or integer.
 
     Returns:
-        bool: A boolean indicating whether the octal is a Unix permissions code.
+        bool: A boolean indicating whether the octal is a Unix permissions mode.
     """
     try:
-        _ = from_octal_to_permissions_code(octal=octal)
-        is_perms_code = True
+        _ = from_octal_to_permissions_mode(octal=octal)
+        is_perms_mode = True
     except InvalidOctalError:
-        is_perms_code = False
-    return is_perms_code
+        is_perms_mode = False
+    return is_perms_mode
```

### Comparing `unix_perms-0.1.0/unix_perms/permissions.py` & `unix_perms-0.2.0/unix_perms/permissions.py`

 * *Files identical despite different names*

### Comparing `unix_perms-0.1.0/unix_perms/types.py` & `unix_perms-0.2.0/unix_perms/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Literal, Union
 
 from pydantic import BaseModel
 
 from unix_perms.octals import (OctalConfig, from_octal_digit_to_config,
-                               from_octal_to_permissions_code)
+                               from_octal_to_permissions_mode)
 from unix_perms.permissions import OctalPermissions
 from unix_perms.utils import get_all_class_parameters
 
 
 class PermissionsConfig(BaseModel):
     """
     File permissions configuration for an octal digit. Can specify whether
@@ -55,31 +55,31 @@
     ):
         self.authority = authority
         self._config = config
 
         # Set permissions for specific authority
         self.permissions = OctalPermissions(authority=self.authority)
 
-    def __add__(self, permission_byte: 'PermissionsByte') -> 'PermissionsCode':
+    def __add__(self, permission_byte: 'PermissionsByte') -> 'PermissionsMode':
         if not isinstance(permission_byte, PermissionsByte):
             raise TypeError(
                 f'can only add PermissionsByte (not "{type(permission_byte)}") to PermissionsByte'
             )
 
-        return PermissionsCode._from_permissions_bytes(
+        return PermissionsMode._from_permissions_bytes(
             permissions_byte_one=self, permissions_byte_two=permission_byte
         )
 
     def __str__(self) -> str:
         return repr(self)
 
     def __repr__(self) -> str:
         return (
             f'<{self.__class__.__name__} authority={self.authority} '
-            f'permissions_code={self.permissions_code}>'
+            f'permissions_mode={self.permissions_mode}>'
         )
 
     @property
     def read_permission(self) -> bool:
         """A boolean indicating whether read permission is included."""
         return self._config.read
 
@@ -90,67 +90,67 @@
 
     @property
     def execute_permission(self) -> bool:
         """A boolean indicating whether execute permission is included."""
         return self._config.execute
 
     @property
-    def permissions_code(self) -> str:
-        """The Unix permissions code."""
+    def permissions_mode(self) -> str:
+        """The Unix permissions mode."""
         base_permissions = self.permissions.no_permissions
         if self._config.read:
             base_permissions |= self.permissions.read
 
         if self._config.write:
             base_permissions |= self.permissions.write
 
         if self._config.execute:
             base_permissions |= self.permissions.execute
 
         return format(base_permissions, 'o').zfill(3)
 
     @property
     def permissions_description(self) -> str:
-        """A string description of the Unix permissions code."""
-        permissions_code = self.permissions_code.strip('0')
-        permissions_code = permissions_code or 0
-        permissions_code = int(permissions_code)
-        octal_config: OctalConfig = from_octal_digit_to_config(octal_digit=permissions_code)
+        """A string description of the Unix permissions mode."""
+        permissions_mode = self.permissions_mode.strip('0')
+        permissions_mode = permissions_mode or 0
+        permissions_mode = int(permissions_mode)
+        octal_config: OctalConfig = from_octal_digit_to_config(octal_digit=permissions_mode)
         return octal_config.description
 
     @property
     def permissions_description_detailed(self) -> Dict[str, Union[str, bool]]:
-        """A more detailed description of the Unix permissions code, as a dict."""
+        """A more detailed description of the Unix permissions mode, as a dict."""
         return {
             'authority': self.authority,
-            'code': self.permissions_code,
+            'mode': self.permissions_mode,
             'read': self.read_permission,
             'write': self.write_permission,
             'execute': self.execute_permission
         }
 
     @property
-    def permissions_code_as_decimal_repr(self) -> int:
-        """The decimal representation of the Unix permissions code"""
-        return int(self.permissions_code, 8)
+    def permissions_mode_as_decimal_repr(self) -> int:
+        """The decimal representation of the Unix permissions mode"""
+        return int(self.permissions_mode, 8)
 
     @property
-    def permissions_code_as_int(self) -> int:
-        """The integer representation of the Unix permissions code"""
-        return int(self.permissions_code)
+    def permissions_mode_as_int(self) -> int:
+        """The integer representation of the Unix permissions mode"""
+        return int(self.permissions_mode)
 
     @property
-    def permissions_code_as_octal_literal(self) -> str:
-        """The string octal literal representation of the Unix permissions code."""
-        return f'0o{self.permissions_code}'
+    def permissions_mode_as_octal_literal(self) -> str:
+        """The string octal literal representation of the Unix permissions mode."""
+        return f'0o{self.permissions_mode}'
 
 
-class PermissionsCode:
+class PermissionsMode:
     """
-    A simple structure representing a full Unix permissions code, including all
+    A simple structure representing a full Unix permissions mode, including all
     of the following authorites: ('owner', 'group', 'others').
 
     Args:
         owner (PermissionsByte): A PermissionsByte instance for the owner authority.
         group (PermissionsByte): A PermissionsByte instance for the group authority.
         others (PermissionsByte): A PermissionsByte instance for the others authority.
     """
@@ -160,93 +160,93 @@
         group: PermissionsByte,
         others: PermissionsByte
     ):
         self.owner = owner
         self.group = group
         self.others = others
 
-    def __sub__(self, permission_byte: PermissionsByte) -> 'PermissionsCode':
+    def __sub__(self, permission_byte: PermissionsByte) -> 'PermissionsMode':
         if not isinstance(permission_byte, PermissionsByte):
             raise TypeError(
-                f'can only subtract PermissionsByte (not "{type(permission_byte)}") from PermissionsCode'
+                f'can only subtract PermissionsByte (not "{type(permission_byte)}") from PermissionsMode'
             )
 
-        permissions_code: int = self.permissions_code_as_decimal_repr
-        permissions_code_updated: int = (
-            permissions_code & ~permission_byte.permissions_code_as_decimal_repr
+        permissions_mode: int = self.permissions_mode_as_decimal_repr
+        permissions_mode_updated: int = (
+            permissions_mode & ~permission_byte.permissions_mode_as_decimal_repr
         )
-        class_arguments: Dict[str, PermissionsByte] = PermissionsCode.__transform_permission_code(
-            permissions_code_updated=permissions_code_updated
+        class_arguments: Dict[str, PermissionsByte] = PermissionsMode.__transform_permission_mode(
+            permissions_mode_updated=permissions_mode_updated
         )
 
-        return PermissionsCode(**class_arguments)
+        return PermissionsMode(**class_arguments)
 
-    def __add__(self, permission_byte: PermissionsByte) -> 'PermissionsCode':
+    def __add__(self, permission_byte: PermissionsByte) -> 'PermissionsMode':
         if not isinstance(permission_byte, PermissionsByte):
             raise TypeError(
-                f'can only add PermissionsByte (not "{type(permission_byte)}") to PermissionsCode'
+                f'can only add PermissionsByte (not "{type(permission_byte)}") to PermissionsMode'
             )
 
-        permissions_code: int = self.permissions_code_as_decimal_repr
-        permissions_code_updated: int = (
-            permissions_code | permission_byte.permissions_code_as_decimal_repr
+        permissions_mode: int = self.permissions_mode_as_decimal_repr
+        permissions_mode_updated: int = (
+            permissions_mode | permission_byte.permissions_mode_as_decimal_repr
         )
-        class_arguments: Dict[str, PermissionsByte] = PermissionsCode.__transform_permission_code(
-            permissions_code_updated=permissions_code_updated
+        class_arguments: Dict[str, PermissionsByte] = PermissionsMode.__transform_permission_mode(
+            permissions_mode_updated=permissions_mode_updated
         )
 
-        return PermissionsCode(**class_arguments)
+        return PermissionsMode(**class_arguments)
 
     def __str__(self) -> str:
         return repr(self)
 
     def __repr__(self) -> str:
         return (
-            f'<{self.__class__.__name__} permissions_code={self.permissions_code}>'
+            f'<{self.__class__.__name__} permissions_mode={self.permissions_mode}>'
         )
 
     @staticmethod
-    def __transform_permission_code(permissions_code_updated: int) -> Dict[str, PermissionsByte]:
+    def __transform_permission_mode(permissions_mode_updated: int) -> Dict[str, PermissionsByte]:
         """
         Private static method to take the decimal representation of a transformed permissions
-        code from __add__ or __sub__, convert to the Unix permissions code, and generate
-        updated class arguments for a new PermissionsCode instance.
+        mode from __add__ or __sub__, convert to the Unix permissions mode, and generate
+        updated class arguments for a new PermissionsMode instance.
         """
-        permission_code: str = from_octal_to_permissions_code(octal=permissions_code_updated)
-        class_arguments: Dict[str, PermissionsByte] = PermissionsCode.__generate_class_arguments_from_code(
-            permission_code=permission_code
+        permission_mode: str = from_octal_to_permissions_mode(octal=permissions_mode_updated)
+        class_arguments: Dict[str, PermissionsByte] = PermissionsMode.__generate_class_arguments_from_mode(
+            permission_mode=permission_mode
         )
         return class_arguments
 
     @staticmethod
-    def __generate_class_arguments_from_code(permission_code: str) -> Dict[str, PermissionsByte]:
+    def __generate_class_arguments_from_mode(permission_mode: str) -> Dict[str, PermissionsByte]:
         """
-        Private static method to generate class arguments for a PermissionsCode instance based on
-        a Unix permission code.
+        Private static method to generate class arguments for a PermissionsMode instance based on
+        a Unix permission mode.
         """
-        owner_config = PermissionsConfig.from_octal_digit(octal_digit=permission_code[0])
-        group_config = PermissionsConfig.from_octal_digit(octal_digit=permission_code[1])
-        others_config = PermissionsConfig.from_octal_digit(octal_digit=permission_code[2])
+        owner_config = PermissionsConfig.from_octal_digit(octal_digit=permission_mode[0])
+        group_config = PermissionsConfig.from_octal_digit(octal_digit=permission_mode[1])
+        others_config = PermissionsConfig.from_octal_digit(octal_digit=permission_mode[2])
 
         class_arguments = {
             'owner': PermissionsByte(authority='owner', config=owner_config),
             'group': PermissionsByte(authority='group', config=group_config),
             'others': PermissionsByte(authority='others',config=others_config)
         }
 
         return class_arguments
 
     @classmethod
     def _from_permissions_bytes(
         cls,
         permissions_byte_one: PermissionsByte,
         permissions_byte_two: PermissionsByte
-    ) -> 'PermissionsCode':
+    ) -> 'PermissionsMode':
         """
-        Private class method to generate a PermissionsCode instance from two PermissionByte
+        Private class method to generate a PermissionsMode instance from two PermissionByte
         instances.
         """
         class_arguments = dict()
         class_parameters = get_all_class_parameters(class_object=cls)
         if permissions_byte_one.authority == permissions_byte_two.authority:
             raise ValueError("'authority' cannot be the same for both PermissionsByte objects")
 
@@ -258,55 +258,55 @@
             class_arguments.update(
                 {parameter: PermissionsByte(authority=parameter, config=PermissionsConfig())}
             )
 
         return cls(**class_arguments)
 
     @classmethod
-    def from_octal_representation(cls, octal: Union[str, int]) -> 'PermissionsCode':
+    def from_octal_representation(cls, octal: Union[str, int]) -> 'PermissionsMode':
         """
-        Creates a PermissionsCode instance from an octal representation.
+        Creates a PermissionsMode instance from an octal representation.
 
         This function accepts either a string or an integer as input. If the argument is
         a string, the value must be either in the format of an octal literal (e.g., '0o777')
-        or as a Unix permissions code (e.g., '777'). If the value is an integer, it must be a
+        or as a Unix permissions mode (e.g., '777'). If the value is an integer, it must be a
         decimal representation of an octal as an octal literal (e.g., 0o777) or directly as an
         integer (e.g., 511).
 
         Args:
             octal (str | int): An octal representation as a string or integer.
 
         Returns:
-            PermissionsCode: A new instance of PermissionsCode corresponding to the
+            PermissionsMode: A new instance of PermissionsMode corresponding to the
                 provided octal value.
         """
-        permission_code: str = from_octal_to_permissions_code(octal=octal)
-        class_arguments: Dict[str, PermissionsByte] = PermissionsCode.__generate_class_arguments_from_code(
-            permission_code=permission_code
+        permission_mode: str = from_octal_to_permissions_mode(octal=octal)
+        class_arguments: Dict[str, PermissionsByte] = PermissionsMode.__generate_class_arguments_from_mode(
+            permission_mode=permission_mode
         )
 
         return cls(**class_arguments)
 
     @property
-    def permissions_code(self) -> str:
-        """The Unix permissions code."""
-        permissions_code = (
-            self.owner.permissions_code_as_decimal_repr |
-            self.group.permissions_code_as_decimal_repr |
-            self.others.permissions_code_as_decimal_repr
+    def permissions_mode(self) -> str:
+        """The Unix permissions mode."""
+        permissions_mode = (
+            self.owner.permissions_mode_as_decimal_repr |
+            self.group.permissions_mode_as_decimal_repr |
+            self.others.permissions_mode_as_decimal_repr
         )
-        return format(permissions_code, 'o').zfill(3)
+        return format(permissions_mode, 'o').zfill(3)
 
     @property
-    def permissions_code_as_decimal_repr(self) -> int:
-        """The decimal representation of the Unix permissions code"""
-        return int(self.permissions_code, 8)
+    def permissions_mode_as_decimal_repr(self) -> int:
+        """The decimal representation of the Unix permissions mode"""
+        return int(self.permissions_mode, 8)
 
     @property
-    def permissions_code_as_int(self) -> int:
-        """The integer representation of the Unix permissions code"""
-        return int(self.permissions_code)
+    def permissions_mode_as_int(self) -> int:
+        """The integer representation of the Unix permissions mode"""
+        return int(self.permissions_mode)
 
     @property
-    def permissions_code_as_octal_literal(self) -> str:
-        """The string octal literal representation of the Unix permissions code."""
-        return f'0o{self.permissions_code}'
+    def permissions_mode_as_octal_literal(self) -> str:
+        """The string octal literal representation of the Unix permissions mode."""
+        return f'0o{self.permissions_mode}'
```

### Comparing `unix_perms-0.1.0/PKG-INFO` & `unix_perms-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: unix-perms
-Version: 0.1.0
-Summary: Manage and interpret Linux file permissions with a Python package that provides intuitive tools for creating, validating, and describing permission codes.
+Version: 0.2.0
+Summary: Manage and interpret Unix file permissions with a Python package that provides intuitive tools for creating, validating, and describing permission modes.
 License: MIT
 Keywords: unix,permissions,files
 Author: galactixx
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # unix_perms
-Manage and interpret Unix file permissions with a Python package that provides intuitive tools for creating, validating, and describing permission codes.
+Manage and interpret Unix file permissions with a Python package that provides intuitive tools for creating, validating, and describing permission modes.
```

