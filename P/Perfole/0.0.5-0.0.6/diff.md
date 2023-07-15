# Comparing `tmp/Perfole-0.0.5.tar.gz` & `tmp/Perfole-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Perfole-0.0.5.tar", last modified: Tue Jul 11 21:11:11 2023, max compression
+gzip compressed data, was "Perfole-0.0.6.tar", last modified: Sat Jul 15 20:12:59 2023, max compression
```

## Comparing `Perfole-0.0.5.tar` & `Perfole-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-11 21:11:11.086309 Perfole-0.0.5/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1402 2023-07-11 21:11:11.086030 Perfole-0.0.5/PKG-INFO
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-11 21:11:11.084350 Perfole-0.0.5/Perfole/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12878 2023-07-11 21:05:52.000000 Perfole-0.0.5/Perfole/Perfole.py
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.5/Perfole/__init__.py
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-11 21:11:11.085526 Perfole-0.0.5/Perfole.egg-info/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1402 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/PKG-INFO
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/SOURCES.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/dependency_links.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/requires.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-11 21:11:11.000000 Perfole-0.0.5/Perfole.egg-info/top_level.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1211 2023-07-10 13:19:25.000000 Perfole-0.0.5/README.md
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.5/license.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-11 21:11:11.086367 Perfole-0.0.5/setup.cfg
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      501 2023-07-11 21:09:13.000000 Perfole-0.0.5/setup.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-15 20:12:59.842972 Perfole-0.0.6/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1402 2023-07-15 20:12:59.842836 Perfole-0.0.6/PKG-INFO
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-15 20:12:59.842002 Perfole-0.0.6/Perfole/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12878 2023-07-15 20:11:35.000000 Perfole-0.0.6/Perfole/Perfole.py
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.6/Perfole/__init__.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-15 20:12:59.842650 Perfole-0.0.6/Perfole.egg-info/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1402 2023-07-15 20:12:59.000000 Perfole-0.0.6/Perfole.egg-info/PKG-INFO
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-15 20:12:59.000000 Perfole-0.0.6/Perfole.egg-info/SOURCES.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-15 20:12:59.000000 Perfole-0.0.6/Perfole.egg-info/dependency_links.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-15 20:12:59.000000 Perfole-0.0.6/Perfole.egg-info/requires.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-15 20:12:59.000000 Perfole-0.0.6/Perfole.egg-info/top_level.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1211 2023-07-10 13:19:25.000000 Perfole-0.0.6/README.md
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     3808 2023-07-15 20:10:07.000000 Perfole-0.0.6/license.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-15 20:12:59.843012 Perfole-0.0.6/setup.cfg
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      501 2023-07-15 20:12:23.000000 Perfole-0.0.6/setup.py
```

### Comparing `Perfole-0.0.5/PKG-INFO` & `Perfole-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.5
+Version: 0.0.6
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `Perfole-0.0.5/Perfole/Perfole.py` & `Perfole-0.0.6/Perfole/Perfole.py`

 * *Files identical despite different names*

### Comparing `Perfole-0.0.5/Perfole.egg-info/PKG-INFO` & `Perfole-0.0.6/Perfole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.5
+Version: 0.0.6
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `Perfole-0.0.5/README.md` & `Perfole-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Perfole-0.0.5/license.txt` & `Perfole-0.0.6/license.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-Software License Agreement
-1. This Software License Agreement (the "Agreement") constitutes a legally binding agreement between Smiljana Radlović PR Breeze Testing (the "Vendor") and you as the user (the "Licensee" or "You") of this Software.
-2. The Vendor allows you to use this Software only under the terms and conditions of this Agreement.
+End User License Agreement
+1. This End User License Agreement (the "Agreement") constitutes a legally binding agreement between Smiljana Radlović PR Računarsko programiranje Breeze testing Novi Sad (the "Licensor") and you as the user (the "Licensee" or "You") of a license to use this Software.
+2. The Licensor allows you to use this Software only under the terms and conditions of this Agreement.
 3. By using this Software, you expressly agree to this Agreement and all terms and conditions of this Agreement (the "Acceptance").
-4. Under this Agreement, the Vendor grants to the Licensee a non-exclusive, non-transferable, perpetual, worldwide License (the "License") to use Perfole (the "Software"). 
-The term "Software", whenever used in this Agreement, means any software, tool, plugin, feature and file made available to Licensee under this Agreement.
-5. Title, copyright, intellectual property rights and distribution rights of the Software remain exclusively with the Vendor. Intellectual property rights include the look and feel of the Software. This Agreement constitutes a license for use only and is not in any way a transfer of ownership rights to the Software.
- 
-6. You may use the Software only for the following purpose: Measuring the performance of third-party software.
-7. The Licensee may not transfer or assign any of the rights or obligations granted under this Agreement to any other person or legal entity. The Licensee is permitted to distribute the Software in applications the Licensee develop, only for a specific part - the Distribution Code.
-8. The Software may not be modified, reverse-engineered, or de-compiled in any manner through current or future available technologies. The Licensee may not share, publish, rent or lease the Software or provide the Software as a stand-alone offering for others to use.
+4. Under this Agreement, the Licensor grants to the Licensee a non-exclusive, non-transferable, non-sublicensable, perpetual and worldwide License (the "License") to use perfole (the "Software"). 
+5. The term "Software", whenever used in this Agreement, means any software, source code, product, package, tool, plugin, feature and file made available to Licensee under this Agreement.
+6. This Agreement is in compliance with the Apache 2.0 License ("Apache License"). You acknowledge that you have received and read a copy of the Apache License, which is also available at the following link: https://www.apache.org/licenses/LICENSE-2.0
+7. Title, copyright, intellectual property rights and distribution rights of the Software remain exclusively with the Licensor.  Intellectual property rights include the look and feel of the Software. This Agreement constitutes a license for use only and is not in any way a transfer of ownership rights to the Software. 
+8. The Licensee may use the Software only for the functioning and operation of the Licensee's applications. Licensee may not sell or sublicense the Software as such.
+9. The Software may not be modified, reverse-engineered, or de-compiled in any manner through current or future available technologies. 
+10. Failure to comply with any of the terms under the License section will be considered a material breach of this Agreement and the License may be revoked in such event.
+11. The Software is provided by the Licensor and accepted by the Licensee "as is". Liability of the Licensor will be limited to the maximum extent permitted by law. The Licensor will not be liable for any general, special, incidental or consequential damages including, but not limited to, loss of production, loss of profits, loss of revenue, loss of data, or any other business or economic disadvantage suffered by the Licensee arising out of the use or failure to use the Software. 
+The Licensee is obliged to conform his use of the Software with all applicable laws and other regulations. The Licensor shall not be responsible in any way for the use of the Software in a manner that violates laws or other regulations.
+12. The Licensor makes no warranty expressed or implied regarding the fitness of the Software for a particular purpose or that the Software will be suitable or appropriate for the specific requirements of the Licensee. 
+13. The Licensor does not warrant that use of the Software will be uninterrupted or error-free. The Licensee accepts that software in general is prone to bugs and flaws within an acceptable level as determined in the industry. 
+14. The term of this Agreement will begin on Acceptance and is perpetual. 
+15. This Agreement will be terminated and the License forfeited where the Licensee has failed to comply with any of the terms of this Agreement or is in breach of this Agreement. On termination of this Agreement for any reason, the Licensee will promptly destroy the Software or return the Software to the Licensor. 
+16. The Parties to this Agreement submit to the jurisdiction of the courts of the Serbia for the enforcement of this Agreement or any arbitration award or decision arising from this Agreement. This Agreement will be enforced or construed according to the laws of the Serbia. 
+
+
 
-9. Failure to comply with any of the terms under the License section will be considered a material breach of this Agreement and the License may be revoked in such event.
-10. The Software is provided by the Vendor and accepted by the Licensee "as is". Liability of the Vendor will be limited to the maximum extent permitted by law. The Vendor will not be liable for any general, special, incidental or consequential damages including, but not limited to, loss of production, loss of profits, loss of revenue, loss of data, or any other business or economic disadvantage suffered by the Licensee arising out of the use or failure to use the Software. 
-The Licensee is obliged to conform his use of the Software with all applicable laws and other regulations. The Vendor shall not be responsible in any way for the use of the Software in a manner that violates laws or other regulations.
-11. The Vendor makes no warranty expressed or implied regarding the fitness of the Software for a particular purpose or that the Software will be suitable or appropriate for the specific requirements of the Licensee. 
-12. The Vendor does not warrant that use of the Software will be uninterrupted or error-free. The Licensee accepts that software in general is prone to bugs and flaws within an acceptable level as determined in the industry. 
-13. The Vendor warrants and represents that it is the copyright holder of the Software. The Vendor warrants and represents that granting the License to use this Software is not in violation of any other agreement, copyright or applicable statute. 
-14. The Licensee shall indemnify and hold harmless Vendor and related Open Source Provider from and against any and all claims, actions, damages, suits, liabilities, obligations, costs, fees, charges, and any other expenses whatsoever, including reasonable attorneys’ fees and costs, that may be asserted by a third party against and related Open Source Provider in connection with the breach of this Agreement, misrepresentation, negligence or misconduct of the Licensee.
-15. The term of this Agreement will begin on Acceptance and is perpetual. 
-16. This Agreement will be terminated and the License forfeited where the Licensee has failed to comply with any of the terms of this Agreement or is in breach of this Agreement. On termination of this Agreement for any reason, the Licensee will promptly destroy the Software or return the Software to the Vendor. 
-17. The Parties to this Agreement submit to the jurisdiction of the courts of the Republic of Serbia for the enforcement of this Agreement or any arbitration award or decision arising from this Agreement. This Agreement will be enforced or construed according to the laws of the Republic of Serbia.
```

