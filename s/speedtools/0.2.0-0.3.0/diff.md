# Comparing `tmp/speedtools-0.2.0.tar.gz` & `tmp/speedtools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtools-0.2.0.tar", last modified: Fri Jun 23 21:02:04 2023, max compression
+gzip compressed data, was "speedtools-0.3.0.tar", last modified: Sat Jul 15 20:58:21 2023, max compression
```

## Comparing `speedtools-0.2.0.tar` & `speedtools-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 21:01:49.000000 speedtools-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-23 21:02:04.323625 speedtools-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-23 21:01:49.000000 speedtools-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-23 21:01:49.000000 speedtools-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:02:04.323625 speedtools-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 21:01:49.000000 speedtools-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/blender/
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/blender/io_nfs4_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/frd_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/qfs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/refpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/fce.ksy
--rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/frd.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/fsh.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/qfs.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/viv.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/speedtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/tr_ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/viv_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 20:58:05.000000 speedtools-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-15 20:58:21.587999 speedtools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-15 20:58:05.000000 speedtools-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-15 20:58:05.000000 speedtools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:58:21.587999 speedtools-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-15 20:58:05.000000 speedtools-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/blender/io_nfs4_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/frd_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/qfs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/refpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/fce.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/frd.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/fsh.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/qfs.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/viv.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/speedtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/tr_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/viv_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/top_level.txt
```

### Comparing `speedtools-0.2.0/LICENSE` & `speedtools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/PKG-INFO` & `speedtools-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -60,10 +60,10 @@
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
 
-[1]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
-[2]: https://pypi.org/project/speedtools/
+[1]: https://pypi.org/project/speedtools/
+[2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.2.0/README.md` & `speedtools-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
 
-[1]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
-[2]: https://pypi.org/project/speedtools/
+[1]: https://pypi.org/project/speedtools/
+[2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.2.0/pyproject.toml` & `speedtools-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedtools"
-version = "0.2.0"
+version = "0.3.0"
 description = "NFS4 HS (PC) resource utilities"
 authors = [{ name = "Rafał Kuźnia" }, { email = "rafal.kuznia@protonmail.com" }]
 readme = { file = 'README.md', content-type = 'text/markdown' }
 dependencies = ["kaitaistruct", "pillow", "click", "more-itertools", "parse"]
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

### Comparing `speedtools-0.2.0/setup.py` & `speedtools-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/blender/io_nfs4_import.py` & `speedtools-0.3.0/speedtools/blender/io_nfs4_import.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from bpy.props import BoolProperty, EnumProperty, StringProperty
 from more_itertools import collapse
 
 from speedtools import TrackData, VivData
 from speedtools.types import (
     Animation,
     BaseMesh,
+    DirectionalLight,
     DrawableMesh,
     Light,
     Part,
     Polygon,
     Resource,
     Vector3d,
 )
@@ -161,14 +162,24 @@
         bpy_light.specular_factor = 0.2
         bpy_light.energy = 500  # type: ignore[attr-defined]
         bpy_light.use_shadow = False  # type: ignore[attr-defined]
         bpy_obj = bpy.data.objects.new(name=name, object_data=bpy_light)
         self.set_object_location(obj=bpy_obj, location=light.location)
         return bpy_obj
 
+    def make_directional_light_object(
+        self, name: str, light: DirectionalLight
+    ) -> bpy.types.Object:
+        bpy_sun = bpy.data.lights.new(name=name, type="SUN")
+        bpy_obj = bpy.data.objects.new(name=name, object_data=bpy_sun)
+        mu_euler = mathutils.Euler(light.euler_xyz)
+        bpy_obj.rotation_mode = "XYZ"
+        bpy_obj.rotation_euler = mu_euler  # type: ignore[assignment]
+        return bpy_obj
+
 
 class TrackImportStrategy(metaclass=ABCMeta):
     @abstractmethod
     def import_track(self, track: TrackData) -> None:
         pass
 
 
@@ -188,14 +199,18 @@
             if obj.animation:
                 self.set_object_animation(obj=bpy_obj, animation=obj.animation)
             track_collection.objects.link(bpy_obj)
         for index, light in enumerate(track.lights):
             name = f"Track light {index}"
             bpy_obj = self.make_light_object(name=name, light=light)
             track_collection.objects.link(bpy_obj)
+        directional_light = track.directional_light
+        if directional_light:
+            bpy_obj = self.make_directional_light_object(name="sun", light=directional_light)
+            track_collection.objects.link(bpy_obj)
 
 
 class TrackImportAdvanced(TrackImportStrategy, BaseImporter):
     def import_track(self, track: TrackData) -> None:
         track_collection = bpy.data.collections.new("Track segments")
         bpy.context.scene.collection.children.link(track_collection)
         for index, segment in enumerate(track.track_segments):
@@ -218,14 +233,18 @@
             if obj.animation:
                 self.set_object_animation(obj=bpy_obj, animation=obj.animation)
             track_collection.objects.link(bpy_obj)
         for index, light in enumerate(track.lights):
             name = f"Track light {index}"
             bpy_obj = self.make_light_object(name=name, light=light)
             track_collection.objects.link(bpy_obj)
+        directional_light = track.directional_light
+        if directional_light:
+            bpy_obj = self.make_directional_light_object(name="sun", light=directional_light)
+            track_collection.objects.link(bpy_obj)
 
 
 class CarImporterSimple(BaseImporter):
     def import_car(self, parts: Iterable[Part]) -> None:
         car_collection = bpy.data.collections.new("Car parts")
         bpy.context.scene.collection.children.link(car_collection)
         for part in parts:
```

### Comparing `speedtools-0.2.0/speedtools/frd_data.py` & `speedtools-0.3.0/speedtools/frd_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/qfs_data.py` & `speedtools-0.3.0/speedtools/qfs_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/refpack.py` & `speedtools-0.3.0/speedtools/refpack.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/specs/fce.ksy` & `speedtools-0.3.0/speedtools/specs/fce.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/specs/frd.ksy` & `speedtools-0.3.0/speedtools/specs/frd.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/specs/fsh.ksy` & `speedtools-0.3.0/speedtools/specs/fsh.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/specs/viv.ksy` & `speedtools-0.3.0/speedtools/specs/viv.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/speedtool.py` & `speedtools-0.3.0/speedtools/speedtool.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/tr_ini.py` & `speedtools-0.3.0/speedtools/tr_ini.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,24 +5,35 @@
 #
 
 from __future__ import annotations
 
 import logging
 from collections.abc import Iterator
 from configparser import ConfigParser
+from dataclasses import dataclass
 from itertools import starmap
 from pathlib import Path
 
 from parse import parse, search  # type: ignore[import]
 
 from speedtools.types import Color, LightAttributes
 
 logger = logging.getLogger(__name__)
 
 
+@dataclass(frozen=True)
+class SunIni:
+    angle_theta: float
+    angle_rho: float
+    radius: float
+    rotates: bool
+    additive: bool
+    in_front: bool
+
+
 class TrackIni:
     def __init__(self, parser: ConfigParser) -> None:
         self.parser = parser
 
     @classmethod
     def from_file(cls, path: Path) -> TrackIni:
         parser = ConfigParser()
@@ -44,7 +55,24 @@
             blink_interval_ms=blink_interval,
             flare_size=flare_size,
         )
 
     @property
     def glows(self) -> Iterator[LightAttributes]:
         return starmap(self._make_glow, self.parser["track glows"].items())
+
+    @property
+    def sun(self) -> SunIni | None:
+        try:
+            sun = self.parser["sun"]
+            if bool(sun["hasSun"]) is False:
+                return None
+            return SunIni(
+                angle_theta=float(sun["angleTheta"]),
+                angle_rho=float(sun["angleRho"]),
+                radius=float(sun["radius"]),
+                rotates=bool(sun.get("rotates", "0")),
+                additive=bool(sun.get("additive", "0")),
+                in_front=bool(sun.get("inFront", "0")),
+            )
+        except KeyError:
+            return None
```

### Comparing `speedtools-0.2.0/speedtools/track_data.py` & `speedtools-0.3.0/speedtools/track_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 import logging
 from collections.abc import Callable, Iterator
 from contextlib import suppress
+from math import atan2, cos, tau
 from pathlib import Path
 from typing import TypeVar
 
 from speedtools.frd_data import FrdData
 from speedtools.qfs_data import QfsData
 from speedtools.tr_ini import TrackIni
 from speedtools.types import (
+    DirectionalLight,
     Light,
     LightAttributes,
     LightStub,
     Polygon,
     Resource,
     TrackObject,
     TrackSegment,
@@ -26,14 +28,16 @@
 from speedtools.utils import count_repeats_and_map
 
 logger = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 class TrackData:
+    SUN_DISTANCE = 3000
+
     def __init__(
         self, directory: Path, mirrored: bool = False, night: bool = False, weather: bool = False
     ) -> None:
         logger.debug(f"Opening directory {directory}")
         self.frd: FrdData = self.tr_open(
             constructor=FrdData.from_file,
             directory=directory,
@@ -145,7 +149,21 @@
 
     @property
     def lights(self) -> Iterator[Light]:
         if not self.light_glows:
             for attribute in self.ini.glows:
                 self.light_glows[attribute.identifier] = attribute
         return map(self._make_light, self.frd.light_dummies)
+
+    @property
+    def directional_light(self) -> DirectionalLight | None:
+        sun = self.ini.sun
+        if sun is None:
+            return None
+        # Angles in INI are in turns. Turns are converted to radians here.
+        # The INI angleRho value is not really a spherical coordinate.
+        # Some approximations are done here to convert to spherical coordinates.
+        rho = sun.angle_rho * tau
+        z = self.SUN_DISTANCE * cos(rho)
+        phi = atan2(z, self.SUN_DISTANCE)
+        theta = sun.angle_theta * tau
+        return DirectionalLight(rho=phi, theta=theta, radius=sun.radius)
```

### Comparing `speedtools-0.2.0/speedtools/types.py` & `speedtools-0.3.0/speedtools/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
+from __future__ import annotations
+
 from collections.abc import Sequence
 from dataclasses import dataclass, field
+from math import pi
 from typing import NamedTuple, Optional, TypeAlias
 
 from speedtools.parsers import FrdParser, FshParser
 
 RoadEffect: TypeAlias = FrdParser.DriveablePolygon.RoadEffect
 CollisionType: TypeAlias = FrdParser.ObjectAttribute.CollisionType
 ObjectType: TypeAlias = FrdParser.ObjectHeader.ObjectType
@@ -150,7 +153,20 @@
     attributes: LightAttributes
 
 
 @dataclass(frozen=True)
 class LightStub:
     location: Vector3d
     glow_id: int
+
+
+@dataclass(frozen=True)
+class DirectionalLight:
+    rho: float
+    theta: float
+    radius: float
+
+    @property
+    def euler_xyz(self) -> Vector3d:
+        z = pi / 2 - self.rho
+        y = self.theta
+        return Vector3d(x=0, y=y, z=z)
```

### Comparing `speedtools-0.2.0/speedtools/utils.py` & `speedtools-0.3.0/speedtools/utils.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools/viv_data.py` & `speedtools-0.3.0/speedtools/viv_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.2.0/speedtools.egg-info/PKG-INFO` & `speedtools-0.3.0/speedtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -60,10 +60,10 @@
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
 
-[1]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
-[2]: https://pypi.org/project/speedtools/
+[1]: https://pypi.org/project/speedtools/
+[2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.2.0/speedtools.egg-info/SOURCES.txt` & `speedtools-0.3.0/speedtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

