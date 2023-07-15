# Comparing `tmp/vios-1.0.7-py3-none-any.whl.zip` & `tmp/vios-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 33887 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat      781 b- defN 23-Jun-26 13:01 vios/__init__.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-Jul-04 14:13 vios/collection/__init__.py
+Zip file size: 33995 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat      781 b- defN 23-Jul-15 06:38 vios/__init__.py
+-rw-rw-rw-  2.0 fat     6314 b- defN 23-Jul-13 12:34 vios/collection/__init__.py
 -rw-rw-rw-  2.0 fat     3515 b- defN 23-Jul-04 13:33 vios/collection/support.py
 -rw-rw-rw-  2.0 fat    11254 b- defN 23-Jun-19 15:11 vios/collection/tasks.py
 -rw-rw-rw-  2.0 fat    10198 b- defN 23-Jun-28 07:10 vios/collection/uapi.py
--rw-rw-rw-  2.0 fat     4756 b- defN 23-Jun-19 15:11 vios/driver/VirtualDevice.py
+-rw-rw-rw-  2.0 fat     4756 b- defN 23-Jul-15 07:53 vios/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat     2962 b- defN 23-Jun-19 15:11 vios/driver/__init__.py
 -rw-rw-rw-  2.0 fat      209 b- defN 23-Jun-26 11:28 vios/driver/common/__init__.py
 -rw-rw-rw-  2.0 fat     4192 b- defN 23-Jun-28 07:10 vios/driver/common/basedriver.py
 -rw-rw-rw-  2.0 fat     4666 b- defN 23-Jun-19 15:11 vios/driver/common/quantity.py
 -rw-rw-rw-  2.0 fat     5546 b- defN 23-Jun-19 15:11 vios/driver/common/visadriver.py
--rw-rw-rw-  2.0 fat      784 b- defN 23-Jun-30 06:18 vios/envelope/__init__.py
+-rw-rw-rw-  2.0 fat      979 b- defN 23-Jul-15 07:14 vios/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    13446 b- defN 23-Jul-06 02:54 vios/envelope/assembler.py
 -rw-rw-rw-  2.0 fat    10541 b- defN 23-Jun-26 11:28 vios/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-Jun-19 15:11 vios/envelope/device.py
--rw-rw-rw-  2.0 fat     1719 b- defN 23-Jun-26 11:28 vios/envelope/processor.py
+-rw-rw-rw-  2.0 fat     1719 b- defN 23-Jul-15 07:54 vios/envelope/processor.py
 -rw-rw-rw-  2.0 fat     2980 b- defN 23-Jun-26 12:50 vios/envelope/rule.py
 -rw-rw-rw-  2.0 fat      522 b- defN 23-Jun-26 11:28 vios/tools/__init__.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1000 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1857 b- defN 23-Jul-06 03:28 vios-1.0.7.dist-info/RECORD
-23 files, 89473 bytes uncompressed, 30907 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-15 07:56 vios-1.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1000 b- defN 23-Jul-15 07:56 vios-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-15 07:56 vios-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-15 07:56 vios-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1857 b- defN 23-Jul-15 07:56 vios-1.0.8.dist-info/RECORD
+23 files, 89670 bytes uncompressed, 31015 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: vios/envelope/rule.py
 Comment: 
 
 Filename: vios/tools/__init__.py
 Comment: 
 
-Filename: vios-1.0.7.dist-info/LICENSE
+Filename: vios-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: vios-1.0.7.dist-info/METADATA
+Filename: vios-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: vios-1.0.7.dist-info/WHEEL
+Filename: vios-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: vios-1.0.7.dist-info/top_level.txt
+Filename: vios-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-1.0.7.dist-info/RECORD
+Filename: vios-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vios/collection/__init__.py

```diff
@@ -157,15 +157,15 @@
             self.progress.finish(success)
             self.handles[tid].cancel()
         except Exception as e:
             # print(e)
             pass
 
     def bar(self):
-        self.stop(self.taskid)
+        # self.stop(self.taskid)
         bar = JupyterProgressBar(description=self.name)
         bar.listen(self.progress)
         bar.display()
         self.join()
 
 
 def transform(app: App):
```

## vios/envelope/__init__.py

```diff
@@ -5,12 +5,24 @@
         ↓           ↑    ↓            ↑  ↓             ↑     ↓          ↑   ↓ 
         &ccompile   ↑    &calculate -->  &read|write -->     &process -->   &postprocess --->
         ↓           ↑
         &assemble -->
 """
 
 
+import time
+
+
+class Future(object):
+    def __init__(self, index: int = -1) -> None:
+        self.index = index
+
+    def result(self):
+        return self.quark.result(self.index)
+
+
+
 from .assembler import MAPPING, assemble, ccompile, decode, initialize
 from .calculator import calculate
 from .device import read, write
 from .processor import process
 from .rule import postprocess
```

## Comparing `vios-1.0.7.dist-info/LICENSE` & `vios-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-1.0.7.dist-info/METADATA` & `vios-1.0.8.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 1.0.7
+Version: 1.0.8
 Summary: runtime requirements for systemq
 Author-email: YL <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-1.0.7.dist-info/RECORD` & `vios-1.0.8.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 vios/__init__.py,sha256=pQ_BUjQ_ZCki4pI_wid9yJbQi_YK2uWG3rixAEbC670,781
-vios/collection/__init__.py,sha256=RytWzptUCjh2nCNazuNTNg0rEe807ntVkw0ukkRzTKU,6312
+vios/collection/__init__.py,sha256=cKUpYHEREjZVHr6PZy_b1DL9c-dF--hAcVW1Wpc2OQM,6314
 vios/collection/support.py,sha256=78G1G0vyDInEfW4j4RGdt7uM8gt_M3_Ucm_3_zm7jB0,3515
 vios/collection/tasks.py,sha256=FUAGla2yjy4apdM5PLZ7yJP0YsbMajat1gm8bt7y7QI,11254
 vios/collection/uapi.py,sha256=bmjnw6XokSU-0Zkt7XTldjAY0kF48RbHuFVVnE-EkSI,10198
 vios/driver/VirtualDevice.py,sha256=sf87LAcRvJIVZW-OyP8Hw-CWu7isonbr2-TjFGZHYSk,4756
 vios/driver/__init__.py,sha256=rvTlhtDHO_l1rHNsgb3PA9LnEirl4TIm0bvlgRseRnY,2962
 vios/driver/common/__init__.py,sha256=rwnAg6V2hY1vinIHlvGwKTXn34SRQHX8bnIleycTM6k,209
 vios/driver/common/basedriver.py,sha256=jQ3svU_t1v0Zt8lRX8ij8MhwilmIwziozwuTFeRxRnE,4192
 vios/driver/common/quantity.py,sha256=70feNhld2lF04KHQ3zWDliS_cmD1q97Yi0oFqlwYijs,4666
 vios/driver/common/visadriver.py,sha256=WY6TqGmow_K5ePAYIYkG12IxjHfAczuxYTvPk4VmVG4,5546
-vios/envelope/__init__.py,sha256=97kXED9oaUd56J2OoVCTQpctkQZDcAZWxpEQakTxCRM,784
+vios/envelope/__init__.py,sha256=1XevWes-wBaeEaSsJEG3OMJglYsKrdTf06--dfIXE5Y,979
 vios/envelope/assembler.py,sha256=KE4Fcrid5UfBsbpOPz7eV2WJY1f7jXwVY0VtjwMvPBk,13446
 vios/envelope/calculator.py,sha256=eE7730YFzArrukuDh0dI0JabG2PiEz3eo3N4Czqgk88,10541
 vios/envelope/device.py,sha256=rQeLe_Y9MTwLZfJsSK9MhvZxdOnrtJNcOZriS6Rm1Io,1047
 vios/envelope/processor.py,sha256=4py3AwLurBTrhXXJCvdfHrMeKGzOFl-gICQTNjpoyQM,1719
 vios/envelope/rule.py,sha256=ANiUVCtozVP6B6m8En55VLqOHWdeMkuA7KqiAiFyAnQ,2980
 vios/tools/__init__.py,sha256=vq-1N9Zjm_ZYcD9_lwX9fKlcMT9Rx7Kd3BDRqmKhMT0,522
-vios-1.0.7.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
-vios-1.0.7.dist-info/METADATA,sha256=aYJAj7l0t3xW48dCs3R0GzZ7NNsUBWfoQN_1zi4ATj8,1000
-vios-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vios-1.0.7.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
-vios-1.0.7.dist-info/RECORD,,
+vios-1.0.8.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
+vios-1.0.8.dist-info/METADATA,sha256=dZ0ABAoFTGLWnh46duBuSFYsYRs0nno2uAQ_UbJawwU,1000
+vios-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vios-1.0.8.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
+vios-1.0.8.dist-info/RECORD,,
```

