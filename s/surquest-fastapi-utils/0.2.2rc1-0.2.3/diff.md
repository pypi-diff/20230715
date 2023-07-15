# Comparing `tmp/surquest_fastapi_utils-0.2.2rc1.tar.gz` & `tmp/surquest_fastapi_utils-0.2.3.tar.gz`

## Comparing `surquest_fastapi_utils-0.2.2rc1.tar` & `surquest_fastapi_utils-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/package.base.dockerfile
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/.github/workflows/test.yml
--rw-r--r--   0        0        0    43478 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/assets/img/logs.png
--rw-r--r--   0        0        0    66316 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/assets/img/trace.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/base.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/info.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/message.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/metadata.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/responses.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/status.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/__init__.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/args.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/auth.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/route.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/GCP.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/catcher.py
--rw-r--r--   0        0        0     6510 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/formatter.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/http_context.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/logging.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/middleware.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/tracer.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/test/pytest.ini
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/test/utils/test_catcher.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/LICENSE
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/README.md
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/pyproject.toml
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.2rc1/PKG-INFO
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/package.base.dockerfile
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0    43478 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/assets/img/logs.png
+-rw-r--r--   0        0        0    66316 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/assets/img/trace.png
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/base.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/info.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/message.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/metadata.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/responses.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/status.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/__init__.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/args.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/auth.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/route.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/GCP.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/__init__.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/catcher.py
+-rw-r--r--   0        0        0     6510 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/formatter.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/http_context.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/logging.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/middleware.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/tracer.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/test/pytest.ini
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/test/utils/test_catcher.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/README.md
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.3/PKG-INFO
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/package.base.dockerfile` & `surquest_fastapi_utils-0.2.3/package.base.dockerfile`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/.github/workflows/release.yml` & `surquest_fastapi_utils-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/assets/img/logs.png` & `surquest_fastapi_utils-0.2.3/assets/img/logs.png`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/assets/img/trace.png` & `surquest_fastapi_utils-0.2.3/assets/img/trace.png`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/metadata.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/metadata.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from pydantic import Field
-from .base import Base
-
-class Metadata(Base):
-
-    offset: int = Field(
-        default=0,
-        title="Offset",
-        description="Number of records to skip from the beginning",
-        ge=0,
-        example=0,
-    )
-
-    limit: int = Field(
-        default=0,
-        title="Offset",
-        description="Number of records to skip from the beginning",
-        ge=0,
-        example=0,
-    )
-
-    count: int = Field(
-        ...,
-        title="Count of records",
-        description="Count of records returned by the call",
-        example=391,
-        ge=0,
-    )
-
-    total: int = Field(
-        ...,
-        title="Total records",
-        description="Total number of records in the database",
-        example=18301,
-        ge=0,
-    )
+from pydantic import Field
+from .base import Base
+
+class Metadata(Base):
+
+    offset: int = Field(
+        default=0,
+        title="Offset",
+        description="Number of records to skip from the beginning",
+        ge=0,
+        example=0,
+    )
+
+    limit: int = Field(
+        default=0,
+        title="Offset",
+        description="Number of records to skip from the beginning",
+        ge=0,
+        example=0,
+    )
+
+    count: int = Field(
+        ...,
+        title="Count of records",
+        description="Count of records returned by the call",
+        example=391,
+        ge=0,
+    )
+
+    total: int = Field(
+        ...,
+        title="Total records",
+        description="Total number of records in the database",
+        example=18301,
+        ge=0,
+    )
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/schemas/responses/responses.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/schemas/responses/responses.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from .base import Base
-from .info import InfoSuccess, InfoWarning, InfoError
-from typing import Union, List, Dict, Optional
-from starlette.responses import JSONResponse, Response
-from fastapi.encoders import jsonable_encoder
-
-
-class Success(Base):
-    info: InfoSuccess = InfoSuccess()
-    data: Optional[Union[List, Dict]]= None
-
-    @classmethod
-    def set(cls, data, metadata=None):
-        return cls(
-            info=InfoSuccess(metadata=metadata),
-            data=data
-        )
-
-
-class Warnings(Base):
-
-    info: InfoWarning = InfoWarning()
-    data: Optional[Union[List, Dict]] = None
-
-    @classmethod
-    def set(cls, warnings, data, metadata=None):
-
-        return cls(
-            info=InfoWarning(warnings=warnings, metadata=metadata),
-            data=data
-        )
-
-
-class Errors(Base):
-    info: InfoError = InfoError()
-
-    @classmethod
-    def set(cls, errors, warnings=None):
-        return cls(
-            info=InfoError(
-                warnings=warnings,
-                errors=errors
-            )
-        )
-
-class Response:
-
-    @classmethod
-    def set(
-        cls,
-        status_code=None,
-        data=None,
-        metadata=None,
-        warnings=None,
-        errors=None
-    ):
-
-        status_code = cls.get_status_code(status_code, warnings, errors)
-
-        if errors is not None:
-
-            return JSONResponse(
-                status_code=status_code,
-                content=jsonable_encoder(
-                    Errors.set(
-                        errors=errors,
-                        warnings=warnings
-                    )
-                )
-            )
-        if errors is None and warnings is not None:
-
-            return JSONResponse(
-                status_code=status_code,
-                content=jsonable_encoder(
-                    Warnings.set(
-                        warnings=warnings,
-                        data=data,
-                        metadata=metadata
-                    )
-                )
-            )
-
-        return JSONResponse(
-            status_code=status_code,
-            content=jsonable_encoder(
-                Success.set(
-                    data=data,
-                    metadata=metadata
-                )
-            )
-        )
-
-    @staticmethod
-    def get_status_code(status_code, warnings, errors):
-
-        if isinstance(status_code, int):
-            return status_code
-
-        if errors is not None:
-            return 500
-
-        if errors is None and warnings is not None:
-            return 299
-
-        return 200
-
-class Responses:
-
-    @classmethod
-    def get(cls):
-
-        return {
-            200: {"model": Success},
-            299: {"model": Warnings},
-            400: {"model": Errors},
-            422: {"model": Errors},
-            500: {"model": Errors},
-        }
+from .base import Base
+from .info import InfoSuccess, InfoWarning, InfoError
+from typing import Union, List, Dict, Optional
+from starlette.responses import JSONResponse, Response
+from fastapi.encoders import jsonable_encoder
+
+
+class Success(Base):
+    info: InfoSuccess = InfoSuccess()
+    data: Optional[Union[List, Dict]]= None
+
+    @classmethod
+    def set(cls, data, metadata=None):
+        return cls(
+            info=InfoSuccess(metadata=metadata),
+            data=data
+        )
+
+
+class Warnings(Base):
+
+    info: InfoWarning = InfoWarning()
+    data: Optional[Union[List, Dict]] = None
+
+    @classmethod
+    def set(cls, warnings, data, metadata=None):
+
+        return cls(
+            info=InfoWarning(warnings=warnings, metadata=metadata),
+            data=data
+        )
+
+
+class Errors(Base):
+    info: InfoError = InfoError()
+
+    @classmethod
+    def set(cls, errors, warnings=None):
+        return cls(
+            info=InfoError(
+                warnings=warnings,
+                errors=errors
+            )
+        )
+
+class Response:
+
+    @classmethod
+    def set(
+        cls,
+        status_code=None,
+        data=None,
+        metadata=None,
+        warnings=None,
+        errors=None
+    ):
+
+        status_code = cls.get_status_code(status_code, warnings, errors)
+
+        if errors is not None:
+
+            return JSONResponse(
+                status_code=status_code,
+                content=jsonable_encoder(
+                    Errors.set(
+                        errors=errors,
+                        warnings=warnings
+                    )
+                )
+            )
+        if errors is None and warnings is not None:
+
+            return JSONResponse(
+                status_code=status_code,
+                content=jsonable_encoder(
+                    Warnings.set(
+                        warnings=warnings,
+                        data=data,
+                        metadata=metadata
+                    )
+                )
+            )
+
+        return JSONResponse(
+            status_code=status_code,
+            content=jsonable_encoder(
+                Success.set(
+                    data=data,
+                    metadata=metadata
+                )
+            )
+        )
+
+    @staticmethod
+    def get_status_code(status_code, warnings, errors):
+
+        if isinstance(status_code, int):
+            return status_code
+
+        if errors is not None:
+            return 500
+
+        if errors is None and warnings is not None:
+            return 299
+
+        return 200
+
+class Responses:
+
+    @classmethod
+    def get(cls):
+
+        return {
+            200: {"model": Success},
+            299: {"model": Warnings},
+            400: {"model": Errors},
+            422: {"model": Errors},
+            500: {"model": Errors},
+        }
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/auth.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/auth.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import typing
-from fastapi.security.api_key import APIKeyQuery
-from fastapi import HTTPException, Security, Request
-
-
-api_key_query = APIKeyQuery(name="apiKey", auto_error=False)
-
-async def check_api_key(
-    request: Request,
-    api_key_query: str = Security(api_key_query),
-):
-
-    # check if app has defined API key
-    if "api_key" in request.app.extra:
-
-        # check if passed API key is equal to app's API key
-        if api_key_query == request.app.extra.get("api_key"):
-            return api_key_query
-        else:
-            raise AUTHException()
-
-
-class AUTHException(HTTPException):
-    def __init__(
-        self,
-        status_code: int = 401, # HTTP status code for Unauthorized
-        detail: typing.Optional[str] = "Unauthorized: Invalid API Key",
-        loc: typing.Optional[list] = ["query", "apiKey"],
-        type: typing.Optional[str] = "AUTH.ERROR"
-    ) -> None:
-        self.status_code = status_code
-        self.detail = detail
-        self.loc = loc
-        self.type = type
-
-    def __repr__(self) -> str:
-        class_name = self.__class__.__name__
+import typing
+from fastapi.security.api_key import APIKeyQuery
+from fastapi import HTTPException, Security, Request
+
+
+api_key_query = APIKeyQuery(name="apiKey", auto_error=False)
+
+async def check_api_key(
+    request: Request,
+    api_key_query: str = Security(api_key_query),
+):
+
+    # check if app has defined API key
+    if "api_key" in request.app.extra:
+
+        # check if passed API key is equal to app's API key
+        if api_key_query == request.app.extra.get("api_key"):
+            return api_key_query
+        else:
+            raise AUTHException()
+
+
+class AUTHException(HTTPException):
+    def __init__(
+        self,
+        status_code: int = 401, # HTTP status code for Unauthorized
+        detail: typing.Optional[str] = "Unauthorized: Invalid API Key",
+        loc: typing.Optional[list] = ["query", "apiKey"],
+        type: typing.Optional[str] = "AUTH.ERROR"
+    ) -> None:
+        self.status_code = status_code
+        self.detail = detail
+        self.loc = loc
+        self.type = type
+
+    def __repr__(self) -> str:
+        class_name = self.__class__.__name__
         return f"{class_name}(status_code={self.status_code!r}, detail={self.detail!r})"
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/catcher.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/catcher.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-# import external modules
-import os
-from fastapi import Request
-from fastapi.exceptions import RequestValidationError
-from starlette.exceptions import HTTPException as StarletteHTTPException
-import traceback
-
-from surquest.fastapi.schemas.responses import Response, Message
-
-from .logging import Logger
-from .http_context import (
-    HTTP_REQUEST_CONTEXT,
-    CLOUD_TRACE_CONTEXT
-)
-
-__all__ = [
-    "Catcher",
-    "catch_validation_exceptions",
-    "catch_http_exceptions"
-]
-
-
-async def catch_validation_exceptions(request: Request, exc):
-    return await Catcher.catch_validation_error(request, exc)
-
-
-async def catch_http_exceptions(request: Request, exc):
-    return await Catcher.catch_http_exception(request, exc)
-
-
-class Catcher:
-
-    OUPS = "Oups, something went wrong"
-
-    @classmethod
-    async def catch_internal_error(
-            cls,
-            request: Request,
-            exc: BaseException
-    ):
-
-        tb = traceback.format_exc(chain=False).split("\n")
-
-        ctx = {
-            "trace": CLOUD_TRACE_CONTEXT.get()
-        }
-
-        if os.getenv("ENV", "DEV").upper() not in ["PROD", "PRODUCTION"] or \
-            os.getenv("ENVIRONMENT", "DEV").upper() not in ["PROD", "PRODUCTION"]:
-
-            ctx["traceback"] = tb
-
-        message = Message(
-            msg=F"{str(exc)} ({type(exc).__name__})",
-            type="SERVER.ERROR",
-            ctx=ctx,
-        )
-
-        Logger.error(
-            F"{str(exc)} ({type(exc).__name__})",
-            extra={
-                "error": message.dict(exclude_none=True),
-                "request": HTTP_REQUEST_CONTEXT.get(),
-                "traceback": tb
-            }
-        )
-
-        return Response.set(
-            status_code=500,
-            errors=[message]
-        )
-
-    @classmethod
-    async def catch_validation_error(
-            cls,
-            request: Request,
-            exc: RequestValidationError
-    ):
-        errors = []
-
-        for error in exc.errors():
-            errors.append(
-                Message(
-                    msg=error.get("msg"),
-                    type=error.get("type"),
-                    loc=error.get("loc"),
-                    ctx=error.get("ctx"),
-                ).dict(exclude_none=True)
-            )
-
-        Logger.error(
-            "Validation Error",
-            extra={
-                "errors": errors,
-                "request": HTTP_REQUEST_CONTEXT.get()
-            }
-        )
-
-        return Response.set(
-            status_code=422,
-            errors=errors
-        )
-
-    @classmethod
-    async def catch_http_exception(
-            cls,
-            request: Request,
-            exc: StarletteHTTPException
-    ):
-
-        message = Message(
-            msg=getattr(exc, "detail", f"Not Found: ({request.url})"),
-            type=getattr(exc, "type", "NOT.FOUND"),
-            loc=getattr(exc, "loc", [F"{request.url}"]),
-            ctx=getattr(exc, "ctx", {"trace": CLOUD_TRACE_CONTEXT.get()})
-        )
-
-        Logger.error(
-            F"{message.msg}: ({message.loc[0]})",
-            extra={
-                "error": message.dict(exclude_none=True),
-                "request": HTTP_REQUEST_CONTEXT.get()
-            }
-        )
-
-        return Response.set(
-            status_code=getattr(exc, "status_code", 404),
-            errors=[message]
-        )
+# import external modules
+import os
+from fastapi import Request
+from fastapi.exceptions import RequestValidationError
+from starlette.exceptions import HTTPException as StarletteHTTPException
+import traceback
+
+from surquest.fastapi.schemas.responses import Response, Message
+
+from .logging import Logger
+from .http_context import (
+    HTTP_REQUEST_CONTEXT,
+    CLOUD_TRACE_CONTEXT
+)
+
+__all__ = [
+    "Catcher",
+    "catch_validation_exceptions",
+    "catch_http_exceptions"
+]
+
+
+async def catch_validation_exceptions(request: Request, exc):
+    return await Catcher.catch_validation_error(request, exc)
+
+
+async def catch_http_exceptions(request: Request, exc):
+    return await Catcher.catch_http_exception(request, exc)
+
+
+class Catcher:
+
+    OUPS = "Oups, something went wrong"
+
+    @classmethod
+    async def catch_internal_error(
+            cls,
+            request: Request,
+            exc: BaseException
+    ):
+
+        tb = traceback.format_exc(chain=False).split("\n")
+
+        ctx = {
+            "trace": CLOUD_TRACE_CONTEXT.get()
+        }
+
+        if os.getenv("ENV", "DEV").upper() not in ["PROD", "PRODUCTION"] or \
+            os.getenv("ENVIRONMENT", "DEV").upper() not in ["PROD", "PRODUCTION"]:
+
+            ctx["traceback"] = tb
+
+        message = Message(
+            msg=F"{str(exc)} ({type(exc).__name__})",
+            type="SERVER.ERROR",
+            ctx=ctx,
+        )
+
+        Logger.error(
+            F"{str(exc)} ({type(exc).__name__})",
+            extra={
+                "error": message.dict(exclude_none=True),
+                "request": HTTP_REQUEST_CONTEXT.get(),
+                "traceback": tb
+            }
+        )
+
+        return Response.set(
+            status_code=500,
+            errors=[message]
+        )
+
+    @classmethod
+    async def catch_validation_error(
+            cls,
+            request: Request,
+            exc: RequestValidationError
+    ):
+        errors = []
+
+        for error in exc.errors():
+            errors.append(
+                Message(
+                    msg=error.get("msg"),
+                    type=error.get("type"),
+                    loc=error.get("loc"),
+                    ctx=error.get("ctx"),
+                ).dict(exclude_none=True)
+            )
+
+        Logger.error(
+            "Validation Error",
+            extra={
+                "errors": errors,
+                "request": HTTP_REQUEST_CONTEXT.get()
+            }
+        )
+
+        return Response.set(
+            status_code=422,
+            errors=errors
+        )
+
+    @classmethod
+    async def catch_http_exception(
+            cls,
+            request: Request,
+            exc: StarletteHTTPException
+    ):
+
+        message = Message(
+            msg=getattr(exc, "detail", f"Not Found: ({request.url})"),
+            type=getattr(exc, "type", "NOT.FOUND"),
+            loc=getattr(exc, "loc", [F"{request.url}"]),
+            ctx=getattr(exc, "ctx", {"trace": CLOUD_TRACE_CONTEXT.get()})
+        )
+
+        Logger.error(
+            F"{message.msg}: ({message.loc[0]})",
+            extra={
+                "error": message.dict(exclude_none=True),
+                "request": HTTP_REQUEST_CONTEXT.get()
+            }
+        )
+
+        return Response.set(
+            status_code=getattr(exc, "status_code", 404),
+            errors=[message]
+        )
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/formatter.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/formatter.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/http_context.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/http_context.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/logging.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/logging.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/middleware.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/middleware.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/surquest/fastapi/utils/GCP/tracer.py` & `surquest_fastapi_utils-0.2.3/surquest/fastapi/utils/GCP/tracer.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,29 @@
     "Tracer"
 ]
 
 DEFAULT_TRACER_NAME = os.getenv('APP_NAME', "APILogger")
 
 tracer_provider = TracerProvider(sampler=ALWAYS_ON)  # always trace
 trace.set_tracer_provider(tracer_provider)
-cloud_trace_exporter = CloudTraceSpanExporter()
-tracer_provider.add_span_processor(
-    # BatchSpanProcessor buffers spans and sends them in batches in a
-    # background thread. The default parameters are sensible, but can be
-    # tweaked to optimize your performance
-    BatchSpanProcessor(cloud_trace_exporter)
-)
+# cloud_trace_exporter = CloudTraceSpanExporter()
+try:
+    cloud_trace_exporter = CloudTraceSpanExporter()
+except Exception as e:
+    print("CloudTraceSpanExporter not initialized")
+    print(e)
+    cloud_trace_exporter = None
+
+if cloud_trace_exporter is not None:    
+    tracer_provider.add_span_processor(
+        # BatchSpanProcessor buffers spans and sends them in batches in a
+        # background thread. The default parameters are sensible, but can be
+        # tweaked to optimize your performance
+        BatchSpanProcessor(cloud_trace_exporter)
+    )
 
 class Tracer:
 
     @classmethod
     def start_span(cls, name):
 
         (
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/test/utils/test_catcher.py` & `surquest_fastapi_utils-0.2.3/test/utils/test_catcher.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/.gitignore` & `surquest_fastapi_utils-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.2rc1/README.md` & `surquest_fastapi_utils-0.2.3/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-![GitHub](https://img.shields.io/github/license/surquest/python-fastapi-utils?style=flat-square)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/surquest-fastapi-utils?style=flat-square)
-![PyPI](https://img.shields.io/pypi/v/surquest-fastapi-utils)
-
-# Introduction
-
-This project provides collection of utilities for smooth integration of FastAPI framework with Google Cloud Platform services as logging and tracing.
-
-The key features of this project are:
-
-* Logging to Cloud Logging
-* Tracing to Cloud Logging
-* Error Reporting via Cloud Logging
-* Custom middleware for configuration of logging
-* Custom exception handlers treating HTTP and validation exceptions
-* Custom routes for documentation and favicon
-* Custom responses with statuses `success`, `warning` and `error` and standardized error messages
-
-# Quick Start
-
-This section shows how to use the utilities provided by this project:
-
-```python
-"""File main.py with FastAPI app"""
-import os
-from fastapi.exceptions import RequestValidationError
-from starlette.exceptions import HTTPException
-from fastapi import FastAPI, Request, Query
-
-# import surquest modules and objects
-from surquest.fastapi.utils.route import Route  # custom routes for documentation and FavIcon
-from surquest.fastapi.utils.GCP.tracer import Tracer
-from surquest.fastapi.utils.GCP.logging import Logger
-from surquest.fastapi.schemas.responses import Response
-from surquest.fastapi.utils.GCP.middleware import LoggingMiddleware
-from surquest.fastapi.utils.GCP.catcher import (
-    catch_validation_exceptions,
-    catch_http_exceptions,
-)
-
-PATH_PREFIX = os.getenv('PATH_PREFIX','')
-
-app = FastAPI(
-    title="Exchange Rates ETL",
-    openapi_url=F"{PATH_PREFIX}/openapi.json"
-)
-
-# add middleware
-app.add_middleware(LoggingMiddleware)
-
-# exception handlers
-app.add_exception_handler(HTTPException, catch_http_exceptions)
-app.add_exception_handler(RequestValidationError, catch_validation_exceptions)
-
-# custom routes to documentation and favicon
-app.add_api_route(path=F"{PATH_PREFIX}/", endpoint=Route.get_documentation, include_in_schema=False)
-app.add_api_route(path=PATH_PREFIX, endpoint=Route.get_favicon, include_in_schema=False)
-
-# custom route to illustrate logging and tracing
-@app.get(F"{PATH_PREFIX}/users")
-async def get_users(
-    age: int = Query(
-        default=18,
-        description="Minimal age of the user",
-        example=30,
-
-    ),
-):
-
-    with Tracer.start_span("Generate users"):
-
-        users = [
-            {"name": "John Doe", "age": 30, "email": "john@doe.com"},
-            {"name": "Will Smith", "age": 42, "email": "will@smith.com"}
-        ]
-
-        Logger.info('Found %s users', len(users), extra={"users": users})
-
-    with Tracer.start_span("Filtering users"):
-
-        output = []
-        excluded = []
-        Logger.debug(F"Filtering users by age > {age}")
-
-        for user in users:
-
-            if user["age"] > age:
-                output.append(user)
-            else:
-                excluded.append(user)
-
-        Logger.debug(
-            'Number of excluded users: %s', len(excluded),
-            extra={"excluded": excluded}
-        )
-
-    return Response.set(data=output)
-```
-
-The endpoint `/users` will return the following standard response:
-
-```json
-{
-  "info": {
-    "status": "success"
-  },
-  "data": [
-    {
-      "name": "John Doe",
-      "age": 30,
-      "email": "john@doe.com"
-    },
-    {
-      "name": "Will Smith",
-      "age": 42,
-      "email": "will@smith.com"
-    }
-  ]
-}
-```
-
-and the logs will are available in Google Cloud Platform console within Stackdriver Logging:
-
-![Log Entries](https://github.com/surquest/python-fastapi-utils/blob/main/assets/img/logs.png?raw=true)
-
-as well as the traces are available in Google Cloud Platform console within Stackdriver Trace:
-
-![Trace](https://github.com/surquest/python-fastapi-utils/blob/main/assets/img/trace.png?raw=true)
-
-
-# Local development
-
-You are more than welcome to contribute to this project. To make your start easier we have prepared a docker image with all the necessary tools to run it as interpreter for Pycharm or to run tests.
-
-
-## Build docker image
-```
-docker build `
-     --tag surquest/fastapi/utils `
-     --file package.base.dockerfile `
-     --target test .
-```
-
-## Run tests
-```
-docker run --rm -it `
- -v "${pwd}:/opt/project" `
- -e "GOOGLE_APPLICATION_CREDENTIALS=/opt/project/credentials/keyfile.json" `
- -w "/opt/project/test" `
- surquest/fastapi/utils pytest
-```
+![GitHub](https://img.shields.io/github/license/surquest/python-fastapi-utils?style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/surquest-fastapi-utils?style=flat-square)
+![PyPI](https://img.shields.io/pypi/v/surquest-fastapi-utils)
+
+# Introduction
+
+This project provides collection of utilities for smooth integration of FastAPI framework with Google Cloud Platform services as logging and tracing.
+
+The key features of this project are:
+
+* Logging to Cloud Logging
+* Tracing to Cloud Logging
+* Error Reporting via Cloud Logging
+* Custom middleware for configuration of logging
+* Custom exception handlers treating HTTP and validation exceptions
+* Custom routes for documentation and favicon
+* Custom responses with statuses `success`, `warning` and `error` and standardized error messages
+
+# Quick Start
+
+This section shows how to use the utilities provided by this project:
+
+```python
+"""File main.py with FastAPI app"""
+import os
+from fastapi.exceptions import RequestValidationError
+from starlette.exceptions import HTTPException
+from fastapi import FastAPI, Request, Query
+
+# import surquest modules and objects
+from surquest.fastapi.utils.route import Route  # custom routes for documentation and FavIcon
+from surquest.fastapi.utils.GCP.tracer import Tracer
+from surquest.fastapi.utils.GCP.logging import Logger
+from surquest.fastapi.schemas.responses import Response
+from surquest.fastapi.utils.GCP.middleware import LoggingMiddleware
+from surquest.fastapi.utils.GCP.catcher import (
+    catch_validation_exceptions,
+    catch_http_exceptions,
+)
+
+PATH_PREFIX = os.getenv('PATH_PREFIX','')
+
+app = FastAPI(
+    title="Exchange Rates ETL",
+    openapi_url=F"{PATH_PREFIX}/openapi.json"
+)
+
+# add middleware
+app.add_middleware(LoggingMiddleware)
+
+# exception handlers
+app.add_exception_handler(HTTPException, catch_http_exceptions)
+app.add_exception_handler(RequestValidationError, catch_validation_exceptions)
+
+# custom routes to documentation and favicon
+app.add_api_route(path=F"{PATH_PREFIX}/", endpoint=Route.get_documentation, include_in_schema=False)
+app.add_api_route(path=PATH_PREFIX, endpoint=Route.get_favicon, include_in_schema=False)
+
+# custom route to illustrate logging and tracing
+@app.get(F"{PATH_PREFIX}/users")
+async def get_users(
+    age: int = Query(
+        default=18,
+        description="Minimal age of the user",
+        example=30,
+
+    ),
+):
+
+    with Tracer.start_span("Generate users"):
+
+        users = [
+            {"name": "John Doe", "age": 30, "email": "john@doe.com"},
+            {"name": "Will Smith", "age": 42, "email": "will@smith.com"}
+        ]
+
+        Logger.info('Found %s users', len(users), extra={"users": users})
+
+    with Tracer.start_span("Filtering users"):
+
+        output = []
+        excluded = []
+        Logger.debug(F"Filtering users by age > {age}")
+
+        for user in users:
+
+            if user["age"] > age:
+                output.append(user)
+            else:
+                excluded.append(user)
+
+        Logger.debug(
+            'Number of excluded users: %s', len(excluded),
+            extra={"excluded": excluded}
+        )
+
+    return Response.set(data=output)
+```
+
+The endpoint `/users` will return the following standard response:
+
+```json
+{
+  "info": {
+    "status": "success"
+  },
+  "data": [
+    {
+      "name": "John Doe",
+      "age": 30,
+      "email": "john@doe.com"
+    },
+    {
+      "name": "Will Smith",
+      "age": 42,
+      "email": "will@smith.com"
+    }
+  ]
+}
+```
+
+and the logs will are available in Google Cloud Platform console within Stackdriver Logging:
+
+![Log Entries](https://github.com/surquest/python-fastapi-utils/blob/main/assets/img/logs.png?raw=true)
+
+as well as the traces are available in Google Cloud Platform console within Stackdriver Trace:
+
+![Trace](https://github.com/surquest/python-fastapi-utils/blob/main/assets/img/trace.png?raw=true)
+
+
+# Local development
+
+You are more than welcome to contribute to this project. To make your start easier we have prepared a docker image with all the necessary tools to run it as interpreter for Pycharm or to run tests.
+
+
+## Build docker image
+```
+docker build `
+     --tag surquest/fastapi/utils `
+     --file package.base.dockerfile `
+     --target test .
+```
+
+## Run tests
+```
+docker run --rm -it `
+ -v "${pwd}:/opt/project" `
+ -e "GOOGLE_APPLICATION_CREDENTIALS=/opt/project/credentials/keyfile.json" `
+ -w "/opt/project/test" `
+ surquest/fastapi/utils pytest
+```
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/pyproject.toml` & `surquest_fastapi_utils-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "surquest-fastapi-utils"
-version = "0.2.2.rc1"
+version = "0.2.3"
 description = "This project provides collection of utilities for FastAPI framework as: Catcher, Middleware, etc."
 authors = [
     {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
 ]
 readme = "README.md"
 dependencies = [
     "fastapi >= 0.81.0",
```

### Comparing `surquest_fastapi_utils-0.2.2rc1/PKG-INFO` & `surquest_fastapi_utils-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surquest-fastapi-utils
-Version: 0.2.2rc1
+Version: 0.2.3
 Summary: This project provides collection of utilities for FastAPI framework as: Catcher, Middleware, etc.
 Project-URL: Homepage, https://github.com/surquest/python-fastapi-utils
 Project-URL: Bug Tracker, https://github.com/surquest/python-fastapi-utils/issues
 Author-email: Michal Švarc <michal.svarc@surquest.com>
 License-File: LICENSE
 Requires-Dist: fastapi>=0.81.0
 Requires-Dist: google-cloud-logging>=3.1.0
```

