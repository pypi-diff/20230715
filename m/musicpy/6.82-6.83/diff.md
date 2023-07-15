# Comparing `tmp/musicpy-6.82.tar.gz` & `tmp/musicpy-6.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\musicpy-6.82.tar", last modified: Sun Jul  9 12:33:05 2023, max compression
+gzip compressed data, was "dist\musicpy-6.83.tar", last modified: Sat Jul 15 16:24:09 2023, max compression
```

## Comparing `musicpy-6.82.tar` & `musicpy-6.83.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 12:33:05.000000 musicpy-6.82/
--rw-rw-rw-   0        0        0    27030 2021-09-24 07:05:14.000000 musicpy-6.82/LICENSE
--rw-rw-rw-   0        0        0       40 2021-10-04 19:46:56.000000 musicpy-6.82/MANIFEST.in
--rw-rw-rw-   0        0        0    16335 2023-07-09 12:33:06.000000 musicpy-6.82/PKG-INFO
--rw-rw-rw-   0        0        0    14214 2023-04-18 07:20:38.000000 musicpy-6.82/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 12:33:05.000000 musicpy-6.82/musicpy/
--rw-rw-rw-   0        0        0       90 2022-05-24 06:43:42.000000 musicpy-6.82/musicpy/__init__.py
--rw-rw-rw-   0        0        0   114541 2023-07-08 14:22:54.000000 musicpy-6.82/musicpy/algorithms.py
--rw-rw-rw-   0        0        0    10091 2023-07-03 18:50:48.000000 musicpy-6.82/musicpy/control.py
--rw-rw-rw-   0        0        0    29186 2023-07-06 04:17:40.000000 musicpy-6.82/musicpy/database.py
--rw-rw-rw-   0        0        0    59778 2023-07-04 15:40:36.000000 musicpy-6.82/musicpy/daw.py
--rw-rw-rw-   0        0        0    84158 2023-07-08 13:42:42.000000 musicpy-6.82/musicpy/musicpy.py
--rw-rw-rw-   0        0        0       38 2023-03-06 07:58:48.000000 musicpy-6.82/musicpy/requirements for musicpy daw.txt
--rw-rw-rw-   0        0        0       18 2022-10-11 02:50:12.000000 musicpy-6.82/musicpy/requirements.txt
--rw-rw-rw-   0        0        0   266874 2023-07-09 08:40:56.000000 musicpy-6.82/musicpy/structures.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:33:05.000000 musicpy-6.82/musicpy.egg-info/
--rw-rw-rw-   0        0        0    16335 2023-07-09 12:33:06.000000 musicpy-6.82/musicpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-07-09 12:33:06.000000 musicpy-6.82/musicpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 12:33:06.000000 musicpy-6.82/musicpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-09 12:33:06.000000 musicpy-6.82/musicpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-09 12:33:06.000000 musicpy-6.82/musicpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-09 12:33:06.000000 musicpy-6.82/setup.cfg
--rw-rw-rw-   0        0        0     1402 2023-07-09 08:18:56.000000 musicpy-6.82/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:24:09.000000 musicpy-6.83/
+-rw-rw-rw-   0        0        0    27030 2021-09-24 07:05:14.000000 musicpy-6.83/LICENSE
+-rw-rw-rw-   0        0        0       40 2021-10-04 19:46:56.000000 musicpy-6.83/MANIFEST.in
+-rw-rw-rw-   0        0        0    16335 2023-07-15 16:24:10.000000 musicpy-6.83/PKG-INFO
+-rw-rw-rw-   0        0        0    14214 2023-04-18 07:20:38.000000 musicpy-6.83/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 16:24:09.000000 musicpy-6.83/musicpy/
+-rw-rw-rw-   0        0        0       90 2022-05-24 06:43:42.000000 musicpy-6.83/musicpy/__init__.py
+-rw-rw-rw-   0        0        0   114541 2023-07-08 14:22:54.000000 musicpy-6.83/musicpy/algorithms.py
+-rw-rw-rw-   0        0        0    10091 2023-07-03 18:50:48.000000 musicpy-6.83/musicpy/control.py
+-rw-rw-rw-   0        0        0    29578 2023-07-15 15:22:38.000000 musicpy-6.83/musicpy/database.py
+-rw-rw-rw-   0        0        0    59778 2023-07-04 15:40:36.000000 musicpy-6.83/musicpy/daw.py
+-rw-rw-rw-   0        0        0    84158 2023-07-08 13:42:42.000000 musicpy-6.83/musicpy/musicpy.py
+-rw-rw-rw-   0        0        0       38 2023-03-06 07:58:48.000000 musicpy-6.83/musicpy/requirements for musicpy daw.txt
+-rw-rw-rw-   0        0        0       18 2022-10-11 02:50:12.000000 musicpy-6.83/musicpy/requirements.txt
+-rw-rw-rw-   0        0        0   266704 2023-07-15 15:22:22.000000 musicpy-6.83/musicpy/structures.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:24:09.000000 musicpy-6.83/musicpy.egg-info/
+-rw-rw-rw-   0        0        0    16335 2023-07-15 16:24:10.000000 musicpy-6.83/musicpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-07-15 16:24:10.000000 musicpy-6.83/musicpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 16:24:10.000000 musicpy-6.83/musicpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-15 16:24:10.000000 musicpy-6.83/musicpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-15 16:24:10.000000 musicpy-6.83/musicpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 16:24:10.000000 musicpy-6.83/setup.cfg
+-rw-rw-rw-   0        0        0     1402 2023-07-15 11:04:42.000000 musicpy-6.83/setup.py
```

### Comparing `musicpy-6.82/LICENSE` & `musicpy-6.83/LICENSE`

 * *Files identical despite different names*

### Comparing `musicpy-6.82/PKG-INFO` & `musicpy-6.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: musicpy
-Version: 6.82
+Version: 6.83
 Summary: Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms.
 Home-page: https://github.com/Rainbow-Dreamer/musicpy.git
 Author: Rainbow-Dreamer
 Author-email: 1036889495@qq.com
 License: LGPLv2.1
-Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.82.tar.gz
+Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.83.tar.gz
 Description: musicpy
         =======
         [中文](https://github.com/Rainbow-Dreamer/musicpy/blob/master/README_cn.md)
         
         Have you ever thought about writing music with codes in a very concise, human-readable syntax?
         
         Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms. It is easy to learn and write, easy to read, and incorporates a fully computerized music theory system.
```

### Comparing `musicpy-6.82/README.md` & `musicpy-6.83/README.md`

 * *Files identical despite different names*

### Comparing `musicpy-6.82/musicpy/algorithms.py` & `musicpy-6.83/musicpy/algorithms.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.82/musicpy/control.py` & `musicpy-6.83/musicpy/control.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.82/musicpy/database.py` & `musicpy-6.83/musicpy/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,18 @@
             current_pitch_name = other.name.upper()[0]
             current_pitch_name_ind = standard_pitch_name.index(
                 current_pitch_name)
             new_other_name = standard_pitch_name[(current_pitch_name_ind +
                                                   self.direction *
                                                   (self.number - 1)) %
                                                  len(standard_pitch_name)]
-            result = mp.degree_to_note(other.degree + self.value)
+            result = mp.degree_to_note(degree=other.degree + self.value,
+                                       duration=other.duration,
+                                       volume=other.volume,
+                                       channel=other.channel)
             result.name = mp.relative_note(result.name, new_other_name)
         else:
             result = self.value + other
         return result
 
     def __radd__(self, other):
         return self.__add__(other)
@@ -162,15 +165,18 @@
             current_pitch_name = other.name.upper()[0]
             current_pitch_name_ind = standard_pitch_name.index(
                 current_pitch_name)
             new_other_name = standard_pitch_name[(current_pitch_name_ind -
                                                   self.direction *
                                                   (self.number - 1)) %
                                                  len(standard_pitch_name)]
-            result = mp.degree_to_note(other.degree - self.value)
+            result = mp.degree_to_note(degree=other.degree - self.value,
+                                       duration=other.duration,
+                                       volume=other.volume,
+                                       channel=other.channel)
             result.name = mp.relative_note(result.name, new_other_name)
         else:
             result = other - self.value
         return result
 
     def __neg__(self):
         result = copy(self)
```

### Comparing `musicpy-6.82/musicpy/daw.py` & `musicpy-6.83/musicpy/daw.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.82/musicpy/musicpy.py` & `musicpy-6.83/musicpy/musicpy.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.82/musicpy/structures.py` & `musicpy-6.83/musicpy/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,31 +128,30 @@
         if isinstance(other, chord):
             temp = copy(other)
             temp.insert(ind, copy(self))
             temp.interval.insert(ind, interval)
             return temp
 
     def up(self, unit=1):
-        return mp.degree_to_note(self.degree + unit, self.duration,
-                                 self.volume, self.channel)
+        if isinstance(unit, database.Interval):
+            return self + unit
+        else:
+            return mp.degree_to_note(self.degree + unit, self.duration,
+                                     self.volume, self.channel)
 
     def down(self, unit=1):
         return self.up(-unit)
 
     def sharp(self, unit=1):
-        if isinstance(unit, database.Interval):
-            return self + unit
         temp = self
         for i in range(unit):
             temp += database.A1
         return temp
 
     def flat(self, unit=1):
-        if isinstance(unit, database.Interval):
-            return self - unit
         temp = self
         for i in range(unit):
             temp -= database.A1
         return temp
 
     def __pos__(self):
         return self.up()
@@ -763,25 +762,23 @@
         if not isinstance(note1, note):
             note1 = mp.to_note(note1)
             if note1.name in database.standard_dict:
                 note1.name = database.standard_dict[note1.name]
         return note1 in self.same_accidentals().notes
 
     def __add__(self, obj):
-        if isinstance(obj, (int, list)):
+        if isinstance(obj, (int, list, database.Interval)):
             return self.up(obj)
         elif isinstance(obj, tuple):
             if isinstance(obj[0], chord):
                 return self | obj
             else:
                 return self.up(*obj)
         elif isinstance(obj, rest):
             return self.rest(obj.get_duration())
-        elif isinstance(obj, database.Interval):
-            return self.sharp(obj)
         temp = copy(self)
         if isinstance(obj, note):
             temp.notes.append(copy(obj))
             temp.interval.append(temp.interval[-1])
         elif isinstance(obj, str):
             return temp + mp.to_note(obj)
         elif isinstance(obj, chord):
@@ -996,20 +993,18 @@
             self.interval.pop()
         else:
             result = self.notes.pop(ind)
             self.interval.pop(ind)
         return result
 
     def __sub__(self, obj):
-        if isinstance(obj, (int, list)):
+        if isinstance(obj, (int, list, database.Interval)):
             return self.down(obj)
         elif isinstance(obj, tuple):
             return self.down(*obj)
-        elif isinstance(obj, database.Interval):
-            return self.flat(obj)
         if not isinstance(obj, note):
             obj = mp.to_note(obj)
         temp = copy(self)
         if obj in temp:
             ind = temp.notes.index(obj)
             del temp.notes[ind]
             del temp.interval[ind]
@@ -1323,18 +1318,18 @@
                 root = list(root)
             else:
                 root = [mp.to_note(i) for i in root]
             return [self.on(x, duration, interval) for x in root]
 
     def up(self, unit=1, ind=None, ind2=None):
         temp = copy(self)
-        if not isinstance(unit, int):
+        if not isinstance(unit, (int, database.Interval)):
             temp.notes = [temp.notes[k].up(unit[k]) for k in range(len(unit))]
             return temp
-        if not isinstance(ind, int) and ind is not None:
+        if not isinstance(ind, (int, database.Interval)) and ind is not None:
             temp.notes = [
                 temp.notes[i].up(unit) if i in ind else temp.notes[i]
                 for i in range(len(temp.notes))
             ]
             return temp
         if ind2 is None:
             if ind is None:
@@ -1344,15 +1339,15 @@
         else:
             temp.notes = temp.notes[:ind] + [
                 each.up(unit) for each in temp.notes[ind:ind2]
             ] + temp.notes[ind2:]
         return temp
 
     def down(self, unit=1, ind=None, ind2=None):
-        if not isinstance(unit, int):
+        if not isinstance(unit, (int, database.Interval)):
             unit = [-i for i in unit]
             return self.up(unit, ind, ind2)
         return self.up(-unit, ind, ind2)
 
     def sharp(self, unit=1):
         temp = copy(self)
         temp.notes = [i.sharp(unit=unit) for i in temp.notes]
@@ -2438,23 +2433,23 @@
         high = False
         if degree1 == 7:
             degree1 = 0
             high = True
         temp = copy(self)
         scale_notes = temp.notes[:-1]
         for i in range(degree1, degree1 + step * num, step):
-            result.append(scale_notes[i % 7])
+            result.append(scale_notes[i % 7].name)
         result_chord = chord(result,
                              rootpitch=temp[0].num,
                              interval=interval,
                              duration=duration)
         if standardize:
             result_chord = result_chord.standardize()
         if high:
-            result_chord = result_chord.up(database.octave)
+            result_chord = result_chord + database.octave
         return result_chord
 
     def pattern(self, indlist, duration=1 / 4, interval=0, num=3, step=2):
         if isinstance(indlist, str):
             indlist = [int(i) for i in indlist]
         elif isinstance(indlist, int):
             indlist = [int(i) for i in str(indlist)]
@@ -2719,28 +2714,24 @@
         result.mode = result.detect()
         return result
 
     def play(self, intervals=1 / 4, durations=None, *args, **kwargs):
         mp.play(self.get_scale(intervals, durations), *args, **kwargs)
 
     def __add__(self, obj):
-        if isinstance(obj, int):
+        if isinstance(obj, (int, database.Interval)):
             return self.up(obj)
         elif isinstance(obj, tuple):
             return self.up(*obj)
-        elif isinstance(obj, database.Interval):
-            return self.sharp(obj)
 
     def __sub__(self, obj):
-        if isinstance(obj, int):
+        if isinstance(obj, (int, database.Interval)):
             return self.down(obj)
         elif isinstance(obj, tuple):
             return self.down(*obj)
-        elif isinstance(obj, database.Interval):
-            return self.flat(obj)
 
     def chord_progression(self,
                           chords,
                           durations=1 / 4,
                           intervals=0,
                           volumes=None,
                           chords_interval=None,
@@ -3396,23 +3387,23 @@
         if isinstance(n, tuple):
             n, start_time = n
         else:
             start_time = 0
         return self.merge_track(n, mode='head', start_time=start_time)
 
     def __add__(self, n):
-        if isinstance(n, int):
+        if isinstance(n, (int, database.Interval)):
             return self.up(n)
         elif isinstance(n, piece):
             return self.merge_track(n, mode='after')
         elif isinstance(n, tuple):
             return self.up(*n)
 
     def __sub__(self, n):
-        if isinstance(n, int):
+        if isinstance(n, (int, database.Interval)):
             return self.down(n)
         elif isinstance(n, tuple):
             return self.down(*n)
 
     def __neg__(self):
         return self.down()
 
@@ -4509,23 +4500,23 @@
     def __pos__(self):
         return self.up()
 
     def __neg__(self):
         return self.down()
 
     def __add__(self, i):
-        if isinstance(i, int):
+        if isinstance(i, (int, database.Interval)):
             return self.up(i)
         else:
             temp = copy(self)
             temp.content += i
             return temp
 
     def __sub__(self, i):
-        if isinstance(i, int):
+        if isinstance(i, (int, database.Interval)):
             return self.down(i)
 
     def __or__(self, i):
         temp = copy(self)
         temp.content |= i
         return temp
```

### Comparing `musicpy-6.82/musicpy.egg-info/PKG-INFO` & `musicpy-6.83/musicpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: musicpy
-Version: 6.82
+Version: 6.83
 Summary: Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms.
 Home-page: https://github.com/Rainbow-Dreamer/musicpy.git
 Author: Rainbow-Dreamer
 Author-email: 1036889495@qq.com
 License: LGPLv2.1
-Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.82.tar.gz
+Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.83.tar.gz
 Description: musicpy
         =======
         [中文](https://github.com/Rainbow-Dreamer/musicpy/blob/master/README_cn.md)
         
         Have you ever thought about writing music with codes in a very concise, human-readable syntax?
         
         Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms. It is easy to learn and write, easy to read, and incorporates a fully computerized music theory system.
```

### Comparing `musicpy-6.82/setup.py` & `musicpy-6.83/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='musicpy',
     packages=find_packages(),
     package_data={'musicpy': ['./*']},
-    version='6.82',
+    version='6.83',
     license='LGPLv2.1',
     description=
     'Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms.',
     author='Rainbow-Dreamer',
     author_email='1036889495@qq.com',
     url='https://github.com/Rainbow-Dreamer/musicpy.git',
     download_url=
-    'https://github.com/Rainbow-Dreamer/musicpy/archive/6.82.tar.gz',
+    'https://github.com/Rainbow-Dreamer/musicpy/archive/6.83.tar.gz',
     keywords=[
         'music language', 'use codes to write music', 'music language for AI'
     ],
     install_requires=['mido-fix', 'pygame', 'dataclasses'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

