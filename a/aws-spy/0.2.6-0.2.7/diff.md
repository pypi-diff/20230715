# Comparing `tmp/aws_spy-0.2.6.tar.gz` & `tmp/aws_spy-0.2.7.tar.gz`

## Comparing `aws_spy-0.2.6.tar` & `aws_spy-0.2.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 aws_spy-0.2.6/Makefile
--rw-r--r--   0        0        0    81872 2020-02-02 00:00:00.000000 aws_spy-0.2.6/pdm.lock
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.2.6/.vscode/settings.json
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/dependencies.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/main.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/responses.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/encoders.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/event_utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/exceptions.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/logging.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/params.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/params_alias.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/responses.py
--rw-r--r--   0        0        0     8927 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/schemas.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/schemas_utils.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/core/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/helpers/__init__.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/helpers/cli.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/helpers/documentation.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/helpers/exceptions.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/helpers/utils.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/layer/spy-layer.yml
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/layer/spy/python/pydantic_core/__init__.py
--rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0        0        0   129458 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/layer/spy/python/pydantic_core/core_schema.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_spy-0.2.6/aws_spy/layer/spy/python/pydantic_core/py.typed
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 aws_spy-0.2.6/docker/Dockerfile
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aws_spy-0.2.6/docker/docker-compose.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/integration/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/integration/test_params.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/integration/test_request_body.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/integration/test_response_class.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/integration/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/unit/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/unit/test_encoders.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/unit/test_event_utils.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/unit/test_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/unit/test_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.6/tests/unit/test_utils.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 aws_spy-0.2.6/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.2.6/LICENSE
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.2.6/README.md
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aws_spy-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aws_spy-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 aws_spy-0.2.7/Makefile
+-rw-r--r--   0        0        0    81872 2020-02-02 00:00:00.000000 aws_spy-0.2.7/pdm.lock
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.2.7/.vscode/settings.json
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/dependencies.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/main.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/responses.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/encoders.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/event_utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/exceptions.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/logging.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/params.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/params_alias.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/responses.py
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/schemas.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/schemas_utils.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/core/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/helpers/__init__.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/helpers/cli.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/helpers/documentation.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/helpers/exceptions.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/helpers/utils.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/layer/spy-layer.yml
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/layer/spy/python/annotated_types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/layer/spy/python/annotated_types/py.typed
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/layer/spy/python/pydantic_core/__init__.py
+-rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0        0        0   129458 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/layer/spy/python/pydantic_core/core_schema.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_spy-0.2.7/aws_spy/layer/spy/python/pydantic_core/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/integration/test_params.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/integration/test_request_body.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/integration/test_response_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/integration/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/unit/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/unit/test_encoders.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/unit/test_event_utils.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/unit/test_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/unit/test_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.7/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 aws_spy-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.2.7/LICENSE
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.2.7/README.md
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aws_spy-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aws_spy-0.2.7/PKG-INFO
```

### Comparing `aws_spy-0.2.6/.pre-commit-config.yaml` & `aws_spy-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/Makefile` & `aws_spy-0.2.7/Makefile`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/pdm.lock` & `aws_spy-0.2.7/pdm.lock`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/__init__.py` & `aws_spy-0.2.7/aws_spy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ServerlessPy package ;D"""
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 from aws_spy import responses
 from aws_spy.core.logging import logger
 from aws_spy.core.params_alias import Header, Path, Query
 from aws_spy.core.schemas import (
     CORS,
     VPC,
```

### Comparing `aws_spy-0.2.6/aws_spy/dependencies.py` & `aws_spy-0.2.7/aws_spy/dependencies.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/main.py` & `aws_spy-0.2.7/aws_spy/main.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/responses.py` & `aws_spy-0.2.7/aws_spy/responses.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/test.py` & `aws_spy-0.2.7/aws_spy/test.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/core/event_utils.py` & `aws_spy-0.2.7/aws_spy/core/event_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/core/schemas.py` & `aws_spy-0.2.7/aws_spy/core/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Methods.PUT: "200",
     Methods.PATCH: "200",
 }
 
 
 class Functions(str, Enum):
     LAYER = "layer"
-    OPENAPI = "openapi"
+    # OPENAPI = "openapi"
     SLS = "sls"
 
 
 class SpyRoute(BaseModel):
     name: str
     path: str
     method: Methods
@@ -175,15 +175,15 @@
 
 
 def build_cognito_issue_url(user_pool_id: str | CloudFormationRef | JSONFileRef) -> str:
     return f"https://cognito-idp.${{region}}.amazonaws.com/{user_pool_id}"
 
 
 class Authorizer(BaseModel):
-    type: Literal["jwt"] = "jwt"  # noqa: A003
+    type: Literal["jwt"] = Field("jwt", frozen=True)  # noqa: A003
     identitySource: str = "$request.header.Authorization"  # noqa: N815
     issuerUrl: str  # noqa: N815
     audience: list[str | CloudFormationRef | JSONFileRef]
 
 
 class CORS(BaseModel):
     allowedHeaders: list[str]  # noqa: N815
@@ -235,27 +235,28 @@
                     *route.layers,  # type: ignore
                 )
             ),
         )
 
 
 class Provider(BaseModel):
-    name: str = "aws"
-    runtime: str = "python3.10"
+    name: Literal["aws"] = Field("aws", frozen=True)
+    runtime: Literal["python3.10"] = Field("python3.10", frozen=True)
     region: str = "eu_central_1"
+    architecture: Literal["arm64", "x86_64"] = Field("arm64", frozen=True)  # pydantic_core
     role: str | CloudFormationRef | JSONFileRef | None = Field(None)
     httpApi: HTTPApi | None = Field(None)  # noqa: N815
     vpc: VPC | None = Field(None)
 
 
 class ServerlessConfig(YamlModel):
     service: str
     custom: dict[str, Any] | None = Field(None)
     plugins: list[str]
-    configValidationMode: str = "error"  # noqa: N815
+    configValidationMode: Literal["error", "warn"] = Field("warn", frozen=True)  # noqa: N815
     provider: Provider
     package: dict[str, bool] = Field({"individually": True})
     functions: dict[str, Function] | None = Field(None)
 
     @field_validator("plugins", mode="before")
     def set_default_plugins(cls: type[Self], value: list[str] | None) -> list[str]:  # type: ignore  # noqa: N805
         value = value if value is not None else []
```

### Comparing `aws_spy-0.2.6/aws_spy/core/schemas_utils.py` & `aws_spy-0.2.7/aws_spy/core/schemas_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/core/types.py` & `aws_spy-0.2.7/aws_spy/core/types.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/helpers/cli.py` & `aws_spy-0.2.7/aws_spy/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/helpers/documentation.py` & `aws_spy-0.2.7/aws_spy/helpers/documentation.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/helpers/utils.py` & `aws_spy-0.2.7/aws_spy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/layer/spy/python/pydantic_core/__init__.py` & `aws_spy-0.2.7/aws_spy/layer/spy/python/pydantic_core/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi` & `aws_spy-0.2.7/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/aws_spy/layer/spy/python/pydantic_core/core_schema.py` & `aws_spy-0.2.7/aws_spy/layer/spy/python/pydantic_core/core_schema.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/tests/conftest.py` & `aws_spy-0.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/tests/test_app.py` & `aws_spy-0.2.7/tests/test_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from aws_spy import ServerlessConfig, SpyAPI, SpyRouter, __version__
 from aws_spy.core.schemas import Methods
 
 
 def test_app() -> None:
-    assert __version__ == "0.2.6"
+    assert __version__ == "0.2.7"
 
 
 def test_app_conf(app: SpyAPI, config: ServerlessConfig) -> None:
     assert app.config == config
 
 
 @pytest.mark.parametrize("prefix", ["api", "/api", "/somet_other_prefix"])
```

### Comparing `aws_spy-0.2.6/tests/integration/test_params.py` & `aws_spy-0.2.7/tests/integration/test_params.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/tests/integration/test_request_body.py` & `aws_spy-0.2.7/tests/integration/test_request_body.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/tests/integration/test_response_class.py` & `aws_spy-0.2.7/tests/integration/test_response_class.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/tests/unit/test_encoders.py` & `aws_spy-0.2.7/tests/unit/test_encoders.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/tests/unit/test_event_utils.py` & `aws_spy-0.2.7/tests/unit/test_event_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/tests/unit/test_responses.py` & `aws_spy-0.2.7/tests/unit/test_responses.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/.gitignore` & `aws_spy-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/LICENSE` & `aws_spy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/pyproject.toml` & `aws_spy-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.6/PKG-INFO` & `aws_spy-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-spy
-Version: 0.2.6
+Version: 0.2.7
 Project-URL: Homepage, https://github.com/PiochU19/aws-spy
 Project-URL: Documentation, https://github.com/PiochU19/aws-spy#readme
 Project-URL: Issues, https://github.com/PiochU19/aws-spy/issues
 Project-URL: Source, https://github.com/PiochU19/aws-spy
 Author-email: Dominik Pioś <792954018@wp.pl>
 License: The MIT License (MIT)
```

