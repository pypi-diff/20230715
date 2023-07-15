# Comparing `tmp/fastapi_authtools-0.2.tar.gz` & `tmp/fastapi_authtools-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_authtools-0.2.tar", last modified: Fri Jul 14 18:42:08 2023, max compression
+gzip compressed data, was "fastapi_authtools-0.3.tar", last modified: Sat Jul 15 09:33:23 2023, max compression
```

## Comparing `fastapi_authtools-0.2.tar` & `fastapi_authtools-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-14 18:42:08.438499 fastapi_authtools-0.2/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1073 2023-07-13 17:55:37.000000 fastapi_authtools-0.2/LICENSE
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2262 2023-07-14 18:42:08.434499 fastapi_authtools-0.2/PKG-INFO
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1597 2023-07-14 17:51:40.000000 fastapi_authtools-0.2/README.md
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-14 18:42:08.434499 fastapi_authtools-0.2/fastapi_authtools/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2660 2023-07-14 18:25:23.000000 fastapi_authtools-0.2/fastapi_authtools/__init__.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1765 2023-07-14 18:12:34.000000 fastapi_authtools-0.2/fastapi_authtools/backend.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      500 2023-07-14 05:43:40.000000 fastapi_authtools-0.2/fastapi_authtools/exceptions.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      966 2023-07-14 18:25:23.000000 fastapi_authtools-0.2/fastapi_authtools/middleware.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      681 2023-07-14 05:43:40.000000 fastapi_authtools-0.2/fastapi_authtools/models.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1000 2023-07-13 17:55:37.000000 fastapi_authtools-0.2/fastapi_authtools/token.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      988 2023-07-13 17:55:37.000000 fastapi_authtools-0.2/fastapi_authtools/user.py
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-14 18:42:08.434499 fastapi_authtools-0.2/fastapi_authtools.egg-info/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2262 2023-07-14 18:42:08.000000 fastapi_authtools-0.2/fastapi_authtools.egg-info/PKG-INFO
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      489 2023-07-14 18:42:08.000000 fastapi_authtools-0.2/fastapi_authtools.egg-info/SOURCES.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-14 18:42:08.000000 fastapi_authtools-0.2/fastapi_authtools.egg-info/dependency_links.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-14 18:42:08.000000 fastapi_authtools-0.2/fastapi_authtools.egg-info/not-zip-safe
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       20 2023-07-14 18:42:08.000000 fastapi_authtools-0.2/fastapi_authtools.egg-info/requires.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       18 2023-07-14 18:42:08.000000 fastapi_authtools-0.2/fastapi_authtools.egg-info/top_level.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      631 2023-07-14 18:41:22.000000 fastapi_authtools-0.2/pyproject.toml
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       38 2023-07-14 18:42:08.438499 fastapi_authtools-0.2/setup.cfg
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      515 2023-07-14 18:36:48.000000 fastapi_authtools-0.2/setup.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1073 2023-07-13 17:55:37.000000 fastapi_authtools-0.3/LICENSE
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2262 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/PKG-INFO
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1597 2023-07-14 17:51:40.000000 fastapi_authtools-0.3/README.md
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-15 09:33:23.480769 fastapi_authtools-0.3/fastapi_authtools/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2660 2023-07-14 18:25:23.000000 fastapi_authtools-0.3/fastapi_authtools/__init__.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1759 2023-07-15 09:32:31.000000 fastapi_authtools-0.3/fastapi_authtools/backend.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      500 2023-07-14 05:43:40.000000 fastapi_authtools-0.3/fastapi_authtools/exceptions.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      966 2023-07-14 18:25:23.000000 fastapi_authtools-0.3/fastapi_authtools/middleware.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      681 2023-07-14 05:43:40.000000 fastapi_authtools-0.3/fastapi_authtools/models.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      994 2023-07-15 09:32:31.000000 fastapi_authtools-0.3/fastapi_authtools/token.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      988 2023-07-13 17:55:37.000000 fastapi_authtools-0.3/fastapi_authtools/user.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/fastapi_authtools.egg-info/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2262 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/PKG-INFO
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      489 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/not-zip-safe
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       20 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/requires.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       18 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/top_level.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      631 2023-07-15 09:33:10.000000 fastapi_authtools-0.3/pyproject.toml
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       38 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/setup.cfg
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      515 2023-07-15 09:33:10.000000 fastapi_authtools-0.3/setup.py
```

### Comparing `fastapi_authtools-0.2/LICENSE` & `fastapi_authtools-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.2/PKG-INFO` & `fastapi_authtools-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_authtools
-Version: 0.2
+Version: 0.3
 Summary: A small example package
 Home-page: https://github.com/michael7nightinglae/fastapi_authtools
 Author: Michael Nightingale
 Author-email: Michael Nightingale <suslanchikmopl@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/michael7nightinglae/fastapi_authtools
 Project-URL: Bug Tracker, https://github.com/michael7nightinglae/fastapi_authtools/issues
```

### Comparing `fastapi_authtools-0.2/README.md` & `fastapi_authtools-0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.2/fastapi_authtools/__init__.py` & `fastapi_authtools-0.3/fastapi_authtools/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.2/fastapi_authtools/backend.py` & `fastapi_authtools-0.3/fastapi_authtools/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             token=token,
             secret_key=self.jwt_config.secret_key,
             algorithm=self.jwt_config.algorithm
         )
         if user_data is None:
             return scopes, None
 
-        user = FastAPIUser(**user_data.model_dump()) if isinstance(user_data, BaseModel) else FastAPIUser(**user_data)
+        user = FastAPIUser(**user_data.dict()) if isinstance(user_data, BaseModel) else FastAPIUser(**user_data)
         return scopes, user
 
     async def authenticate(
         self, conn: HTTPConnection
     ) -> typing.Optional[typing.Tuple[authentication.AuthCredentials, authentication.BaseUser | None]]:
         if conn.url.path in self.excluded_urls:
             return authentication.AuthCredentials([]), None
```

### Comparing `fastapi_authtools-0.2/fastapi_authtools/middleware.py` & `fastapi_authtools-0.3/fastapi_authtools/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.2/fastapi_authtools/models.py` & `fastapi_authtools-0.3/fastapi_authtools/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.2/fastapi_authtools/token.py` & `fastapi_authtools-0.3/fastapi_authtools/token.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def encode_jwt_token(
         user_data: dict | BaseModel,
         secret_key: str,
         algorithm: str,
         expire_minutes: int
 ) -> str:
     if isinstance(user_data, BaseModel):
-        user_data = user_data.model_dump()
+        user_data = user_data.dict()
     user_data.update(exp=datetime.now() + timedelta(minutes=expire_minutes))
     token = jwt.encode(
         user_data,
         key=secret_key,
         algorithm=algorithm
     )
     return token
```

### Comparing `fastapi_authtools-0.2/fastapi_authtools/user.py` & `fastapi_authtools-0.3/fastapi_authtools/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.2/fastapi_authtools.egg-info/PKG-INFO` & `fastapi_authtools-0.3/fastapi_authtools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-authtools
-Version: 0.2
+Version: 0.3
 Summary: A small example package
 Home-page: https://github.com/michael7nightinglae/fastapi_authtools
 Author: Michael Nightingale
 Author-email: Michael Nightingale <suslanchikmopl@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/michael7nightinglae/fastapi_authtools
 Project-URL: Bug Tracker, https://github.com/michael7nightinglae/fastapi_authtools/issues
```

### Comparing `fastapi_authtools-0.2/pyproject.toml` & `fastapi_authtools-0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fastapi_authtools"
-version = "0.2"
+version = "0.3"
 authors = [
   { name="Michael Nightingale", email="suslanchikmopl@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_authtools-0.2/setup.py` & `fastapi_authtools-0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fastapi_authtools',
-    version='0.2',
+    version='0.3',
     url='https://github.com/michael7nightinglae/fastapi_authtools',
     install_requires=[
         "fastapi", "python-jose"
     ],
     license='MIT',
     author='Michael Nightingale',
     author_email='suslanchikmopl@gmail.com',
```

