# Comparing `tmp/offat-0.2.0.tar.gz` & `tmp/offat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offat-0.2.0.tar", max compression
+gzip compressed data, was "offat-0.3.0.tar", max compression
```

## Comparing `offat-0.2.0.tar` & `offat-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-07-08 13:53:24.791561 offat-0.2.0/LICENSE
--rw-r--r--   0        0        0     5063 2023-07-08 13:53:24.791561 offat-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-08 13:53:24.791561 offat-0.2.0/offat/__init__.py
--rw-r--r--   0        0        0     1366 2023-07-08 13:53:24.791561 offat-0.2.0/offat/__main__.py
--rw-r--r--   0        0        0     4276 2023-07-08 13:53:24.791561 offat-0.2.0/offat/http.py
--rw-r--r--   0        0        0     1121 2023-07-08 13:53:24.791561 offat-0.2.0/offat/logger.py
--rw-r--r--   0        0        0     3767 2023-07-08 13:53:24.791561 offat-0.2.0/offat/openapi.py
--rw-r--r--   0        0        0        0 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/__init__.py
--rw-r--r--   0        0        0      262 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/fuzzer.py
--rw-r--r--   0        0        0     8427 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/test_generator.py
--rw-r--r--   0        0        0     1230 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/test_results.py
--rw-r--r--   0        0        0     2609 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/test_runner.py
--rw-r--r--   0        0        0     1775 2023-07-08 13:53:24.791561 offat-0.2.0/offat/utils.py
--rw-r--r--   0        0        0      873 2023-07-08 13:53:24.791561 offat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6031 1970-01-01 00:00:00.000000 offat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-15 11:22:03.008874 offat-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5632 2023-07-15 11:22:03.008874 offat-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 11:22:03.008874 offat-0.3.0/offat/__init__.py
+-rw-r--r--   0        0        0      662 2023-07-15 11:22:03.008874 offat-0.3.0/offat/__main__.py
+-rw-r--r--   0        0        0     4327 2023-07-15 11:22:03.008874 offat-0.3.0/offat/http.py
+-rw-r--r--   0        0        0     1122 2023-07-15 11:22:03.008874 offat-0.3.0/offat/logger.py
+-rw-r--r--   0        0        0     3767 2023-07-15 11:22:03.008874 offat-0.3.0/offat/openapi.py
+-rw-r--r--   0        0        0        0 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/__init__.py
+-rw-r--r--   0        0        0     3158 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/fuzzer.py
+-rw-r--r--   0        0        0    11990 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/test_generator.py
+-rw-r--r--   0        0        0     1274 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/test_results.py
+-rw-r--r--   0        0        0     3903 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/test_runner.py
+-rw-r--r--   0        0        0     1403 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/tester_utils.py
+-rw-r--r--   0        0        0     2021 2023-07-15 11:22:03.008874 offat-0.3.0/offat/utils.py
+-rw-r--r--   0        0        0      873 2023-07-15 11:22:03.008874 offat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6600 1970-01-01 00:00:00.000000 offat-0.3.0/PKG-INFO
```

### Comparing `offat-0.2.0/LICENSE` & `offat-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offat-0.2.0/README.md` & `offat-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 # OFFAT - OFFensive Api Tester
 
-Automatically Tests for vulnerabilities after generating tests from openapi specification file.
+Automatically Tests for vulnerabilities after generating tests from openapi specification file. Project is in Beta stage, so sometimes it might crash while running.
 
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
 
+## Features
+
+- [X] Restricted HTTP Methods
+- [X] SQLi
+- [X] BOLA (Might need few bug fixes)
+- [ ] Broken Authentication
+- [ ] Mass Assignment
+- [ ] Data Exposure
+
+## Demo
+
+[![asciicast](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF.svg)](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF)
+
 ## PyPi Downloads
 
+[![Upload offat Python Package to PyPi](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml)
+
 |Period|Count|
 |:----:|:---:|
 |Weekly|[![Downloads](https://static.pepy.tech/personalized-badge/offat?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/offat)|
 |Monthy|[![Downloads](https://static.pepy.tech/personalized-badge/offat?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/offat)|
 |Total|[![Downloads](https://static.pepy.tech/personalized-badge/offat?period=totalPu&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/offat)|
 
 ## Disclaimer
```

### Comparing `offat-0.2.0/offat/__main__.py` & `offat-0.3.0/offat/tester/tester_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from argparse import ArgumentParser
 from asyncio import run
-# from pprint import pprint as print
-from .openapi import OpenAPIParser
-from .tester.test_generator import TestGenerator
-from .tester.test_runner import TestRunner
-from .tester.test_results import TestResultTable
-
-
-def start():
-    '''Starts cli tool'''
-    parser = ArgumentParser(prog='offat')
-    parser.add_argument('-f','--file', dest='fpath', type=str, help='path of openapi/swagger specification file', required=True)
-    
-    args = parser.parse_args()
-
-    api_parser = OpenAPIParser(args.fpath)
-
-    # create tester objs
-    test_runner = TestRunner()
-    test_table_generator = TestResultTable()
-    test_generator = TestGenerator()
+from .test_generator import TestGenerator
+from .test_runner import TestRunner
+from .test_results import TestResultTable
+from ..logger import create_logger
+from ..openapi import OpenAPIParser
 
-    
-    # test for unsupported http methods
-    # unsupported_http_endpoint_tests = test_generator.check_unsupported_http_methods(api_parser.base_url, api_parser._get_endpoints())
-    # test_results = run(test_runner.run_tests(unsupported_http_endpoint_tests))
-    # results = test_table_generator.generate_result_table(test_results)
-    # print(results)
 
+logger = create_logger(__name__)
 
-    # sqli fuzz test
-    sqli_fuzz_tests = test_generator.sqli_fuzz_params(api_parser)
-    test_results = run(test_runner.run_tests(sqli_fuzz_tests))
+# create tester objs
+test_runner = TestRunner()
+test_table_generator = TestResultTable()
+test_generator = TestGenerator()
+
+
+def run_test(tests:list[dict]):
+    '''Run tests and print result on console'''
+    global test_runner, test_table_generator
+    test_results = run(test_runner.run_tests(tests))
     results = test_table_generator.generate_result_table(test_results)
     print(results)
 
-    # generate results
+ 
+def generate_and_run_tests(api_parser:OpenAPIParser):
+    global test_runner, test_table_generator, logger
 
-if __name__ == '__main__':
-    start()
+    # test for unsupported http methods
+    logger.info('Checking for Unsupported HTTP methods:')
+    unsupported_http_endpoint_tests = test_generator.check_unsupported_http_methods(api_parser.base_url, api_parser._get_endpoints())
+    run_test(unsupported_http_endpoint_tests)
+
+    # sqli fuzz test
+    logger.info('Checking for SQLi vulnerability:')
+    sqli_fuzz_tests = test_generator.sqli_fuzz_params_test(api_parser)
+    run_test(sqli_fuzz_tests)
+   
+    # BOLA path tests
+    logger.info('Checking for BOLA in PATH:')
+    bola_path_tests = test_generator.bola_path_test(api_parser, success_codes=[200, 201, 301])
+    run_test(bola_path_tests)
```

### Comparing `offat-0.2.0/offat/http.py` & `offat-0.3.0/offat/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,30 @@
             case 'HEAD':
                 sent_req = session.head(url, *args, **kwargs)
             case 'OPTIONS':
                 sent_req = session.options(url, *args, **kwargs)
             case 'DELETE':
                 sent_req = session.delete(url, *args, **kwargs)
 
-
         resp_data = None
         async with sent_req as response:
             resp_data = {
                         "status": response.status,
                         "req_url": str(response.request_info.real_url),
+                        "query_url":str(response.url),
                         "req_method": response.request_info.method,
                         "req_headers": dict(**response.request_info.headers),
                         "res_redirection": str(response.history),
                         "res_headers": dict(response.headers),
                         "res_body": await response.text(),
                     }
+        
             if is_new_session:
                 await session.close()
-            
+
         return resp_data
 
 
 class AsyncRLRequests(AsyncRequests):
     '''
     Send Asynchronous rate limited HTTP requests.
     '''
```

### Comparing `offat-0.2.0/offat/logger.py` & `offat-0.3.0/offat/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from colorama import Fore, Style, init
-init(autoreset=True)
-
 import logging
 
 
+init(autoreset=True)
+
+
 class ColoredLogger(logging.Formatter):
     grey = Fore.WHITE
     yellow = Fore.YELLOW + Style.BRIGHT
     red = Fore.RED 
     bold_red = Fore.RED + Style.BRIGHT
     reset = "\x1b[0m" 
     format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s (%(filename)s:%(lineno)d)"
```

### Comparing `offat-0.2.0/offat/openapi.py` & `offat-0.3.0/offat/openapi.py`

 * *Files identical despite different names*

### Comparing `offat-0.2.0/offat/tester/test_generator.py` & `offat-0.3.0/offat/tester/test_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from .test_runner import TestRunnerFiltersEnum
 from copy import deepcopy
+from random import randint
+from .test_runner import TestRunnerFiltersEnum
 from ..openapi import OpenAPIParser
-from pprint import pprint as print
+from .fuzzer import fill_params
 
 
 class TestGenerator:
     """
     Class to generate API test checks.
 
     This class provides methods to generate API test checks for various scenarios.
@@ -72,20 +73,22 @@
             for restricted_method in restricted_methods:
                 
                 tasks.append({
                     'test_name':'UnSupported HTTP Method Check',
                     'url': f'{base_url}{endpoint}',
                     'endpoint': endpoint,
                     'method': restricted_method.upper(),
+                    'malicious_payload':[],
                     'args': args,
                     'kwargs': kwargs,
                     'result_details':{
                         True: 'Endpoint does not perform any HTTP method which is not documented', # passed
                         False: 'Endpoint performs HTTP method which is not documented', # failed
                     },
+                    'body_params':[],
                     'success_codes':success_codes,
                     'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER
                 })
 
         return tasks
     
 
@@ -142,15 +145,15 @@
                 new_request = deepcopy(request_param_data)
                 new_request['value'] = sqli_payload
                 malicious_params.append(new_request)
 
         return malicious_params
         
 
-    def sqli_fuzz_params(
+    def sqli_fuzz_params_test(
             self,
             openapi_parser:OpenAPIParser,
             success_codes:list[int]=[403,405,500],
             *args,
             **kwargs
     ):
         '''Performs SQL injection (SQLi) parameter fuzzing based on the provided OpenAPIParser instance.
@@ -158,15 +161,15 @@
         Args:
             openapi_parser (OpenAPIParser): An instance of the OpenAPIParser class containing the parsed OpenAPI specification.
             success_codes (list[int], optional): A list of HTTP success codes to consider as successful SQLi responses. Defaults to [500].
             *args: Variable-length positional arguments.
             **kwargs: Arbitrary keyword arguments.
         
         Returns:
-            None
+            List: List of dictionaries containing tests for SQLi
         
         Raises:
             Any exceptions raised during the execution.
         '''
         base_url:str = openapi_parser.base_url
         request_response_params:dict = openapi_parser.request_response_params
 
@@ -185,16 +188,16 @@
         # TODO: handle path params in future
         # NOTE: skip paths containing in path variables and no body params for now!!.
         request_response_params = list(filter(lambda x: len(x.get('path_params',[]))==0 and len(x.get('request_params',[]))>0, request_response_params))
 
         # inject SQLi payloads in string variables
         for sqli_payload in basic_sqli_payloads:
             for request_obj in request_response_params:
-                request_params = request_obj.get('request_params')
-                request_path = request_obj.get('path')
+                request_params = request_obj.get('request_params',[])
+                request_path = request_obj.get('path',[])
 
                 malicious_request_params = self.__inject_sqli_payload_in_params(request_params, sqli_payload)
 
                 tasks.append({
                     'test_name':'SQLi Test',
                     'url': f'{base_url}{request_path}',
                     'endpoint': request_path,
@@ -207,8 +210,89 @@
                         True:'Parameters are not vulnerable to SQLi Payload', # passed
                         False:'One or more parameter is vulnerable to SQL Injection Attack', # failed
                     },
                     'success_codes':success_codes,
                     'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER
                 })
 
+        return tasks
+    
+
+    def bola_path_test(
+            self,
+            openapi_parser:OpenAPIParser,
+            success_codes:list[int]=[200, 201, 301],
+            *args,
+            **kwargs
+    ):
+        '''Generate Tests for BOLA in endpoint path
+        
+        Args:
+            openapi_parser (OpenAPIParser): An instance of the OpenAPIParser class containing the parsed OpenAPI specification.
+            success_codes (list[int], optional): A list of HTTP success codes to consider as successful BOLA responses. Defaults to [200, 201, 301].
+            *args: Variable-length positional arguments.
+            **kwargs: Arbitrary keyword arguments.
+        
+        Returns:
+            None
+        
+        Raises:
+            Any exceptions raised during the execution.
+        '''
+        base_url:str = openapi_parser.base_url
+        request_response_params:list[dict] = openapi_parser.request_response_params
+
+        # get request params list
+        # request_params_list = list(map(lambda x: self.__get_request_params_list(x.get('request_params',[])), request_response_params))
+
+        # filter path containing params in path
+        endpoints_with_param_in_path = list(filter(lambda path_obj: '/{' in path_obj.get('path'), request_response_params))
+
+        tasks = []
+        for path_obj in endpoints_with_param_in_path:
+            # handle path params from request_params
+            request_params = path_obj.get('request_params',[])
+            request_params = fill_params(request_params)
+
+            # get request body params
+            request_body_params = list(filter(lambda x: x.get('in') == 'body', request_params))
+            
+
+            # handle path params from path_params
+            # and replace path params by value in 
+            # endpoint path
+            endpoint_path:str = path_obj.get('path')
+
+            path_params = path_obj.get('path_params',[])
+            path_params_in_body = list(filter(lambda x: x.get('in') == 'path', request_params))
+            path_params += path_params_in_body
+            path_params = fill_params(path_params)
+
+            for path_param in path_params:
+                path_param_name = path_param.get('name')
+                path_param_value = path_param.get('value')
+                endpoint_path = endpoint_path.replace('{' + str(path_param_name) + '}', str(path_param_value))
+
+            # TODO: handle request query params
+            request_query_params = list(filter(lambda x: x.get('in') == 'query', request_params))
+            # print(request_query_params)
+            # print('-'*30)
+
+            tasks.append({
+                'test_name':'BOLA Path Test',
+                'url': f'{base_url}{endpoint_path}',
+                'endpoint': path_obj.get('path'),
+                'method': path_obj.get('http_method').upper(),
+                'body_params':request_body_params,
+                'query_params':request_query_params,
+                'malicious_payload':path_params,
+                'args': args,
+                'kwargs': kwargs,
+                'result_details':{
+                    True:'Endpoint is not vulnerable to BOLA', # passed
+                    False:'Endpoint might be vulnerable to BOLA', # failed
+                },
+                'success_codes':success_codes,
+                'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER
+            })
+
         return tasks
```

### Comparing `offat-0.2.0/offat/tester/test_results.py` & `offat-0.3.0/offat/tester/test_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,9 +24,10 @@
             del result['url']
             del result['args']
             del result['kwargs']
             del result['test_name']
             del result['response_filter']
             del result['success_codes']
             del result['body_params']
+            del result['malicious_payload']
             
         return results
```

### Comparing `offat-0.2.0/offat/utils.py` & `offat-0.3.0/offat/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 from json import loads as json_load, JSONDecodeError
 from os.path import isfile
 from yaml import safe_load, YAMLError
+from pkg_resources import get_distribution
+
+
+def get_package_version():
+    '''Returns package current version
+    
+    Args:
+        None
+
+    Returns:
+        String: current package version
+    '''
+    return get_distribution('offat').version    
 
 
 def read_yaml(file_path:str) -> dict:
     '''Reads YAML file and returns as python dict. 
     returns file not found or yaml errors as dict.
 
     Args:
@@ -60,8 +73,7 @@
     match file_ext:
         case 'json':
             return read_json(file_path)
         case 'yaml':
             return read_yaml(file_path)
         case _:
             return {"error":"Invalid file extension"}
-
```

### Comparing `offat-0.2.0/pyproject.toml` & `offat-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "offat"
-version = "0.2.0"
+version = "0.3.0"
 description = "Offensive API tester tool automates checks for common API vulnerabilities"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `offat-0.2.0/PKG-INFO` & `offat-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offat
-Version: 0.2.0
+Version: 0.3.0
 Summary: Offensive API tester tool automates checks for common API vulnerabilities
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,20 +19,35 @@
 Project-URL: Home, https://github.com/dmdhrumilmistry/offat
 Project-URL: PayPal, https://paypal.me/dmdhrumilmistry
 Project-URL: Support, https://github.com/sponsors/dmdhrumilmistry/
 Description-Content-Type: text/markdown
 
 # OFFAT - OFFensive Api Tester
 
-Automatically Tests for vulnerabilities after generating tests from openapi specification file.
+Automatically Tests for vulnerabilities after generating tests from openapi specification file. Project is in Beta stage, so sometimes it might crash while running.
 
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
 
+## Features
+
+- [X] Restricted HTTP Methods
+- [X] SQLi
+- [X] BOLA (Might need few bug fixes)
+- [ ] Broken Authentication
+- [ ] Mass Assignment
+- [ ] Data Exposure
+
+## Demo
+
+[![asciicast](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF.svg)](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF)
+
 ## PyPi Downloads
 
+[![Upload offat Python Package to PyPi](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml)
+
 |Period|Count|
 |:----:|:---:|
 |Weekly|[![Downloads](https://static.pepy.tech/personalized-badge/offat?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/offat)|
 |Monthy|[![Downloads](https://static.pepy.tech/personalized-badge/offat?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/offat)|
 |Total|[![Downloads](https://static.pepy.tech/personalized-badge/offat?period=totalPu&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/offat)|
 
 ## Disclaimer
```

