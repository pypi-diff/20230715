# Comparing `tmp/apiosintDS-2.0.tar.gz` & `tmp/apiosintDS-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiosintDS-2.0.tar", last modified: Fri Jul  7 23:14:31 2023, max compression
+gzip compressed data, was "apiosintDS-2.0.1.tar", last modified: Sat Jul 15 10:16:41 2023, max compression
```

## Comparing `apiosintDS-2.0.tar` & `apiosintDS-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-07 23:14:31.212091 apiosintDS-2.0/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1072 2023-06-27 15:06:33.000000 apiosintDS-2.0/LICENSE.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)    17873 2023-07-07 23:14:31.212091 apiosintDS-2.0/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)    17177 2023-07-07 23:12:25.000000 apiosintDS-2.0/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-07 23:14:31.212091 apiosintDS-2.0/apiosintDS/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2023-06-27 15:06:33.000000 apiosintDS-2.0/apiosintDS/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    15960 2023-07-07 08:51:02.000000 apiosintDS-2.0/apiosintDS/apiosintDS.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-07 23:14:31.212091 apiosintDS-2.0/apiosintDS/modules/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2023-06-27 15:06:33.000000 apiosintDS-2.0/apiosintDS/modules/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    11304 2023-07-07 22:35:32.000000 apiosintDS-2.0/apiosintDS/modules/dosearch.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    13507 2023-07-03 05:49:06.000000 apiosintDS-2.0/apiosintDS/modules/listutils.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      726 2023-07-01 15:42:49.000000 apiosintDS-2.0/apiosintDS/modules/scriptinfo.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     8506 2023-07-01 08:44:22.000000 apiosintDS-2.0/apiosintDS/modules/stixreport.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-07 23:14:31.212091 apiosintDS-2.0/apiosintDS/schema/
--rw-rw-r--   0 davide    (1000) davide    (1000)    56184 2023-07-06 19:00:23.000000 apiosintDS-2.0/apiosintDS/schema/schema.json
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-07 23:14:31.212091 apiosintDS-2.0/apiosintDS/utilities/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2023-06-27 15:06:33.000000 apiosintDS-2.0/apiosintDS/utilities/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2150 2023-06-30 16:39:24.000000 apiosintDS-2.0/apiosintDS/utilities/logutils.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    15965 2023-07-07 07:35:33.000000 apiosintDS-2.0/apiosintDS/utilities/prettycli.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-07 23:14:31.212091 apiosintDS-2.0/apiosintDS.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)    17873 2023-07-07 23:14:31.000000 apiosintDS-2.0/apiosintDS.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      584 2023-07-07 23:14:31.000000 apiosintDS-2.0/apiosintDS.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-07-07 23:14:31.000000 apiosintDS-2.0/apiosintDS.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       59 2023-07-07 23:14:31.000000 apiosintDS-2.0/apiosintDS.egg-info/entry_points.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       55 2023-07-07 23:14:31.000000 apiosintDS-2.0/apiosintDS.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       11 2023-07-07 23:14:31.000000 apiosintDS-2.0/apiosintDS.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       79 2023-07-07 23:14:31.212091 apiosintDS-2.0/setup.cfg
--rw-rw-r--   0 davide    (1000) davide    (1000)     3195 2023-07-07 17:15:24.000000 apiosintDS-2.0/setup.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-15 10:16:41.967698 apiosintDS-2.0.1/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1072 2023-06-27 15:06:33.000000 apiosintDS-2.0.1/LICENSE.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)    18120 2023-07-15 10:16:41.967698 apiosintDS-2.0.1/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)    17422 2023-07-09 09:02:38.000000 apiosintDS-2.0.1/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-15 10:16:41.967698 apiosintDS-2.0.1/apiosintDS/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2023-06-27 15:06:33.000000 apiosintDS-2.0.1/apiosintDS/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15960 2023-07-07 08:51:02.000000 apiosintDS-2.0.1/apiosintDS/apiosintDS.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-15 10:16:41.967698 apiosintDS-2.0.1/apiosintDS/modules/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2023-06-27 15:06:33.000000 apiosintDS-2.0.1/apiosintDS/modules/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11304 2023-07-07 22:35:32.000000 apiosintDS-2.0.1/apiosintDS/modules/dosearch.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    13507 2023-07-03 05:49:06.000000 apiosintDS-2.0.1/apiosintDS/modules/listutils.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      726 2023-07-01 15:42:49.000000 apiosintDS-2.0.1/apiosintDS/modules/scriptinfo.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8511 2023-07-15 10:02:44.000000 apiosintDS-2.0.1/apiosintDS/modules/stixreport.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-15 10:16:41.967698 apiosintDS-2.0.1/apiosintDS/schema/
+-rw-rw-r--   0 davide    (1000) davide    (1000)    56184 2023-07-06 19:00:23.000000 apiosintDS-2.0.1/apiosintDS/schema/schema.json
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-15 10:16:41.967698 apiosintDS-2.0.1/apiosintDS/utilities/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2023-06-27 15:06:33.000000 apiosintDS-2.0.1/apiosintDS/utilities/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2150 2023-06-30 16:39:24.000000 apiosintDS-2.0.1/apiosintDS/utilities/logutils.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    15965 2023-07-07 07:35:33.000000 apiosintDS-2.0.1/apiosintDS/utilities/prettycli.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-15 10:16:41.967698 apiosintDS-2.0.1/apiosintDS.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)    18120 2023-07-15 10:16:41.000000 apiosintDS-2.0.1/apiosintDS.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      584 2023-07-15 10:16:41.000000 apiosintDS-2.0.1/apiosintDS.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-07-15 10:16:41.000000 apiosintDS-2.0.1/apiosintDS.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       59 2023-07-15 10:16:41.000000 apiosintDS-2.0.1/apiosintDS.egg-info/entry_points.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       55 2023-07-15 10:16:41.000000 apiosintDS-2.0.1/apiosintDS.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       11 2023-07-15 10:16:41.000000 apiosintDS-2.0.1/apiosintDS.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       79 2023-07-15 10:16:41.971698 apiosintDS-2.0.1/setup.cfg
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3197 2023-07-15 10:15:01.000000 apiosintDS-2.0.1/setup.py
```

### Comparing `apiosintDS-2.0/LICENSE.txt` & `apiosintDS-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/PKG-INFO` & `apiosintDS-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiosintDS
-Version: 2.0
+Version: 2.0.1
 Summary: On demand query API for OSINT.digitalside.it project. You can query for souspicious domains, urls, IPv4 and file hashes.
 Home-page: https://github.com/davidonzo/apiosintDS
 Author: Davide Baglieri
 Author-email: info@digitalside.it
 License: MIT
 Keywords: apiosintDS,OSINT,Threat-Intel,IoC,Security
 Platform: UNKNOWN
@@ -16,20 +16,22 @@
 Requires-Python: >3.5.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # apiosintDS
 Latest stable release is **v2.0**
 
-**apiosintDS** is a [python client library](https://github.com/davidonzo/apiosintDS) for public *API* lookup service over *OSINT* IoCs stored  at [DigitalSide Threat-Intel](https://osint.digitalside.it) repository. It can be defined a **service as a library** tool designed to act both as a standard Python library to be included in your own Python application and as command line tool. Query can be performed against souspicious IPs, domains, urls and file hashes. Data stored has a 7 days retention.
+**apiosintDS** is a [python client library](https://github.com/davidonzo/apiosintDS) for public *API* lookup service over *OSINT* IoCs stored  at [DigitalSide Threat-Intel](https://osint.digitalside.it) repository. It can be defined a **Service as a Library** tool designed to act both as a standard Python library to be included in your own Python application and as command line tool. Query can be performed against souspicious IPs, domains, urls and file hashes. Data stored has a 7 days retention.
 
 ![apiosintDS v2.0](https://raw.githubusercontent.com/davidonzo/apiosintDS/master/docs/_static/img/apiosintDS.png)
 
 [DigitalSide Threat-Intel (also on GitHub.com)](https://github.com/davidonzo/Threat-Intel) shares a set of **Open Source Cyber Threat Intellegence** information, monstly based on malware analysis and compromised URLs, IPs and domains. The purpose of the project is to develop and test new wayes to hunt, analyze, collect and share relevants sets of IoCs to be used by SOC/CSIRT/CERT with minimun effort. 
 
+**apiosintDS** is also available as [enrichment MISP Modules](https://misp.github.io/misp-modules/expansion/#apiosintds). Documentation is available on [apiosintDS Read The Docs](https://apiosintds.readthedocs.io/en/latest/userguidemisp.html).
+
 This library has been specially designed for people and organizations don't want to import the whole [DigitalSide Threat-Intel](https://osint.digitalside.it) dataset and prefer to use it as an on demand service.
 
 ## Documentation
 Complete documentation availables at [apiosintDS.ReadTheDocs.org](https://apiosintds.readthedocs.io/en/latest/)
 
 ## Install
 ### The easy way via pip
```

### Comparing `apiosintDS-2.0/README.md` & `apiosintDS-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # apiosintDS
 Latest stable release is **v2.0**
 
-**apiosintDS** is a [python client library](https://github.com/davidonzo/apiosintDS) for public *API* lookup service over *OSINT* IoCs stored  at [DigitalSide Threat-Intel](https://osint.digitalside.it) repository. It can be defined a **service as a library** tool designed to act both as a standard Python library to be included in your own Python application and as command line tool. Query can be performed against souspicious IPs, domains, urls and file hashes. Data stored has a 7 days retention.
+**apiosintDS** is a [python client library](https://github.com/davidonzo/apiosintDS) for public *API* lookup service over *OSINT* IoCs stored  at [DigitalSide Threat-Intel](https://osint.digitalside.it) repository. It can be defined a **Service as a Library** tool designed to act both as a standard Python library to be included in your own Python application and as command line tool. Query can be performed against souspicious IPs, domains, urls and file hashes. Data stored has a 7 days retention.
 
 ![apiosintDS v2.0](https://raw.githubusercontent.com/davidonzo/apiosintDS/master/docs/_static/img/apiosintDS.png)
 
 [DigitalSide Threat-Intel (also on GitHub.com)](https://github.com/davidonzo/Threat-Intel) shares a set of **Open Source Cyber Threat Intellegence** information, monstly based on malware analysis and compromised URLs, IPs and domains. The purpose of the project is to develop and test new wayes to hunt, analyze, collect and share relevants sets of IoCs to be used by SOC/CSIRT/CERT with minimun effort. 
 
+**apiosintDS** is also available as [enrichment MISP Modules](https://misp.github.io/misp-modules/expansion/#apiosintds). Documentation is available on [apiosintDS Read The Docs](https://apiosintds.readthedocs.io/en/latest/userguidemisp.html).
+
 This library has been specially designed for people and organizations don't want to import the whole [DigitalSide Threat-Intel](https://osint.digitalside.it) dataset and prefer to use it as an on demand service.
 
 ## Documentation
 Complete documentation availables at [apiosintDS.ReadTheDocs.org](https://apiosintds.readthedocs.io/en/latest/)
 
 ## Install
 ### The easy way via pip
```

### Comparing `apiosintDS-2.0/apiosintDS/apiosintDS.py` & `apiosintDS-2.0.1/apiosintDS/apiosintDS.py`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/apiosintDS/modules/dosearch.py` & `apiosintDS-2.0.1/apiosintDS/modules/dosearch.py`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/apiosintDS/modules/listutils.py` & `apiosintDS-2.0.1/apiosintDS/modules/listutils.py`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/apiosintDS/modules/scriptinfo.py` & `apiosintDS-2.0.1/apiosintDS/modules/scriptinfo.py`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/apiosintDS/modules/stixreport.py` & `apiosintDS-2.0.1/apiosintDS/modules/stixreport.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                     dwreport = json.loads(content)
                 
                 if self.cachetimeout > 0:
                     reportDate = self.getListDate(dwreport)
                     diffdate = ((self.checkdate-reportDate).total_seconds())/3600
                 
                     if diffdate < self.cachetimeout:
-                        logger.info("Report "+self.report+" loaded from cache")
+                        self.logger.info("Report "+self.report+" loaded from cache")
                     else:
                         dwreport = self.downloadReport()
                 else:
                     dwreport = self.downloadReport()
             else:
                 dwreport = self.downloadReport()
         else:
```

### Comparing `apiosintDS-2.0/apiosintDS/schema/schema.json` & `apiosintDS-2.0.1/apiosintDS/schema/schema.json`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/apiosintDS/utilities/logutils.py` & `apiosintDS-2.0.1/apiosintDS/utilities/logutils.py`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/apiosintDS/utilities/prettycli.py` & `apiosintDS-2.0.1/apiosintDS/utilities/prettycli.py`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/apiosintDS.egg-info/PKG-INFO` & `apiosintDS-2.0.1/apiosintDS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiosintDS
-Version: 2.0
+Version: 2.0.1
 Summary: On demand query API for OSINT.digitalside.it project. You can query for souspicious domains, urls, IPv4 and file hashes.
 Home-page: https://github.com/davidonzo/apiosintDS
 Author: Davide Baglieri
 Author-email: info@digitalside.it
 License: MIT
 Keywords: apiosintDS,OSINT,Threat-Intel,IoC,Security
 Platform: UNKNOWN
@@ -16,20 +16,22 @@
 Requires-Python: >3.5.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # apiosintDS
 Latest stable release is **v2.0**
 
-**apiosintDS** is a [python client library](https://github.com/davidonzo/apiosintDS) for public *API* lookup service over *OSINT* IoCs stored  at [DigitalSide Threat-Intel](https://osint.digitalside.it) repository. It can be defined a **service as a library** tool designed to act both as a standard Python library to be included in your own Python application and as command line tool. Query can be performed against souspicious IPs, domains, urls and file hashes. Data stored has a 7 days retention.
+**apiosintDS** is a [python client library](https://github.com/davidonzo/apiosintDS) for public *API* lookup service over *OSINT* IoCs stored  at [DigitalSide Threat-Intel](https://osint.digitalside.it) repository. It can be defined a **Service as a Library** tool designed to act both as a standard Python library to be included in your own Python application and as command line tool. Query can be performed against souspicious IPs, domains, urls and file hashes. Data stored has a 7 days retention.
 
 ![apiosintDS v2.0](https://raw.githubusercontent.com/davidonzo/apiosintDS/master/docs/_static/img/apiosintDS.png)
 
 [DigitalSide Threat-Intel (also on GitHub.com)](https://github.com/davidonzo/Threat-Intel) shares a set of **Open Source Cyber Threat Intellegence** information, monstly based on malware analysis and compromised URLs, IPs and domains. The purpose of the project is to develop and test new wayes to hunt, analyze, collect and share relevants sets of IoCs to be used by SOC/CSIRT/CERT with minimun effort. 
 
+**apiosintDS** is also available as [enrichment MISP Modules](https://misp.github.io/misp-modules/expansion/#apiosintds). Documentation is available on [apiosintDS Read The Docs](https://apiosintds.readthedocs.io/en/latest/userguidemisp.html).
+
 This library has been specially designed for people and organizations don't want to import the whole [DigitalSide Threat-Intel](https://osint.digitalside.it) dataset and prefer to use it as an on demand service.
 
 ## Documentation
 Complete documentation availables at [apiosintDS.ReadTheDocs.org](https://apiosintds.readthedocs.io/en/latest/)
 
 ## Install
 ### The easy way via pip
```

### Comparing `apiosintDS-2.0/apiosintDS.egg-info/SOURCES.txt` & `apiosintDS-2.0.1/apiosintDS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apiosintDS-2.0/setup.py` & `apiosintDS-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from codecs import open
 
 requirements = [line.rstrip('\n') for line in open('requirements.txt')]
 with open("README.md", "r") as fh:
     mylong_description = fh.read()
 scriptinfo = {"scriptname": "apiosintDS",
               "majorversion": "2",
-              "minorversion": "0",
+              "minorversion": "0.1",
               "license": "MIT",
               "licenseurl": "https://raw.githubusercontent.com/davidonzo/Threat-Intel/master/LICENSE",
               "author": "Davide Baglieri",
               "mail": "info@digitalside.it",
               "pgp": "30B31BDA",
               "fingerprint": "0B4C F801 E8FF E9A3 A602  D2C7 9C36 93B2 30B3 1BDA",
               "git": "https://github.com/davidonzo/Threat-Intel/blob/master/tools/DigitalSide-API/v1",
```

