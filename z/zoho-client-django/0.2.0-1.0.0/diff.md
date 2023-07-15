# Comparing `tmp/zoho-client-django-0.2.0.tar.gz` & `tmp/zoho-client-django-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho-client-django-0.2.0.tar", last modified: Sat Jul 15 09:39:05 2023, max compression
+gzip compressed data, was "zoho-client-django-1.0.0.tar", last modified: Sat Jul 15 15:25:51 2023, max compression
```

## Comparing `zoho-client-django-0.2.0.tar` & `zoho-client-django-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 09:39:05.732669 zoho-client-django-0.2.0/
--rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-0.2.0/LICENSE
--rw-r--r--   0 guy        (501) staff       (20)     1513 2023-07-15 09:39:05.732531 zoho-client-django-0.2.0/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)     1177 2023-07-14 23:53:42.000000 zoho-client-django-0.2.0/README.md
--rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-15 09:39:05.732708 zoho-client-django-0.2.0/setup.cfg
--rw-r--r--   0 guy        (501) staff       (20)      768 2023-07-15 09:35:52.000000 zoho-client-django-0.2.0/setup.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 09:39:05.730038 zoho-client-django-0.2.0/zoho_client/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-0.2.0/zoho_client/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      205 2023-07-14 12:53:50.000000 zoho-client-django-0.2.0/zoho_client/admin.py
--rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-0.2.0/zoho_client/apps.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 09:39:05.730741 zoho-client-django-0.2.0/zoho_client/migrations/
--rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-0.2.0/zoho_client/migrations/0001_initial.py
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-0.2.0/zoho_client/migrations/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-0.2.0/zoho_client/models.py
--rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-0.2.0/zoho_client/tests.py
--rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-0.2.0/zoho_client/views.py
--rw-r--r--   0 guy        (501) staff       (20)     2998 2023-07-14 22:11:49.000000 zoho-client-django-0.2.0/zoho_client/zoho.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 09:39:05.731382 zoho-client-django-0.2.0/zoho_client_django.egg-info/
--rw-r--r--   0 guy        (501) staff       (20)     1513 2023-07-15 09:39:05.000000 zoho-client-django-0.2.0/zoho_client_django.egg-info/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)      596 2023-07-15 09:39:05.000000 zoho-client-django-0.2.0/zoho_client_django.egg-info/SOURCES.txt
--rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-15 09:39:05.000000 zoho-client-django-0.2.0/zoho_client_django.egg-info/dependency_links.txt
--rw-r--r--   0 guy        (501) staff       (20)       41 2023-07-15 09:39:05.000000 zoho-client-django-0.2.0/zoho_client_django.egg-info/requires.txt
--rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-15 09:39:05.000000 zoho-client-django-0.2.0/zoho_client_django.egg-info/top_level.txt
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 09:39:05.732208 zoho-client-django-0.2.0/zoho_test_project/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-0.2.0/zoho_test_project/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-0.2.0/zoho_test_project/asgi.py
--rw-r--r--   0 guy        (501) staff       (20)     3576 2023-07-14 21:39:09.000000 zoho-client-django-0.2.0/zoho_test_project/settings.py
--rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-0.2.0/zoho_test_project/urls.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-0.2.0/zoho_test_project/wsgi.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.325658 zoho-client-django-1.0.0/
+-rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-1.0.0/LICENSE
+-rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-15 15:25:51.325521 zoho-client-django-1.0.0/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)     2234 2023-07-15 15:22:00.000000 zoho-client-django-1.0.0/README.md
+-rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-15 15:25:51.325697 zoho-client-django-1.0.0/setup.cfg
+-rw-r--r--   0 guy        (501) staff       (20)      768 2023-07-15 15:25:06.000000 zoho-client-django-1.0.0/setup.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.322791 zoho-client-django-1.0.0/zoho_client/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)     1445 2023-07-15 13:55:44.000000 zoho-client-django-1.0.0/zoho_client/admin.py
+-rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-1.0.0/zoho_client/apps.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.323560 zoho-client-django-1.0.0/zoho_client/migrations/
+-rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-1.0.0/zoho_client/migrations/0001_initial.py
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/migrations/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-1.0.0/zoho_client/models.py
+-rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/tests.py
+-rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/views.py
+-rw-r--r--   0 guy        (501) staff       (20)     2998 2023-07-14 22:11:49.000000 zoho-client-django-1.0.0/zoho_client/zoho.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.324264 zoho-client-django-1.0.0/zoho_client_django.egg-info/
+-rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)      596 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/SOURCES.txt
+-rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/dependency_links.txt
+-rw-r--r--   0 guy        (501) staff       (20)       41 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/requires.txt
+-rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/top_level.txt
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.325184 zoho-client-django-1.0.0/zoho_test_project/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-1.0.0/zoho_test_project/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.0.0/zoho_test_project/asgi.py
+-rw-r--r--   0 guy        (501) staff       (20)     3639 2023-07-15 10:11:01.000000 zoho-client-django-1.0.0/zoho_test_project/settings.py
+-rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-1.0.0/zoho_test_project/urls.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.0.0/zoho_test_project/wsgi.py
```

### Comparing `zoho-client-django-0.2.0/LICENSE` & `zoho-client-django-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoho-client-django-0.2.0/PKG-INFO` & `zoho-client-django-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 0.2.0
+Version: 1.0.0
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # zoho-client-django
 
 A modest Zoho CRM API client which will do the oAuth2 for you.
 
+## Usage
+
 ```python
  from zoho_client.zoho import ZohoClient
  client = ZohoClient()
  # GET all Sales_Orders
  res = client.make_request(api_endpoint="Sales_Orders")
  for sales_order in res['data']:
     print(f"sales order #{sales_order['id']}")
@@ -29,25 +31,74 @@
  payload = {'data': [ {'Subject': 'CHNAGED'}]}
  res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", data=payload)
  print(res['data'][0]['status'])
  # => success
 
 ```
 
-# setup
+# Setup
+
+## ENV
+
+the package expects to have it's configuration in the settings.py:
+
+```python
+# read it from .env
+ZOHO_CLIENT_ID = env("ZOHO_CLIENT_ID")
+ZOHO_CLIENT_SECRET = env("ZOHO_CLIENT_SECRET")
+ZOHO_API_VERSION = "v2.1"
+# sandbox
+ZOHO_BASE_URL = "https://crmsandbox.zoho.com"
+# production
+# ZOHO_BASE_URL = "https://zohoapis.com"
+```
+
+and naturally, don't forget to include the app in your INSALLED_APS:
+
+```python
+INSTALLED_APPS = [
+    ...
+    "zoho_client",
+]
+
+```
+
+## Initilization of the client (one off)
 
-generate the refresh token
+goto https://api-console.zoho.com/ :
 
-fetch the auth code:
+copy the client id and secret and save them in your django settings. the recommended way would be to save them as ENV variables.
+
+![step 1](images/01_zoho.png)
+
+generate an authorization code
 
 scope:
 ZohoCRM.modules.ALL,ZohoCRM.settings.ALL,ZohoCRM.users.ALL,ZohoCRM.bulk.ALL,ZohoCRM.notifications.ALL
 
+![step 2](images/02_zoho.png)
+
 choose either production or sandbox
+
+![step 3](images/03_zoho.png)
+
 press generate and copy the code and run this from the django console:
+![step 4](images/04_zoho.png)
+
+go to django admin to zoho_client/zoho_token and press the regenerate zoho oauth tokens
+
+![step 5](images/06_django_admin.png)
+
+paste the authorization code you have copied before
+
+![step 6](images/05_django_admin.png)
+
+you are good to go!
+
+### Programmatically:
 
 ```python
 from zoho_client.zoho import ZohoClient
 # the code you have just copied
 code = "1000.12c557408797e20c8432216dca0bbb5f.f1896d4f9e2329136806637798859a99"
 ZohoClient().fetch_tokens(code)
 # -> '1000.03b32b6490d8573e242664710bbc4f2c.e009198b6ab4b89013485657409e4913'
```

### Comparing `zoho-client-django-0.2.0/setup.py` & `zoho-client-django-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="zoho-client-django",
-    version="0.2.0",  # Update this for new versions
+    version="1.0.0",  # Update this for new versions
     description="Django app which is a client for the Zoho CRM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Guy Moller",
     author_email="guy.moller@gmail.com",
     url="https://github.com/gosourcellc/zoho-client-django",
     packages=find_packages(),
```

### Comparing `zoho-client-django-0.2.0/zoho_client/migrations/0001_initial.py` & `zoho-client-django-1.0.0/zoho_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-0.2.0/zoho_client/zoho.py` & `zoho-client-django-1.0.0/zoho_client/zoho.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-0.2.0/zoho_client_django.egg-info/PKG-INFO` & `zoho-client-django-1.0.0/zoho_client_django.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 0.2.0
+Version: 1.0.0
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # zoho-client-django
 
 A modest Zoho CRM API client which will do the oAuth2 for you.
 
+## Usage
+
 ```python
  from zoho_client.zoho import ZohoClient
  client = ZohoClient()
  # GET all Sales_Orders
  res = client.make_request(api_endpoint="Sales_Orders")
  for sales_order in res['data']:
     print(f"sales order #{sales_order['id']}")
@@ -29,25 +31,74 @@
  payload = {'data': [ {'Subject': 'CHNAGED'}]}
  res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", data=payload)
  print(res['data'][0]['status'])
  # => success
 
 ```
 
-# setup
+# Setup
+
+## ENV
+
+the package expects to have it's configuration in the settings.py:
+
+```python
+# read it from .env
+ZOHO_CLIENT_ID = env("ZOHO_CLIENT_ID")
+ZOHO_CLIENT_SECRET = env("ZOHO_CLIENT_SECRET")
+ZOHO_API_VERSION = "v2.1"
+# sandbox
+ZOHO_BASE_URL = "https://crmsandbox.zoho.com"
+# production
+# ZOHO_BASE_URL = "https://zohoapis.com"
+```
+
+and naturally, don't forget to include the app in your INSALLED_APS:
+
+```python
+INSTALLED_APPS = [
+    ...
+    "zoho_client",
+]
+
+```
+
+## Initilization of the client (one off)
 
-generate the refresh token
+goto https://api-console.zoho.com/ :
 
-fetch the auth code:
+copy the client id and secret and save them in your django settings. the recommended way would be to save them as ENV variables.
+
+![step 1](images/01_zoho.png)
+
+generate an authorization code
 
 scope:
 ZohoCRM.modules.ALL,ZohoCRM.settings.ALL,ZohoCRM.users.ALL,ZohoCRM.bulk.ALL,ZohoCRM.notifications.ALL
 
+![step 2](images/02_zoho.png)
+
 choose either production or sandbox
+
+![step 3](images/03_zoho.png)
+
 press generate and copy the code and run this from the django console:
+![step 4](images/04_zoho.png)
+
+go to django admin to zoho_client/zoho_token and press the regenerate zoho oauth tokens
+
+![step 5](images/06_django_admin.png)
+
+paste the authorization code you have copied before
+
+![step 6](images/05_django_admin.png)
+
+you are good to go!
+
+### Programmatically:
 
 ```python
 from zoho_client.zoho import ZohoClient
 # the code you have just copied
 code = "1000.12c557408797e20c8432216dca0bbb5f.f1896d4f9e2329136806637798859a99"
 ZohoClient().fetch_tokens(code)
 # -> '1000.03b32b6490d8573e242664710bbc4f2c.e009198b6ab4b89013485657409e4913'
```

### Comparing `zoho-client-django-0.2.0/zoho_client_django.egg-info/SOURCES.txt` & `zoho-client-django-1.0.0/zoho_client_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zoho-client-django-0.2.0/zoho_test_project/settings.py` & `zoho-client-django-1.0.0/zoho_test_project/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,22 @@
 https://docs.djangoproject.com/en/4.1/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/4.1/ref/settings/
 """
 
 from pathlib import Path
+import environ
+import os
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
+env = environ.Env()
+environ.Env.read_env(os.path.join(BASE_DIR, ".env"))
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "django-insecure--@qx33)h1c34f0zc5$ll!rmbv-wbh^rhtd=7(g-6kkoqzf9l6-"
 
@@ -121,14 +125,14 @@
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/4.1/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 
 # read it from .env
-ZOHO_CLIENT_ID = "1000.JL56S7MEKTKJU3XWR1JZ9JA8B36TGA"
-ZOHO_CLIENT_SECRET = "59cb4f7b4ba0b71bce194adb279c76fdbb68ff91bc"
+ZOHO_CLIENT_ID = env("ZOHO_CLIENT_ID")
+ZOHO_CLIENT_SECRET = env("ZOHO_CLIENT_SECRET")
 ZOHO_API_VERSION = "v2.1"
 # sandbox
 ZOHO_BASE_URL = "https://crmsandbox.zoho.com"
 # production
 # ZOHO_BASE_URL = "https://zohoapis.com"
```

### Comparing `zoho-client-django-0.2.0/zoho_test_project/urls.py` & `zoho-client-django-1.0.0/zoho_test_project/urls.py`

 * *Files identical despite different names*

