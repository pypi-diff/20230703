# Comparing `tmp/fastapi-jsonrpc-2.4.1.tar.gz` & `tmp/fastapi_jsonrpc-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-jsonrpc-2.4.1.tar", max compression
+gzip compressed data, was "fastapi_jsonrpc-2.5.0.tar", max compression
```

## Comparing `fastapi-jsonrpc-2.4.1.tar` & `fastapi_jsonrpc-2.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1082 2021-06-08 10:10:56.676877 fastapi-jsonrpc-2.4.1/LICENSE
--rw-r--r--   0        0        0     7059 2022-08-10 19:58:12.687323 fastapi-jsonrpc-2.4.1/README.rst
--rw-r--r--   0        0        0    44225 2022-11-09 13:03:01.092699 fastapi-jsonrpc-2.4.1/fastapi_jsonrpc/__init__.py
--rw-r--r--   0        0        0      787 2022-11-09 13:15:31.765709 fastapi-jsonrpc-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     8193 2022-11-09 13:17:00.586918 fastapi-jsonrpc-2.4.1/setup.py
--rw-r--r--   0        0        0     7929 2022-11-09 13:17:00.587792 fastapi-jsonrpc-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2021-06-08 10:10:56.676877 fastapi_jsonrpc-2.5.0/LICENSE
+-rw-r--r--   0        0        0     7059 2022-08-10 19:58:12.687323 fastapi_jsonrpc-2.5.0/README.rst
+-rw-r--r--   0        0        0    44396 2023-07-03 13:08:10.001865 fastapi_jsonrpc-2.5.0/fastapi_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     1023 2023-07-03 13:19:50.823524 fastapi_jsonrpc-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8355 1970-01-01 00:00:00.000000 fastapi_jsonrpc-2.5.0/setup.py
+-rw-r--r--   0        0        0     8153 1970-01-01 00:00:00.000000 fastapi_jsonrpc-2.5.0/PKG-INFO
```

### Comparing `fastapi-jsonrpc-2.4.1/LICENSE` & `fastapi_jsonrpc-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-jsonrpc-2.4.1/README.rst` & `fastapi_jsonrpc-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `fastapi-jsonrpc-2.4.1/fastapi_jsonrpc/__init__.py` & `fastapi_jsonrpc-2.5.0/fastapi_jsonrpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,17 @@
     else:
         _JsonRpcRequestParams = ModelMetaclass.__new__(ModelMetaclass, '_JsonRpcRequestParams', (BaseModel,), {})
 
         for f in body_params:
             example = f.field_info.example  # noqa
             if example is not Undefined:
                 f.field_info.extra['example'] = jsonable_encoder(example)
+            examples = f.field_info.extra.get('examples')
+            if examples is not None:
+                f.field_info.extra['examples'] = jsonable_encoder(examples)
             _JsonRpcRequestParams.__fields__[f.name] = f
 
         _JsonRpcRequestParams = component_name(f'_Params[{name}]', module)(_JsonRpcRequestParams)
 
         params_field = ModelField(
             name='params',
             type_=_JsonRpcRequestParams,
```

### Comparing `fastapi-jsonrpc-2.4.1/pyproject.toml` & `fastapi_jsonrpc-2.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 [tool.poetry]
 name = "fastapi-jsonrpc"
-version = "2.4.1"
+version = "2.5.0"
 description = "JSON-RPC server based on fastapi"
 license = "MIT"
 authors = ["Sergey Magafurov <magafurov@tochka.com>"]
 readme = "README.rst"
 repository = "https://github.com/smagafurov/fastapi-jsonrpc"
 homepage = "https://github.com/smagafurov/fastapi-jsonrpc"
 keywords = ['json-rpc', 'asgi', 'swagger', 'openapi', 'fastapi', 'pydantic', 'starlette']
 exclude = ["example1.py", "example2.py"]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 aiojobs = ">0.2.2"
-fastapi = ">0.55"
-pydantic = ">0.0.0"
+fastapi = [
+    {version = ">0.55.0", python = "<3.11"},
+    {version = ">=0.86.0", python = ">=3.11"},
+]
+pydantic = [
+    {version = ">0.0.0", python = "<3.11"},
+    {version = ">=1.10.0", python = ">=3.11"},
+]
 starlette = ">0.0.0"
 
 [tool.poetry.dev-dependencies]
-uvicorn = "^0.14.0"
+uvicorn = "^0.17.0"
 rst_include = "^2.1.0"
 pytest = "^6.2"
 sentry-sdk = "^1.3.0"
 requests = ">0.0.0"
+httpx = ">=0.23.0,<0.24.0"  # FastAPI/Starlette extra test deps
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `fastapi-jsonrpc-2.4.1/setup.py` & `fastapi_jsonrpc-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 packages = \
 ['fastapi_jsonrpc']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiojobs>0.2.2', 'fastapi>0.55', 'pydantic>0.0.0', 'starlette>0.0.0']
+['aiojobs>0.2.2', 'starlette>0.0.0']
+
+extras_require = \
+{':python_version < "3.11"': ['fastapi>0.55.0', 'pydantic>0.0.0'],
+ ':python_version >= "3.11"': ['fastapi>=0.86.0', 'pydantic>=1.10.0']}
 
 setup_kwargs = {
     'name': 'fastapi-jsonrpc',
-    'version': '2.4.1',
+    'version': '2.5.0',
     'description': 'JSON-RPC server based on fastapi',
     'long_description': '|tests|\n\n.. |tests| image:: https://github.com/smagafurov/fastapi-jsonrpc/actions/workflows/tests.yml/badge.svg\n   :target: https://github.com/smagafurov/fastapi-jsonrpc/actions/workflows/tests.yml\n\n\nDescription\n===========\n\nJSON-RPC server based on fastapi:\n\n    https://fastapi.tiangolo.com\n\nMotivation\n^^^^^^^^^^\n\nAutogenerated **OpenAPI** and **Swagger** (thanks to fastapi) for JSON-RPC!!!\n\nInstallation\n============\n\n.. code-block:: bash\n\n    pip install fastapi-jsonrpc\n\nDocumentation\n=============\n\nRead FastAPI documentation and see usage examples bellow\n\nSimple usage example\n====================\n\n.. code-block:: bash\n\n    pip install uvicorn\n\nexample1.py\n\n.. code-block:: python\n\n    import fastapi_jsonrpc as jsonrpc\n    from pydantic import BaseModel\n    from fastapi import Body\n\n\n    app = jsonrpc.API()\n\n    api_v1 = jsonrpc.Entrypoint(\'/api/v1/jsonrpc\')\n\n\n    class MyError(jsonrpc.BaseError):\n        CODE = 5000\n        MESSAGE = \'My error\'\n\n        class DataModel(BaseModel):\n            details: str\n\n\n    @api_v1.method(errors=[MyError])\n    def echo(\n        data: str = Body(..., example=\'123\'),\n    ) -> str:\n        if data == \'error\':\n            raise MyError(data={\'details\': \'error\'})\n        else:\n            return data\n\n\n    app.bind_entrypoint(api_v1)\n\n\n    if __name__ == \'__main__\':\n        import uvicorn\n        uvicorn.run(\'example1:app\', port=5000, debug=True, access_log=False)\n\nGo to:\n\n    http://127.0.0.1:5000/docs\n\nFastAPI dependencies usage example\n==================================\n\n.. code-block:: bash\n\n    pip install uvicorn\n\nexample2.py\n\n.. code-block:: python\n\n    import logging\n    from contextlib import asynccontextmanager\n\n    from pydantic import BaseModel, Field\n    import fastapi_jsonrpc as jsonrpc\n    from fastapi import Body, Header, Depends\n\n\n    logger = logging.getLogger(__name__)\n\n\n    # database models\n\n    class User:\n        def __init__(self, name):\n            self.name = name\n\n        def __eq__(self, other):\n            if not isinstance(other, User):\n                return False\n            return self.name == other.name\n\n\n    class Account:\n        def __init__(self, account_id, owner, amount, currency):\n            self.account_id = account_id\n            self.owner = owner\n            self.amount = amount\n            self.currency = currency\n\n        def owned_by(self, user: User):\n            return self.owner == user\n\n\n    # fake database\n\n    users = {\n        \'1\': User(\'user1\'),\n        \'2\': User(\'user2\'),\n    }\n\n    accounts = {\n        \'1.1\': Account(\'1.1\', users[\'1\'], 100, \'USD\'),\n        \'1.2\': Account(\'1.2\', users[\'1\'], 200, \'EUR\'),\n        \'2.1\': Account(\'2.1\', users[\'2\'], 300, \'USD\'),\n    }\n\n\n    def get_user_by_token(auth_token) -> User:\n        return users[auth_token]\n\n\n    def get_account_by_id(account_id) -> Account:\n        return accounts[account_id]\n\n\n    # schemas\n\n    class Balance(BaseModel):\n        """Account balance"""\n        amount: int = Field(..., example=100)\n        currency: str = Field(..., example=\'USD\')\n\n\n    # errors\n\n    class AuthError(jsonrpc.BaseError):\n        CODE = 7000\n        MESSAGE = \'Auth error\'\n\n\n    class AccountNotFound(jsonrpc.BaseError):\n        CODE = 6000\n        MESSAGE = \'Account not found\'\n\n\n    class NotEnoughMoney(jsonrpc.BaseError):\n        CODE = 6001\n        MESSAGE = \'Not enough money\'\n\n        class DataModel(BaseModel):\n            balance: Balance\n\n\n    # dependencies\n\n    def get_auth_user(\n        # this will become the header-parameter of json-rpc method that uses this dependency\n        auth_token: str = Header(\n            None,\n            alias=\'user-auth-token\',\n        ),\n    ) -> User:\n        if not auth_token:\n            raise AuthError\n\n        try:\n            return get_user_by_token(auth_token)\n        except KeyError:\n            raise AuthError\n\n\n    def get_account(\n        # this will become the parameter of the json-rpc method that uses this dependency\n        account_id: str = Body(..., example=\'1.1\'),\n        user: User = Depends(get_auth_user),\n    ) -> Account:\n        try:\n            account = get_account_by_id(account_id)\n        except KeyError:\n            raise AccountNotFound\n\n        if not account.owned_by(user):\n            raise AccountNotFound\n\n        return account\n\n\n    # JSON-RPC middlewares\n\n    @asynccontextmanager\n    async def logging_middleware(ctx: jsonrpc.JsonRpcContext):\n        logger.info(\'Request: %r\', ctx.raw_request)\n        try:\n            yield\n        finally:\n            logger.info(\'Response: %r\', ctx.raw_response)\n\n\n    # JSON-RPC entrypoint\n\n    common_errors = [AccountNotFound, AuthError]\n    common_errors.extend(jsonrpc.Entrypoint.default_errors)\n\n    api_v1 = jsonrpc.Entrypoint(\n        # Swagger shows for entrypoint common parameters gathered by dependencies and common_dependencies:\n        #    - json-rpc-parameter \'account_id\'\n        #    - header parameter \'user-auth-token\'\n        \'/api/v1/jsonrpc\',\n        errors=common_errors,\n        middlewares=[logging_middleware],\n        # this dependencies called once for whole json-rpc batch request\n        dependencies=[Depends(get_auth_user)],\n        # this dependencies called separately for every json-rpc request in batch request\n        common_dependencies=[Depends(get_account)],\n    )\n\n\n    # JSON-RPC methods of this entrypoint\n\n    # this json-rpc method has one json-rpc-parameter \'account_id\' and one header parameter \'user-auth-token\'\n    @api_v1.method()\n    def get_balance(\n        account: Account = Depends(get_account),\n    ) -> Balance:\n        return Balance(\n            amount=account.amount,\n            currency=account.currency,\n        )\n\n\n    # this json-rpc method has two json-rpc-parameters \'account_id\', \'amount\' and one header parameter \'user-auth-token\'\n    @api_v1.method(errors=[NotEnoughMoney])\n    def withdraw(\n        account: Account = Depends(get_account),\n        amount: int = Body(..., gt=0, example=10),\n    ) -> Balance:\n        if account.amount - amount < 0:\n            raise NotEnoughMoney(data={\'balance\': get_balance(account)})\n        account.amount -= amount\n        return get_balance(account)\n\n\n    # JSON-RPC API\n\n    app = jsonrpc.API()\n    app.bind_entrypoint(api_v1)\n\n\n    if __name__ == \'__main__\':\n        import uvicorn\n        uvicorn.run(\'example2:app\', port=5000, debug=True, access_log=False)\n\nGo to:\n\n    http://127.0.0.1:5000/docs\n\n.. image:: ./images/fastapi-jsonrpc.png\n\nDevelopment\n===========\n\n* Install poetry\n\n    https://github.com/sdispater/poetry#installation\n\n* Install dependencies\n\n    .. code-block:: bash\n\n        poetry update\n\n* Regenerate README.rst\n\n    .. code-block:: bash\n\n        rst_include include -q README.src.rst README.rst\n\n* Change dependencies\n\n    Edit ``pyproject.toml``\n\n    .. code-block:: bash\n\n        poetry update\n\n* Bump version\n\n    .. code-block:: bash\n\n        poetry version patch\n        poetry version minor\n        poetry version major\n\n* Publish to pypi\n\n    .. code-block:: bash\n\n        poetry publish --build\n\n',
     'author': 'Sergey Magafurov',
     'author_email': 'magafurov@tochka.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/smagafurov/fastapi-jsonrpc',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0.0',
+    'extras_require': extras_require,
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fastapi-jsonrpc-2.4.1/PKG-INFO` & `fastapi_jsonrpc-2.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: fastapi-jsonrpc
-Version: 2.4.1
+Version: 2.5.0
 Summary: JSON-RPC server based on fastapi
 Home-page: https://github.com/smagafurov/fastapi-jsonrpc
 License: MIT
 Keywords: json-rpc,asgi,swagger,openapi,fastapi,pydantic,starlette
 Author: Sergey Magafurov
 Author-email: magafurov@tochka.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiojobs (>0.2.2)
-Requires-Dist: fastapi (>0.55)
-Requires-Dist: pydantic (>0.0.0)
+Requires-Dist: fastapi (>0.55.0) ; python_version < "3.11"
+Requires-Dist: fastapi (>=0.86.0) ; python_version >= "3.11"
+Requires-Dist: pydantic (>0.0.0) ; python_version < "3.11"
+Requires-Dist: pydantic (>=1.10.0) ; python_version >= "3.11"
 Requires-Dist: starlette (>0.0.0)
 Project-URL: Repository, https://github.com/smagafurov/fastapi-jsonrpc
 Description-Content-Type: text/x-rst
 
 |tests|
 
 .. |tests| image:: https://github.com/smagafurov/fastapi-jsonrpc/actions/workflows/tests.yml/badge.svg
```

