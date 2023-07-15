# Comparing `tmp/common-osint-model-0.4.7.tar.gz` & `tmp/common-osint-model-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-osint-model-0.4.7.tar", max compression
+gzip compressed data, was "common-osint-model-0.4.9.tar", max compression
```

## Comparing `common-osint-model-0.4.7.tar` & `common-osint-model-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2021-09-16 09:34:52.907153 common-osint-model-0.4.7/LICENSE
--rw-r--r--   0        0        0    21751 2021-09-22 14:03:50.635546 common-osint-model-0.4.7/README.md
--rw-r--r--   0        0        0      755 2021-09-22 14:03:50.635825 common-osint-model-0.4.7/common_osint_model/__init__.py
--rw-r--r--   0        0        0        0 2021-09-16 09:34:52.908333 common-osint-model-0.4.7/common_osint_model/censys/__init__.py
--rw-r--r--   0        0        0    10490 2021-09-16 09:34:52.908622 common-osint-model-0.4.7/common_osint_model/censys/v1.py
--rw-r--r--   0        0        0     5231 2021-09-16 09:34:52.908860 common-osint-model-0.4.7/common_osint_model/censys/v2.py
--rw-r--r--   0        0        0     4823 2021-09-16 09:34:52.909103 common-osint-model-0.4.7/common_osint_model/certificate.py
--rw-r--r--   0        0        0     2169 2021-09-16 09:34:52.909303 common-osint-model-0.4.7/common_osint_model/cli.py
--rw-r--r--   0        0        0     1060 2021-09-16 09:34:52.909590 common-osint-model-0.4.7/common_osint_model/models/__init__.py
--rw-r--r--   0        0        0     2029 2021-11-18 12:51:44.145049 common-osint-model-0.4.7/common_osint_model/models/autonomous_system.py
--rw-r--r--   0        0        0      566 2021-09-16 09:34:52.910171 common-osint-model-0.4.7/common_osint_model/models/dns.py
--rw-r--r--   0        0        0      807 2021-09-22 14:03:50.636391 common-osint-model-0.4.7/common_osint_model/models/domain.py
--rw-r--r--   0        0        0     7988 2021-10-28 14:42:34.968237 common-osint-model-0.4.7/common_osint_model/models/host.py
--rw-r--r--   0        0        0     9242 2021-09-16 09:34:52.910804 common-osint-model-0.4.7/common_osint_model/models/http.py
--rw-r--r--   0        0        0     5809 2021-09-22 14:03:50.637195 common-osint-model-0.4.7/common_osint_model/models/service.py
--rw-r--r--   0        0        0     7727 2021-09-16 09:34:52.911169 common-osint-model-0.4.7/common_osint_model/models/ssh.py
--rw-r--r--   0        0        0    13019 2021-10-28 14:42:34.968577 common-osint-model-0.4.7/common_osint_model/models/tls.py
--rw-r--r--   0        0        0     9865 2021-09-16 09:34:52.911690 common-osint-model-0.4.7/common_osint_model/shodan.py
--rw-r--r--   0        0        0     2792 2021-09-16 09:34:52.911993 common-osint-model-0.4.7/common_osint_model/utils.py
--rw-r--r--   0        0        0     1016 2021-11-18 12:51:48.600104 common-osint-model-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    23730 2021-11-18 12:52:08.304161 common-osint-model-0.4.7/setup.py
--rw-r--r--   0        0        0    22560 2021-11-18 12:52:08.305203 common-osint-model-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-09-16 09:34:52.907153 common-osint-model-0.4.9/LICENSE
+-rw-r--r--   0        0        0    21751 2021-09-22 14:03:50.635546 common-osint-model-0.4.9/README.md
+-rw-r--r--   0        0        0      755 2021-09-22 14:03:50.635825 common-osint-model-0.4.9/common_osint_model/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-16 09:34:52.908333 common-osint-model-0.4.9/common_osint_model/censys/__init__.py
+-rw-r--r--   0        0        0    10490 2021-09-16 09:34:52.908622 common-osint-model-0.4.9/common_osint_model/censys/v1.py
+-rw-r--r--   0        0        0     5231 2021-09-16 09:34:52.908860 common-osint-model-0.4.9/common_osint_model/censys/v2.py
+-rw-r--r--   0        0        0     4823 2021-09-16 09:34:52.909103 common-osint-model-0.4.9/common_osint_model/certificate.py
+-rw-r--r--   0        0        0     2169 2021-09-16 09:34:52.909303 common-osint-model-0.4.9/common_osint_model/cli.py
+-rw-r--r--   0        0        0     1310 2022-02-11 13:15:38.813028 common-osint-model-0.4.9/common_osint_model/models/__init__.py
+-rw-r--r--   0        0        0     2029 2021-11-18 12:51:44.145049 common-osint-model-0.4.9/common_osint_model/models/autonomous_system.py
+-rw-r--r--   0        0        0      566 2021-09-16 09:34:52.910171 common-osint-model-0.4.9/common_osint_model/models/dns.py
+-rw-r--r--   0        0        0      807 2021-09-22 14:03:50.636391 common-osint-model-0.4.9/common_osint_model/models/domain.py
+-rw-r--r--   0        0        0     7988 2021-10-28 14:42:34.968237 common-osint-model-0.4.9/common_osint_model/models/host.py
+-rw-r--r--   0        0        0     9935 2022-05-23 12:32:12.481304 common-osint-model-0.4.9/common_osint_model/models/http.py
+-rw-r--r--   0        0        0     5809 2021-09-22 14:03:50.637195 common-osint-model-0.4.9/common_osint_model/models/service.py
+-rw-r--r--   0        0        0     7727 2021-09-16 09:34:52.911169 common-osint-model-0.4.9/common_osint_model/models/ssh.py
+-rw-r--r--   0        0        0    13286 2022-02-11 13:15:38.813372 common-osint-model-0.4.9/common_osint_model/models/tls.py
+-rw-r--r--   0        0        0     9865 2021-09-16 09:34:52.911690 common-osint-model-0.4.9/common_osint_model/shodan.py
+-rw-r--r--   0        0        0     2792 2021-09-16 09:34:52.911993 common-osint-model-0.4.9/common_osint_model/utils.py
+-rw-r--r--   0        0        0     1016 2022-05-23 12:32:12.482204 common-osint-model-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0    23730 2022-05-23 12:32:52.521420 common-osint-model-0.4.9/setup.py
+-rw-r--r--   0        0        0    22560 2022-05-23 12:32:52.522772 common-osint-model-0.4.9/PKG-INFO
```

### Comparing `common-osint-model-0.4.7/LICENSE` & `common-osint-model-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/README.md` & `common-osint-model-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/__init__.py` & `common-osint-model-0.4.9/common_osint_model/__init__.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/censys/v1.py` & `common-osint-model-0.4.9/common_osint_model/censys/v1.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/censys/v2.py` & `common-osint-model-0.4.9/common_osint_model/censys/v2.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/certificate.py` & `common-osint-model-0.4.9/common_osint_model/certificate.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/cli.py` & `common-osint-model-0.4.9/common_osint_model/cli.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/models/__init__.py` & `common-osint-model-0.4.9/common_osint_model/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,24 @@
         logger.info(message)
 
     @classmethod
     def debug(cls, message: str):
         logger = getLogger(cls.__name__)
         logger.debug(message)
 
+    @classmethod
+    def warning(cls, message: str):
+        logger = getLogger(cls.__name__)
+        logger.warning(message)
+
+    @classmethod
+    def error(cls, message: str):
+        logger = getLogger(cls.__name__)
+        logger.error(message)
+
 
 class ShodanDataHandler(ABC):
     """Abstract base class indicating that a class implements from_shodan()."""
 
     @classmethod
     def from_shodan(cls, d: Dict):
         pass
```

### Comparing `common-osint-model-0.4.7/common_osint_model/models/autonomous_system.py` & `common-osint-model-0.4.9/common_osint_model/models/autonomous_system.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/models/dns.py` & `common-osint-model-0.4.9/common_osint_model/models/dns.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/models/domain.py` & `common-osint-model-0.4.9/common_osint_model/models/domain.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/models/host.py` & `common-osint-model-0.4.9/common_osint_model/models/host.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/models/http.py` & `common-osint-model-0.4.9/common_osint_model/models/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,20 @@
             security_txt = HTTPComponentContentSecurity.from_shodan(d)
 
         robots_txt = None
         if d["http"]["robots"]:
             cls.debug("Robots.txt key found in Shodan data.")
             robots_txt = HTTPComponentContentRobots.from_shodan(d)
 
-        raw = d["http"]["html"].encode("utf-8")
+        raw = d["http"].get("html", "")
+        if not raw:
+            raw = ""
+
+        raw = raw.encode("utf-8")
+
         md5, sha1, sha256, murmur = hash_all(raw)
         return HTTPComponentContent(
             raw=raw,
             length=len(raw),
             md5=md5,
             sha1=sha1,
             sha256=sha256,
@@ -209,50 +214,64 @@
         )
 
 
 class HTTPComponent(BaseModel, ShodanDataHandler, CensysDataHandler, BinaryEdgeDataHandler):
     """Represents the HTTP component of services."""
     headers: Optional[Dict[str, str]]
     content: Optional[HTTPComponentContent]
+    shodan_headers_hash: Optional[str]
 
     @classmethod
     def from_shodan(cls, d: Dict):
         """Creates an instance of this class based on Shodan data given as dictionary."""
         if not isinstance(d, Dict):
             raise TypeError(f"Method HTTPComponent.from_shodan expects parameter d to be a dictionary, "
                             f"but it was {type(d)}.")
 
         content = HTTPComponentContent.from_shodan(d)
         banner = d["data"]
         lines = banner.split("\r\n")
         headers = {}
+        banner_keys = lines[0]
         for line in lines:
             if ":" in line:
                 key, value = line.split(":", maxsplit=1)
                 headers[key.strip()] = value.strip()
 
         return HTTPComponent(
             headers=headers,
-            content=content
+            content=content,
+            shodan_headers_hash=d.get("http", {}).get("headers_hash", None)
         )
 
     @classmethod
     def from_censys(cls, d: Dict):
+        """Todo: Is parsing from services.banner better than just looping over the headers found by Censys?"""
         http = d["http"]["response"]
         headers = {}
         for k, v in http["headers"].items():
             if k[0] == "_":
                 continue
 
             headers.update({
                 k.replace("_", "-"): " ".join(v)
             })
+
+        banner_lines = d["banner"].replace("\r", "").split("\n")
+        banner_keys = banner_lines[0]
+        for line in banner_lines:
+            if ":" in line:
+                k, _ = line.split(":", maxsplit=1)
+                banner_keys += "\n" + k
+        headers_hash = mmh3.hash(banner_keys.encode("utf-8"))
+
         return HTTPComponent(
             headers=headers,
-            content=HTTPComponentContent.from_censys(d)
+            content=HTTPComponentContent.from_censys(d),
+            shodan_headers_hash=headers_hash
         )
 
     @classmethod
     def from_binaryedge(cls, d: Union[Dict, List]):
         http_response = d["result"]["data"]["response"]
         headers = http_response["headers"]["headers"]
         return HTTPComponent(
```

### Comparing `common-osint-model-0.4.7/common_osint_model/models/service.py` & `common-osint-model-0.4.9/common_osint_model/models/service.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/models/ssh.py` & `common-osint-model-0.4.9/common_osint_model/models/ssh.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/models/tls.py` & `common-osint-model-0.4.9/common_osint_model/models/tls.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         )
 
     @classmethod
     def from_censys(cls, d: Dict):
         """Creates an instance of this class based on Censys data given as dictionary."""
         if all(key not in d for key in ["common_name", "locality", "organization", "organizational_unit", "province"]):
             raise KeyError("The dictionary given to TLSComponentCertificateEntity.from_shodan is missing the typical "
-                           "shodan keys.")
+                           "censys keys.")
 
         c = d.get("country", [])
         st = d.get("province", [])
         l = d.get("locality", [])
         o = d.get("organization", [])
         ou = d.get("organizational_unit", [])
         cn = d.get("common_name", [])
@@ -313,15 +313,15 @@
             pem=pem,
             md5=md5,
             sha1=sha1,
             sha256=sha256
         )
 
 
-class TLSComponent(BaseModel, ShodanDataHandler, CensysDataHandler, BinaryEdgeDataHandler):
+class TLSComponent(BaseModel, ShodanDataHandler, CensysDataHandler, BinaryEdgeDataHandler, Logger):
     """Represents the TLS component of services."""
     certificate: TLSComponentCertificate
 
     # Todo: Add other attributes relevant to TLS such as CipherSuits etc.
 
     @classmethod
     def from_shodan(cls, d: Dict):
@@ -332,18 +332,23 @@
 
         return TLSComponent(
             certificate=TLSComponentCertificate.from_shodan(d)
         )
 
     @classmethod
     def from_censys(cls, d: Dict):
-        tls = d["tls"]
-        return TLSComponent(
-            certificate=TLSComponentCertificate.from_censys(tls["certificates"]["leaf_data"])
-        )
+        try:
+            tls = d["tls"]
+            return TLSComponent(
+                certificate=TLSComponentCertificate.from_censys(tls["certificates"]["leaf_data"])
+            )
+        except KeyError as e:
+            cls.error(f"Exception during certificate data extraction. "
+                      f"The key 'tls.certificates.leaf_data' is not available: {e}\nReturning None...")
+            return None
 
     @classmethod
     def from_binaryedge(cls, d: Union[Dict, List]):
         """Creates an instance of this class based on BinaryEdge data given as dictionary."""
         certificate_chain = d["result"]["data"]["cert_info"]["certificate_chain"]
         return TLSComponent(
             certificate=TLSComponentCertificate.from_binaryedge(certificate_chain[0])
```

### Comparing `common-osint-model-0.4.7/common_osint_model/shodan.py` & `common-osint-model-0.4.9/common_osint_model/shodan.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/common_osint_model/utils.py` & `common-osint-model-0.4.9/common_osint_model/utils.py`

 * *Files identical despite different names*

### Comparing `common-osint-model-0.4.7/pyproject.toml` & `common-osint-model-0.4.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "common-osint-model"
-version = "0.4.7"
+version = "0.4.9"
 description = "Converting data from services like BinaryEdge, Censys and Shodan to a common data model."
 authors = ["3c7 <3c7@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/3c7/common-osint-model"
 repository = "https://github.com/3c7/common-osint-model"
 classifiers = [
```

### Comparing `common-osint-model-0.4.7/setup.py` & `common-osint-model-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                      'convcensys2 = common_osint_model.cli:convcensys2',
                      'convcensyscert = common_osint_model.cli:convcensyscert',
                      'convcert = common_osint_model.cli:convcert',
                      'convshodan = common_osint_model.cli:convshodan']}
 
 setup_kwargs = {
     'name': 'common-osint-model',
-    'version': '0.4.7',
+    'version': '0.4.9',
     'description': 'Converting data from services like BinaryEdge, Censys and Shodan to a common data model.',
     'long_description': '# Common OSINT Model\n\n**Note:** This is work in progress and probably only covers my specific use case. If you find bugs or know how to\nenhance this project, please open an issue or - even better - create a pull request. The presented data model is\nevolving continuously. Therefore, it is recommended to use it in your project with a fixed version constraint (e.g. \n`common-osint-model==0.4.1`) and take a look at what has changed here before updating `common-osint-model` as a\ndependency.\n\nThis project aims to create an easy to use data model as well as implement converters for commonly used sources. As my\nuse case often includes HTTP(S), TLS and SSH only, data delivered for other protocols by the given sources might not\nshow up correctly or just by the banner included. Because the available scanning services use different hashes for \ndifferent purposes, one might be not able to search across services with the available data. This model automatically \ncalculates hashes wherever raw data is available.\n\n## Todos\n- [ ] Implement additional SSH ciphers for Censys data. Currently only RSA is supported. Censys do not provide raw \n public keys in their data, but the public key can be built through the components given.\n\n## The data model\n\n**Note:** The model was restructured with version 0.4.0. The previously provieded functionality can still be used,\nhowever, the old model is considered deprecated and is not further developed.\n\nSince version 0.4.0 the model changed. During refactoring, all model components were implemented as\n[pydantic](https://pydantic-docs.helpmanual.io/) classes in order to provide a more "pythonic" way of interacting with\nthe data. Also, this enables an easy to read and structurized view of the model itself. Please take a look at the model\nfiles available in [models](common_osint_model/models) for more details. The model starts with a host which has an IP,\ndomains pointing to it and provides multiple services:\n\n```python\nclass Host:\n    ip: str\n    autonomous_system: Optional[AutonomousSystem]\n    services: List[Service]\n    first_seen: Optional[datetime] = datetime.utcnow()\n    last_seen: Optional[datetime] = datetime.utcnow()\n    domains: Optional[List[Domain]]\n```\n\nA service listens on a specific port, has various components (currently only HTTP, TLS and SSH implemented), a banner\nand a source (e.g. Shodan) as well as some timestamps.\n\n```python\nclass Service:\n    port: int\n    banner: Optional[str]\n    md5: Optional[str]\n    sha1: Optional[str]\n    sha256: Optional[str]\n    murmur: Optional[str]\n    first_seen: Optional[datetime] = datetime.utcnow()\n    last_seen: Optional[datetime] = datetime.utcnow()\n    timestamp: Optional[datetime]\n    http: Optional[HTTPComponent]\n    tls: Optional[TLSComponent]\n    ssh: Optional[SSHComponent]\n    source: str\n```\n\nThe further model classes are designed in a similar way, please have a look at the\n[source files](common_osint_model/models).\n\n## How to use\n\n### Installation\n\n```bash\npip install common-osint-model\n```\n\n### Convert all the things\n\n```python\n# Post-v0.4.0 (Pydantic model)\nimport shodan\nfrom common_osint_model import Host\n\nshodan_client = shodan.Shodan("My API key")\nraw_shodan_response = shodan_client.host("140.82.121.4")\nhost = Host.from_shodan(raw_shodan_response)\n# Similarly:\n# Host.from_censys(raw_censys_response)\n# Host.from_binaryedge(raw_binaryedge_response)\n# Make sure to only pass results for *one* host. Currently there is no functionality provided to wrap around different \n# return types, such as lists of hosts from a query. You need to loop through them yourself.\nprint(f"Got {host.ip}.")\nprint(f"Providing {len(host.services)} services.")\n\nfor idx, service in enumerate(host.services):\n    print(f"Banner for Service {idx + 1}:")\n    print(f"\\t{service.banner}")\n    print(f"\\tMD5: {service.md5}")\n    print(f"\\tSHA1: {service.sha1}")\n    print(f"\\tSHA256: {service.sha256}")\n    print(f"\\tMurmur: {service.murmur}")\n\nprint("Exporting data as flattened json blob for further use, e.g. Elasticsearch indexing...")\nprint(host.flattened_json())\n\n# Pre-v0.4.0 (Dictionary based approach - DEPRECATED)\nfrom common_osint_model import from_shodan, from_shodan_flattened, from_censys_ipv4, from_censys_ipv4_flattened,\n    from_x509_pem, from_x509_pem_flattened\n\nraw_shodan = get_my_shodan_data()\nconverted_s = from_shodan(raw_shodan)  # Deprecated\nflattened_s = from_shodan_flattened(raw_shodan)  # Deprecated\n\nraw_censys_ipv4 = get_my_censys_ipv4_data()\nconverted_c = from_censys_ipv4(raw_censys_ipv4)\nflattened_c = from_censys_ipv4_flattened(raw_censys_ipv4)\n\nraw_certificate = open(\'certificate.pem\').read()\nconverted_certificate = from_x509_pem(raw_shodan)\nflattened_certificate = from_x509_pem_flattened(raw_shodan)\n```\n\n### Example output\n\n```python\nimport shodan\nfrom common_osint_model import Host\n\nshodan_client = shodan.Shodan("My API key")\nraw_shodan_response = shodan_client.host("140.82.121.4")\nhost = Host.from_shodan(raw_shodan_response)\nprint(f"Host: {host.ip}")\nprint(f"AS: {host.autonomous_system.dict(exclude_none=True)}")\n\nfor service in host.services:\n    print(f"Service: {service}")\n\nprint("--- flattened JSON dump ---")\nprint(host.flattened_json())\n```\n\n```\nHost: 140.82.121.4\nAS: {\'number\': 36459, \'name\': \'GitHub, Inc.\', \'country\': \'DE\', \'source\': \'shodan\'}\nService: port=443 banner=\'HTTP/1.1 301 Moved Permanently\\r\\nContent-Length: 0\\r\\nLocation: https://github.com/\\r\\n\\r\\n\' md5=\'d402a6212741f3690b4fa1e46d9bd8b6\' sha1=\'a24eb4ba0332776d38050a7b41d0366742dbf262\' sha256=\'5fbe0315395986d131e4948888987319e88e3e1da6c5460e8a0bf8b7a1e639f0\' murmur=\'-1655207803\' first_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656097) last_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656099) timestamp=datetime.datetime(2021, 8, 16, 20, 42, 40, 325940) http=HTTPComponent(headers={\'Content-Length\': \'0\', \'Location\': \'https://github.com/\'}, content=HTTPComponentContent(raw=\'\', length=0, md5=\'d41d8cd98f00b204e9800998ecf8427e\', sha1=\'da39a3ee5e6b4b0d3255bfef95601890afd80709\', sha256=\'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855\', murmur=\'0\', favicon=None, robots_txt=None, security_txt=None)) tls=TLSComponent(certificate=TLSComponentCertificate(issuer=TLSComponentCertificateEntity(dn=\'C=US, O=DigiCert, Inc., CN=DigiCert High Assurance TLS Hybrid ECC SHA256 2020 CA1\', country=\'US\', state=None, locality=None, organization=\'DigiCert, Inc.\', organizational_unit=None, common_name=\'DigiCert High Assurance TLS Hybrid ECC SHA256 2020 CA1\', email_address=None), subject=TLSComponentCertificateEntity(dn=\'C=US, ST=California, L=San Francisco, O=GitHub, Inc., CN=github.com\', country=\'US\', state=\'California\', locality=\'San Francisco\', organization=\'GitHub, Inc.\', organizational_unit=None, common_name=\'github.com\', email_address=None), issued=datetime.datetime(2021, 3, 25, 0, 0), expires=datetime.datetime(2022, 3, 30, 23, 59, 59), expired=False, alternative_names=[\'www.github.com\', \'github.com\'], pem=\'-----BEGIN CERTIFICATE-----\\nMIIFBjCCBK2gAwIBAgIQDovzdw2S0Zbwu2H5PEFmvjAKBggqhkjOPQQDAjBnMQsw\\nCQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQsIEluYy4xPzA9BgNVBAMTNkRp\\nZ2lDZXJ0IEhpZ2ggQXNzdXJhbmNlIFRMUyBIeWJyaWQgRUNDIFNIQTI1NiAyMDIw\\nIENBMTAeFw0yMTAzMjUwMDAwMDBaFw0yMjAzMzAyMzU5NTlaMGYxCzAJBgNVBAYT\\nAlVTMRMwEQYDVQQIEwpDYWxpZm9ybmlhMRYwFAYDVQQHEw1TYW4gRnJhbmNpc2Nv\\nMRUwEwYDVQQKEwxHaXRIdWIsIEluYy4xEzARBgNVBAMTCmdpdGh1Yi5jb20wWTAT\\nBgcqhkjOPQIBBggqhkjOPQMBBwNCAASt9vd1sdNJVApdEHG93CUGSyIcoiNOn6H+\\nudCMvTm8DCPHz5GmkFrYRasDE77BI3q5xMidR/aW4Ll2a1A2ZvcNo4IDOjCCAzYw\\nHwYDVR0jBBgwFoAUUGGmoNI1xBEqII0fD6xC8M0pz0swHQYDVR0OBBYEFCexfp+7\\nJplQ2PPDU1v+MRawux5yMCUGA1UdEQQeMByCCmdpdGh1Yi5jb22CDnd3dy5naXRo\\ndWIuY29tMA4GA1UdDwEB/wQEAwIHgDAdBgNVHSUEFjAUBggrBgEFBQcDAQYIKwYB\\nBQUHAwIwgbEGA1UdHwSBqTCBpjBRoE+gTYZLaHR0cDovL2NybDMuZGlnaWNlcnQu\\nY29tL0RpZ2lDZXJ0SGlnaEFzc3VyYW5jZVRMU0h5YnJpZEVDQ1NIQTI1NjIwMjBD\\nQTEuY3JsMFGgT6BNhktodHRwOi8vY3JsNC5kaWdpY2VydC5jb20vRGlnaUNlcnRI\\naWdoQXNzdXJhbmNlVExTSHlicmlkRUNDU0hBMjU2MjAyMENBMS5jcmwwPgYDVR0g\\nBDcwNTAzBgZngQwBAgIwKTAnBggrBgEFBQcCARYbaHR0cDovL3d3dy5kaWdpY2Vy\\ndC5jb20vQ1BTMIGSBggrBgEFBQcBAQSBhTCBgjAkBggrBgEFBQcwAYYYaHR0cDov\\nL29jc3AuZGlnaWNlcnQuY29tMFoGCCsGAQUFBzAChk5odHRwOi8vY2FjZXJ0cy5k\\naWdpY2VydC5jb20vRGlnaUNlcnRIaWdoQXNzdXJhbmNlVExTSHlicmlkRUNDU0hB\\nMjU2MjAyMENBMS5jcnQwDAYDVR0TAQH/BAIwADCCAQUGCisGAQQB1nkCBAIEgfYE\\ngfMA8QB2ACl5vvCeOTkh8FZzn2Old+W+V32cYAr4+U1dJlwlXceEAAABeGq/vRoA\\nAAQDAEcwRQIhAJ7miER//DRFnDJNn6uUhgau3WMt4vVfY5dGigulOdjXAiBIVCfR\\nxjK1v4F31+sVaKzyyO7JAa0fzDQM7skQckSYWQB3ACJFRQdZVSRWlj+hL/H3bYbg\\nIyZjrcBLf13Gg1xu4g8CAAABeGq/vTkAAAQDAEgwRgIhAJgAEkoJQRivBlwo7x67\\n3oVsf1ip096WshZqmRCuL/JpAiEA3cX4rb3waLDLq4C48NSoUmcw56PwO/m2uwnQ\\nprb+yh0wCgYIKoZIzj0EAwIDRwAwRAIgK+Kv7G+/KkWkNZg3PcQFp866Z7G6soxo\\na4etSZ+SRlYCIBSiXS20Wc+yjD111nPzvQUCfsP4+DKZ3K+2GKsERD6d\\n-----END CERTIFICATE-----\\n\', md5=\'a07ee2076a6e392e1e96481e99ba094b\', sha1=\'8463b3a92912ccfd1d314705989bec139937d0d7\', sha256=\'0ae384bfd4dde9d13e50c5857c05a442c93f8e01445ee4b34540d22bd1e37f1b\', murmur=None)) ssh=None source=\'shodan\'\n\nService: port=80 banner=\'HTTP/1.1 301 Moved Permanently\\r\\nContent-Length: 0\\r\\nLocation: https://140.82.121.4/\\r\\n\\r\\n\' md5=\'86c9c13165fff2c41db667dd1f6500db\' sha1=\'8ecee0314c63c092d449b0d37d00f0ff62448dd1\' sha256=\'715fd6cec44f12bb5e59f57bf9a1691708a5a2d2ef253399358ac3ff88f47781\' murmur=\'1256792822\' first_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656097) last_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656099) timestamp=datetime.datetime(2021, 8, 16, 20, 42, 38, 12570) http=HTTPComponent(headers={\'Content-Length\': \'0\', \'Location\': \'https://140.82.121.4/\'}, content=HTTPComponentContent(raw=\'\', length=0, md5=\'d41d8cd98f00b204e9800998ecf8427e\', sha1=\'da39a3ee5e6b4b0d3255bfef95601890afd80709\', sha256=\'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855\', murmur=\'0\', favicon=None, robots_txt=None, security_txt=None)) tls=None ssh=None source=\'shodan\'\n\nService: port=9418 banner=\'0020ERR \\n  Repository not found.\' md5=\'fc79d10176a28462bc071909fb99d59e\' sha1=\'0df752dd6b3d3a461f30691ff89ee67ef3dd21b1\' sha256=\'5f355dafa7999d06265bb17e949b76eab283e9966ef8e27908c4e1058a891121\' murmur=\'-1636861384\' first_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656097) last_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656099) timestamp=datetime.datetime(2021, 8, 12, 2, 10, 13, 136596) http=None tls=None ssh=None source=\'shodan\'\n\nService: port=22 banner=\'SSH-2.0-babeld-968490c5\\nKey type: ssh-rsa\\nKey: AAAAB3NzaC1yc2EAAAABIwAAAQEAq2A7hRGmdnm9tUDbO9IDSwBK6TbQa+PXYPCPy6rbTrTtw7PH\\nkccKrpp0yVhp5HdEIcKr6pLlVDBfOLX9QUsyCOV0wzfjIJNlGEYsdlLJizHhbn2mUjvSAHQqZETY\\nP81eFzLQNnPHt4EVVUh7VfDESU84KezmD5QlWpXLmvU31/yMf+Se8xhHTvKSCZIFImWwoG6mbUoW\\nf9nzpIoaSjB+weqqUUmpaaasXVal72J+UX2B+2RPW3RcT0eOzQgqlJL3RKrTJvdsjE3JEAvGq3lG\\nHSZXy28G3skua2SmVi/w4yCE6gbODqnTWlg7+wC604ydGXA8VJiS5ap43JXiUFFAaQ==\\nFingerprint: 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48\\n\\nKex Algorithms:\\n\\tcurve25519-sha256\\n\\tcurve25519-sha256@libssh.org\\n\\tecdh-sha2-nistp256\\n\\tecdh-sha2-nistp384\\n\\tecdh-sha2-nistp521\\n\\tdiffie-hellman-group-exchange-sha256\\n\\nServer Host Key Algorithms:\\n\\trsa-sha2-512\\n\\trsa-sha2-256\\n\\tssh-rsa\\n\\tssh-dss\\n\\nEncryption Algorithms:\\n\\tchacha20-poly1305@openssh.com\\n\\taes256-gcm@openssh.com\\n\\taes128-gcm@openssh.com\\n\\taes256-ctr\\n\\taes192-ctr\\n\\taes128-ctr\\n\\taes256-cbc\\n\\taes192-cbc\\n\\taes128-cbc\\n\\nMAC Algorithms:\\n\\thmac-sha2-512-etm@openssh.com\\n\\thmac-sha2-256-etm@openssh.com\\n\\thmac-sha2-512\\n\\thmac-sha2-256\\n\\thmac-sha1-etm@openssh.com\\n\\thmac-sha1\\n\\nCompression Algorithms:\\n\\tnone\\n\\n\' md5=\'d652c84a47553c66047cf67e51f1345a\' sha1=\'679cc04ce70413f639351328bb2f0a70545d0cb6\' sha256=\'2431ffe5d8acbb77b6db91ee84f75baa0422d56947e0b85331dde2560e5454d5\' murmur=\'1023136053\' first_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656097) last_seen=datetime.datetime(2021, 8, 20, 16, 10, 27, 656099) timestamp=datetime.datetime(2021, 8, 3, 21, 10, 29, 568093) http=None tls=None ssh=SSHComponent(algorithms=SSHComponentAlgorithms(encryption=[\'chacha20-poly1305@openssh.com\', \'aes256-gcm@openssh.com\', \'aes128-gcm@openssh.com\', \'aes256-ctr\', \'aes192-ctr\', \'aes128-ctr\', \'aes256-cbc\', \'aes192-cbc\', \'aes128-cbc\'], key_exchange=[\'curve25519-sha256\', \'curve25519-sha256@libssh.org\', \'ecdh-sha2-nistp256\', \'ecdh-sha2-nistp384\', \'ecdh-sha2-nistp521\', \'diffie-hellman-group-exchange-sha256\'], mac=[\'hmac-sha2-512-etm@openssh.com\', \'hmac-sha2-256-etm@openssh.com\', \'hmac-sha2-512\', \'hmac-sha2-256\', \'hmac-sha1-etm@openssh.com\', \'hmac-sha1\'], key_algorithms=[\'rsa-sha2-512\', \'rsa-sha2-256\', \'ssh-rsa\', \'ssh-dss\'], compression=[\'none\']), key=SSHComponentKey(raw=\'AAAAB3NzaC1yc2EAAAABIwAAAQEAq2A7hRGmdnm9tUDbO9IDSwBK6TbQa+PXYPCPy6rbTrTtw7PH\\nkccKrpp0yVhp5HdEIcKr6pLlVDBfOLX9QUsyCOV0wzfjIJNlGEYsdlLJizHhbn2mUjvSAHQqZETY\\nP81eFzLQNnPHt4EVVUh7VfDESU84KezmD5QlWpXLmvU31/yMf+Se8xhHTvKSCZIFImWwoG6mbUoW\\nf9nzpIoaSjB+weqqUUmpaaasXVal72J+UX2B+2RPW3RcT0eOzQgqlJL3RKrTJvdsjE3JEAvGq3lG\\nHSZXy28G3skua2SmVi/w4yCE6gbODqnTWlg7+wC604ydGXA8VJiS5ap43JXiUFFAaQ==\\n\', type=\'ssh-rsa\', md5=\'1627aca576282d36631b564debdfa648\', sha1=\'bf6b6825d2977c511a475bbefb88aad54a92ac73\', sha256=\'9d385b83a9175292561a5ec4d4818e0aca51a264f17420112ef88ac3a139498f\', murmur=\'-388505952\')) source=\'shodan\'\n\n--- flattened JSON dump ---\n{\n  "443.port": 443,\n  "443.banner": "HTTP/1.1 301 Moved Permanently\\r\\nContent-Length: 0\\r\\nLocation: https://github.com/\\r\\n\\r\\n",\n  "443.md5": "d402a6212741f3690b4fa1e46d9bd8b6",\n  "443.sha1": "a24eb4ba0332776d38050a7b41d0366742dbf262",\n  "443.sha256": "5fbe0315395986d131e4948888987319e88e3e1da6c5460e8a0bf8b7a1e639f0",\n  "443.murmur": "-1655207803",\n  "443.first_seen": "2021-08-20T16:10:27.656097",\n  "443.last_seen": "2021-08-20T16:10:27.656099",\n  "443.timestamp": "2021-08-16T20:42:40.325940",\n  "443.http.headers.Content-Length": "0",\n  "443.http.headers.Location": "https://github.com/",\n  "443.http.content.raw": "",\n  "443.http.content.length": 0,\n  "443.http.content.md5": "d41d8cd98f00b204e9800998ecf8427e",\n  "443.http.content.sha1": "da39a3ee5e6b4b0d3255bfef95601890afd80709",\n  "443.http.content.sha256": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",\n  "443.http.content.murmur": "0",\n  "443.tls.certificate.issuer.dn": "C=US, O=DigiCert, Inc., CN=DigiCert High Assurance TLS Hybrid ECC SHA256 2020 CA1",\n  "443.tls.certificate.issuer.country": "US",\n  "443.tls.certificate.issuer.organization": "DigiCert, Inc.",\n  "443.tls.certificate.issuer.common_name": "DigiCert High Assurance TLS Hybrid ECC SHA256 2020 CA1",\n  "443.tls.certificate.subject.dn": "C=US, ST=California, L=San Francisco, O=GitHub, Inc., CN=github.com",\n  "443.tls.certificate.subject.country": "US",\n  "443.tls.certificate.subject.state": "California",\n  "443.tls.certificate.subject.locality": "San Francisco",\n  "443.tls.certificate.subject.organization": "GitHub, Inc.",\n  "443.tls.certificate.subject.common_name": "github.com",\n  "443.tls.certificate.issued": "2021-03-25T00:00:00",\n  "443.tls.certificate.expires": "2022-03-30T23:59:59",\n  "443.tls.certificate.expired": false,\n  "443.tls.certificate.alternative_names": [\n    "www.github.com",\n    "github.com"\n  ],\n  "443.tls.certificate.pem": "-----BEGIN CERTIFICATE-----\\nMIIFBjCCBK2gAwIBAgIQDovzdw2S0Zbwu2H5PEFmvjAKBggqhkjOPQQDAjBnMQsw\\nCQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQsIEluYy4xPzA9BgNVBAMTNkRp\\nZ2lDZXJ0IEhpZ2ggQXNzdXJhbmNlIFRMUyBIeWJyaWQgRUNDIFNIQTI1NiAyMDIw\\nIENBMTAeFw0yMTAzMjUwMDAwMDBaFw0yMjAzMzAyMzU5NTlaMGYxCzAJBgNVBAYT\\nAlVTMRMwEQYDVQQIEwpDYWxpZm9ybmlhMRYwFAYDVQQHEw1TYW4gRnJhbmNpc2Nv\\nMRUwEwYDVQQKEwxHaXRIdWIsIEluYy4xEzARBgNVBAMTCmdpdGh1Yi5jb20wWTAT\\nBgcqhkjOPQIBBggqhkjOPQMBBwNCAASt9vd1sdNJVApdEHG93CUGSyIcoiNOn6H+\\nudCMvTm8DCPHz5GmkFrYRasDE77BI3q5xMidR/aW4Ll2a1A2ZvcNo4IDOjCCAzYw\\nHwYDVR0jBBgwFoAUUGGmoNI1xBEqII0fD6xC8M0pz0swHQYDVR0OBBYEFCexfp+7\\nJplQ2PPDU1v+MRawux5yMCUGA1UdEQQeMByCCmdpdGh1Yi5jb22CDnd3dy5naXRo\\ndWIuY29tMA4GA1UdDwEB/wQEAwIHgDAdBgNVHSUEFjAUBggrBgEFBQcDAQYIKwYB\\nBQUHAwIwgbEGA1UdHwSBqTCBpjBRoE+gTYZLaHR0cDovL2NybDMuZGlnaWNlcnQu\\nY29tL0RpZ2lDZXJ0SGlnaEFzc3VyYW5jZVRMU0h5YnJpZEVDQ1NIQTI1NjIwMjBD\\nQTEuY3JsMFGgT6BNhktodHRwOi8vY3JsNC5kaWdpY2VydC5jb20vRGlnaUNlcnRI\\naWdoQXNzdXJhbmNlVExTSHlicmlkRUNDU0hBMjU2MjAyMENBMS5jcmwwPgYDVR0g\\nBDcwNTAzBgZngQwBAgIwKTAnBggrBgEFBQcCARYbaHR0cDovL3d3dy5kaWdpY2Vy\\ndC5jb20vQ1BTMIGSBggrBgEFBQcBAQSBhTCBgjAkBggrBgEFBQcwAYYYaHR0cDov\\nL29jc3AuZGlnaWNlcnQuY29tMFoGCCsGAQUFBzAChk5odHRwOi8vY2FjZXJ0cy5k\\naWdpY2VydC5jb20vRGlnaUNlcnRIaWdoQXNzdXJhbmNlVExTSHlicmlkRUNDU0hB\\nMjU2MjAyMENBMS5jcnQwDAYDVR0TAQH/BAIwADCCAQUGCisGAQQB1nkCBAIEgfYE\\ngfMA8QB2ACl5vvCeOTkh8FZzn2Old+W+V32cYAr4+U1dJlwlXceEAAABeGq/vRoA\\nAAQDAEcwRQIhAJ7miER//DRFnDJNn6uUhgau3WMt4vVfY5dGigulOdjXAiBIVCfR\\nxjK1v4F31+sVaKzyyO7JAa0fzDQM7skQckSYWQB3ACJFRQdZVSRWlj+hL/H3bYbg\\nIyZjrcBLf13Gg1xu4g8CAAABeGq/vTkAAAQDAEgwRgIhAJgAEkoJQRivBlwo7x67\\n3oVsf1ip096WshZqmRCuL/JpAiEA3cX4rb3waLDLq4C48NSoUmcw56PwO/m2uwnQ\\nprb+yh0wCgYIKoZIzj0EAwIDRwAwRAIgK+Kv7G+/KkWkNZg3PcQFp866Z7G6soxo\\na4etSZ+SRlYCIBSiXS20Wc+yjD111nPzvQUCfsP4+DKZ3K+2GKsERD6d\\n-----END CERTIFICATE-----\\n",\n  "443.tls.certificate.md5": "a07ee2076a6e392e1e96481e99ba094b",\n  "443.tls.certificate.sha1": "8463b3a92912ccfd1d314705989bec139937d0d7",\n  "443.tls.certificate.sha256": "0ae384bfd4dde9d13e50c5857c05a442c93f8e01445ee4b34540d22bd1e37f1b",\n  "443.source": "shodan",\n  "80.port": 80,\n  "80.banner": "HTTP/1.1 301 Moved Permanently\\r\\nContent-Length: 0\\r\\nLocation: https://140.82.121.4/\\r\\n\\r\\n",\n  "80.md5": "86c9c13165fff2c41db667dd1f6500db",\n  "80.sha1": "8ecee0314c63c092d449b0d37d00f0ff62448dd1",\n  "80.sha256": "715fd6cec44f12bb5e59f57bf9a1691708a5a2d2ef253399358ac3ff88f47781",\n  "80.murmur": "1256792822",\n  "80.first_seen": "2021-08-20T16:10:27.656097",\n  "80.last_seen": "2021-08-20T16:10:27.656099",\n  "80.timestamp": "2021-08-16T20:42:38.012570",\n  "80.http.headers.Content-Length": "0",\n  "80.http.headers.Location": "https://140.82.121.4/",\n  "80.http.content.raw": "",\n  "80.http.content.length": 0,\n  "80.http.content.md5": "d41d8cd98f00b204e9800998ecf8427e",\n  "80.http.content.sha1": "da39a3ee5e6b4b0d3255bfef95601890afd80709",\n  "80.http.content.sha256": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",\n  "80.http.content.murmur": "0",\n  "80.source": "shodan",\n  "9418.port": 9418,\n  "9418.banner": "0020ERR \\n  Repository not found.",\n  "9418.md5": "fc79d10176a28462bc071909fb99d59e",\n  "9418.sha1": "0df752dd6b3d3a461f30691ff89ee67ef3dd21b1",\n  "9418.sha256": "5f355dafa7999d06265bb17e949b76eab283e9966ef8e27908c4e1058a891121",\n  "9418.murmur": "-1636861384",\n  "9418.first_seen": "2021-08-20T16:10:27.656097",\n  "9418.last_seen": "2021-08-20T16:10:27.656099",\n  "9418.timestamp": "2021-08-12T02:10:13.136596",\n  "9418.source": "shodan",\n  "22.port": 22,\n  "22.banner": "SSH-2.0-babeld-968490c5\\nKey type: ssh-rsa\\nKey: AAAAB3NzaC1yc2EAAAABIwAAAQEAq2A7hRGmdnm9tUDbO9IDSwBK6TbQa+PXYPCPy6rbTrTtw7PH\\nkccKrpp0yVhp5HdEIcKr6pLlVDBfOLX9QUsyCOV0wzfjIJNlGEYsdlLJizHhbn2mUjvSAHQqZETY\\nP81eFzLQNnPHt4EVVUh7VfDESU84KezmD5QlWpXLmvU31/yMf+Se8xhHTvKSCZIFImWwoG6mbUoW\\nf9nzpIoaSjB+weqqUUmpaaasXVal72J+UX2B+2RPW3RcT0eOzQgqlJL3RKrTJvdsjE3JEAvGq3lG\\nHSZXy28G3skua2SmVi/w4yCE6gbODqnTWlg7+wC604ydGXA8VJiS5ap43JXiUFFAaQ==\\nFingerprint: 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48\\n\\nKex Algorithms:\\n\\tcurve25519-sha256\\n\\tcurve25519-sha256@libssh.org\\n\\tecdh-sha2-nistp256\\n\\tecdh-sha2-nistp384\\n\\tecdh-sha2-nistp521\\n\\tdiffie-hellman-group-exchange-sha256\\n\\nServer Host Key Algorithms:\\n\\trsa-sha2-512\\n\\trsa-sha2-256\\n\\tssh-rsa\\n\\tssh-dss\\n\\nEncryption Algorithms:\\n\\tchacha20-poly1305@openssh.com\\n\\taes256-gcm@openssh.com\\n\\taes128-gcm@openssh.com\\n\\taes256-ctr\\n\\taes192-ctr\\n\\taes128-ctr\\n\\taes256-cbc\\n\\taes192-cbc\\n\\taes128-cbc\\n\\nMAC Algorithms:\\n\\thmac-sha2-512-etm@openssh.com\\n\\thmac-sha2-256-etm@openssh.com\\n\\thmac-sha2-512\\n\\thmac-sha2-256\\n\\thmac-sha1-etm@openssh.com\\n\\thmac-sha1\\n\\nCompression Algorithms:\\n\\tnone\\n\\n",\n  "22.md5": "d652c84a47553c66047cf67e51f1345a",\n  "22.sha1": "679cc04ce70413f639351328bb2f0a70545d0cb6",\n  "22.sha256": "2431ffe5d8acbb77b6db91ee84f75baa0422d56947e0b85331dde2560e5454d5",\n  "22.murmur": "1023136053",\n  "22.first_seen": "2021-08-20T16:10:27.656097",\n  "22.last_seen": "2021-08-20T16:10:27.656099",\n  "22.timestamp": "2021-08-03T21:10:29.568093",\n  "22.ssh.algorithms.encryption": [\n    "chacha20-poly1305@openssh.com",\n    "aes256-gcm@openssh.com",\n    "aes128-gcm@openssh.com",\n    "aes256-ctr",\n    "aes192-ctr",\n    "aes128-ctr",\n    "aes256-cbc",\n    "aes192-cbc",\n    "aes128-cbc"\n  ],\n  "22.ssh.algorithms.key_exchange": [\n    "curve25519-sha256",\n    "curve25519-sha256@libssh.org",\n    "ecdh-sha2-nistp256",\n    "ecdh-sha2-nistp384",\n    "ecdh-sha2-nistp521",\n    "diffie-hellman-group-exchange-sha256"\n  ],\n  "22.ssh.algorithms.mac": [\n    "hmac-sha2-512-etm@openssh.com",\n    "hmac-sha2-256-etm@openssh.com",\n    "hmac-sha2-512",\n    "hmac-sha2-256",\n    "hmac-sha1-etm@openssh.com",\n    "hmac-sha1"\n  ],\n  "22.ssh.algorithms.key_algorithms": [\n    "rsa-sha2-512",\n    "rsa-sha2-256",\n    "ssh-rsa",\n    "ssh-dss"\n  ],\n  "22.ssh.algorithms.compression": [\n    "none"\n  ],\n  "22.ssh.key.raw": "AAAAB3NzaC1yc2EAAAABIwAAAQEAq2A7hRGmdnm9tUDbO9IDSwBK6TbQa+PXYPCPy6rbTrTtw7PH\\nkccKrpp0yVhp5HdEIcKr6pLlVDBfOLX9QUsyCOV0wzfjIJNlGEYsdlLJizHhbn2mUjvSAHQqZETY\\nP81eFzLQNnPHt4EVVUh7VfDESU84KezmD5QlWpXLmvU31/yMf+Se8xhHTvKSCZIFImWwoG6mbUoW\\nf9nzpIoaSjB+weqqUUmpaaasXVal72J+UX2B+2RPW3RcT0eOzQgqlJL3RKrTJvdsjE3JEAvGq3lG\\nHSZXy28G3skua2SmVi/w4yCE6gbODqnTWlg7+wC604ydGXA8VJiS5ap43JXiUFFAaQ==\\n",\n  "22.ssh.key.type": "ssh-rsa",\n  "22.ssh.key.md5": "1627aca576282d36631b564debdfa648",\n  "22.ssh.key.sha1": "bf6b6825d2977c511a475bbefb88aad54a92ac73",\n  "22.ssh.key.sha256": "9d385b83a9175292561a5ec4d4818e0aca51a264f17420112ef88ac3a139498f",\n  "22.ssh.key.murmur": "-388505952",\n  "22.source": "shodan"\n}\n```',
     'author': '3c7',
     'author_email': '3c7@posteo.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/3c7/common-osint-model',
```

### Comparing `common-osint-model-0.4.7/PKG-INFO` & `common-osint-model-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-osint-model
-Version: 0.4.7
+Version: 0.4.9
 Summary: Converting data from services like BinaryEdge, Censys and Shodan to a common data model.
 Home-page: https://github.com/3c7/common-osint-model
 License: MIT
 Author: 3c7
 Author-email: 3c7@posteo.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

