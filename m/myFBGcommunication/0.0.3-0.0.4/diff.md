# Comparing `tmp/myFBGcommunication-0.0.3-py3-none-any.whl.zip` & `tmp/myFBGcommunication-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3995 bytes, number of entries: 7
+Zip file size: 3993 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       51 b- defN 22-Dec-20 04:46 myFBGcommunication/__init__.py
--rw-rw-rw-  2.0 fat     7528 b- defN 23-Jan-04 07:53 myFBGcommunication/myFBGcommunication.py
+-rw-rw-rw-  2.0 fat     7512 b- defN 23-Jul-15 04:46 myFBGcommunication/myFBGcommunication.py
 -rw-rw-rw-  2.0 fat       86 b- defN 22-Dec-20 08:22 myFBGcommunication/params.ini
--rw-rw-rw-  2.0 fat      252 b- defN 23-Jan-04 07:55 myFBGcommunication-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-04 07:55 myFBGcommunication-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jan-04 07:55 myFBGcommunication-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      607 b- defN 23-Jan-04 07:55 myFBGcommunication-0.0.3.dist-info/RECORD
-7 files, 8635 bytes uncompressed, 2899 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat      252 b- defN 23-Jul-15 04:48 myFBGcommunication-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-15 04:48 myFBGcommunication-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jul-15 04:48 myFBGcommunication-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      607 b- defN 23-Jul-15 04:48 myFBGcommunication-0.0.4.dist-info/RECORD
+7 files, 8619 bytes uncompressed, 2897 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: myFBGcommunication/myFBGcommunication.py
 Comment: 
 
 Filename: myFBGcommunication/params.ini
 Comment: 
 
-Filename: myFBGcommunication-0.0.3.dist-info/METADATA
+Filename: myFBGcommunication-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: myFBGcommunication-0.0.3.dist-info/WHEEL
+Filename: myFBGcommunication-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: myFBGcommunication-0.0.3.dist-info/top_level.txt
+Filename: myFBGcommunication-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: myFBGcommunication-0.0.3.dist-info/RECORD
+Filename: myFBGcommunication-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myFBGcommunication/myFBGcommunication.py

```diff
@@ -1,8 +1,8 @@
-# 0.0.3
+# 0.0.4
 import time
 import serial
 import scipy
 import pandas as pd
 import pkg_resources
 import os
 
@@ -38,14 +38,15 @@
         except serial.serialutil.SerialException:
             return -1
 
         self.auto_setting()
         self.set_param()
         return 1
 
+
     def auto_setting(self):
         # ----FBGセンサの検出-----
         spectrum_raw = b''
         WLL_raw = b''
         self._ser.write(b's>')
         time.sleep(0.1)
         while len(spectrum_raw) != 2052:
@@ -158,16 +159,16 @@
                     tmp_line = line[ende_idx + 4:len(line)]
                     line = line[0:ende_idx + 4]
                     dataOK = True
         if self._on_boradCalculation:
             now_data = [int.from_bytes(line[8 * i:8 * i + 4], byteorder='little', signed=True)/10000 for i in Targets]
         else:
             now_data = [int.from_bytes(line[8 * i:8 * i + 4], byteorder='little', signed=True) for i in Targets]
-        return now_data, line
+        return now_data
 
     def read_all(self):
-        now_data, line = self.read(range(self.FBG_num))
-        return now_data, line
+        now_data = self.read(range(self.FBG_num))
+        return now_data
 
     def _make_default_paramsfile(self):
         _paramas = [['FBG_width',3.0], ['integration_time',0.05], ['Averaging',1],['on_boradCalc',True],['defaultTemp',21]]
         pd.DataFrame(_paramas, columns=None).to_csv('params.ini', index=None, header=None)
```

## Comparing `myFBGcommunication-0.0.3.dist-info/RECORD` & `myFBGcommunication-0.0.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 myFBGcommunication/__init__.py,sha256=ZOrh5pW1-iIa65TnFGotuQbJRDeFkMmh3Z5nb33_U5c,51
-myFBGcommunication/myFBGcommunication.py,sha256=FEgF36M1YBLcagkfhyR_yCUecqRwCU5QBK6fiN9-TME,7528
+myFBGcommunication/myFBGcommunication.py,sha256=SAwhCJzO-5-zQQ-RjrBYQlTTW-QsH2RnX3MbuB2xTlA,7512
 myFBGcommunication/params.ini,sha256=kBDoInBTdWn8zhaCbJa24G4q-s_DcAdNm5rRVX1UDlc,86
-myFBGcommunication-0.0.3.dist-info/METADATA,sha256=PMdzHZ8XYwkSp9K4LURQEPI6m7llgMz9PlvTgsXb0dI,252
-myFBGcommunication-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-myFBGcommunication-0.0.3.dist-info/top_level.txt,sha256=CvHWPRjXmDQYOLrsg43G9A-JYHPLoLCC1Wl1dG6P7gY,19
-myFBGcommunication-0.0.3.dist-info/RECORD,,
+myFBGcommunication-0.0.4.dist-info/METADATA,sha256=-ba5Cv9F0oCjMJK7MEJ6w-rITieu7P0AHwKJlIkzOSU,252
+myFBGcommunication-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+myFBGcommunication-0.0.4.dist-info/top_level.txt,sha256=CvHWPRjXmDQYOLrsg43G9A-JYHPLoLCC1Wl1dG6P7gY,19
+myFBGcommunication-0.0.4.dist-info/RECORD,,
```

