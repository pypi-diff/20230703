# Comparing `tmp/oauth2_lib-1.3.0.tar.gz` & `tmp/oauth2_lib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2_lib-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "oauth2_lib-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `oauth2_lib-1.3.0.tar` & `oauth2_lib-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      363 2023-07-03 07:19:02.701044 oauth2_lib-1.3.0/.bumpversion.cfg
--rw-r--r--   0        0        0      550 2023-07-03 07:19:02.701044 oauth2_lib-1.3.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0      389 2023-07-03 07:19:02.701044 oauth2_lib-1.3.0/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1894 2023-07-03 07:19:02.701044 oauth2_lib-1.3.0/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1486 2023-07-03 07:19:02.701044 oauth2_lib-1.3.0/.github/workflows/test-package.yml
--rw-r--r--   0        0        0     1115 2023-07-03 07:19:02.701044 oauth2_lib-1.3.0/.gitignore
--rw-r--r--   0        0        0     1668 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/LICENSE
--rw-r--r--   0        0        0     1754 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/README.md
--rwxr-xr-x   0        0        0      150 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/fmt_code.sh
--rw-r--r--   0        0        0      671 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/oauth2_lib/__init__.py
--rw-r--r--   0        0        0     5407 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/oauth2_lib/async_api_client.py
--rw-r--r--   0        0        0    15662 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/oauth2_lib/fastapi.py
--rw-r--r--   0        0        0     6098 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/oauth2_lib/graphql_authentication.py
--rw-r--r--   0        0        0        0 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/oauth2_lib/py.typed
--rw-r--r--   0        0        0      943 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/oauth2_lib/settings.py
--rw-r--r--   0        0        0     2803 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1151 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3273 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     2795 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/graphql/conftest.py
--rw-r--r--   0        0        0     1541 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/graphql/test_authenticated_federated_field.py
--rw-r--r--   0        0        0     2360 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/graphql/test_authenticated_field.py
--rw-r--r--   0        0        0     3052 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/graphql/test_authenticated_mutation_field.py
--rw-r--r--   0        0        0     5764 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/test_async_api_client.py
--rw-r--r--   0        0        0    13734 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/test_fastapi.py
--rw-r--r--   0        0        0     6570 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/test_opa_decision.py
--rw-r--r--   0        0        0     4289 2023-07-03 07:19:02.705044 oauth2_lib-1.3.0/tests/test_opa_graphql_decision.py
--rw-r--r--   0        0        0     4000 1970-01-01 00:00:00.000000 oauth2_lib-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-07-03 07:25:16.304500 oauth2_lib-1.3.1/.bumpversion.cfg
+-rw-r--r--   0        0        0      550 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0      389 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1894 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1451 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/test-package.yml
+-rw-r--r--   0        0        0     1115 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1668 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1754 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/README.md
+-rwxr-xr-x   0        0        0      150 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/fmt_code.sh
+-rw-r--r--   0        0        0      671 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/__init__.py
+-rw-r--r--   0        0        0     5328 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/async_api_client.py
+-rw-r--r--   0        0        0    15661 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/fastapi.py
+-rw-r--r--   0        0        0     6098 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/graphql_authentication.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/py.typed
+-rw-r--r--   0        0        0      943 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/settings.py
+-rw-r--r--   0        0        0     2803 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1151 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     2795 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/conftest.py
+-rw-r--r--   0        0        0     1541 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/test_authenticated_federated_field.py
+-rw-r--r--   0        0        0     2360 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/test_authenticated_field.py
+-rw-r--r--   0        0        0     3052 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/test_authenticated_mutation_field.py
+-rw-r--r--   0        0        0     5708 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_async_api_client.py
+-rw-r--r--   0        0        0    13734 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_fastapi.py
+-rw-r--r--   0        0        0     6570 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_opa_decision.py
+-rw-r--r--   0        0        0     4289 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_opa_graphql_decision.py
+-rw-r--r--   0        0        0     4000 1970-01-01 00:00:00.000000 oauth2_lib-1.3.1/PKG-INFO
```

### Comparing `oauth2_lib-1.3.0/.github/workflows/publish-release.yml` & `oauth2_lib-1.3.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/.github/workflows/scheduled-build.yml` & `oauth2_lib-1.3.1/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/.github/workflows/test-package.yml` & `oauth2_lib-1.3.1/.github/workflows/test-package.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flit
           flit install --deps develop --symlink
-      - name: Black, Ruff and MyPy
       - name: Lint
         run: |
           black . --check
           ruff .
       - name: MyPy
         run: |
           mypy -p oauth2_lib
```

### Comparing `oauth2_lib-1.3.0/.gitignore` & `oauth2_lib-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/.pre-commit-config.yaml` & `oauth2_lib-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/LICENSE` & `oauth2_lib-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/README.md` & `oauth2_lib-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/oauth2_lib/__init__.py` & `oauth2_lib-1.3.1/oauth2_lib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the SURF Oauth2 module that interfaces with the oauth2 setup."""
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
```

### Comparing `oauth2_lib-1.3.0/oauth2_lib/async_api_client.py` & `oauth2_lib-1.3.1/oauth2_lib/async_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,20 @@
     _token: Union[dict, None]
 
     def __init__(
         self,
         oauth_client: BaseOAuth,
         oauth_client_name: str,
         oauth_active: bool,
-        tracing_enabled: bool,
         *args: Any,
         **kwargs: Any,
     ):
         super().__init__(*args, **kwargs)
         self._oauth_client: BaseOAuth = getattr(oauth_client, oauth_client_name)
         self._oauth_active = oauth_active
-        self._tracing_enabled = tracing_enabled
         self._token = None
 
     def add_client_creds_token_header(self, headers: dict[str, Any]) -> None:
         """Add header with credentials to an existing set of headers.
 
         This function assumes the `access_token` has been set in the application configuration
         by `refresh_client_creds_token or by acquire_token`.
```

### Comparing `oauth2_lib-1.3.0/oauth2_lib/fastapi.py` & `oauth2_lib-1.3.1/oauth2_lib/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         return set(re.split("[ ,]", self.get("scope", "")))
 
     @property
     def is_resource_server(self) -> bool:
         return self.get("is_resource_server", False)
 
     @property
-    def surf_crm_id(self) -> bool:
+    def surf_crm_id(self) -> str:
         return self.get("surf-crm-id", "")
 
 
 async def async_client() -> AsyncGenerator[AsyncClient, None]:
     async with AsyncClient(http1=True) as client:
         yield client
```

### Comparing `oauth2_lib-1.3.0/oauth2_lib/graphql_authentication.py` & `oauth2_lib-1.3.1/oauth2_lib/graphql_authentication.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/oauth2_lib/settings.py` & `oauth2_lib-1.3.1/oauth2_lib/settings.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/pyproject.toml` & `oauth2_lib-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/setup.cfg` & `oauth2_lib-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/tests/graphql/conftest.py` & `oauth2_lib-1.3.1/tests/graphql/conftest.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/tests/graphql/test_authenticated_federated_field.py` & `oauth2_lib-1.3.1/tests/graphql/test_authenticated_federated_field.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/tests/graphql/test_authenticated_field.py` & `oauth2_lib-1.3.1/tests/graphql/test_authenticated_field.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/tests/graphql/test_authenticated_mutation_field.py` & `oauth2_lib-1.3.1/tests/graphql/test_authenticated_mutation_field.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/tests/test_async_api_client.py` & `oauth2_lib-1.3.1/tests/test_async_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,14 @@
             oauth_client = mock.MagicMock()
             oauth_client.fetch_access_token = mock_fetch_access_token
             base_oauth_client.actualclient = oauth_client
             super().__init__(
                 oauth_client=base_oauth_client,
                 oauth_client_name="actualclient",
                 oauth_active=True,
-                tracing_enabled=True,
                 configuration=config,
             )
 
             self._token = {"access_token": token}
 
     return FakeFinalApiClient(url)
 
@@ -124,15 +123,15 @@
             "/app/endpoint",
             body=json.dumps({"error": "not found"}),
             status=HTTPStatus.NOT_FOUND,
             content_type="application/json",
         )
 
 
-def test_asyncauthmixin_request_200(tracing, responses):
+def test_asyncauthmixin_request_200(responses):
     """Test that making a request with valid token works."""
 
     # given
     client = make_api_client()
 
     apimock = ApiMock(responses)
     apimock.get_endpoint()
@@ -141,15 +140,15 @@
     res = client.request("GET", f"{BASE_URL}/app/endpoint")
 
     # then
     assert res.status == HTTPStatus.OK
     assert len(responses.calls) == 1
 
 
-def test_asyncauthmixin_request_401_then_200(tracing, responses):
+def test_asyncauthmixin_request_401_then_200(responses):
     """Test that a request with expired token is retried with a valid token."""
     # given
     client = make_api_client(token=EXPIRED_TOKEN)
     apimock = ApiMock(responses)
     apimock.get_endpoint()
 
     # when
```

### Comparing `oauth2_lib-1.3.0/tests/test_fastapi.py` & `oauth2_lib-1.3.1/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/tests/test_opa_decision.py` & `oauth2_lib-1.3.1/tests/test_opa_decision.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/tests/test_opa_graphql_decision.py` & `oauth2_lib-1.3.1/tests/test_opa_graphql_decision.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.0/PKG-INFO` & `oauth2_lib-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-lib
-Version: 1.3.0
+Version: 1.3.1
 Summary: This is the SURF Oauth2 module that interfaces with the oauth2 setup.
 Home-page: https://github.com/workfloworchestrator/oauth2-lib
 Author: SURF
 Author-email: automation-beheer@surf.nl
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

