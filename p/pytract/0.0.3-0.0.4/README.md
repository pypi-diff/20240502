# Comparing `tmp/pytract-0.0.3.tar.gz` & `tmp/pytract-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytract-0.0.3.tar", last modified: Wed Apr 24 08:27:38 2024, max compression
+gzip compressed data, was "pytract-0.0.4.tar", last modified: Thu May  2 11:09:31 2024, max compression
```

## Comparing `pytract-0.0.3.tar` & `pytract-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.230000 pytract-0.0.3/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5315 2024-04-24 08:27:38.230000 pytract-0.0.3/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3991 2024-04-22 07:54:42.000000 pytract-0.0.3/README.md
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.220000 pytract-0.0.3/pytract/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      115 2024-04-11 17:26:05.000000 pytract-0.0.3/pytract/__init__.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      801 2024-04-11 19:26:57.000000 pytract-0.0.3/pytract/__main__.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)    12280 2024-04-24 07:07:40.000000 pytract-0.0.3/pytract/abi2api.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       83 2024-04-11 05:38:49.000000 pytract-0.0.3/pytract/constants.py
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.230000 pytract-0.0.3/pytract/templates/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3345 2024-04-24 06:55:37.000000 pytract-0.0.3/pytract/templates/api.py.j2
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      234 2024-04-11 14:59:51.000000 pytract-0.0.3/pytract/utils.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)    12865 2024-04-24 07:21:41.000000 pytract-0.0.3/pytract/vm.py
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.230000 pytract-0.0.3/pytract.egg-info/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5315 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      345 2024-04-24 08:27:38.000000 pytract-0.0.3/pytract.egg-info/SOURCES.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/dependency_links.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       51 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/entry_points.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       53 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/requires.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        8 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/top_level.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-24 08:27:38.230000 pytract-0.0.3/setup.cfg
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      765 2024-04-24 08:25:26.000000 pytract-0.0.3/setup.py
+drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-05-02 11:09:31.810000 pytract-0.0.4/
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     1058 2024-04-12 09:24:01.000000 pytract-0.0.4/LICENSE
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     4400 2024-05-02 11:09:31.810000 pytract-0.0.4/PKG-INFO
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     4145 2024-04-24 08:35:08.000000 pytract-0.0.4/README.md
+drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-05-02 11:09:31.810000 pytract-0.0.4/pytract/
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      148 2024-04-28 02:56:08.000000 pytract-0.0.4/pytract/__init__.py
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      801 2024-04-11 19:26:57.000000 pytract-0.0.4/pytract/__main__.py
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)    12945 2024-04-26 06:26:01.000000 pytract-0.0.4/pytract/abi2api.py
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       83 2024-04-11 05:38:49.000000 pytract-0.0.4/pytract/constants.py
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     3310 2024-04-29 09:31:50.000000 pytract-0.0.4/pytract/evm.py
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     1382 2024-04-29 08:14:27.000000 pytract-0.0.4/pytract/locksmith.py
+drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-05-02 11:09:31.810000 pytract-0.0.4/pytract/templates/
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     3345 2024-04-24 06:55:37.000000 pytract-0.0.4/pytract/templates/api.py.j2
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     3395 2024-04-29 08:16:37.000000 pytract-0.0.4/pytract/utils.py
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)    15499 2024-04-29 08:16:12.000000 pytract-0.0.4/pytract/vm.py
+drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-05-02 11:09:31.810000 pytract-0.0.4/pytract.egg-info/
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     4400 2024-05-02 11:09:31.000000 pytract-0.0.4/pytract.egg-info/PKG-INFO
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      389 2024-05-02 11:09:31.000000 pytract-0.0.4/pytract.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        1 2024-05-02 11:09:31.000000 pytract-0.0.4/pytract.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       50 2024-05-02 11:09:31.000000 pytract-0.0.4/pytract.egg-info/entry_points.txt
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      184 2024-05-02 11:09:31.000000 pytract-0.0.4/pytract.egg-info/requires.txt
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        8 2024-05-02 11:09:31.000000 pytract-0.0.4/pytract.egg-info/top_level.txt
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       38 2024-05-02 11:09:31.810000 pytract-0.0.4/setup.cfg
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)     1295 2024-05-02 11:09:17.000000 pytract-0.0.4/setup.py
```

### Comparing `pytract-0.0.3/PKG-INFO` & `pytract-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,145 +1,148 @@
 Metadata-Version: 2.1
 Name: pytract
-Version: 0.0.3
+Version: 0.0.4
 Summary: Smart contract Python API generator.
 Home-page: https://github.com/james4ever0/pytract
-License: UNKNOWN
-Description: # pytract
-        
-        [![PyPI download month](https://img.shields.io/pypi/dm/pytract.svg)](https://pypi.python.org/pypi/pytract/)
-        
-        Smart contract Python API generator.
-        
-        It works by interpreting smart contract ABI and generate corresponding Python API code.
-        
-        ## Usage
-        
-        Install from PyPI:
-        
-        ```bash
-        pip install pytract
-        ```
-        
-        Create Python API code for your `brownie` project:
-        
-        ```bash
-        usage: pytract process [-h] project_path
-        
-        positional arguments:
-          project_path  Path of the project to process
-        
-        optional arguments:
-          -h, --help    show this help message and exit
-        ```
-        
-        And you shall import all available contracts and programmatically.
-        
-        If your project folder name is `brownie_project` then write:
-        
-        ```python
-        from brownie_project.api import project_info, contracts
-        
-        print(dir(contracts)) # list available contract classes
-        print(dir(project_info)) # list project info attributes
-        ```
-        
-        Note the difference of using it with `brownie` alone, you now have a fully portable python package, which you can write static typed code without the need for copying and pasting from `brownie console`.
-        
-        You can view all generated API code under folder `<your brownie project>/api`.
-        
-        Example generated contract API class is given below:
-        
-        ```python
-        class Faucet(abi2api.ContractInstance):
-            _project = project_info.project
-            _contract_info = project_info.contracts_info["Faucet"]
-            _contract_name = "Faucet"
-        
-            class Function(abi2api.FunctionBase):
-                def returnVars(
-                    self,
-                ):
-                    """
-                    Function Type: pure
-        
-                    Inputs:
-                        (No parameters)
-        
-                    Outputs:
-                        (uint256, uint256, uint256)
-                    """
-                    values = self._contract.returnVars()
-                    return values
-        
-                def withdraw(
-                    self,
-                    withdraw_amount,
-                    _txparams: Optional[abi2api.TransactionParameters] = None,
-                ):
-                    """
-                    Function Type: nonpayable
-        
-                    Inputs:
-                        withdraw_amount: uint256
-        
-                    Outputs:
-                        (No parameters)
-                    """
-                    values = self._contract.withdraw(
-                        withdraw_amount, self.txparams_with_fallback(_txparams).dict()
-                    )
-                    return values
-        
-            def __init__(
-                self,
-                contract: Union[Contract, ProjectContract],
-                issuer: Optional[Account] = None,
-                _txparams: Optional[abi2api.TransactionParameters] = None,
-            ):  # to create you need to either deploy or load contract by address
-                super().__init__(contract, issuer)
-                self.function = self.Function(contract, _txparams)
-                """
-                Available functions of this smart contract.
-                """
-        
-            @classmethod
-            def deploy(cls, _txparams: abi2api.TransactionParameters):
-                """
-                Inputs:
-                    transaction_parameters: TransactionParameters
-        
-                Output:
-                    contract: Faucet
-                """
-                args = []
-        
-                parameters = _txparams.to_contract_deploy_parameters(args)
-        
-                deployed_contract: ProjectContract = cls._contract_info.contract_container.deploy(*parameters.to_args())  # type: ignore
-        
-                return cls(deployed_contract, _txparams.issuer, _txparams)
-        
-        ```
-        
-        ## Roadmap
-        
-        - [x] Create a binding to smart contract and APIs for Brownie
-        - [ ] Create a simple pure Python transaction and smart contract platform without blockchain
-        
-        ## Related projects
-        
-        - [simular](https://pypi.org/project/simular-evm/)
-        - [pyrevm](https://pypi.org/project/pyrevm/)
-        - [pyevm](https://github.com/ethereum/py-evm)
-        - [viem](https://viem.sh)
-        - [hardhat](https://hardhat.org/)
-        - [titanoboa](https://titanoboa.readthedocs.io/en/latest/index.html)
-        - [TypeChain](https://github.com/dethcrypto/TypeChain)
-        - [eth-sdk](https://github.com/dethcrypto/eth-sdk)
-        - [ethereum-abi-types-generator](https://github.com/joshstevens19/ethereum-abi-types-generator)
-        
-        ## Stargazers
-        
-        [![Stargazers over time](https://starchart.cc/James4Ever0/pytract.svg)](https://starchart.cc/James4Ever0/pytract)
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: simular
+Provides-Extra: all
+License-File: LICENSE
+
+# pytract
+
+[![PyPI download month](https://img.shields.io/pypi/dm/pytract.svg)](https://pypi.python.org/pypi/pytract/)
+
+Smart contract Python API generator.
+
+It works by interpreting smart contract ABI and generate corresponding Python API code.
+
+## Usage
+
+Install from PyPI:
+
+```bash
+pip install pytract
+```
+
+Create Python API code for your `brownie` project:
+
+```bash
+usage: pytract process [-h] project_path
+
+positional arguments:
+  project_path  Path of the project to process
+
+optional arguments:
+  -h, --help    show this help message and exit
+```
+
+And you shall import all available contracts and programmatically.
+
+If your project folder name is `brownie_project` then write:
+
+```python
+from brownie_project.api import project_info, contracts
+
+print(dir(contracts)) # list available contract classes
+print(dir(project_info)) # list project info attributes
+```
+
+Note the difference of using it with `brownie` alone, you now have a fully portable python package, which you can write static typed code without the need for copying and pasting from `brownie console`.
+
+You can view all generated API code under folder `<your brownie project>/api`.
+
+Example generated contract API class is given below:
+
+```python
+class Faucet(abi2api.ContractInstance):
+    _project = project_info.project
+    _contract_info = project_info.contracts_info["Faucet"]
+    _contract_name = "Faucet"
+
+    class Function(abi2api.FunctionBase):
+        def returnVars(
+            self,
+        ):
+            """
+            Function Type: pure
+
+            Inputs:
+                (No parameters)
+
+            Outputs:
+                (uint256, uint256, uint256)
+            """
+            values = self._contract.returnVars()
+            return values
+
+        def withdraw(
+            self,
+            withdraw_amount,
+            _txparams: Optional[abi2api.TransactionParameters] = None,
+        ):
+            """
+            Function Type: nonpayable
+
+            Inputs:
+                withdraw_amount: uint256
+
+            Outputs:
+                (No parameters)
+            """
+            values = self._contract.withdraw(
+                withdraw_amount, self.txparams_with_fallback(_txparams).dict()
+            )
+            return values
+
+    def __init__(
+        self,
+        contract: Union[Contract, ProjectContract],
+        issuer: Optional[Account] = None,
+        _txparams: Optional[abi2api.TransactionParameters] = None,
+    ):  # to create you need to either deploy or load contract by address
+        super().__init__(contract, issuer)
+        self.function = self.Function(contract, _txparams)
+        """
+        Available functions of this smart contract.
+        """
+
+    @classmethod
+    def deploy(cls, _txparams: abi2api.TransactionParameters):
+        """
+        Inputs:
+            transaction_parameters: TransactionParameters
+
+        Output:
+            contract: Faucet
+        """
+        args = []
+
+        parameters = _txparams.to_contract_deploy_parameters(args)
+
+        deployed_contract: ProjectContract = cls._contract_info.contract_container.deploy(*parameters.to_args())  # type: ignore
+
+        return cls(deployed_contract, _txparams.issuer, _txparams)
+
+```
+
+## Roadmap
+
+- [x] Create a binding to smart contract and APIs for Brownie
+- [ ] Create a simple pure Python transaction and smart contract platform without blockchain
+- [ ] Create a [TypeChain](https://npmjs.com/package/typechain)-like commandline tool for generating standalone package from a list of contract ABI files
+
+## Related projects
+
+- [simular](https://pypi.org/project/simular-evm/)
+- [pyrevm](https://pypi.org/project/pyrevm/)
+- [pyevm](https://github.com/ethereum/py-evm)
+- [viem](https://viem.sh)
+- [hardhat](https://hardhat.org/)
+- [titanoboa](https://titanoboa.readthedocs.io/en/latest/index.html)
+- [TypeChain](https://github.com/dethcrypto/TypeChain)
+- [eth-sdk](https://github.com/dethcrypto/eth-sdk)
+- [ethereum-abi-types-generator](https://github.com/joshstevens19/ethereum-abi-types-generator)
+
+## Stargazers
+
+[![Stargazers over time](https://starchart.cc/James4Ever0/pytract.svg)](https://starchart.cc/James4Ever0/pytract)
```

### Comparing `pytract-0.0.3/README.md` & `pytract-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 
 ```
 
 ## Roadmap
 
 - [x] Create a binding to smart contract and APIs for Brownie
 - [ ] Create a simple pure Python transaction and smart contract platform without blockchain
+- [ ] Create a [TypeChain](https://npmjs.com/package/typechain)-like commandline tool for generating standalone package from a list of contract ABI files
 
 ## Related projects
 
 - [simular](https://pypi.org/project/simular-evm/)
 - [pyrevm](https://pypi.org/project/pyrevm/)
 - [pyevm](https://github.com/ethereum/py-evm)
 - [viem](https://viem.sh)
```

### Comparing `pytract-0.0.3/pytract/__main__.py` & `pytract-0.0.4/pytract/__main__.py`

 * *Files identical despite different names*

### Comparing `pytract-0.0.3/pytract/abi2api.py` & `pytract-0.0.4/pytract/abi2api.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     def from_contract(cls, contract: Union[ProjectContract, Contract], issuer: Account):
         return cls(contract=contract, issuer=issuer)
 
 
 # TODO: recursively resolve and create tuple type hints for languages like vyper
 class ParamType(pydantic.BaseModel):
     type: str
-    name: str = "" # mostly ignored
+    name: str = ""  # mostly ignored
     components: list["ParamType"] = []
 
     # internalType: str
     @property
     def type_hint(self):
         return self.resolve_type_hint(self)
 
@@ -369,7 +369,33 @@
         content = """from pytract import abi2api
 project_info = abi2api.load_project_info_for_api()"""
         f.write(content)
 
     with open(os.path.join(project_path, "__init__.py"), "w+") as f:
         content = """from . import api"""
         f.write(content)
+
+
+# TODO: handle multi-dimentional type specification
+
+# class TypeAnnotation(pydantic.BaseModel):
+#     name: str
+#     length: int
+
+
+# def parse_single_type_annotation(type_annotation: str):
+#     length = 0
+#     if type_annotation.endswith("]"):
+#         type_name, length_text = type_annotation.split("[")
+#         length_text = length_text.strip("]")
+#         length = int(length_text)
+#     else:
+#         type_name = type_annotation
+#     ret = TypeAnnotation(name=type_name, length=length)
+#     return ret
+
+TYPE_PREFIX_TRANSLATION_TABLE_INVERTED = {
+    "tuple": ["tuple"],
+    "int": ["uint", "int"],
+    "bytes": ["bytes"],
+    "str": ['string']
+}
```

### Comparing `pytract-0.0.3/pytract/templates/api.py.j2` & `pytract-0.0.4/pytract/templates/api.py.j2`

 * *Files identical despite different names*

### Comparing `pytract-0.0.3/pytract/vm.py` & `pytract-0.0.4/pytract/vm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,51 @@
 # smart contract web3 virtual machine
+from .utils import AtomicTinyDB, generate_address_and_key, check_key_validity
 import tinydb
 
 # import abc
 import pydantic
-import web3
 import beartype
-from typing_extensions import Self, Optional, Literal
+import filelock
+
+try:
+    from typing_extensions import Self
+except:
+    from typing import Self  # type: ignore
+try:
+    from typing_extensions import Optional
+except:
+    from typing import Optional
+try:
+    from typing_extensions import Literal
+except:
+    from typing import Literal
+
 from typing import Union
 from contextlib import contextmanager
 import os
 import pathlib
-import filelock
-import functools
 import json
 import hashlib
+import typing_extensions
+
 # import dill
 import typing
 
-
-# TODO: use tinydb context with filelock to ensure data consistency
-@contextmanager
-def tinydb_context(db_path: str):
-    prefix, suffix = os.path.split(db_path)
-    db_lockpath = os.path.join(prefix, f".{suffix}.lock")
-    with filelock.FileLock(db_lockpath):
-        with tinydb.TinyDB(db_path) as db:
-            yield db
-
-
-@beartype.beartype
-class AtomicTinyDB:
-    def __init__(self, db_path: str):
-        self._db_context_builder = functools.partial(tinydb_context, db_path)
-
-    def update(self, *args, **kwargs):
-        with self._db_context_builder() as db:
-            return db.update(*args, **kwargs)
-
-    def search(self, *args, **kwargs):
-        with self._db_context_builder() as db:
-            return db.search(*args, **kwargs)
-
-    def get(self, *args, **kwargs):
-        with self._db_context_builder() as db:
-            return db.get(*args, **kwargs)
-
-    def insert(self, *args, **kwargs):
-        with self._db_context_builder() as db:
-            return db.insert(*args, **kwargs)
+Number = Union[int, float]
+P = typing_extensions.ParamSpec("P")
+R = typing.TypeVar("R")
 
 
 def generate_account_static_info():
-    account = web3.Account.create()
-    ret = AccountStaticInfo(address=account.address, key=account.key.hex())
-    return ret
-
-
-def check_key_validity(address: str, key: str):
-    ret = False
-    try:
-        account = web3.Account.from_key(key)
-        assert account.address == address, f"Key '{key}' is not for address '{address}'"
-        ret = True
-    except:
-        pass
+    address, key = generate_address_and_key()
+    ret = AccountStaticInfo(address=address, key=key)
     return ret
 
 
-def check_if_serializable(data) -> bool:
-    serializable = False
-    try:
-        json.dumps(data, ensure_ascii=False)
-        serializable = True
-    except:
-        print("data not serializable")
-    return serializable
-
-
 _default_vm: Optional["VM"] = None
 
 
 class EngageException(Exception): ...
 
 
 class AccountBase(pydantic.BaseModel):
@@ -98,15 +63,15 @@
             assert check_key_validity(
                 address, key
             ), f"Key '{key} is not valid for {address}"
         return v
 
 
 class AccountVolatileInfo(pydantic.BaseModel):
-    balance: float
+    balance: Number
 
     @pydantic.validator("balance")
     def validate_balance(cls, v):
         assert v >= 0, "Balance must be non-negative"
         return v
 
 
@@ -138,26 +103,26 @@
         self._contract_data_dir = pathlib.Path(contract_data_dir)
         self._contract_data_db_dir = self._contract_data_dir / "db"
         self._contract_data_lock_dir = self._contract_data_dir / ".lock"
         ensure_dir(self._contract_data_dir)
         ensure_dir(self._contract_data_db_dir)
         ensure_dir(self._contract_data_lock_dir)
 
-    def transfer(self, sender: "Account", receiver: "Account", amount: float):
+    def transfer(self, sender: "Account", receiver: "Account", amount: Number):
         assert amount > 0, "Transfer amount must be positive"
         sender_balance = sender.balance
         sender_new_balance = sender_balance - amount
         if sender_new_balance > 0:
             # able to transact
             receiver_new_balance = receiver.balance + amount
             # this is atomic operation.
             self.set_balance(sender, sender_new_balance)
             self.set_balance(receiver, receiver_new_balance)
 
-    def set_balance(self, account: "Account", balance: float):
+    def set_balance(self, account: "Account", balance: Number):
         assert balance >= 0, "Balance must be non-negative"
         doc_id = self.query_for_single_account_document_id(account)
         updated_ids = self._db.update(
             AccountVolatileInfo(balance=balance).dict(), doc_ids=[doc_id]
         )
         assert len(updated_ids) == 1, "Failed to set balance because of having "
 
@@ -204,15 +169,15 @@
 
         with filelock.FileLock(contract_lock_filepath):
             data = contract.serialize()
             # you may need filelock.
             with open(contract_db_filepath, "w+") as f:
                 f.write(data)
 
-    def create_account(self, init_balance: float = 0):
+    def create_account(self, init_balance: Number = 0):
         assert init_balance >= 0, "Initial balance must be non-negative"
         account_static_info = generate_account_static_info()
         # private key
         self._db.insert(
             AccountInfo(**account_static_info.dict(), balance=init_balance).dict()
         )
 
@@ -250,14 +215,33 @@
 
 
 # vm.create_contract(Contract1)(*contract1_init_arguments)
 # vm.create_contract()
 # account = vm.create_account()
 
 
+def payable(
+    func: typing.Callable[typing_extensions.Concatenate["typing.Any", P], R]
+) -> typing.Callable[
+    typing_extensions.Concatenate["typing.Any", "Account", Number, P], R
+]:
+    def payable_func(
+        self: "SmartContract",
+        caller: Account,
+        amount: Number,
+        *args: P.args,
+        **kwargs: P.kwargs,
+    ) -> R:
+        with self.engage(caller):
+            with self.receive(amount):
+                return func(self, *args, **kwargs)
+
+    return payable_func
+
+
 @beartype.beartype
 class Account:
     def __init__(
         self, address: str, key: Optional[str] = None, vm: Optional[VM] = None
     ):
         self._vm = get_vm_with_fallback(vm)
         self._address = address
@@ -271,15 +255,15 @@
         if self._key is not None:
             raise Exception("Account already unlocked")
         if check_key_validity(self._address, key):
             self._key = key
         else:
             raise Exception("Key invalid. Cannot unlock account.")
 
-    def pay(self, amount: int, recepient: Optional[Self] = None):
+    def pay(self, amount: Number, recepient: Optional[Self] = None):
         if self._key is None:
             raise Exception("Account is not unlocked.")
         if recepient is None:
             if self._default_receipent is None:
                 raise EngageException("Account not engaged")
             else:
                 recepient = self._default_receipent
@@ -302,32 +286,62 @@
     def engage(self, recepient: Self):
         try:
             self._engage(recepient)
             yield self
         finally:
             self._disengage()
 
+
 class PersistantDataDict(dict):
     def __init__(self, contract: "SmartContract", data: dict = {}):
         self.contract = contract
+        self.ISSUER = "_issuer"
+        self.ACCOUNT = "_account"
+        self.ACCOUNT_KEY = "_account_key"
+        self.read_only_keys = [self.ISSUER, self.ACCOUNT, self.ACCOUNT_KEY]
         super().__init__(**data)
+
+    def init_issuer(self, issuer: Account):
+        with self.persist_context() as data_context:
+            data_context[data_context.ISSUER] = issuer._address
+
+    def init_account(self, account: Account):
+        with self.persist_context() as data_context:
+            data_context[data_context.ACCOUNT] = account._address
+            data_context[data_context.ACCOUNT_KEY] = account._key
+
+    def init_issuer_and_account(self, issuer: Account, account: Account):
+        self.init_issuer(issuer)
+        self.init_account(account)
+
     @contextmanager
     def persist_context(self):
         try:
             yield self
         finally:
             self.persist()
-    def __setitem__(self, key, value): # TODO: to handle nested statement like a[0][0] = 0, we need to use a contextmanager approach instead of this.
+
+    def check_key_if_is_readonly(self, key):
+        for it in self.read_only_keys:
+            if key == it:
+                if key in self.keys():
+                    # this is readonly. refuse to set it again.
+                    raise Exception(f"Cannot reset read-only key '{it}'")
+
+    def __setitem__(
+        self, key, value
+    ):  # TODO: to handle nested statement like a[0][0] = 0, we need to use a contextmanager approach instead of this.
+        self.check_key_if_is_readonly(key)
         super().__setitem__(key, value)
         self.persist()
-    
+
     def __delitem__(self, key):
         super().__delitem__(key)
         self.persist()
-    
+
     def persist(self):
         self.contract.store()
 
     # def __setattr__(self, name, value):
     #     self.contract.store()
     #     super().__setattr__(name, value)
 
@@ -335,49 +349,93 @@
     #     self.contract.store()
     #     super().__getattribute__(name)
 
     # def __delattr__(self, name):
     #     self.contract.store()
     #     super().__delattr__(name)
 
+
 # ref:
 # https://docs.python.org/3/library/shelve.html
 # https://docs.python.org/3/library/dbm.html
 # https://github.com/dagnelies/pysos
 # https://github.com/balena/python-pqueue (persistent queue)
 # https://github.com/croqaz/Stones (with credits)
 class SmartContract:  # anything done to a smart contract shall be stored.
     def __init__(
-        self, address, issuer: Optional[Account] = None, vm: Optional[VM] = None
+        self,
+        account: Account,
+        vm: VM,
+        issuer: Optional[Account] = None,
     ):
         # if contract found at address, just load it from dill.
-        self._address = address
+        # self._address = address
+        self._account = account
         self._issuer = issuer
-        self._vm = get_vm_with_fallback(vm)
-        data = self._vm.load_contract_data(self)
-        self._data = PersistantDataDict(self, data if data is not None else {})
+        self._vm = vm
+        self._address = account._address
+        self._transfer_amount = 0
+        self._serialized_data_history_hash = ""
+
+        self.load_data_and_register_issuer()
+
+        if self._issuer is None:
+            self._issuer = Account(self.data[self.data.ISSUER], vm=self._vm)
+
+        if self._account._key is None:
+            self._account.unlock(self.data[self.data.ACCOUNT_KEY])
 
         # if contract not found at address, then create new one.
-        self._serialized_data_history_hash = self._data_hash
         # self._account = Account(vm, issuer)
-        self._default_account = None
+        self._caller_account = None
         self.store()
 
+    @classmethod
+    def load(
+        cls, address: str, issuer: Optional[Account] = None, vm: Optional[VM] = None
+    ):
+        vm = get_vm_with_fallback(vm)
+        account = Account(address, vm=vm)
+        ret = cls(account=account, issuer=issuer, vm=vm)
+        return ret
+
+    @classmethod
+    def create(cls, issuer: Account, vm: Optional[VM] = None):
+        vm = get_vm_with_fallback(vm)
+        account = vm.create_account()
+        return cls(account=account, issuer=issuer, vm=vm)
+
+    def load_data_and_register_issuer(self):
+        data = self._vm.load_contract_data(self)
+        if data is not None:
+            self._data = PersistantDataDict(self, data)
+        else:
+            self._data = PersistantDataDict(self, {})
+            if self._issuer is not None:
+                self.data.init_issuer(self._issuer)
+            else:
+                raise Exception("Cannot create new contract without specifying issuer")
+
+            if self._account is not None:
+                self.data.init_account(self._account)
+            else:
+                raise Exception("Cannot create new contract without specifying account")
+
     @property
     def data(self):
         return self._data
 
     def _engage(self, account: Account):
-        if self._default_account is not None:
+        if self._caller_account is not None:
             raise EngageException("Contract already engaged")
         else:
-            self._default_account = account
+            self._caller_account = account
 
     def _disengage(self):
-        self._default_account = None
+        self._caller_account = None
         self.persist_contract_data()
 
     @contextmanager
     def engage(self, account: Account):
         try:
             self._engage(account)
             yield self
@@ -394,12 +452,37 @@
 
     @property
     def _data_hash(self):
         serialized_data = self.serialize()
         serialized_data_hash = hashlib.sha256(serialized_data.encode()).hexdigest()
         return serialized_data_hash
 
+    def pay_from_caller(self, amount: Number, caller: Optional[Account] = None):
+        caller = self.resolve_caller(caller)
+        caller.pay(amount, recepient=self._account)
+        self._transfer_amount += amount
+
+    def resolve_caller(self, caller: Optional[Account] = None):
+        if caller is None:
+            if self._caller_account is not None:
+                caller = self._caller_account
+            else:
+                raise Exception("Unable to resolve caller account")
+        return caller
+
+    @property
+    def balance(self):
+        return self._account.balance
+
+    @contextmanager
+    def receive(self, amount: Number, account: Optional[Account] = None):
+        try:
+            self.pay_from_caller(amount, account)
+            yield self
+        finally:
+            self._transfer_amount = 0
+
     def store(self):
         serialized_data_hash = self._data_hash
         if serialized_data_hash != self._serialized_data_history_hash:
             self.persist_contract_data()
             self._serialized_data_history_hash = serialized_data_hash
```

### Comparing `pytract-0.0.3/pytract.egg-info/PKG-INFO` & `pytract-0.0.4/pytract.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,145 +1,148 @@
 Metadata-Version: 2.1
 Name: pytract
-Version: 0.0.3
+Version: 0.0.4
 Summary: Smart contract Python API generator.
 Home-page: https://github.com/james4ever0/pytract
-License: UNKNOWN
-Description: # pytract
-        
-        [![PyPI download month](https://img.shields.io/pypi/dm/pytract.svg)](https://pypi.python.org/pypi/pytract/)
-        
-        Smart contract Python API generator.
-        
-        It works by interpreting smart contract ABI and generate corresponding Python API code.
-        
-        ## Usage
-        
-        Install from PyPI:
-        
-        ```bash
-        pip install pytract
-        ```
-        
-        Create Python API code for your `brownie` project:
-        
-        ```bash
-        usage: pytract process [-h] project_path
-        
-        positional arguments:
-          project_path  Path of the project to process
-        
-        optional arguments:
-          -h, --help    show this help message and exit
-        ```
-        
-        And you shall import all available contracts and programmatically.
-        
-        If your project folder name is `brownie_project` then write:
-        
-        ```python
-        from brownie_project.api import project_info, contracts
-        
-        print(dir(contracts)) # list available contract classes
-        print(dir(project_info)) # list project info attributes
-        ```
-        
-        Note the difference of using it with `brownie` alone, you now have a fully portable python package, which you can write static typed code without the need for copying and pasting from `brownie console`.
-        
-        You can view all generated API code under folder `<your brownie project>/api`.
-        
-        Example generated contract API class is given below:
-        
-        ```python
-        class Faucet(abi2api.ContractInstance):
-            _project = project_info.project
-            _contract_info = project_info.contracts_info["Faucet"]
-            _contract_name = "Faucet"
-        
-            class Function(abi2api.FunctionBase):
-                def returnVars(
-                    self,
-                ):
-                    """
-                    Function Type: pure
-        
-                    Inputs:
-                        (No parameters)
-        
-                    Outputs:
-                        (uint256, uint256, uint256)
-                    """
-                    values = self._contract.returnVars()
-                    return values
-        
-                def withdraw(
-                    self,
-                    withdraw_amount,
-                    _txparams: Optional[abi2api.TransactionParameters] = None,
-                ):
-                    """
-                    Function Type: nonpayable
-        
-                    Inputs:
-                        withdraw_amount: uint256
-        
-                    Outputs:
-                        (No parameters)
-                    """
-                    values = self._contract.withdraw(
-                        withdraw_amount, self.txparams_with_fallback(_txparams).dict()
-                    )
-                    return values
-        
-            def __init__(
-                self,
-                contract: Union[Contract, ProjectContract],
-                issuer: Optional[Account] = None,
-                _txparams: Optional[abi2api.TransactionParameters] = None,
-            ):  # to create you need to either deploy or load contract by address
-                super().__init__(contract, issuer)
-                self.function = self.Function(contract, _txparams)
-                """
-                Available functions of this smart contract.
-                """
-        
-            @classmethod
-            def deploy(cls, _txparams: abi2api.TransactionParameters):
-                """
-                Inputs:
-                    transaction_parameters: TransactionParameters
-        
-                Output:
-                    contract: Faucet
-                """
-                args = []
-        
-                parameters = _txparams.to_contract_deploy_parameters(args)
-        
-                deployed_contract: ProjectContract = cls._contract_info.contract_container.deploy(*parameters.to_args())  # type: ignore
-        
-                return cls(deployed_contract, _txparams.issuer, _txparams)
-        
-        ```
-        
-        ## Roadmap
-        
-        - [x] Create a binding to smart contract and APIs for Brownie
-        - [ ] Create a simple pure Python transaction and smart contract platform without blockchain
-        
-        ## Related projects
-        
-        - [simular](https://pypi.org/project/simular-evm/)
-        - [pyrevm](https://pypi.org/project/pyrevm/)
-        - [pyevm](https://github.com/ethereum/py-evm)
-        - [viem](https://viem.sh)
-        - [hardhat](https://hardhat.org/)
-        - [titanoboa](https://titanoboa.readthedocs.io/en/latest/index.html)
-        - [TypeChain](https://github.com/dethcrypto/TypeChain)
-        - [eth-sdk](https://github.com/dethcrypto/eth-sdk)
-        - [ethereum-abi-types-generator](https://github.com/joshstevens19/ethereum-abi-types-generator)
-        
-        ## Stargazers
-        
-        [![Stargazers over time](https://starchart.cc/James4Ever0/pytract.svg)](https://starchart.cc/James4Ever0/pytract)
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: simular
+Provides-Extra: all
+License-File: LICENSE
+
+# pytract
+
+[![PyPI download month](https://img.shields.io/pypi/dm/pytract.svg)](https://pypi.python.org/pypi/pytract/)
+
+Smart contract Python API generator.
+
+It works by interpreting smart contract ABI and generate corresponding Python API code.
+
+## Usage
+
+Install from PyPI:
+
+```bash
+pip install pytract
+```
+
+Create Python API code for your `brownie` project:
+
+```bash
+usage: pytract process [-h] project_path
+
+positional arguments:
+  project_path  Path of the project to process
+
+optional arguments:
+  -h, --help    show this help message and exit
+```
+
+And you shall import all available contracts and programmatically.
+
+If your project folder name is `brownie_project` then write:
+
+```python
+from brownie_project.api import project_info, contracts
+
+print(dir(contracts)) # list available contract classes
+print(dir(project_info)) # list project info attributes
+```
+
+Note the difference of using it with `brownie` alone, you now have a fully portable python package, which you can write static typed code without the need for copying and pasting from `brownie console`.
+
+You can view all generated API code under folder `<your brownie project>/api`.
+
+Example generated contract API class is given below:
+
+```python
+class Faucet(abi2api.ContractInstance):
+    _project = project_info.project
+    _contract_info = project_info.contracts_info["Faucet"]
+    _contract_name = "Faucet"
+
+    class Function(abi2api.FunctionBase):
+        def returnVars(
+            self,
+        ):
+            """
+            Function Type: pure
+
+            Inputs:
+                (No parameters)
+
+            Outputs:
+                (uint256, uint256, uint256)
+            """
+            values = self._contract.returnVars()
+            return values
+
+        def withdraw(
+            self,
+            withdraw_amount,
+            _txparams: Optional[abi2api.TransactionParameters] = None,
+        ):
+            """
+            Function Type: nonpayable
+
+            Inputs:
+                withdraw_amount: uint256
+
+            Outputs:
+                (No parameters)
+            """
+            values = self._contract.withdraw(
+                withdraw_amount, self.txparams_with_fallback(_txparams).dict()
+            )
+            return values
+
+    def __init__(
+        self,
+        contract: Union[Contract, ProjectContract],
+        issuer: Optional[Account] = None,
+        _txparams: Optional[abi2api.TransactionParameters] = None,
+    ):  # to create you need to either deploy or load contract by address
+        super().__init__(contract, issuer)
+        self.function = self.Function(contract, _txparams)
+        """
+        Available functions of this smart contract.
+        """
+
+    @classmethod
+    def deploy(cls, _txparams: abi2api.TransactionParameters):
+        """
+        Inputs:
+            transaction_parameters: TransactionParameters
+
+        Output:
+            contract: Faucet
+        """
+        args = []
+
+        parameters = _txparams.to_contract_deploy_parameters(args)
+
+        deployed_contract: ProjectContract = cls._contract_info.contract_container.deploy(*parameters.to_args())  # type: ignore
+
+        return cls(deployed_contract, _txparams.issuer, _txparams)
+
+```
+
+## Roadmap
+
+- [x] Create a binding to smart contract and APIs for Brownie
+- [ ] Create a simple pure Python transaction and smart contract platform without blockchain
+- [ ] Create a [TypeChain](https://npmjs.com/package/typechain)-like commandline tool for generating standalone package from a list of contract ABI files
+
+## Related projects
+
+- [simular](https://pypi.org/project/simular-evm/)
+- [pyrevm](https://pypi.org/project/pyrevm/)
+- [pyevm](https://github.com/ethereum/py-evm)
+- [viem](https://viem.sh)
+- [hardhat](https://hardhat.org/)
+- [titanoboa](https://titanoboa.readthedocs.io/en/latest/index.html)
+- [TypeChain](https://github.com/dethcrypto/TypeChain)
+- [eth-sdk](https://github.com/dethcrypto/eth-sdk)
+- [ethereum-abi-types-generator](https://github.com/joshstevens19/ethereum-abi-types-generator)
+
+## Stargazers
+
+[![Stargazers over time](https://starchart.cc/James4Ever0/pytract.svg)](https://starchart.cc/James4Ever0/pytract)
```

