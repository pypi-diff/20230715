# Comparing `tmp/lvmgort-0.1.0.tar.gz` & `tmp/lvmgort-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvmgort-0.1.0.tar", max compression
+gzip compressed data, was "lvmgort-0.1.1.tar", max compression
```

## Comparing `lvmgort-0.1.0.tar` & `lvmgort-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1504 2023-07-14 16:56:19.603748 lvmgort-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      713 2023-07-14 16:56:19.604127 lvmgort-0.1.0/README.md
--rw-r--r--   0        0        0     2665 2023-07-14 16:56:19.615186 lvmgort-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      540 2023-07-14 16:56:19.615994 lvmgort-0.1.0/src/gort/__init__.py
--rw-r--r--   0        0        0      713 2023-07-14 16:56:19.617255 lvmgort-0.1.0/src/gort/__main__.py
--rw-r--r--   0        0        0     6727 2023-07-14 16:56:19.617743 lvmgort-0.1.0/src/gort/core.py
--rw-r--r--   0        0        0      386 2023-07-14 16:56:19.618283 lvmgort-0.1.0/src/gort/devices/__init__.py
--rw-r--r--   0        0        0     3604 2023-07-14 16:56:19.618808 lvmgort-0.1.0/src/gort/devices/ag.py
--rw-r--r--   0        0        0     2917 2023-07-14 16:56:19.619210 lvmgort-0.1.0/src/gort/devices/enclosure.py
--rw-r--r--   0        0        0    12353 2023-07-14 16:56:19.619787 lvmgort-0.1.0/src/gort/devices/guider.py
--rw-r--r--   0        0        0     1446 2023-07-14 16:56:19.620242 lvmgort-0.1.0/src/gort/devices/nps.py
--rw-r--r--   0        0        0    16357 2023-07-14 16:56:19.620714 lvmgort-0.1.0/src/gort/devices/spec.py
--rw-r--r--   0        0        0    24865 2023-07-14 16:56:19.621236 lvmgort-0.1.0/src/gort/devices/telescope.py
--rw-r--r--   0        0        0     5088 2023-07-14 16:56:19.621943 lvmgort-0.1.0/src/gort/etc/lvmgort.yml
--rw-r--r--   0        0        0     3511 2023-07-14 16:56:19.622485 lvmgort-0.1.0/src/gort/exceptions.py
--rw-r--r--   0        0        0    14444 2023-07-14 16:56:19.622953 lvmgort-0.1.0/src/gort/gort.py
--rw-r--r--   0        0        0     4582 2023-07-14 16:56:19.623402 lvmgort-0.1.0/src/gort/kubernetes.py
--rw-r--r--   0        0        0     1002 2023-07-14 16:56:19.623986 lvmgort-0.1.0/src/gort/maskbits.py
--rw-r--r--   0        0        0    16513 2023-07-14 16:56:19.624397 lvmgort-0.1.0/src/gort/observer.py
--rw-r--r--   0        0        0    16950 2023-07-14 16:56:19.624833 lvmgort-0.1.0/src/gort/tile.py
--rw-r--r--   0        0        0    15629 2023-07-14 16:56:19.625237 lvmgort-0.1.0/src/gort/tools.py
--rw-r--r--   0        0        0     7494 2023-07-14 16:56:19.625620 lvmgort-0.1.0/src/gort/transforms.py
--rw-r--r--   0        0        0     5161 2023-07-14 16:56:19.625956 lvmgort-0.1.0/src/gort/websocket.py
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 lvmgort-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-14 22:08:11.780650 lvmgort-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      713 2023-07-14 22:08:11.781031 lvmgort-0.1.1/README.md
+-rw-r--r--   0        0        0     2665 2023-07-14 22:08:11.794285 lvmgort-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      540 2023-07-14 22:08:11.795162 lvmgort-0.1.1/src/gort/__init__.py
+-rw-r--r--   0        0        0      713 2023-07-14 22:08:11.795511 lvmgort-0.1.1/src/gort/__main__.py
+-rw-r--r--   0        0        0     6727 2023-07-14 22:08:11.795895 lvmgort-0.1.1/src/gort/core.py
+-rw-r--r--   0        0        0      386 2023-07-14 22:08:11.796299 lvmgort-0.1.1/src/gort/devices/__init__.py
+-rw-r--r--   0        0        0     3604 2023-07-14 22:08:11.796655 lvmgort-0.1.1/src/gort/devices/ag.py
+-rw-r--r--   0        0        0     2917 2023-07-14 22:08:11.797012 lvmgort-0.1.1/src/gort/devices/enclosure.py
+-rw-r--r--   0        0        0    12353 2023-07-14 22:08:11.797381 lvmgort-0.1.1/src/gort/devices/guider.py
+-rw-r--r--   0        0        0     1446 2023-07-14 22:08:11.797701 lvmgort-0.1.1/src/gort/devices/nps.py
+-rw-r--r--   0        0        0    16357 2023-07-14 22:08:11.798098 lvmgort-0.1.1/src/gort/devices/spec.py
+-rw-r--r--   0        0        0    24865 2023-07-14 22:08:11.798519 lvmgort-0.1.1/src/gort/devices/telescope.py
+-rw-r--r--   0        0        0     5088 2023-07-14 22:08:11.799030 lvmgort-0.1.1/src/gort/etc/lvmgort.yml
+-rw-r--r--   0        0        0     3511 2023-07-14 22:08:11.799343 lvmgort-0.1.1/src/gort/exceptions.py
+-rw-r--r--   0        0        0    14444 2023-07-14 22:08:11.799967 lvmgort-0.1.1/src/gort/gort.py
+-rw-r--r--   0        0        0     4582 2023-07-14 22:08:11.800754 lvmgort-0.1.1/src/gort/kubernetes.py
+-rw-r--r--   0        0        0     1002 2023-07-14 22:08:11.801127 lvmgort-0.1.1/src/gort/maskbits.py
+-rw-r--r--   0        0        0    16601 2023-07-14 22:08:11.801560 lvmgort-0.1.1/src/gort/observer.py
+-rw-r--r--   0        0        0    17411 2023-07-14 22:08:11.802025 lvmgort-0.1.1/src/gort/tile.py
+-rw-r--r--   0        0        0    15629 2023-07-14 22:08:11.802492 lvmgort-0.1.1/src/gort/tools.py
+-rw-r--r--   0        0        0     8584 2023-07-14 22:08:11.802931 lvmgort-0.1.1/src/gort/transforms.py
+-rw-r--r--   0        0        0     5161 2023-07-14 22:08:11.803310 lvmgort-0.1.1/src/gort/websocket.py
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 lvmgort-0.1.1/PKG-INFO
```

### Comparing `lvmgort-0.1.0/LICENSE.md` & `lvmgort-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/README.md` & `lvmgort-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/pyproject.toml` & `lvmgort-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lvmgort"
-version = "0.1.0"
+version = "0.1.1"
 description = "The brains of LVM observing"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmgort"
 repository = "https://github.com/sdss/lvmgort"
 documentation = "https://lvmgort.readthedocs.org"
```

### Comparing `lvmgort-0.1.0/src/gort/__init__.py` & `lvmgort-0.1.1/src/gort/__init__.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/__main__.py` & `lvmgort-0.1.1/src/gort/__main__.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/core.py` & `lvmgort-0.1.1/src/gort/core.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/devices/ag.py` & `lvmgort-0.1.1/src/gort/devices/ag.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/devices/enclosure.py` & `lvmgort-0.1.1/src/gort/devices/enclosure.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/devices/guider.py` & `lvmgort-0.1.1/src/gort/devices/guider.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/devices/nps.py` & `lvmgort-0.1.1/src/gort/devices/nps.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/devices/spec.py` & `lvmgort-0.1.1/src/gort/devices/spec.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/devices/telescope.py` & `lvmgort-0.1.1/src/gort/devices/telescope.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/etc/lvmgort.yml` & `lvmgort-0.1.1/src/gort/etc/lvmgort.yml`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/exceptions.py` & `lvmgort-0.1.1/src/gort/exceptions.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/gort.py` & `lvmgort-0.1.1/src/gort/gort.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/kubernetes.py` & `lvmgort-0.1.1/src/gort/kubernetes.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/maskbits.py` & `lvmgort-0.1.1/src/gort/maskbits.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/observer.py` & `lvmgort-0.1.1/src/gort/observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
         self.gort = gort
         self.tile = tile
 
         self.mask_positions = self._get_mask_positions(mask_positions_pattern)
 
         self.guide_task: asyncio.Future | None = None
 
+    def __repr__(self):
+        return f"<GortObserver (tile_id={self.tile.tile_id})>"
+
     async def slew(self):
         """Slew to the telescope fields."""
 
         cotasks = []
 
         # Stops guiders.
         await self.gort.guiders.stop()
```

### Comparing `lvmgort-0.1.0/src/gort/tile.py` & `lvmgort-0.1.1/src/gort/tile.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import pandas
 from astropy.coordinates import EarthLocation, SkyCoord
 from astropy.time import Time
 from httpx import RequestError
 
 from gort.exceptions import GortNotImplemented, GortWarning, TileError
 from gort.tools import get_calibrators_sync, get_db_connection, get_next_tile_id_sync
-from gort.transforms import offset_to_master_frame_pixel, read_fibermap
+from gort.transforms import fibre_to_master_frame
 
 
 __all__ = [
     "Coordinates",
     "QuerableCoordinates",
     "ScienceCoordinates",
     "SkyCoordinates",
@@ -180,34 +180,49 @@
 
     def __init__(self, ra: float, dec: float, centre_on_fibre: str | None = None):
         super().__init__(ra, dec)
 
         self.centre_on_fibre = centre_on_fibre
 
         # The MF pixel on which to guide/centre the target.
-        self._mf_pixel = self._set_mf_pixel(centre_on_fibre)
+        self._mf_pixel = self.set_mf_pixel(centre_on_fibre)
 
-    def _set_mf_pixel(self, fibre_name: str | None = None):
-        """Calculates the MF pixel on which to centre the target."""
+    def set_mf_pixel(self, fibre_name: str | None = None, xz: CoordTuple | None = None):
+        """Calculates and sets the master frame pixel on which to centre the target.
 
-        if fibre_name is None:
-            self._mf_pixel = None
-            return None
-
-        fibermap = read_fibermap()
+        If neither ``fibre_name`` or ``xz`` are passed, resets to centring
+        the target on the central fibre of the IFU.
 
-        if fibre_name not in fibermap.fibername.values:
-            raise NameError(f"Fibre {fibre_name} not found in fibermap.")
+        Parameters
+        ----------
+        fibre_name
+            The fibre to which to centre the target, with the format
+            ``<ifulabel>-<finifu>``.
+        xz
+            The coordinates, in master frame pixels, on which to centre
+            the target.
+
+        Returns
+        -------
+        pixel
+            A tuple with the x and z coordinates of the pixel in the master frame,
+            or `None` if resetting to the central fibre.
 
-        fibre = fibermap.loc[fibermap.fibername == fibre_name, :]
-        xpmm, ypmm = fibre.loc[:, ["xpmm", "ypmm"]].values[0]
+        """
 
-        xmf, zmf = offset_to_master_frame_pixel(xmm=xpmm, ymm=ypmm)
+        if fibre_name is not None:
+            xmf, zmf = fibre_to_master_frame(fibre_name)
+        elif xz is not None:
+            xmf, zmf = xz
+        else:
+            self._mf_pixel = None
+            return None
 
         self._mf_pixel = (xmf, zmf)
+
         return (xmf, zmf)
 
 
 class SkyCoordinates(QuerableCoordinates):
     """A sky position."""
 
     __db_table__ = "lvmopsdb.sky"
@@ -273,15 +288,16 @@
                 "spec": self.spec_coords,
             },
         )
 
     def __repr__(self):
         return (
             "<Tile "
-            f"(science ra={self.sci_coords.ra:.6f}, dec={self.sci_coords.dec:.6f}; "
+            f"(tile_id={self.tile_id}, "
+            f"science ra={self.sci_coords.ra:.6f}, dec={self.sci_coords.dec:.6f}; "
             f"n_skies={len(self.sky_coords)}; n_standards={len(self.spec_coords)})>"
         )
 
     @classmethod
     def from_coordinates(
         cls,
         ra: float,
@@ -394,14 +410,15 @@
 
         new_obj = cls(
             sci_coords,
             sky_coords=sky_coords,
             spec_coords=spec_coords,
             dither_position=dither_pos,
         )
+        new_obj.tile_id = tile_id
 
         return new_obj
 
     def set_sci_coords(
         self,
         sci_coords: ScienceCoordinates | CoordTuple,
     ) -> ScienceCoordinates:
```

### Comparing `lvmgort-0.1.0/src/gort/tools.py` & `lvmgort-0.1.1/src/gort/tools.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/src/gort/transforms.py` & `lvmgort-0.1.1/src/gort/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 __all__ = [
     "read_fibermap",
     "offset_to_master_frame_pixel",
     "xy_to_radec_offset",
     "fibre_slew_coordinates",
     "radec_sexagesimal_to_decimal",
+    "fibre_to_master_frame",
 ]
 
 
 _FIBERMAP_CACHE: pandas.DataFrame | None = None
 
 
 def read_fibermap(
@@ -208,15 +209,15 @@
 
     Parameters
     ----------
     ra,dec
         The RA and Dec of the target to which to slew.
     fibre_name
         The fibre to which to slew the target, with the format
-        ``<ifulabel>-<finufu>``.
+        ``<ifulabel>-<finifu>``.
 
     Returns
     -------
     slew_coordinates
         A tuple of RA/Dec coordinates to slew, which should place
         the target near the desired fibre.
 
@@ -260,7 +261,46 @@
 
     if dec_deg >= 0:
         dec_deg += float(dec_groups[1]) / 60 + float(dec_groups[2]) / 3600
     else:
         dec_deg -= float(dec_groups[1]) / 60 - float(dec_groups[2]) / 3600
 
     return ra_deg, dec_deg
+
+
+def fibre_to_master_frame(fibre_name: str):
+    """Returns the xz coordinates in the master frame of a named fibres.
+
+    Parameters
+    ----------
+    fibre_name
+        The fibre for which to calculate the master frame coordinates,
+        with the format ``<ifulabel>-<finifu>``.
+
+    Returns
+    -------
+    pixel
+        A tuple with the x and z coordinates of the pixel in the master frame.
+
+    Raises
+    ------
+    ValueError
+        If the pixel is out of bounds.
+
+    """
+
+    XZ_0 = (2500, 1000)  # Central pixel in the master frame
+
+    fibermap = read_fibermap()
+
+    if fibre_name not in fibermap.fibername.values:
+        raise NameError(f"Fibre {fibre_name} not found in fibermap.")
+
+    fibre = fibermap.loc[fibermap.fibername == fibre_name, :]
+    xpmm, ypmm = fibre.loc[:, ["xpmm", "ypmm"]].values[0]
+
+    x_mf, z_mf = offset_to_master_frame_pixel(xmm=xpmm, ymm=ypmm)
+
+    if x_mf < 0 or x_mf > 2 * XZ_0[0] or z_mf < 0 or z_mf > 2 * XZ_0[1]:
+        raise ValueError("Pixel is out of bounds.")
+
+    return (round(x_mf, 1), round(z_mf, 1))
```

### Comparing `lvmgort-0.1.0/src/gort/websocket.py` & `lvmgort-0.1.1/src/gort/websocket.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.0/PKG-INFO` & `lvmgort-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvmgort
-Version: 0.1.0
+Version: 0.1.1
 Summary: The brains of LVM observing
 Home-page: https://github.com/sdss/lvmgort
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
```

