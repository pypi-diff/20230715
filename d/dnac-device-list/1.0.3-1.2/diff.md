# Comparing `tmp/dnac_device_list-1.0.3.tar.gz` & `tmp/dnac_device_list-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnac_device_list-1.0.3.tar", last modified: Tue Jul  4 00:25:09 2023, max compression
+gzip compressed data, was "dnac_device_list-1.2.tar", last modified: Sat Jul 15 21:49:40 2023, max compression
```

## Comparing `dnac_device_list-1.0.3.tar` & `dnac_device_list-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 00:25:09.493530 dnac_device_list-1.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-03 01:16:23.000000 dnac_device_list-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3648 2023-07-04 00:25:09.491407 dnac_device_list-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3156 2023-07-04 00:23:49.000000 dnac_device_list-1.0.3/README.md
--rw-rw-rw-   0        0        0      635 2023-07-04 00:23:49.000000 dnac_device_list-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 00:25:09.493530 dnac_device_list-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 00:25:09.462081 dnac_device_list-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 00:25:09.471224 dnac_device_list-1.0.3/src/dnac_device_list/
--rw-rw-rw-   0        0        0        0 2023-07-03 01:11:50.000000 dnac_device_list-1.0.3/src/dnac_device_list/__init__.py
--rw-rw-rw-   0        0        0     8320 2023-07-03 16:03:58.000000 dnac_device_list-1.0.3/src/dnac_device_list/device_list.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:25:09.486729 dnac_device_list-1.0.3/src/dnac_device_list.egg-info/
--rw-rw-rw-   0        0        0     3648 2023-07-04 00:25:09.000000 dnac_device_list-1.0.3/src/dnac_device_list.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-04 00:25:09.000000 dnac_device_list-1.0.3/src/dnac_device_list.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 00:25:09.000000 dnac_device_list-1.0.3/src/dnac_device_list.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-04 00:25:09.000000 dnac_device_list-1.0.3/src/dnac_device_list.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 00:25:09.000000 dnac_device_list-1.0.3/src/dnac_device_list.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 21:49:40.985849 dnac_device_list-1.2/
+-rw-rw-rw-   0        0        0     1094 2023-07-15 21:47:59.000000 dnac_device_list-1.2/LICENSE
+-rw-rw-rw-   0        0        0     4050 2023-07-15 21:49:40.985849 dnac_device_list-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3541 2023-07-15 21:46:49.000000 dnac_device_list-1.2/README.md
+-rw-rw-rw-   0        0        0      652 2023-07-15 21:48:58.000000 dnac_device_list-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 21:49:40.985849 dnac_device_list-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 21:49:40.953273 dnac_device_list-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 21:49:40.970816 dnac_device_list-1.2/src/dnac_device_list/
+-rw-rw-rw-   0        0        0        0 2023-07-03 01:11:50.000000 dnac_device_list-1.2/src/dnac_device_list/__init__.py
+-rw-rw-rw-   0        0        0     9878 2023-07-15 21:43:28.000000 dnac_device_list-1.2/src/dnac_device_list/device_list.py
+drwxrwxrwx   0        0        0        0 2023-07-15 21:49:40.985849 dnac_device_list-1.2/src/dnac_device_list.egg-info/
+-rw-rw-rw-   0        0        0     4050 2023-07-15 21:49:40.000000 dnac_device_list-1.2/src/dnac_device_list.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-15 21:49:40.000000 dnac_device_list-1.2/src/dnac_device_list.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 21:49:40.000000 dnac_device_list-1.2/src/dnac_device_list.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-15 21:49:40.000000 dnac_device_list-1.2/src/dnac_device_list.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 21:49:40.000000 dnac_device_list-1.2/src/dnac_device_list.egg-info/top_level.txt
```

### Comparing `dnac_device_list-1.0.3/LICENSE` & `dnac_device_list-1.2/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
+
+Copyright (c) 2023 Alexios Nersessian
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dnac_device_list-1.0.3/PKG-INFO` & `dnac_device_list-1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-Metadata-Version: 2.1
-Name: dnac_device_list
-Version: 1.0.3
-Summary: Get Device list with location details from DNAC.
-Author-email: Alexios Nersessian <nersessian@gmail.com>
-Project-URL: Homepage, https://github.com/alekos3/DNAC_Device_Location
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dnac_device_list
 
 dnac_device_list is a Python library that makes your life easier when you want to programatically find out 
 the location name and location id of any given device that is managed by Cisco DNA Center.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install dnac_device_list.
 
 ```bash
 pip install dnac_device_list
 ```
 
-## Usage
+## Use Case 1 (Use existing token for authorization)
 
 ```python
 from dnac_device_list import device_list
 
 token = "eyJhbRciOiJSUzI1NiIsInR5cGI6IkpXVCJ9.eyJzdWIiOiI2MTE2YmI0YWU3YjUwODZiNTLjMTI5ZjQiLCJhdXRoU291cmNlIjoiaW50ZXJuYWwiLCJ0ZW5hbnROYW1lIjoiVE5UMCIsInJvbGVzIjpbIjYxMTZiYjQ4ZTliNTA4NmI1M2MxMjlmMyJdLCJ0ZW5hbnRJZCI6IjYxMTZiYjQ4ZTliNTA4NmI1M2MxMjlmMSIsImV4cCI6MTY4ODQwMzMxMSwiaWF0IjoxNjg4Mzk5NzExLCJqdGkiOiJhNzliMjgwMC04NjdkLTRiZmQtYWJmMy02NjJiOGUzNmY4OTgiLCJ1c2VybmFtZSI6ImFkbWluIn0.hqvLkQL-07Oiwjy_RzEj5b556nlDiNpIZw-78xmEUu9FLIBuE0bWvoLgmK-2AIdAsB2bbPZ61uDmrE4YK__IINDNl6zeK6NfBGSDCzpJ9VvT_ywnLdqSpGfBArcnGcr2Wwa1DRSmGBn5uF7o0SBcE-K2--KneGsIKjZblCAPD4G1F8QwmL_FgNv6cVI-FMdhLxtYuM2pCYpE23oBmHaSIm-0xyPc71vlQiAYbZ1vnQVx64zdVNA5SPvyAvOZUY5YTixhOU0qw3rcABSk0GbVO8jZlE-QJLuC6hhh5LwM6yDnWPekWS7KPqdhXGTAEzPhxNvnAmZlXrY0nrJFJBpkkg"
 
 # initializes class
 dnac = device_list.Dnac(base_url="https://dnac.example.com", token=token, verify=False)
 
 # returns 'list of devices'
-devices= dnac.get_device_list_with_location()
+devices = dnac.get_device_list_with_location()
+
+
+```
+
+## Use Case 2 (Use username and password for authorization)
 
+```python
+from dnac_device_list import device_list
 
+# initializes class
+dnac = device_list.Dnac(base_url="https://dnac.example.com", username="admin", password="Cisco123", verify=False)
+
+# returns 'list of devices'
+devices = dnac.get_device_list_with_location()
 ```
 
 ## Response json (devices variable)
 ```json
 {
 	"response": [
 		{
@@ -103,8 +102,8 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Authors
 Alexios Nersessian
-email: nersessian@gmail.com
+email: nersessian@gmail.com
```

### Comparing `dnac_device_list-1.0.3/README.md` & `dnac_device_list-1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,59 @@
+Metadata-Version: 2.1
+Name: dnac_device_list
+Version: 1.2
+Summary: Get complete Device list inventory with location details from DNAC.
+Author-email: Alexios Nersessian <nersessian@gmail.com>
+Project-URL: Homepage, https://github.com/alekos3/DNAC_Device_Location
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dnac_device_list
 
 dnac_device_list is a Python library that makes your life easier when you want to programatically find out 
 the location name and location id of any given device that is managed by Cisco DNA Center.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install dnac_device_list.
 
 ```bash
 pip install dnac_device_list
 ```
 
-## Usage
+## Use Case 1 (Use existing token for authorization)
 
 ```python
 from dnac_device_list import device_list
 
 token = "eyJhbRciOiJSUzI1NiIsInR5cGI6IkpXVCJ9.eyJzdWIiOiI2MTE2YmI0YWU3YjUwODZiNTLjMTI5ZjQiLCJhdXRoU291cmNlIjoiaW50ZXJuYWwiLCJ0ZW5hbnROYW1lIjoiVE5UMCIsInJvbGVzIjpbIjYxMTZiYjQ4ZTliNTA4NmI1M2MxMjlmMyJdLCJ0ZW5hbnRJZCI6IjYxMTZiYjQ4ZTliNTA4NmI1M2MxMjlmMSIsImV4cCI6MTY4ODQwMzMxMSwiaWF0IjoxNjg4Mzk5NzExLCJqdGkiOiJhNzliMjgwMC04NjdkLTRiZmQtYWJmMy02NjJiOGUzNmY4OTgiLCJ1c2VybmFtZSI6ImFkbWluIn0.hqvLkQL-07Oiwjy_RzEj5b556nlDiNpIZw-78xmEUu9FLIBuE0bWvoLgmK-2AIdAsB2bbPZ61uDmrE4YK__IINDNl6zeK6NfBGSDCzpJ9VvT_ywnLdqSpGfBArcnGcr2Wwa1DRSmGBn5uF7o0SBcE-K2--KneGsIKjZblCAPD4G1F8QwmL_FgNv6cVI-FMdhLxtYuM2pCYpE23oBmHaSIm-0xyPc71vlQiAYbZ1vnQVx64zdVNA5SPvyAvOZUY5YTixhOU0qw3rcABSk0GbVO8jZlE-QJLuC6hhh5LwM6yDnWPekWS7KPqdhXGTAEzPhxNvnAmZlXrY0nrJFJBpkkg"
 
 # initializes class
 dnac = device_list.Dnac(base_url="https://dnac.example.com", token=token, verify=False)
 
 # returns 'list of devices'
-devices= dnac.get_device_list_with_location()
+devices = dnac.get_device_list_with_location()
+
+
+```
+
+## Use Case 2 (Use username and password for authorization)
 
+```python
+from dnac_device_list import device_list
 
+# initializes class
+dnac = device_list.Dnac(base_url="https://dnac.example.com", username="admin", password="Cisco123", verify=False)
+
+# returns 'list of devices'
+devices = dnac.get_device_list_with_location()
 ```
 
 ## Response json (devices variable)
 ```json
 {
 	"response": [
 		{
@@ -90,8 +115,8 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Authors
 Alexios Nersessian
-email: nersessian@gmail.com
+email: nersessian@gmail.com
```

### Comparing `dnac_device_list-1.0.3/pyproject.toml` & `dnac_device_list-1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnac_device_list"
-version = "1.0.3"
+version = "1.2"
 authors = [
   { name="Alexios Nersessian", email="nersessian@gmail.com" },
 ]
-description = "Get Device list with location details from DNAC."
+description = "Get complete Device list inventory with location details from DNAC."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `dnac_device_list-1.0.3/src/dnac_device_list/device_list.py` & `dnac_device_list-1.2/src/dnac_device_list/device_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __author__ = "Alexios Nersessian"
 __email__ = "nersessian@gmail.com"
-__version__ = "v1"
+__version__ = "v1.2"
 
+import getpass
 import json
 import requests
 
 """
 Class that gets all network devices from Cisco DNA Center and populates the location and locationName fields. The 3 API
 endpoints below are consumed in order to get the location name and location id.
 
@@ -35,18 +36,55 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 """
 
 
 class Dnac:
-    def __init__(self, base_url, token, verify=None):
+    def __init__(self, base_url, token=None, username=None, password=None, verify=None):
         self.base_url = base_url
         self.token = token
         self.verify = verify if verify is not None else True
+        self.username = username
+        self.password = password
+
+        if not self.token and self.username and self.password:
+            self.token = self.get_auth_token()
+        elif not self.token and (not self.username or not self.password):
+            print("Need a valid Token or credentials to proceed!")
+            exit(1)
+
+    # Function to get the authorization token
+    def get_auth_token(self):
+        # Concatenate the URL variable with the path to get the token
+        auth_url = f"{self.base_url}/dna/system/api/v1/auth/token"
+
+        # Include the proper content-type field here
+        auth_headers = {
+            "Content-Type": "application/json"
+        }
+
+        try:
+            response = requests.request("POST", auth_url, auth=(self.username, self.password), headers=auth_headers, verify=self.verify)
+            print(response.status_code)
+            if response.status_code == 401:
+                for i in range(3):
+                    password = getpass.getpass()
+                    response = requests.request("POST", auth_url, auth=(self.username, password), headers=auth_headers,
+                                                verify=self.verify)
+
+                    if response.status_code == 200:
+                        break
+
+            if response.status_code == requests.codes.ok:
+                token = response.json()["Token"]
+                return token
+
+        except Exception as e:
+            print(e)
 
     def __get_network_devices(self):
         """
         Function gets all DNAC devices in inventory.
         :return: list of dictionaries
         """
         offset = 1
```

### Comparing `dnac_device_list-1.0.3/src/dnac_device_list.egg-info/PKG-INFO` & `dnac_device_list-1.2/src/dnac_device_list.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dnac-device-list
-Version: 1.0.3
-Summary: Get Device list with location details from DNAC.
+Version: 1.2
+Summary: Get complete Device list inventory with location details from DNAC.
 Author-email: Alexios Nersessian <nersessian@gmail.com>
 Project-URL: Homepage, https://github.com/alekos3/DNAC_Device_Location
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -20,30 +20,42 @@
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install dnac_device_list.
 
 ```bash
 pip install dnac_device_list
 ```
 
-## Usage
+## Use Case 1 (Use existing token for authorization)
 
 ```python
 from dnac_device_list import device_list
 
 token = "eyJhbRciOiJSUzI1NiIsInR5cGI6IkpXVCJ9.eyJzdWIiOiI2MTE2YmI0YWU3YjUwODZiNTLjMTI5ZjQiLCJhdXRoU291cmNlIjoiaW50ZXJuYWwiLCJ0ZW5hbnROYW1lIjoiVE5UMCIsInJvbGVzIjpbIjYxMTZiYjQ4ZTliNTA4NmI1M2MxMjlmMyJdLCJ0ZW5hbnRJZCI6IjYxMTZiYjQ4ZTliNTA4NmI1M2MxMjlmMSIsImV4cCI6MTY4ODQwMzMxMSwiaWF0IjoxNjg4Mzk5NzExLCJqdGkiOiJhNzliMjgwMC04NjdkLTRiZmQtYWJmMy02NjJiOGUzNmY4OTgiLCJ1c2VybmFtZSI6ImFkbWluIn0.hqvLkQL-07Oiwjy_RzEj5b556nlDiNpIZw-78xmEUu9FLIBuE0bWvoLgmK-2AIdAsB2bbPZ61uDmrE4YK__IINDNl6zeK6NfBGSDCzpJ9VvT_ywnLdqSpGfBArcnGcr2Wwa1DRSmGBn5uF7o0SBcE-K2--KneGsIKjZblCAPD4G1F8QwmL_FgNv6cVI-FMdhLxtYuM2pCYpE23oBmHaSIm-0xyPc71vlQiAYbZ1vnQVx64zdVNA5SPvyAvOZUY5YTixhOU0qw3rcABSk0GbVO8jZlE-QJLuC6hhh5LwM6yDnWPekWS7KPqdhXGTAEzPhxNvnAmZlXrY0nrJFJBpkkg"
 
 # initializes class
 dnac = device_list.Dnac(base_url="https://dnac.example.com", token=token, verify=False)
 
 # returns 'list of devices'
-devices= dnac.get_device_list_with_location()
+devices = dnac.get_device_list_with_location()
 
 
 ```
 
+## Use Case 2 (Use username and password for authorization)
+
+```python
+from dnac_device_list import device_list
+
+# initializes class
+dnac = device_list.Dnac(base_url="https://dnac.example.com", username="admin", password="Cisco123", verify=False)
+
+# returns 'list of devices'
+devices = dnac.get_device_list_with_location()
+```
+
 ## Response json (devices variable)
 ```json
 {
 	"response": [
 		{
 			"reachabilityFailureReason": "string",
 			"reachabilityStatus": "string",
```

