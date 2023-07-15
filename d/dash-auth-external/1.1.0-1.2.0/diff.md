# Comparing `tmp/dash-auth-external-1.1.0.tar.gz` & `tmp/dash-auth-external-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-auth-external-1.1.0.tar", last modified: Thu Jul  6 22:32:19 2023, max compression
+gzip compressed data, was "dash-auth-external-1.2.0.tar", last modified: Sat Jul 15 18:31:49 2023, max compression
```

## Comparing `dash-auth-external-1.1.0.tar` & `dash-auth-external-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/dash_auth_external/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/dash_auth_external/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/dash_auth_external.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 22:32:19.000000 dash-auth-external-1.1.0/dash_auth_external.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:19.766794 dash-auth-external-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 22:32:09.000000 dash-auth-external-1.1.0/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:31:49.574449 dash-auth-external-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-15 18:31:49.574449 dash-auth-external-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:31:49.570449 dash-auth-external-1.2.0/dash_auth_external/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/dash_auth_external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/dash_auth_external/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/dash_auth_external/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/dash_auth_external/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/dash_auth_external/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/dash_auth_external/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:31:49.570449 dash-auth-external-1.2.0/dash_auth_external.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-15 18:31:49.000000 dash-auth-external-1.2.0/dash_auth_external.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-15 18:31:49.000000 dash-auth-external-1.2.0/dash_auth_external.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:31:49.000000 dash-auth-external-1.2.0/dash_auth_external.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 18:31:49.000000 dash-auth-external-1.2.0/dash_auth_external.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 18:31:49.000000 dash-auth-external-1.2.0/dash_auth_external.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-15 18:31:49.574449 dash-auth-external-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:31:49.574449 dash-auth-external-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-15 18:31:38.000000 dash-auth-external-1.2.0/tests/test_context.py
```

### Comparing `dash-auth-external-1.1.0/LICENSE` & `dash-auth-external-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-auth-external-1.1.0/README.md` & `dash-auth-external-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: dash-auth-external
+Version: 1.2.0
+Summary: Integrate your dashboards with 3rd party APIs and external OAuth providers.
+Home-page: https://github.com/jamesholcombe/dash-auth-external
+Author-email: jholcombe@hotmail.co.uk
+Keywords: Dash,Plotly,Authentication,Auth,External
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dash-auth-external
 
 Integrate your dashboards with 3rd party APIs and external OAuth providers.
 
 ## Overview
 
 Do you want to build a Plotly Dash app which pulls user data from external APIs such as Google, Spotify, Slack etc?
@@ -12,15 +23,15 @@
 
 **Dash-auth-external** is distributed via [PyPi](https://pypi.org/project/dash-auth-external/)
 
 ```
 pip install dash-auth-external
 ```
 
-## Simple Usage
+## Usage
 
 ```python
 #using spotify as an example
 AUTH_URL = "https://accounts.spotify.com/authorize"
 TOKEN_URL = "https://accounts.spotify.com/api/token"
 CLIENT_ID = "YOUR_CLIENT_ID"
 
@@ -51,15 +62,35 @@
 @app.callback(
 Output("example-output", "children"),
 Input("example-input", "value")
 )
 def example_callback(value):
     token = auth.get_token()
      ##The token can only be retrieved in the context of a dash callback
+
+    token_data = auth.get_token_data()
+    # get_token_data can be used to access other data returned by the OAuth Provider
+    print(token)
+    print(token_data)
+
     return token
+
+```
+
+Results in something like:
+
+```bash
+>>> fakeToken123
+>>> {
+    "access_token" : "fakeToken123",
+    "user_id" : "lucifer",
+    "some_other_key" : 666,
+    "expires_at" : "judgmentDay"
+}
+
 ```
 
 ## Refresh Tokens
 
 If your OAuth provider supports refresh tokens, these are automatically checked and handled in the _get_token_ method.
 
 > Check if your OAuth provider requires any additional scopes to support refresh tokens
```

### Comparing `dash-auth-external-1.1.0/dash_auth_external/auth.py` & `dash-auth-external-1.2.0/dash_auth_external/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 from dash_auth_external.token import OAuth2Token
 from dash_auth_external.config import FLASK_SESSION_TOKEN_KEY
 from dash_auth_external.exceptions import TokenExpiredError
 
 from flask import session
 
 
+def generate_secret_key(length: int = 24) -> str:
+    """Generates a secret key for flask app.
+
+    Returns:
+        bytes: Random bytes of the desired length.
+    """
+    return os.urandom(length)
+
+
 def _get_token_data_from_session() -> dict:
     """Gets the token data from the session.
 
     Returns:
         dict: The token data from the session.
     """
     token_data = session.get(FLASK_SESSION_TOKEN_KEY)
@@ -23,64 +32,29 @@
 
 
 def _set_token_data_in_session(token: OAuth2Token):
     session[FLASK_SESSION_TOKEN_KEY] = token
 
 
 class DashAuthExternal:
-    @staticmethod
-    def generate_secret_key(length: int = 24) -> str:
-        """Generates a secret key for flask app.
-
-        Returns:
-            bytes: Random bytes of the desired length.
-        """
-        return os.urandom(length)
-
-    def get_token(self) -> str:
-        """Attempts to get a valid access token.
-
-        Returns:
-            str: Bearer Access token from your OAuth2 Provider
-        """
-        token_data = _get_token_data_from_session()
-
-        token = OAuth2Token(**token_data)
-
-        if not token.is_expired():
-            return token.access_token
-
-        if not token.refresh_token:
-            raise TokenExpiredError(
-                "Token is expired and no refresh token available to refresh token."
-            )
-
-        token_data = refresh_token(
-            self.external_token_url, token_data, self.token_request_headers
-        )
-        _set_token_data_in_session(token_data)
-        return token_data.access_token
-
     def __init__(
         self,
         external_auth_url: str,
         external_token_url: str,
         client_id: str,
         client_secret: str = None,
         with_pkce=True,
         app_url: str = "http://127.0.0.1:8050",
         redirect_suffix: str = "/redirect",
         auth_suffix: str = "/",
         home_suffix="/home",
         _flask_server: Flask = None,
-        _token_field_name: str = "access_token",
         _secret_key: str = None,
         auth_request_headers: dict = None,
         token_request_headers: dict = None,
-        token_body_params: dict = None,
         scope: str = None,
         _server_name: str = __name__,
     ):
         """The interface for obtaining access tokens from 3rd party OAuth2 Providers.
 
         Args:
             external_auth_url (str): The authorization endpoint for the OAuth2 Provider.
@@ -91,15 +65,14 @@
             redirect_suffix (str, optional): The route that OAuth2 provider will redirect back to. Defaults to "/redirect".
             auth_suffix (str, optional): The route that will trigger the initial redirect to the external OAuth provider. Defaults to "/".
             home_suffix (str, optional): The route your dash application will sit, relative to your url. Defaults to "/home".
             _flask_server (Flask, optional): Flask server to use if additional config required. Defaults to None.
             _secret_key (str, optional): Secret key for flask app, normally generated at runtime. Defaults to None.
             auth_request_headers (dict, optional): Additional headers to send to the authorization endpoint. Defaults to None.
             token_request_headers (dict, optional): Additional headers to send to the access token endpoint. Defaults to None.
-            token_body_params (dict, optional): Additional body params to send to the access token endpoint. Defaults to None.
             scope (str, optional): Header required by most Oauth2 Providers. Defaults to None.
             _server_name (str, optional): The name of the Flask Server. Defaults to __name__, ignored if _flask_server is not None.
 
 
         Returns:
            DashAuthExternal: Main package class
         """
@@ -113,15 +86,15 @@
             app = Flask(
                 _server_name, instance_relative_config=False, static_folder="./assets"
             )
         else:
             app = _flask_server
 
         if _secret_key is None:
-            app.secret_key = self.generate_secret_key()
+            app.secret_key = generate_secret_key()
         else:
             app.secret_key = _secret_key
 
         redirect_uri = urljoin(app_url, redirect_suffix)
 
         app = make_auth_route(
             app=app,
@@ -145,31 +118,61 @@
             with_pkce=with_pkce,
         )
 
         self.server = app
         self.home_suffix = home_suffix
         self.redirect_suffix = redirect_suffix
         self.auth_suffix = auth_suffix
-        self._token_field_name = _token_field_name
         self.client_id = client_id
         self.external_token_url = external_token_url
         self.token_request_headers = token_request_headers
         self.scope = scope
 
+    def get_token_data(self) -> OAuth2Token:
+        """Attempts to get a valid access token.
+
+        Returns:
+            OAuth2Token: The token data.
+        """
+        token_data = _get_token_data_from_session()
+
+        token = OAuth2Token(**token_data)
+
+        if not token.is_expired():
+            return token
+
+        if not token.refresh_token:
+            raise TokenExpiredError(
+                "Token is expired and no refresh token available to refresh token."
+            )
+
+        token_data = refresh_token(
+            self.external_token_url, token_data, self.token_request_headers
+        )
+        _set_token_data_in_session(token_data)
+        return token_data
+
+    def get_token(self) -> str:
+        """Attempts to get a valid access token.
+
+        Returns:
+            str: The access token.
+        """
+        return self.get_token_data().access_token
+
 
 def refresh_token(url: str, token_data: OAuth2Token, headers: dict) -> OAuth2Token:
     body = {
         "grant_type": "refresh_token",
         "refresh_token": token_data.refresh_token,
     }
     data = token_request(url, body, headers)
 
-    token_data.access_token = data["access_token"]
+    new_token = OAuth2Token(
+        access_token=data["access_token"],
+        token_type=data.get("token_type"),
+        expires_in=data.get("expires_in"),
+        refresh_token=data.get("refresh_token"),
+        token_data=data,
+    )
 
-    # If the provider does not return a new refresh token, use the old one.
-    if "refresh_token" in data:
-        token_data.refresh_token = data["refresh_token"]
-
-    if "expires_in" in data:
-        token_data.expires_in = data["expires_in"]
-
-    return token_data
+    return new_token
```

### Comparing `dash-auth-external-1.1.0/dash_auth_external/routes.py` & `dash-auth-external-1.2.0/dash_auth_external/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,21 +113,28 @@
         )
 
         response_data = token_request(
             url=external_token_url,
             body=body,
             headers=token_request_headers,
         )
+        token = OAuth2Token(
+            access_token=response_data.get("access_token"),
+            token_type=response_data.get("token_type"),
+            expires_in=response_data.get("expires_in"),
+            refresh_token=response_data.get("refresh_token"),
+            token_data=response_data,
+        )
 
         response = redirect(_home_suffix)
 
-        session[FLASK_SESSION_TOKEN_KEY] = asdict(OAuth2Token(**response_data))
+        session[FLASK_SESSION_TOKEN_KEY] = asdict(token)
 
         return response
 
     return app
 
 
-def token_request(url: str, body: dict, headers: dict):
+def token_request(url: str, body: dict, headers: dict) -> dict:
     r = requests.post(url, data=body, headers=headers)
     r.raise_for_status()
     return r.json()
```

### Comparing `dash-auth-external-1.1.0/dash_auth_external.egg-info/SOURCES.txt` & `dash-auth-external-1.2.0/dash_auth_external.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-auth-external-1.1.0/setup.py` & `dash-auth-external-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 
 NAME = "dash-auth-external"
 
 this_directory = Path(__file__).parent
-long_description = (
+description = (
     "Integrate your dashboards with 3rd party APIs and external OAuth providers."
 )
+
+with open(this_directory / "README.md", encoding="utf-8") as f:
+    long_description = f.read()
+
+
+
 requires = ["dash >= 2.0.0", "requests >= 1.0.0", "requests-oauthlib >= 0.3.0"]
 
 setup(
     name=NAME,
-    version="1.1.0",
-    description=long_description,
+    version="1.2.0",
+    description=description,
     python_requires=">=3.7",
     author_email="jholcombe@hotmail.co.uk",
     url="https://github.com/jamesholcombe/dash-auth-external",
     keywords=["Dash", "Plotly", "Authentication", "Auth", "External"],
     install_requires=requires,
     packages=find_packages(),
     include_package_data=True,
     long_description=long_description,
+    long_description_content_type='text/markdown'
 )
```

### Comparing `dash-auth-external-1.1.0/tests/test_app.py` & `dash-auth-external-1.2.0/tests/test_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     token_request_mock = mocker.patch(
         "dash_auth_external.routes.token_request",
         return_value={
             "access_token": "access_token",
             "refresh_token": "refresh_token",
             "token_type": "Bearer",
             "expires_in": "3599",
+            "arbitrary_key": "some_data",
         },
     )
     expected_token_request_body = {
         "grant_type": "authorization_code",
         "code": "code",
         "redirect_uri": redirect_uri,
         "client_id": CLIENT_ID,
@@ -89,7 +90,8 @@
         assert response.status_code == 302
         with client.session_transaction() as session:
             token_data = session[FLASK_SESSION_TOKEN_KEY]
             assert token_data["access_token"] == "access_token"
             assert token_data["refresh_token"] == "refresh_token"
             assert token_data["token_type"] == "Bearer"
             assert token_data["expires_in"] == "3599"
+            assert token_data["token_data"]["arbitrary_key"] == "some_data"
```

### Comparing `dash-auth-external-1.1.0/tests/test_auth.py` & `dash-auth-external-1.2.0/tests/test_auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,34 @@
 @pytest.fixture()
 def access_token_data_with_refresh():
     return {
         "access_token": "access_token",
         "refresh_token": "refresh_token",
         "token_type": "Bearer",
         "expires_in": 3599,
+        "token_data": {
+            "access_token": "access_token",
+            "refresh_token": "refresh_token",
+            "token_type": "Bearer",
+            "expires_in": 3599,
+        },
     }
 
 
 @pytest.fixture()
 def expired_access_token_data_without_refresh():
     return {
         "access_token": "access_token",
         "token_type": "Bearer",
         "expires_in": -1,
+        "token_data": {
+            "access_token": "access_token",
+            "token_type": "Bearer",
+            "expires_in": -1,
+        },
     }
 
 
 @pytest.fixture()
 def expired_access_token_data_with_refresh(expired_access_token_data_without_refresh):
     return {
         **expired_access_token_data_without_refresh,
@@ -110,7 +121,25 @@
     @dash_app.callback(Output("test-output", "children"), Input("test-input", "value"))
     def test_callback(value):
         token = auth.get_token()
         return token
 
     with pytest.raises(TokenExpiredError):
         test_callback("test")
+
+
+def test_get_token_data_ok(dash_app_and_auth, mocker, access_token_data_with_refresh):
+    dash_app, auth = dash_app_and_auth
+    token = OAuth2Token(
+        **access_token_data_with_refresh,
+    )
+
+    mocker.patch(
+        "dash_auth_external.auth._get_token_data_from_session",
+        return_value=access_token_data_with_refresh,
+    )
+
+    token_compare = auth.get_token_data()
+    assert isinstance(token_compare.expires_at, float)
+    token_compare.expires_at = None
+    token.expires_at = None
+    assert token_compare == token
```

