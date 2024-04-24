# Comparing `tmp/pytract-0.0.2.tar.gz` & `tmp/pytract-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytract-0.0.2.tar", last modified: Fri Apr 12 08:18:45 2024, max compression
+gzip compressed data, was "pytract-0.0.3.tar", last modified: Wed Apr 24 08:27:38 2024, max compression
```

## Comparing `pytract-0.0.2.tar` & `pytract-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.540000 pytract-0.0.2/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     4354 2024-04-12 08:18:45.540000 pytract-0.0.2/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3166 2024-04-12 08:09:44.000000 pytract-0.0.2/README.md
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.530000 pytract-0.0.2/pytract/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      115 2024-04-11 17:26:05.000000 pytract-0.0.2/pytract/__init__.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      801 2024-04-11 19:26:57.000000 pytract-0.0.2/pytract/__main__.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)    11708 2024-04-12 07:24:01.000000 pytract-0.0.2/pytract/abi2api.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      224 2024-04-10 01:41:33.000000 pytract-0.0.2/pytract/classes.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       60 2024-04-11 15:00:14.000000 pytract-0.0.2/pytract/compile.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       83 2024-04-11 05:38:49.000000 pytract-0.0.2/pytract/constants.py
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       61 2024-04-11 13:46:32.000000 pytract-0.0.2/pytract/datatypes.py
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.540000 pytract-0.0.2/pytract/templates/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3335 2024-04-12 07:27:18.000000 pytract-0.0.2/pytract/templates/api.py.j2
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      234 2024-04-11 14:59:51.000000 pytract-0.0.2/pytract/utils.py
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.540000 pytract-0.0.2/pytract.egg-info/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     4354 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      390 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/SOURCES.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/dependency_links.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       51 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/entry_points.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       37 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/requires.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        8 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/top_level.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-12 08:18:45.540000 pytract-0.0.2/setup.cfg
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      746 2024-04-11 19:29:10.000000 pytract-0.0.2/setup.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.230000 pytract-0.0.3/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5315 2024-04-24 08:27:38.230000 pytract-0.0.3/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3991 2024-04-22 07:54:42.000000 pytract-0.0.3/README.md
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.220000 pytract-0.0.3/pytract/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      115 2024-04-11 17:26:05.000000 pytract-0.0.3/pytract/__init__.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      801 2024-04-11 19:26:57.000000 pytract-0.0.3/pytract/__main__.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)    12280 2024-04-24 07:07:40.000000 pytract-0.0.3/pytract/abi2api.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       83 2024-04-11 05:38:49.000000 pytract-0.0.3/pytract/constants.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.230000 pytract-0.0.3/pytract/templates/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3345 2024-04-24 06:55:37.000000 pytract-0.0.3/pytract/templates/api.py.j2
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      234 2024-04-11 14:59:51.000000 pytract-0.0.3/pytract/utils.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)    12865 2024-04-24 07:21:41.000000 pytract-0.0.3/pytract/vm.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 08:27:38.230000 pytract-0.0.3/pytract.egg-info/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5315 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      345 2024-04-24 08:27:38.000000 pytract-0.0.3/pytract.egg-info/SOURCES.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/dependency_links.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       51 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/entry_points.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       53 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/requires.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)        8 2024-04-24 08:27:37.000000 pytract-0.0.3/pytract.egg-info/top_level.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-24 08:27:38.230000 pytract-0.0.3/setup.cfg
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      765 2024-04-24 08:25:26.000000 pytract-0.0.3/setup.py
```

### Comparing `pytract-0.0.2/README.md` & `pytract-0.0.3/pytract/templates/api.py.j2`

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,80 @@
-# pytract
+{# template code for generating contract apis #}
+{# remember to use black formatter after code has been generated. #}
+from brownie.network.account import Account
+from brownie.network.contract import Contract, ProjectContract
+from pytract import abi2api
+from typing import Optional, Union
+from ._project import project_info
 
-Smart contract Python API generator.
-
-It works by interpreting smart contract ABI and generate corresponding Python API code.
-
-## Usage
-
-Install from PyPI:
-
-```bash
-pip install pytract
-```
-
-Create Python API code for your `brownie` project:
-
-```bash
-usage: pytract process [-h] project_path
-
-positional arguments:
-  project_path  Path of the project to process
-
-optional arguments:
-  -h, --help    show this help message and exit
-```
-
-And you shall import all available contracts and programmatically.
-
-If your project folder name is `brownie_project` then write:
-
-```python
-from brownie_project.api import project_info, contracts
-
-print(dir(contracts)) # list available contract classes
-print(dir(project_info)) # list project info attributes
-```
-
-Note the difference of using it with `brownie` alone, you now have a fully portable python package, which you can write static typed code without the need for copying and pasting from `brownie console`.
-
-You can view all generated API code under folder `<your brownie project>/api`.
-
-Example generated contract API class is given below:
-
-```python
-class Faucet(abi2api.ContractInstance):
+{% for contract_name, contract_info in project_info.contracts_info.items() %}
+class {{contract_name}}(abi2api.ContractInstance):
     _project = project_info.project
-    _contract_info = project_info.contracts_info["Faucet"]
-    _contract_name = "Faucet"
+    _contract_info = project_info.contracts_info["{{contract_name}}"]
+    _contract_name = "{{contract_name}}"
 
     class Function(abi2api.FunctionBase):
-        def returnVars(
-            self,
-        ):
+        {% for function_info in contract_info.function_info_list %}
+        {% set function_type = function_info.stateMutability %}
+        {% set not_pure = check_function_type_not_pure(function_type) %}
+        {# is it pure, nonpayable or payable? #}
+        def {{function_info.name}}(self, {{", ".join(get_names_from_list(function_info.inputs))}}{{', _txparams: Optional[abi2api.TransactionParameters]=None' if not_pure else ''}}):
             """
-            Function Type: pure
+            Function Type: {{function_type}}
 
             Inputs:
+            {% if function_info.inputs != [] %}
+                {% for parameter in function_info.inputs %}
+                {{parameter.name}}: {{parameter.type_hint}}
+                {% endfor %}
+            {% else %}
                 (No parameters)
+            {% endif %}
 
             Outputs:
-                (uint256, uint256, uint256)
-            """
-            values = self._contract.returnVars()
-            return values
-
-        def withdraw(
-            self,
-            withdraw_amount,
-            _txparams: Optional[abi2api.TransactionParameters] = None,
-        ):
-            """
-            Function Type: nonpayable
-
-            Inputs:
-                withdraw_amount: uint256
-
-            Outputs:
+            {% if function_info.outputs != [] %}
+                ({{ ", ".join(get_types_from_list(function_info.outputs)) }})
+            {% else %}
                 (No parameters)
+            {% endif %}
             """
-            values = self._contract.withdraw(
-                withdraw_amount, self.txparams_with_fallback(_txparams).dict()
-            )
+            {# # call the underlying contract. #}
+            values = self._contract.{{function_info.name}}(
+            {{", ".join(get_names_from_list(function_info.inputs))}} {{', self.txparams_with_fallback(_txparams).dict()' if not_pure else ''}})
             return values
 
-    def __init__(
-        self,
-        contract: Union[Contract, ProjectContract],
-        issuer: Optional[Account] = None,
-        _txparams: Optional[abi2api.TransactionParameters] = None,
-    ):  # to create you need to either deploy or load contract by address
+        {% endfor %}
+    
+
+    def __init__(self, contract: Union[Contract, ProjectContract], issuer:Optional[Account]=None, _txparams:Optional[abi2api.TransactionParameters] = None): # to create you need to either deploy or load contract by address
         super().__init__(contract, issuer)
         self.function = self.Function(contract, _txparams)
         """
         Available functions of this smart contract.
         """
 
     @classmethod
-    def deploy(cls, _txparams: abi2api.TransactionParameters):
+    def deploy(cls, {{", ".join(get_names_from_list(contract_info.deploy_abi.inputs)+["_txparams: abi2api.TransactionParameters"])}}):
         """
         Inputs:
             transaction_parameters: TransactionParameters
-
+        {% if contract_info.deploy_abi.inputs != [] %}
+            {% for parameter in function_info.inputs %}
+            {{parameter.name}}: {{parameter.type_hint}}
+            {% endfor %}
+        {% endif %}
+        
         Output:
-            contract: Faucet
+            contract: {{contract_name}}
         """
-        args = []
+        args = [{{", ".join(get_names_from_list(contract_info.deploy_abi.inputs))}}]
 
         parameters = _txparams.to_contract_deploy_parameters(args)
 
-        deployed_contract: ProjectContract = cls._contract_info.contract_container.deploy(*parameters.to_args())  # type: ignore
+        deployed_contract: ProjectContract = cls._contract_info.contract_container.deploy( *parameters.to_args()) # type: ignore
 
         return cls(deployed_contract, _txparams.issuer, _txparams)
+    
+{% endfor %}
 
 
-```
-
-## Roadmap
-
-- [x] Create a binding to smart contract and APIs for Brownie
+__all__ = {{list(project_info.contracts_info.keys())}}
```

### Comparing `pytract-0.0.2/pytract/__main__.py` & `pytract-0.0.3/pytract/__main__.py`

 * *Files identical despite different names*

### Comparing `pytract-0.0.2/pytract/abi2api.py` & `pytract-0.0.3/pytract/abi2api.py`

 * *Files 14% similar despite different names*

```diff
@@ -115,18 +115,34 @@
     issuer: Account
 
     @classmethod
     def from_contract(cls, contract: Union[ProjectContract, Contract], issuer: Account):
         return cls(contract=contract, issuer=issuer)
 
 
+# TODO: recursively resolve and create tuple type hints for languages like vyper
 class ParamType(pydantic.BaseModel):
     type: str
-    name: str
-    internalType: str
+    name: str = "" # mostly ignored
+    components: list["ParamType"] = []
+
+    # internalType: str
+    @property
+    def type_hint(self):
+        return self.resolve_type_hint(self)
+
+    @staticmethod
+    def resolve_type_hint(obj: "ParamType"):
+        if obj.components == []:
+            return obj.type
+        else:
+            it_type_hints = []
+            for it in obj.components:
+                it_type_hints.append(ParamType.resolve_type_hint(it))
+            return f"{obj.type}({', '.join(it_type_hints)})"
 
 
 class ContractABI(pydantic.BaseModel):
     inputs: List[ParamType] = []
     outputs: List[ParamType] = []
     type: Optional[str] = None
     stateMutability: Optional[str] = None
@@ -302,15 +318,15 @@
 
 
 def get_names_from_list(obj):
     return [param.name for param in obj]
 
 
 def get_types_from_list(obj):
-    return [param.type for param in obj]
+    return [param.type_hint for param in obj]
 
 
 def check_function_type_not_pure(function_type):
     return function_type not in ["view", "pure"]
 
 
 def generate_api_code_for_project(project_path: str):
```

### Comparing `pytract-0.0.2/setup.py` & `pytract-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup
 
 PKG_NAME = "pytract"
+VERSION = "0.0.3"
+
 # REQUIREMENTS = [
 #     # "vyper",
 #     "jinja2",
 #     "eth-brownie",
 #     "pydantic",
 #     "beartype",
 # ]
 
 setup(
     name=PKG_NAME,
-    version="0.0.2",
+    version=VERSION,
     packages=[PKG_NAME],
     description="Smart contract Python API generator.",
     url=f"https://github.com/james4ever0/{PKG_NAME}",
     package_data={PKG_NAME: ['templates/*.j2']},
     include_package_data=True,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

