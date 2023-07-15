# Comparing `tmp/django-eskiz-sms-0.1.tar.gz` & `tmp/django-eskiz-sms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-eskiz-sms-0.1.tar", last modified: Sat Jul 15 02:36:42 2023, max compression
+gzip compressed data, was "django-eskiz-sms-0.1.1.tar", last modified: Sat Jul 15 02:58:52 2023, max compression
```

## Comparing `django-eskiz-sms-0.1.tar` & `django-eskiz-sms-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 02:36:42.776692 django-eskiz-sms-0.1/
--rw-rw-rw-   0        0        0     1075 2023-07-15 02:08:16.000000 django-eskiz-sms-0.1/LICENCE
--rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      918 2023-07-15 02:36:42.776692 django-eskiz-sms-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-15 02:36:23.000000 django-eskiz-sms-0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-15 02:36:42.728642 django-eskiz-sms-0.1/django_eskiz_sms.egg-info/
--rw-rw-rw-   0        0        0      918 2023-07-15 02:36:42.000000 django-eskiz-sms-0.1/django_eskiz_sms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-15 02:36:42.000000 django-eskiz-sms-0.1/django_eskiz_sms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 02:36:42.000000 django-eskiz-sms-0.1/django_eskiz_sms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 02:36:42.000000 django-eskiz-sms-0.1/django_eskiz_sms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 02:36:42.760674 django-eskiz-sms-0.1/eskiz_sms/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1/eskiz_sms/__init__.py
--rw-rw-rw-   0        0        0      548 2023-07-15 01:07:25.000000 django-eskiz-sms-0.1/eskiz_sms/admin.py
--rw-rw-rw-   0        0        0      155 2023-07-14 21:50:04.000000 django-eskiz-sms-0.1/eskiz_sms/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-15 02:36:42.768637 django-eskiz-sms-0.1/eskiz_sms/migrations/
--rw-rw-rw-   0        0        0     2927 2023-07-15 01:14:42.000000 django-eskiz-sms-0.1/eskiz_sms/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1/eskiz_sms/migrations/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-07-15 01:07:52.000000 django-eskiz-sms-0.1/eskiz_sms/models.py
-drwxrwxrwx   0        0        0        0 2023-07-15 02:36:42.776692 django-eskiz-sms-0.1/eskiz_sms/templates/
--rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1/eskiz_sms/templates/send_sms.html
--rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1/eskiz_sms/urls.py
--rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1/eskiz_sms/views.py
--rw-rw-rw-   0        0        0      892 2023-07-15 02:36:42.786482 django-eskiz-sms-0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-07-15 02:27:20.000000 django-eskiz-sms-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.884720 django-eskiz-sms-0.1.1/
+-rw-rw-rw-   0        0        0     1075 2023-07-15 02:08:16.000000 django-eskiz-sms-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      987 2023-07-15 02:58:52.884720 django-eskiz-sms-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-07-15 02:57:44.000000 django-eskiz-sms-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.836739 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.868733 django-eskiz-sms-0.1.1/eskiz_sms/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.1/eskiz_sms/__init__.py
+-rw-rw-rw-   0        0        0      548 2023-07-15 01:07:25.000000 django-eskiz-sms-0.1.1/eskiz_sms/admin.py
+-rw-rw-rw-   0        0        0      155 2023-07-14 21:50:04.000000 django-eskiz-sms-0.1.1/eskiz_sms/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.876721 django-eskiz-sms-0.1.1/eskiz_sms/migrations/
+-rw-rw-rw-   0        0        0     2927 2023-07-15 01:14:42.000000 django-eskiz-sms-0.1.1/eskiz_sms/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.1/eskiz_sms/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2064 2023-07-15 01:07:52.000000 django-eskiz-sms-0.1.1/eskiz_sms/models.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.884720 django-eskiz-sms-0.1.1/eskiz_sms/templates/
+-rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.1/eskiz_sms/templates/send_sms.html
+-rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.1/eskiz_sms/urls.py
+-rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.1/eskiz_sms/views.py
+-rw-rw-rw-   0        0        0      894 2023-07-15 02:58:52.892728 django-eskiz-sms-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-07-15 02:27:20.000000 django-eskiz-sms-0.1.1/setup.py
```

### Comparing `django-eskiz-sms-0.1/LICENCE` & `django-eskiz-sms-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1/PKG-INFO` & `django-eskiz-sms-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-eskiz-sms
-Version: 0.1
+Version: 0.1.1
 Summary: Djangodan EskizUz orqali SMS yuborish paketi
 Home-page: https://tijorat.org
 Author: Rozmat Otajonov
 Author-email: otajonov@tijorat.org
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,7 +17,9 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENCE
+
+Documentation is here https://docs.tijorat.org/django-eskiz-sms
```

### Comparing `django-eskiz-sms-0.1/django_eskiz_sms.egg-info/PKG-INFO` & `django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-eskiz-sms
-Version: 0.1
+Version: 0.1.1
 Summary: Djangodan EskizUz orqali SMS yuborish paketi
 Home-page: https://tijorat.org
 Author: Rozmat Otajonov
 Author-email: otajonov@tijorat.org
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,7 +17,9 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENCE
+
+Documentation is here https://docs.tijorat.org/django-eskiz-sms
```

### Comparing `django-eskiz-sms-0.1/eskiz_sms/admin.py` & `django-eskiz-sms-0.1.1/eskiz_sms/admin.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1/eskiz_sms/migrations/0001_initial.py` & `django-eskiz-sms-0.1.1/eskiz_sms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1/eskiz_sms/models.py` & `django-eskiz-sms-0.1.1/eskiz_sms/models.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1/eskiz_sms/templates/send_sms.html` & `django-eskiz-sms-0.1.1/eskiz_sms/templates/send_sms.html`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1/eskiz_sms/views.py` & `django-eskiz-sms-0.1.1/eskiz_sms/views.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1/setup.cfg` & `django-eskiz-sms-0.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6573 6b69 7a2d   = django-eskiz-
 00000020: 736d 730d 0a76 6572 7369 6f6e 203d 2030  sms..version = 0
-00000030: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
-00000040: 3d20 446a 616e 676f 6461 6e20 4573 6b69  = Djangodan Eski
-00000050: 7a55 7a20 6f72 7161 6c69 2053 4d53 2079  zUz orqali SMS y
-00000060: 7562 6f72 6973 6820 7061 6b65 7469 0d0a  uborish paketi..
-00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000090: 7273 740d 0a75 726c 203d 2068 7474 7073  rst..url = https
-000000a0: 3a2f 2f74 696a 6f72 6174 2e6f 7267 0d0a  ://tijorat.org..
-000000b0: 6175 7468 6f72 203d 2052 6f7a 6d61 7420  author = Rozmat 
-000000c0: 4f74 616a 6f6e 6f76 0d0a 6175 7468 6f72  Otajonov..author
-000000d0: 5f65 6d61 696c 203d 206f 7461 6a6f 6e6f  _email = otajono
-000000e0: 7640 7469 6a6f 7261 742e 6f72 670d 0a6c  v@tijorat.org..l
-000000f0: 6963 656e 7365 203d 204d 4954 0d0a 636c  icense = MIT..cl
-00000100: 6173 7369 6669 6572 7320 3d20 0d0a 0945  assifiers = ...E
-00000110: 6e76 6972 6f6e 6d65 6e74 203a 3a20 5765  nvironment :: We
-00000120: 6220 456e 7669 726f 6e6d 656e 740d 0a09  b Environment...
-00000130: 4672 616d 6577 6f72 6b20 3a3a 2044 6a61  Framework :: Dja
-00000140: 6e67 6f0d 0a09 4672 616d 6577 6f72 6b20  ngo...Framework 
-00000150: 3a3a 2044 6a61 6e67 6f20 3a3a 2034 2e32  :: Django :: 4.2
-00000160: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
-00000170: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000180: 7273 0d0a 094c 6963 656e 7365 203a 3a20  rs...License :: 
-00000190: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000001a0: 4253 4420 4c69 6365 6e73 650d 0a09 4f70  BSD License...Op
-000001b0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001c0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000001d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001f0: 6e0d 0a09 5072 6f67 7261 6d6d 696e 6720  n...Programming 
-00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000210: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
-00000220: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000230: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
-00000240: 204f 6e6c 790d 0a09 5072 6f67 7261 6d6d   Only...Programm
-00000250: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000260: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000290: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
-000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002b0: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
-000002c0: 0a09 546f 7069 6320 3a3a 2049 6e74 6572  ..Topic :: Inter
-000002d0: 6e65 7420 3a3a 2057 5757 2f48 5454 500d  net :: WWW/HTTP.
-000002e0: 0a09 546f 7069 6320 3a3a 2049 6e74 6572  ..Topic :: Inter
-000002f0: 6e65 7420 3a3a 2057 5757 2f48 5454 5020  net :: WWW/HTTP 
-00000300: 3a3a 2044 796e 616d 6963 2043 6f6e 7465  :: Dynamic Conte
-00000310: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000320: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-00000330: 5f64 6174 6120 3d20 7472 7565 0d0a 7061  _data = true..pa
-00000340: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000350: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000360: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000370: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000030: 2e31 2e31 0d0a 6465 7363 7269 7074 696f  .1.1..descriptio
+00000040: 6e20 3d20 446a 616e 676f 6461 6e20 4573  n = Djangodan Es
+00000050: 6b69 7a55 7a20 6f72 7161 6c69 2053 4d53  kizUz orqali SMS
+00000060: 2079 7562 6f72 6973 6820 7061 6b65 7469   yuborish paketi
+00000070: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000080: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+00000090: 452e 7273 740d 0a75 726c 203d 2068 7474  E.rst..url = htt
+000000a0: 7073 3a2f 2f74 696a 6f72 6174 2e6f 7267  ps://tijorat.org
+000000b0: 0d0a 6175 7468 6f72 203d 2052 6f7a 6d61  ..author = Rozma
+000000c0: 7420 4f74 616a 6f6e 6f76 0d0a 6175 7468  t Otajonov..auth
+000000d0: 6f72 5f65 6d61 696c 203d 206f 7461 6a6f  or_email = otajo
+000000e0: 6e6f 7640 7469 6a6f 7261 742e 6f72 670d  nov@tijorat.org.
+000000f0: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
+00000100: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000110: 0945 6e76 6972 6f6e 6d65 6e74 203a 3a20  .Environment :: 
+00000120: 5765 6220 456e 7669 726f 6e6d 656e 740d  Web Environment.
+00000130: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
+00000140: 6a61 6e67 6f0d 0a09 4672 616d 6577 6f72  jango...Framewor
+00000150: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
+00000160: 2e32 0d0a 0949 6e74 656e 6465 6420 4175  .2...Intended Au
+00000170: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+00000180: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
+00000190: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000001a0: 3a20 4253 4420 4c69 6365 6e73 650d 0a09  : BSD License...
+000001b0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001c0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001d0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
+000001e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001f0: 686f 6e0d 0a09 5072 6f67 7261 6d6d 696e  hon...Programmin
+00000200: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000210: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+00000220: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000230: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+00000240: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
+00000250: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000260: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000270: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000280: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000290: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
+000002a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000002c0: 310d 0a09 546f 7069 6320 3a3a 2049 6e74  1...Topic :: Int
+000002d0: 6572 6e65 7420 3a3a 2057 5757 2f48 5454  ernet :: WWW/HTT
+000002e0: 500d 0a09 546f 7069 6320 3a3a 2049 6e74  P...Topic :: Int
+000002f0: 6572 6e65 7420 3a3a 2057 5757 2f48 5454  ernet :: WWW/HTT
+00000300: 5020 3a3a 2044 796e 616d 6963 2043 6f6e  P :: Dynamic Con
+00000310: 7465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  tent....[options
+00000320: 5d0d 0a69 6e63 6c75 6465 5f70 6163 6b61  ]..include_packa
+00000330: 6765 5f64 6174 6120 3d20 7472 7565 0d0a  ge_data = true..
+00000340: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000350: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000360: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000370: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

