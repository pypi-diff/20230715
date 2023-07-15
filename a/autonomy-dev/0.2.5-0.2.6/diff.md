# Comparing `tmp/autonomy_dev-0.2.5.tar.gz` & `tmp/autonomy_dev-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.2.5.tar", max compression
+gzip compressed data, was "autonomy_dev-0.2.6.tar", max compression
```

## Comparing `autonomy_dev-0.2.5.tar` & `autonomy_dev-0.2.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      578 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/LICENSE
--rw-r--r--   0        0        0      913 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/__init__.py
--rw-r--r--   0        0        0     2716 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/base.py
--rw-r--r--   0        0        0      242 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/cli.py
--rw-r--r--   0        0        0     2758 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/cli_executor.py
--rw-r--r--   0        0        0     3456 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/augment.py
--rw-r--r--   0        0        0     5505 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/deps.py
--rw-r--r--   0        0        0     1890 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/fmt.py
--rw-r--r--   0        0        0     1372 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/fsm.py
--rw-r--r--   0        0        0     2144 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/lint.py
--rw-r--r--   0        0        0     3538 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/release.py
--rw-r--r--   0        0        0     5195 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/repo.py
--rw-r--r--   0        0        0     3400 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/scaffold.py
--rw-r--r--   0        0        0     1450 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/commands/test.py
--rw-r--r--   0        0        0      515 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/constants.py
--rw-r--r--   0        0        0     1482 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/block_explorer.py
--rw-r--r--   0        0        0     5617 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/contract.py
--rw-r--r--   0        0        0     2914 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/contract_functions.py
--rw-r--r--   0        0        0     2238 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/contract_scafolder.py
--rw-r--r--   0        0        0     6086 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/contract_templates.py
--rw-r--r--   0        0        0     1493 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/function.py
--rw-r--r--   0        0        0      525 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/param_type.py
--rw-r--r--   0        0        0     1392 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/utils.py
--rw-r--r--   0        0        0     1534 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/contracts/variable.py
--rw-r--r--   0        0        0     1158 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/data/contracts/header.py
--rw-r--r--   0        0        0      173 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/data/mermaid.py
--rw-r--r--   0        0        0      636 2023-07-14 09:36:36.935242 autonomy_dev-0.2.5/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      532 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/data/repo/templates/python/readme.py
--rw-r--r--   0        0        0     2027 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/fmt.py
--rw-r--r--   0        0        0     3090 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/fsm/chain.py
--rw-r--r--   0        0        0     8368 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/fsm/fsm.py
--rw-r--r--   0        0        0      464 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/lint.py
--rw-r--r--   0        0        0     2153 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/local_fork.py
--rw-r--r--   0        0        0      470 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/test.py
--rw-r--r--   0        0        0     2542 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/auto_dev/utils.py
--rw-r--r--   0        0        0     2635 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      296 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0     1634 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/tests/test_augmenter.py
--rw-r--r--   0        0        0     1084 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/tests/test_cli.py
--rw-r--r--   0        0        0     2459 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/tests/test_contracts.py
--rw-r--r--   0        0        0     5241 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/tests/test_fsm.py
--rw-r--r--   0        0        0     1562 2023-07-14 09:36:36.939242 autonomy_dev-0.2.5/tests/test_local_fork.py
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 autonomy_dev-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/LICENSE
+-rw-r--r--   0        0        0      967 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/__init__.py
+-rw-r--r--   0        0        0     2716 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/base.py
+-rw-r--r--   0        0        0      242 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/cli.py
+-rw-r--r--   0        0        0     2758 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0     3456 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/augment.py
+-rw-r--r--   0        0        0     5505 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/deps.py
+-rw-r--r--   0        0        0     1890 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/fmt.py
+-rw-r--r--   0        0        0     1372 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/fsm.py
+-rw-r--r--   0        0        0     2144 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/lint.py
+-rw-r--r--   0        0        0     3538 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/release.py
+-rw-r--r--   0        0        0     5195 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/repo.py
+-rw-r--r--   0        0        0     3525 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/scaffold.py
+-rw-r--r--   0        0        0     1450 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/commands/test.py
+-rw-r--r--   0        0        0      515 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/constants.py
+-rw-r--r--   0        0        0     1482 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/block_explorer.py
+-rw-r--r--   0        0        0     5786 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/contract.py
+-rw-r--r--   0        0        0     2914 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/contract_functions.py
+-rw-r--r--   0        0        0     2238 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/contract_scafolder.py
+-rw-r--r--   0        0        0     6102 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/contract_templates.py
+-rw-r--r--   0        0        0     1787 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/function.py
+-rw-r--r--   0        0        0      679 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/param_type.py
+-rw-r--r--   0        0        0     1616 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/utils.py
+-rw-r--r--   0        0        0     1636 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/contracts/variable.py
+-rw-r--r--   0        0        0     1158 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/data/contracts/header.py
+-rw-r--r--   0        0        0      173 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/data/mermaid.py
+-rw-r--r--   0        0        0      636 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      532 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/data/repo/templates/python/readme.py
+-rw-r--r--   0        0        0     2027 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/fmt.py
+-rw-r--r--   0        0        0     3090 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/fsm/chain.py
+-rw-r--r--   0        0        0     8368 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/fsm/fsm.py
+-rw-r--r--   0        0        0      464 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/lint.py
+-rw-r--r--   0        0        0     2153 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/local_fork.py
+-rw-r--r--   0        0        0      470 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/test.py
+-rw-r--r--   0        0        0     2542 2023-07-15 01:49:12.096851 autonomy_dev-0.2.6/auto_dev/utils.py
+-rw-r--r--   0        0        0     2633 2023-07-15 01:49:12.100851 autonomy_dev-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-07-15 01:49:12.100851 autonomy_dev-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0     1634 2023-07-15 01:49:12.100851 autonomy_dev-0.2.6/tests/test_augmenter.py
+-rw-r--r--   0        0        0     1084 2023-07-15 01:49:12.100851 autonomy_dev-0.2.6/tests/test_cli.py
+-rw-r--r--   0        0        0     2459 2023-07-15 01:49:12.100851 autonomy_dev-0.2.6/tests/test_contracts.py
+-rw-r--r--   0        0        0     5241 2023-07-15 01:49:12.100851 autonomy_dev-0.2.6/tests/test_fsm.py
+-rw-r--r--   0        0        0     1562 2023-07-15 01:49:12.100851 autonomy_dev-0.2.6/tests/test_local_fork.py
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 autonomy_dev-0.2.6/PKG-INFO
```

### Comparing `autonomy_dev-0.2.5/LICENSE` & `autonomy_dev-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/README.md` & `autonomy_dev-0.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,11 +28,12 @@
 ## Release
 bump the version in pyoproject and create a new branch and tag
 
 ```bash
 export new_version=v0.1.5
 git checkout -b $new_version
 git add .
+git commit -m "[chore] bumping version $new_version"
 git tag $new_version
 git push --set-upstream origin (git rev-parse --abbrev-ref HEAD)
 git push --tag
-```
+```
```

### Comparing `autonomy_dev-0.2.5/auto_dev/base.py` & `autonomy_dev-0.2.6/auto_dev/base.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/cli_executor.py` & `autonomy_dev-0.2.6/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/augment.py` & `autonomy_dev-0.2.6/auto_dev/commands/augment.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/deps.py` & `autonomy_dev-0.2.6/auto_dev/commands/deps.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/fmt.py` & `autonomy_dev-0.2.6/auto_dev/commands/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/fsm.py` & `autonomy_dev-0.2.6/auto_dev/commands/fsm.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/lint.py` & `autonomy_dev-0.2.6/auto_dev/commands/lint.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/release.py` & `autonomy_dev-0.2.6/auto_dev/commands/release.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/repo.py` & `autonomy_dev-0.2.6/auto_dev/commands/repo.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/scaffold.py` & `autonomy_dev-0.2.6/auto_dev/commands/scaffold.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     scaffolder = ContractScaffolder(block_explorer=block_explorer)
     logger.info("Getting abi from block explorer.")
     new_contract = scaffolder.from_block_explorer(address, name)
     logger.info("Generating openaea contract with aea scaffolder.")
     contract_path = scaffolder.generate_openaea_contract(new_contract)
     logger.info("Writing abi to file, Updating contract.yaml with build path. Parsing functions.")
     new_contract.process()
-    logger.info(f"Read Functions: {new_contract.read_functions}")
-    logger.info(f"Write Functions: {new_contract.write_functions}")
+    logger.info("Read Functions:")
+    for function in new_contract.read_functions:
+        logger.info(f"    {function.name}")
+    logger.info("Write Functions:")
+    for function in new_contract.write_functions:
+        logger.info(f"    {function.name}")
+
     logger.info(f"New contract scaffolded at {contract_path}")
 
 
 if __name__ == "__main__":
     cli()  # pylint: disable=no-value-for-parameter
```

### Comparing `autonomy_dev-0.2.5/auto_dev/commands/test.py` & `autonomy_dev-0.2.6/auto_dev/commands/test.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/constants.py` & `autonomy_dev-0.2.6/auto_dev/constants.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/block_explorer.py` & `autonomy_dev-0.2.6/auto_dev/contracts/block_explorer.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/contract.py` & `autonomy_dev-0.2.6/auto_dev/contracts/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,19 @@
             "contract_id = PUBLIC_ID",
         )
         contract_py = contract_py.replace(
             "from aea.configurations.base import PublicId",
             f"from packages.{self.author}.contracts.{self.name} import PUBLIC_ID",
         )
 
+        contract_py = contract_py.replace(
+            "from aea.crypto.base import LedgerApi",
+            "from aea.crypto.base import LedgerApi, Address",
+        )
+
         read_functions = "\n".join([function.to_string() for function in self.read_functions])
         contract_py += read_functions
 
         with contract_py_path.open("w", encoding=DEFAULT_ENCODING) as file_pointer:
             file_pointer.write(contract_py)
 
     def update_contract_init__(self):
```

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/contract_functions.py` & `autonomy_dev-0.2.6/auto_dev/contracts/contract_functions.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/contract_scafolder.py` & `autonomy_dev-0.2.6/auto_dev/contracts/contract_scafolder.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/contract_templates.py` & `autonomy_dev-0.2.6/auto_dev/contracts/contract_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         cls,
         ledger_api: LedgerApi,
         contract_address: str,
         $params
         ) -> JSONLike:
         \"\"\"Handler method for the '$name' requests.\"\"\"
         instance = cls.get_instance(ledger_api, contract_address)
-        result = instance.$name($args).call()
+        result = instance.functions.$camel_name($args).call()
         return {
             $returns
         }
 
 """
 )
```

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/function.py` & `autonomy_dev-0.2.6/auto_dev/contracts/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,29 +24,38 @@
         Returns the function as a string.
         """
         spacer = ",\n" + (" " * 8)
         returns = spacer.join([param.to_str_return() for param in self.outputs])
         args = spacer.join([param.to_str_arg() for param in self.inputs])
         params = spacer.join([param.to_str_params() for param in self.inputs])
         return READ_FUNCTION_TEMPLATE.substitute(
-            name=self.name if self.name != "" else "constructor", params=params, args=args, returns=returns
+            name=self.name if self.name != "" else "constructor",
+            camel_name=self.camel_case_name if self.name != "" else "constructor",
+            params=params,
+            args=args,
+            returns=returns
         )
 
     @property
     def name(self):
         """Return the name of the function."""
         return from_camel_case_to_snake_case(self.abi["name"])
 
     @property
+    def camel_case_name(self):
+        """Return the name of the function."""
+        return self.abi["name"]
+
+    @property
     def inputs(self):
         """Return the inputs as variables."""
-        return [Variable(**param) for param in self.abi["inputs"]]
+        return [Variable(**param, index=ix) for ix, param in enumerate(self.abi["inputs"])]
 
     @property
     def outputs(self):
         """Return the outputs as variables."""
-        return [Variable(**param) for param in self.abi["outputs"]]
+        return [Variable(**param, index=ix) for ix, param in enumerate(self.abi["outputs"])]
 
     @property
     def is_read_only(self):
         """Is the function read only."""
         return self.abi["stateMutability"] == "view"
```

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/param_type.py` & `autonomy_dev-0.2.6/auto_dev/contracts/param_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,21 @@
     """This class represent the type of a parameter in solidity."""
 
     ADDRESS = "address"
     BOOL = "bool"
     UINT256 = "uint256"
     UNINT64 = "uint64"
     UINT8 = "uint8"
+    UINT16 = "uint16"
+    UINT24 = "uint24"
+    UINT128 = "uint128"
     INT128 = "int128"
     INT256 = "int256"
     BYTES32 = "bytes32"
     UINT80 = "uint80"
     TUPLE = "tuple"
     UINT256_ARRAY = "uint256[]"
+    UINT64_ARRAY = "uint64[]"
+    INT80_ARRAY = "int80[]"
     ADDRESS_ARRAY = "address[]"
     STRING = "string"
+    TUPLE_ARRAY = "tuple[]"
```

### Comparing `autonomy_dev-0.2.5/auto_dev/contracts/variable.py` & `autonomy_dev-0.2.6/auto_dev/contracts/variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,33 +12,36 @@
 class Variable:
     """This class represent a variable in solidity."""
 
     internalType: ParamType  # pylint: disable=C0103
     type: ParamType
     name: str
     components: Optional[Any] = None
+    index: Optional[int] = None
 
     def to_str_params(self):
         """Parse the variable to string to be passed as a parameter to a function."""
         return f"{self._name}: {self.python_type}"
 
     def to_str_arg(self):
         """Parse the variable to string to be passed as an argument to a function."""
-        return f"{self._name}={self.name}"
+        if self.name == "":
+            return f"{self._name}"
+        return f"{self._name}={self._name}"
 
     def to_str_return(self):
         """Parse the variable to string to be returned by a function."""
         result_name = self.name if self.name != "" else self.python_type.lower()
         return f"'{result_name}': result"
 
     @property
     def _name(self):
         """Return the name of the variable."""
         if self.name == "":
-            return "constructor"
+            return f"var_{self.index}"
         return self.name
 
     @property
     def solidity_type(self):
         """Return the solidity type of the variable."""
         try:
             return ParamType(self.internalType)
```

### Comparing `autonomy_dev-0.2.5/auto_dev/data/contracts/header.py` & `autonomy_dev-0.2.6/auto_dev/data/contracts/header.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/data/pylama.ini` & `autonomy_dev-0.2.6/auto_dev/data/pylama.ini`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/data/repo/templates/python/readme.py` & `autonomy_dev-0.2.6/auto_dev/data/repo/templates/python/readme.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/fmt.py` & `autonomy_dev-0.2.6/auto_dev/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/fsm/chain.py` & `autonomy_dev-0.2.6/auto_dev/fsm/chain.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/fsm/fsm.py` & `autonomy_dev-0.2.6/auto_dev/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/local_fork.py` & `autonomy_dev-0.2.6/auto_dev/local_fork.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/auto_dev/utils.py` & `autonomy_dev-0.2.6/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/pyproject.toml` & `autonomy_dev-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.2.5"
+version = "0.2.6"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -49,15 +49,15 @@
 mkdocstrings-python = "^0.10.0"
 isort = "~5"
 pylint = "~2"
 open-aea = "^1.35.0"
 open-aea-cli-ipfs = "^1.35.0"
 web3 = "~5"
 open-autonomy = "^0.10"
-docker = "~6.1"
+docker = "~6"
 
 [tool.poetry.dev-dependencies]
 responses = "^0.23.1"
 
 
 [tool.poetry.extras]
 all = [
```

### Comparing `autonomy_dev-0.2.5/tests/test_augmenter.py` & `autonomy_dev-0.2.6/tests/test_augmenter.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/tests/test_cli.py` & `autonomy_dev-0.2.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/tests/test_contracts.py` & `autonomy_dev-0.2.6/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/tests/test_fsm.py` & `autonomy_dev-0.2.6/tests/test_fsm.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/tests/test_local_fork.py` & `autonomy_dev-0.2.6/tests/test_local_fork.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.5/PKG-INFO` & `autonomy_dev-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<=3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "all"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: click (==8.0.2)
-Requires-Dist: docker (>=6.1,<6.2)
+Requires-Dist: docker (>=6,<7)
 Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: isort (>=5,<6) ; extra == "all"
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=3.6.1,<4.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.4.0,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
@@ -79,11 +79,13 @@
 ## Release
 bump the version in pyoproject and create a new branch and tag
 
 ```bash
 export new_version=v0.1.5
 git checkout -b $new_version
 git add .
+git commit -m "[chore] bumping version $new_version"
 git tag $new_version
 git push --set-upstream origin (git rev-parse --abbrev-ref HEAD)
 git push --tag
 ```
+
```

