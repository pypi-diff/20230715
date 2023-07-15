# Comparing `tmp/statprocon-0.0.6.tar.gz` & `tmp/statprocon-0.0.7.tar.gz`

## Comparing `statprocon-0.0.6.tar` & `statprocon-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 statprocon-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.6/requirements-dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/xmr.iml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/charts/__init__.py
--rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/charts/xmr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     8265 2020-02-02 00:00:00.000000 statprocon-0.0.6/tests/test_xmr.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.6/LICENSE
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.6/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 statprocon-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.0.7/CODEOWNERS
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.7/requirements-dev.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/xmr.iml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/charts/xmr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 statprocon-0.0.7/tests/test_xmr.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 statprocon-0.0.7/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 statprocon-0.0.7/PKG-INFO
```

### Comparing `statprocon-0.0.6/requirements-dev.txt` & `statprocon-0.0.7/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.6/.idea/workspace.xml` & `statprocon-0.0.7/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `statprocon-0.0.6/.idea/workspace.xml` & `statprocon-0.0.7/.idea/workspace.xml`

```diff
@@ -1,18 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment="">
-      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/statprocon/charts/xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/statprocon/charts/xmr.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/test_xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_xmr.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -88,15 +85,15 @@
       <changelist id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment=""/>
       <created>1688827023388</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
       <workItem from="1688848868641" duration="17704000"/>
-      <workItem from="1688944372544" duration="9103000"/>
+      <workItem from="1688944372544" duration="17043000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `statprocon-0.0.6/.idea/xmr.iml` & `statprocon-0.0.7/.idea/xmr.iml`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.6/statprocon/charts/xmr.py` & `statprocon-0.0.7/statprocon/charts/xmr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import csv
+import io
+
 from decimal import Decimal
 from typing import cast, Union, Optional
 
-TYPE_COUNTS = list[Decimal | int]
+TYPE_COUNTS = list[Decimal | int | float]
 TYPE_MOVING_RANGES = list[Decimal | int | None]
 
 
 class XmR:
     ROUNDING = 3
 
     def __init__(
@@ -16,41 +19,64 @@
     ):
         """
 
         :param counts: TYPE_COUNTS list of data to be used by the X chart
         :param subset_start_index: Optional starting index of counts to calculate limits from
         :param subset_end_index: Optional ending index of counts to calculate limits to
         """
-        self.counts = counts
+        self.counts = [Decimal(str(x)) for x in counts]
         self._mr: TYPE_MOVING_RANGES = []
         self.i = max(0, subset_start_index)
         self.j = len(counts)
         if subset_end_index:
             self.j = min(self.j, subset_end_index)
 
         assert self.i <= self.j
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         result = ''
         for k, v in self.to_dict().items():
             k_format = '{0: <6}'.format(k)
-            result += f'{k_format}: {v}\n'
+            values = ''
+            if isinstance(v, list):
+                values = '[' + ', '.join(map(str, v)) + ']'
+            else:
+                values = v
+            result += f'{k_format}: {values}\n'
         return result
 
-    def to_dict(self):
+    def to_dict(self) -> dict:
         return {
             'Counts': self.counts,
             'UNPL': self.upper_natural_process_limit(),
             'X bar': self.x_average(),
             'LNPL': self.lower_natural_process_limit(),
             'MR': self.moving_ranges(),
             'URL': self.upper_range_limit(),
             'MR bar': self.mr_average(),
         }
 
+    def to_csv(self) -> str:
+        output = io.StringIO()
+        writer = csv.writer(output)
+
+        unpl = self.upper_natural_process_limit()
+        x_bar = self.x_average()
+        lnpl = self.lower_natural_process_limit()
+        moving_ranges = self.moving_ranges()
+        url = self.upper_range_limit()
+        mr_bar = self.mr_average()
+
+        writer.writerow(['Counts', 'UNPL', 'X Avg', 'LNPL', 'MR', 'URL', 'MR Avg'])
+        for i, x in enumerate(self.counts):
+            row = [x, unpl, x_bar, lnpl, moving_ranges[i], url, mr_bar]
+            writer.writerow(row)
+
+        return output.getvalue()
+
     def moving_ranges(self) -> TYPE_MOVING_RANGES:
         """
         Moving ranges are the absolute differences between successive count values.
         The first element will always be None
         """
         if self._mr:
             return self._mr
```

### Comparing `statprocon-0.0.6/tests/test_xmr.py` & `statprocon-0.0.7/tests/test_xmr.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,25 @@
 LNPL  : 1.340
 MR    : [None, 1, 1]
 URL   : 3.268
 MR bar: 1.000
 """
         self.assertEqual(xmr.__repr__(), expected)
 
+    def test_to_csv(self):
+        counts = [3, 4, 5]
+        xmr = XmR(counts)
+
+        expected = """Counts,UNPL,X Avg,LNPL,MR,URL,MR Avg\r
+3,6.660,4.000,1.340,,3.268,1.000\r
+4,6.660,4.000,1.340,1,3.268,1.000\r
+5,6.660,4.000,1.340,1,3.268,1.000\r
+"""
+        self.assertEqual(xmr.to_csv(), expected)
+
     def test_average_contains_one_more_exponent_as_input(self):
         counts = [3, 3, 4]
         xmr = XmR(counts)
         self.assertEqual(xmr.x_average(), Decimal('3.333'))
 
     def test_moving_range_ints(self):
         counts = [1, 10, 100, 50]
@@ -39,16 +50,23 @@
 
     def test_moving_range_decimals(self):
         counts = [Decimal('1.25'), Decimal('10.99'), Decimal('5')]
         xmr = XmR(counts)
         mr = xmr.moving_ranges()
         self.assertEqual(mr, [None, Decimal('9.74'), Decimal('5.99')])
 
+    def test_float_input(self):
+        counts = [5.4, 3.8, 8.75, 3.6, 3, 6, 7.4, 10, 5.8, 6.6, 3, 8.8]
+        xmr = XmR(counts)
+        mr = xmr.moving_ranges()
+        expected = [None, Decimal('1.6'), Decimal('4.95'), Decimal('5.15'), Decimal('0.6'), Decimal('3'), Decimal('1.4'), Decimal('2.6'), Decimal('4.2'), Decimal('0.8'), Decimal('3.6'), Decimal('5.8')]
+        self.assertListEqual(mr, expected)
+
     def test_upper_range_limit(self):
-        counts = [1, 10, 100, 50]
+        counts = [1,51, 100, 50]
         xmr = XmR(counts)
         url = xmr.upper_range_limit()
         self.assertEqual(url, Decimal('162.312'))
 
     def test_upper_natural_process_limit(self):
         counts = [1, 10, 100, 50]
         xmr = XmR(counts)
```

### Comparing `statprocon-0.0.6/LICENSE` & `statprocon-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.6/README.md` & `statprocon-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,46 @@
 ```
 
 Currently, this library only supports the data for generating an XmR chart.
 An XmR chart is the simplest type of process behaviour chart.
 XmR is short for individual values (X) and a moving range (mR).
 More chart data options can be added via pull requests.
 
-For more information, I invite you to read [Making Sense of Data by Donald Wheeler](https://www.amazon.com/Making-Sense-Data-Donald-Wheeler/dp/0945320728).
+For more information, please read [Making Sense of Data by Donald Wheeler](https://www.amazon.com/Making-Sense-Data-Donald-Wheeler/dp/0945320728).
+
+### CSV
+
+Quickly generate a CSV of all the data needed to create XmR charts.
+
+```python
+print(xmr.to_csv())
+```
+
+### Google Sheets Charts
+
+Quickly generate XmR Charts in Google Sheets
+
+1. Make a copy of the [statprocon XmR Template sheet](https://docs.google.com/spreadsheets/d/1IdCBpE8FK4qP8B7qHQeXX6amLZ8oyhc8OjlBlGHmWTg/edit?usp=sharing)
+1. Paste the CSV output from above into cell A1
+1. Click `Data -> Split Text to Columns`
+
+The X and MR charts will appear on the right.
+
+Note that the Lower Natural Process Limit may not make sense if your count data could not possibly go negative.
+If LNPL is not needed remove it by:
+
+1. Double click on the X Chart
+1. Click the `Setup` tab
+1. Under `Series`, find `LNPL`
+1. Click the 3 dot menu on the right next to `LNPL`
+1. Click `Remove`
+
+The LNPL line will be removed from the X Chart.
+
+
 
 ## Dependencies
 
 There are a few other Python libraries for generating SPC charts but they all contain large dependencies in order to include the ability to graph the chart.
 This package will remain small and light and not require large dependencies.
 The user will need to convert the data into charts on their own.
```

### Comparing `statprocon-0.0.6/pyproject.toml` & `statprocon-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.0.6/PKG-INFO` & `statprocon-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
@@ -44,15 +44,46 @@
 ```
 
 Currently, this library only supports the data for generating an XmR chart.
 An XmR chart is the simplest type of process behaviour chart.
 XmR is short for individual values (X) and a moving range (mR).
 More chart data options can be added via pull requests.
 
-For more information, I invite you to read [Making Sense of Data by Donald Wheeler](https://www.amazon.com/Making-Sense-Data-Donald-Wheeler/dp/0945320728).
+For more information, please read [Making Sense of Data by Donald Wheeler](https://www.amazon.com/Making-Sense-Data-Donald-Wheeler/dp/0945320728).
+
+### CSV
+
+Quickly generate a CSV of all the data needed to create XmR charts.
+
+```python
+print(xmr.to_csv())
+```
+
+### Google Sheets Charts
+
+Quickly generate XmR Charts in Google Sheets
+
+1. Make a copy of the [statprocon XmR Template sheet](https://docs.google.com/spreadsheets/d/1IdCBpE8FK4qP8B7qHQeXX6amLZ8oyhc8OjlBlGHmWTg/edit?usp=sharing)
+1. Paste the CSV output from above into cell A1
+1. Click `Data -> Split Text to Columns`
+
+The X and MR charts will appear on the right.
+
+Note that the Lower Natural Process Limit may not make sense if your count data could not possibly go negative.
+If LNPL is not needed remove it by:
+
+1. Double click on the X Chart
+1. Click the `Setup` tab
+1. Under `Series`, find `LNPL`
+1. Click the 3 dot menu on the right next to `LNPL`
+1. Click `Remove`
+
+The LNPL line will be removed from the X Chart.
+
+
 
 ## Dependencies
 
 There are a few other Python libraries for generating SPC charts but they all contain large dependencies in order to include the ability to graph the chart.
 This package will remain small and light and not require large dependencies.
 The user will need to convert the data into charts on their own.
```

