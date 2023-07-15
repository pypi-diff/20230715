# Comparing `tmp/pydomotic-1.1.0.tar.gz` & `tmp/pydomotic-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydomotic-1.1.0.tar", last modified: Wed Jul 12 00:40:09 2023, max compression
+gzip compressed data, was "pydomotic-1.2.0.tar", last modified: Sat Jul 15 05:51:56 2023, max compression
```

## Comparing `pydomotic-1.1.0.tar` & `pydomotic-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.341011 pydomotic-1.1.0/
--rw-r--r--   0 rabo       (501) staff       (20)     3877 2023-07-12 00:40:09.340868 pydomotic-1.1.0/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)     2770 2023-07-12 00:34:08.000000 pydomotic-1.1.0/README.md
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.338296 pydomotic-1.1.0/pydomotic/
--rw-r--r--   0 rabo       (501) staff       (20)      388 2023-07-05 03:41:17.000000 pydomotic-1.1.0/pydomotic/__init__.py
--rw-r--r--   0 rabo       (501) staff       (20)      113 2023-07-04 19:56:42.000000 pydomotic-1.1.0/pydomotic/__main__.py
--rw-r--r--   0 rabo       (501) staff       (20)     1600 2023-07-08 03:14:05.000000 pydomotic-1.1.0/pydomotic/actions.py
--rw-r--r--   0 rabo       (501) staff       (20)     1268 2023-07-04 20:42:23.000000 pydomotic-1.1.0/pydomotic/components.py
--rw-r--r--   0 rabo       (501) staff       (20)     7881 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/context.py
--rw-r--r--   0 rabo       (501) staff       (20)      165 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/exceptions.py
--rw-r--r--   0 rabo       (501) staff       (20)     2385 2023-07-07 03:00:41.000000 pydomotic-1.1.0/pydomotic/handlers.py
--rw-r--r--   0 rabo       (501) staff       (20)       63 2023-07-05 03:26:18.000000 pydomotic-1.1.0/pydomotic/lambda_handler.py
--rw-r--r--   0 rabo       (501) staff       (20)    21710 2023-07-12 00:11:15.000000 pydomotic-1.1.0/pydomotic/parsers.py
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.340566 pydomotic-1.1.0/pydomotic/providers/
--rw-r--r--   0 rabo       (501) staff       (20)        0 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/__init__.py
--rw-r--r--   0 rabo       (501) staff       (20)     2635 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/airthings.py
--rw-r--r--   0 rabo       (501) staff       (20)      488 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/base.py
--rw-r--r--   0 rabo       (501) staff       (20)      958 2023-07-04 07:17:33.000000 pydomotic-1.1.0/pydomotic/providers/fujitsu.py
--rw-r--r--   0 rabo       (501) staff       (20)     1383 2023-07-08 03:38:52.000000 pydomotic-1.1.0/pydomotic/providers/moen.py
--rw-r--r--   0 rabo       (501) staff       (20)      585 2023-07-04 21:25:43.000000 pydomotic-1.1.0/pydomotic/providers/noop.py
--rw-r--r--   0 rabo       (501) staff       (20)     1040 2023-07-12 00:14:50.000000 pydomotic-1.1.0/pydomotic/providers/tuya.py
--rw-r--r--   0 rabo       (501) staff       (20)     4934 2023-07-10 04:10:04.000000 pydomotic-1.1.0/pydomotic/sensors.py
--rw-r--r--   0 rabo       (501) staff       (20)     3608 2023-07-06 00:52:26.000000 pydomotic-1.1.0/pydomotic/triggers.py
--rw-r--r--   0 rabo       (501) staff       (20)     2931 2023-07-09 23:04:01.000000 pydomotic-1.1.0/pydomotic/utils.py
--rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-12 00:40:00.000000 pydomotic-1.1.0/pydomotic/version.py
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-12 00:40:09.338973 pydomotic-1.1.0/pydomotic.egg-info/
--rw-r--r--   0 rabo       (501) staff       (20)     3877 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)      678 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/SOURCES.txt
--rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/dependency_links.txt
--rw-r--r--   0 rabo       (501) staff       (20)      393 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/requires.txt
--rw-r--r--   0 rabo       (501) staff       (20)       10 2023-07-12 00:40:09.000000 pydomotic-1.1.0/pydomotic.egg-info/top_level.txt
--rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-12 00:40:09.341057 pydomotic-1.1.0/setup.cfg
--rw-r--r--   0 rabo       (501) staff       (20)     2367 2023-07-12 00:19:04.000000 pydomotic-1.1.0/setup.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-15 05:51:56.668703 pydomotic-1.2.0/
+-rw-r--r--   0 rabo       (501) staff       (20)     3877 2023-07-15 05:51:56.668567 pydomotic-1.2.0/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)     2770 2023-07-12 00:34:08.000000 pydomotic-1.2.0/README.md
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-15 05:51:56.666394 pydomotic-1.2.0/pydomotic/
+-rw-r--r--   0 rabo       (501) staff       (20)      388 2023-07-05 03:41:17.000000 pydomotic-1.2.0/pydomotic/__init__.py
+-rw-r--r--   0 rabo       (501) staff       (20)      113 2023-07-04 19:56:42.000000 pydomotic-1.2.0/pydomotic/__main__.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1600 2023-07-08 03:14:05.000000 pydomotic-1.2.0/pydomotic/actions.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1268 2023-07-04 20:42:23.000000 pydomotic-1.2.0/pydomotic/components.py
+-rw-r--r--   0 rabo       (501) staff       (20)     7881 2023-07-04 07:17:33.000000 pydomotic-1.2.0/pydomotic/context.py
+-rw-r--r--   0 rabo       (501) staff       (20)      165 2023-07-04 07:17:33.000000 pydomotic-1.2.0/pydomotic/exceptions.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2385 2023-07-07 03:00:41.000000 pydomotic-1.2.0/pydomotic/handlers.py
+-rw-r--r--   0 rabo       (501) staff       (20)       63 2023-07-05 03:26:18.000000 pydomotic-1.2.0/pydomotic/lambda_handler.py
+-rw-r--r--   0 rabo       (501) staff       (20)    21785 2023-07-15 05:38:56.000000 pydomotic-1.2.0/pydomotic/parsers.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-15 05:51:56.668283 pydomotic-1.2.0/pydomotic/providers/
+-rw-r--r--   0 rabo       (501) staff       (20)        0 2023-07-04 07:17:33.000000 pydomotic-1.2.0/pydomotic/providers/__init__.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2806 2023-07-15 05:43:47.000000 pydomotic-1.2.0/pydomotic/providers/airthings.py
+-rw-r--r--   0 rabo       (501) staff       (20)      488 2023-07-04 07:17:33.000000 pydomotic-1.2.0/pydomotic/providers/base.py
+-rw-r--r--   0 rabo       (501) staff       (20)      958 2023-07-04 07:17:33.000000 pydomotic-1.2.0/pydomotic/providers/fujitsu.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1383 2023-07-08 03:38:52.000000 pydomotic-1.2.0/pydomotic/providers/moen.py
+-rw-r--r--   0 rabo       (501) staff       (20)      585 2023-07-04 21:25:43.000000 pydomotic-1.2.0/pydomotic/providers/noop.py
+-rw-r--r--   0 rabo       (501) staff       (20)     1040 2023-07-12 00:14:50.000000 pydomotic-1.2.0/pydomotic/providers/tuya.py
+-rw-r--r--   0 rabo       (501) staff       (20)     4934 2023-07-10 04:10:04.000000 pydomotic-1.2.0/pydomotic/sensors.py
+-rw-r--r--   0 rabo       (501) staff       (20)     3608 2023-07-06 00:52:26.000000 pydomotic-1.2.0/pydomotic/triggers.py
+-rw-r--r--   0 rabo       (501) staff       (20)     2931 2023-07-09 23:04:01.000000 pydomotic-1.2.0/pydomotic/utils.py
+-rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-15 05:51:51.000000 pydomotic-1.2.0/pydomotic/version.py
+drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-15 05:51:56.667040 pydomotic-1.2.0/pydomotic.egg-info/
+-rw-r--r--   0 rabo       (501) staff       (20)     3877 2023-07-15 05:51:56.000000 pydomotic-1.2.0/pydomotic.egg-info/PKG-INFO
+-rw-r--r--   0 rabo       (501) staff       (20)      678 2023-07-15 05:51:56.000000 pydomotic-1.2.0/pydomotic.egg-info/SOURCES.txt
+-rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-15 05:51:56.000000 pydomotic-1.2.0/pydomotic.egg-info/dependency_links.txt
+-rw-r--r--   0 rabo       (501) staff       (20)      393 2023-07-15 05:51:56.000000 pydomotic-1.2.0/pydomotic.egg-info/requires.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       10 2023-07-15 05:51:56.000000 pydomotic-1.2.0/pydomotic.egg-info/top_level.txt
+-rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-15 05:51:56.668755 pydomotic-1.2.0/setup.cfg
+-rw-r--r--   0 rabo       (501) staff       (20)     2367 2023-07-12 00:19:04.000000 pydomotic-1.2.0/setup.py
```

### Comparing `pydomotic-1.1.0/PKG-INFO` & `pydomotic-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydomotic
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python library for home automation execution, enabling seamless control and management of your IoT devices
 Home-page: https://github.com/purple4reina/pydomotic
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/pydomotic
 Project-URL: Bug Tracker, https://github.com/purple4reina/pydomotic/issues
```

### Comparing `pydomotic-1.1.0/README.md` & `pydomotic-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/actions.py` & `pydomotic-1.2.0/pydomotic/actions.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/components.py` & `pydomotic-1.2.0/pydomotic/components.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/context.py` & `pydomotic-1.2.0/pydomotic/context.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/handlers.py` & `pydomotic-1.2.0/pydomotic/handlers.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/parsers.py` & `pydomotic-1.2.0/pydomotic/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,17 +149,19 @@
             raise PyDomoticConfigParsingError(
                     f'provider airthings requires key "{key}"')
 
     client_id = _parse_string(provider['client_id'])
     client_secret = _parse_string(provider['client_secret'])
 
     cache_secs = provider.get('data_cache_seconds')
+    timeout = provider.get('timeout_seconds')
 
     from .providers.airthings import AirthingsProvider
-    return AirthingsProvider(client_id, client_secret, data_cache_seconds=cache_secs)
+    return AirthingsProvider(client_id, client_secret, data_cache_seconds=cache_secs,
+            timeout=timeout)
 
 def _parse_moen_provider(provider):
     for key in ('username', 'password'):
         if key not in provider:
             raise PyDomoticConfigParsingError(
                     f'provider moen requires key "{key}"')
```

### Comparing `pydomotic-1.1.0/pydomotic/providers/airthings.py` & `pydomotic-1.2.0/pydomotic/providers/airthings.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,36 @@
     _auth_token_data = {
             'grant_type': 'client_credentials',
             'scope': 'read:device:current_values',
     }
     _auth_headers = {}
     _samples_url = 'https://ext-api.airthings.com/v1/devices/{}/latest-samples'
 
-    def __init__(self, client_id, client_secret, data_cache_seconds=None):
+    def __init__(self, client_id, client_secret, data_cache_seconds=None, timeout=None):
         self._auth_credentials = (client_id, client_secret)
+        self._timeout = timeout
         if data_cache_seconds:
             self.fetch_data = cache_value(seconds=data_cache_seconds)(self.fetch_data)
 
     def _get_auth_headers(self):
         resp = requests.post(
                 self._auth_token_url,
                 data=self._auth_token_data,
                 auth=self._auth_credentials,
+                timeout=self._timeout,
         )
         resp.raise_for_status()
         self._auth_headers['Authorization'] = f'Bearer {resp.json().get("access_token")}'
         return self._auth_headers
 
     def fetch_data(self, device_id):
         resp = requests.get(
                 url=self._samples_url.format(device_id),
                 headers=self._get_auth_headers(),
+                timeout=self._timeout,
         )
         resp.raise_for_status()
         return resp.json().get('data')
 
     def get_device(self, device_id):
         return self.device(device_id, self)
 
@@ -58,16 +61,17 @@
             return self.fetch_data()['humidity']
 
         def get_battery(self):
             return self.fetch_data()['battery']
 
 class AirthingsProvider(Provider):
 
-    def __init__(self, client_id, client_secret, data_cache_seconds=None):
-        self.api = AirthingsAPI(client_id, client_secret, data_cache_seconds=data_cache_seconds)
+    def __init__(self, client_id, client_secret, data_cache_seconds=None, timeout=None):
+        self.api = AirthingsAPI(client_id, client_secret,
+                data_cache_seconds=data_cache_seconds, timeout=timeout)
 
     def get_device(self, device_id, device_name, device_description):
         device = self.api.get_device(device_id)
         return AirthingsDevice(device, device_name, device_description)
 
 class AirthingsDevice(Device):
```

### Comparing `pydomotic-1.1.0/pydomotic/providers/fujitsu.py` & `pydomotic-1.2.0/pydomotic/providers/fujitsu.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/providers/moen.py` & `pydomotic-1.2.0/pydomotic/providers/moen.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/providers/noop.py` & `pydomotic-1.2.0/pydomotic/providers/noop.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/providers/tuya.py` & `pydomotic-1.2.0/pydomotic/providers/tuya.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/sensors.py` & `pydomotic-1.2.0/pydomotic/sensors.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/triggers.py` & `pydomotic-1.2.0/pydomotic/triggers.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic/utils.py` & `pydomotic-1.2.0/pydomotic/utils.py`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/pydomotic.egg-info/PKG-INFO` & `pydomotic-1.2.0/pydomotic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydomotic
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python library for home automation execution, enabling seamless control and management of your IoT devices
 Home-page: https://github.com/purple4reina/pydomotic
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/pydomotic
 Project-URL: Bug Tracker, https://github.com/purple4reina/pydomotic/issues
```

### Comparing `pydomotic-1.1.0/pydomotic.egg-info/SOURCES.txt` & `pydomotic-1.2.0/pydomotic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydomotic-1.1.0/setup.py` & `pydomotic-1.2.0/setup.py`

 * *Files identical despite different names*

