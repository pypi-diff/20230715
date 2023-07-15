# Comparing `tmp/volumizer-0.1.0.tar.gz` & `tmp/volumizer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volumizer-0.1.0.tar", max compression
+gzip compressed data, was "volumizer-0.1.1.tar", max compression
```

## Comparing `volumizer-0.1.0.tar` & `volumizer-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1076 2023-07-08 16:14:15.259791 volumizer-0.1.0/LICENSE
--rw-r--r--   0        0        0     5618 2023-07-09 05:12:19.385372 volumizer-0.1.0/README.md
--rw-r--r--   0        0        0      538 2023-07-09 18:40:37.842217 volumizer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 16:14:15.272791 volumizer-0.1.0/volumizer/__init__.py
--rw-r--r--   0        0        0      658 2023-07-08 16:14:15.272791 volumizer-0.1.0/volumizer/align.py
--rw-r--r--   0        0        0      728 2023-07-09 04:25:27.436305 volumizer-0.1.0/volumizer/constants.py
--rw-r--r--   0        0        0     6239 2023-07-08 16:14:15.273791 volumizer-0.1.0/volumizer/fib_sphere.py
--rw-r--r--   0        0        0      203 2023-07-09 18:40:05.790711 volumizer-0.1.0/volumizer/paths.py
--rw-r--r--   0        0        0     7568 2023-07-09 04:24:59.931873 volumizer-0.1.0/volumizer/pdb.py
--rw-r--r--   0        0        0     8393 2023-07-08 16:14:15.273791 volumizer-0.1.0/volumizer/protein_components.py
--rw-r--r--   0        0        0     1196 2023-07-08 16:14:15.273791 volumizer-0.1.0/volumizer/types.py
--rw-r--r--   0        0        0     5863 2023-07-09 03:44:18.870688 volumizer-0.1.0/volumizer/utils.py
--rw-r--r--   0        0        0     4229 2023-07-08 16:45:08.646614 volumizer-0.1.0/volumizer/volumizer.py
--rw-r--r--   0        0        0    24074 2023-07-09 03:46:30.505744 volumizer-0.1.0/volumizer/voxel.py
--rw-r--r--   0        0        0     6437 1970-01-01 00:00:00.000000 volumizer-0.1.0/setup.py
--rw-r--r--   0        0        0     6159 1970-01-01 00:00:00.000000 volumizer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-08 16:14:15.259791 volumizer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7549 2023-07-15 16:57:40.640503 volumizer-0.1.1/README.md
+-rw-r--r--   0        0        0      538 2023-07-15 17:05:11.808723 volumizer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 16:14:15.272791 volumizer-0.1.1/volumizer/__init__.py
+-rw-r--r--   0        0        0      364 2023-07-13 02:14:29.115227 volumizer-0.1.1/volumizer/align.py
+-rw-r--r--   0        0        0      814 2023-07-13 00:38:04.356379 volumizer-0.1.1/volumizer/constants.py
+-rw-r--r--   0        0        0     6239 2023-07-08 16:14:15.273791 volumizer-0.1.1/volumizer/fib_sphere.py
+-rw-r--r--   0        0        0      203 2023-07-09 18:40:05.790711 volumizer-0.1.1/volumizer/paths.py
+-rw-r--r--   0        0        0     7624 2023-07-15 16:44:53.148182 volumizer-0.1.1/volumizer/pdb.py
+-rw-r--r--   0        0        0     8393 2023-07-08 16:14:15.273791 volumizer-0.1.1/volumizer/protein_components.py
+-rw-r--r--   0        0        0     1196 2023-07-14 01:49:45.715179 volumizer-0.1.1/volumizer/types.py
+-rw-r--r--   0        0        0     6005 2023-07-15 16:33:07.883752 volumizer-0.1.1/volumizer/utils.py
+-rw-r--r--   0        0        0     5620 2023-07-15 16:03:48.548894 volumizer-0.1.1/volumizer/volumizer.py
+-rw-r--r--   0        0        0    25086 2023-07-14 02:13:44.025309 volumizer-0.1.1/volumizer/voxel.py
+-rw-r--r--   0        0        0     8377 1970-01-01 00:00:00.000000 volumizer-0.1.1/setup.py
+-rw-r--r--   0        0        0     8090 1970-01-01 00:00:00.000000 volumizer-0.1.1/PKG-INFO
```

### Comparing `volumizer-0.1.0/LICENSE` & `volumizer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.0/pyproject.toml` & `volumizer-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volumizer"
-version = "0.1.0"
+version = "0.1.1"
 description = "Search the RCSB for occluded volumes like cavities, pockets, and pores."
 authors = ["Aron Broom <broomsday@gmail.com>"]
 readme = "README.md"
 packages = [{include = "volumizer"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `volumizer-0.1.0/volumizer/constants.py` & `volumizer-0.1.1/volumizer/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,7 +32,8 @@
 }
 VOXEL_SIZE = 3.0
 OCCLUDED_DIMENSION_LIMIT = 4
 MIN_NUM_VOXELS = 4
 
 VOXEL_TYPE_CHAIN_MAP = {"HUB": "A", "POR": "B", "POK": "C", "CAV": "D", "OCC": "E"}
 VOXEL_TYPE_ATOM_MAP = {"HUB": "F", "POR": "O", "POK": "N", "CAV": "S", "OCC": "H"}
+VOXEL_TYPE_ELEMENT_MAP = {"HUB": "F", "POR": "O", "POK": "N", "CAV": "S", "OCC": "H"}
```

### Comparing `volumizer-0.1.0/volumizer/fib_sphere.py` & `volumizer-0.1.1/volumizer/fib_sphere.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.0/volumizer/protein_components.py` & `volumizer-0.1.1/volumizer/protein_components.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.0/volumizer/types.py` & `volumizer-0.1.1/volumizer/types.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.0/volumizer/utils.py` & `volumizer-0.1.1/volumizer/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 
 from volumizer import constants, protein_components
 from volumizer.types import Annotation, VoxelGroup
 from volumizer.paths import C_CODE_DIR
 
 
 VOXEL_SIZE = constants.VOXEL_SIZE
-VOXEL_VOLUME = VOXEL_SIZE ** 3
-KEEP_MODELS = True  # by default keep all models in case they are other biological assembly units
+VOXEL_VOLUME = VOXEL_SIZE**3
+KEEP_MODELS = (
+    True  # by default keep all models in case they are other biological assembly units
+)
 KEEP_NON_PROTEIN = False  # by default only keep protein residues
 KEEP_HYDROGENS = False  # by default remove hydrogens
 UTILS_PROTEIN_COMPONENTS = protein_components.PROTEIN_COMPONENTS
 
 
 def get_protein_components() -> set[str]:
     """
@@ -32,93 +34,112 @@
     """
     Reset the protein components definition to the default.
     """
     global UTILS_PROTEIN_COMPONENTS
 
     UTILS_PROTEIN_COMPONENTS = protein_components.PROTEIN_COMPONENTS
 
+
 def add_protein_components(additional_components: set[str]) -> None:
     """
     Extend the protein components definition currently in use with additional components
     """
     global UTILS_PROTEIN_COMPONENTS
-    
-    UTILS_PROTEIN_COMPONENTS = UTILS_PROTEIN_COMPONENTS.union(additional_components)
+
+    UTILS_PROTEIN_COMPONENTS = UTILS_PROTEIN_COMPONENTS.union(
+        set(additional_components)
+    )
 
 
 def remove_protein_components(disallowed_components: set[str]) -> None:
     """
     Reduce the protein components definition currently in use with blacklisted components.
     """
     global UTILS_PROTEIN_COMPONENTS
-    
-    UTILS_PROTEIN_COMPONENTS = UTILS_PROTEIN_COMPONENTS - disallowed_components
+
+    UTILS_PROTEIN_COMPONENTS = UTILS_PROTEIN_COMPONENTS - set(disallowed_components)
 
 
 def set_resolution(resolution: float) -> None:
     """
     Set the value of the VOXEL_SIZE and VOXEL_VOLUME global constants.
     """
     global VOXEL_SIZE
     global VOXEL_VOLUME
 
     VOXEL_SIZE = resolution
-    VOXEL_VOLUME = VOXEL_SIZE ** 3
+    VOXEL_VOLUME = VOXEL_SIZE**3
 
 
 def set_non_protein(non_protein: bool) -> None:
     """
     Set whether to include non-protein residues during the calculations.
     """
     global KEEP_NON_PROTEIN
     KEEP_NON_PROTEIN = non_protein
 
 
-def get_volume_summary(voxel_group_dict: dict[int, VoxelGroup], summary_type: str = "total") -> float:
+def get_volume_summary(
+    voxel_group_dict: dict[int, VoxelGroup], summary_type: str = "total"
+) -> float:
     """
     Compute a summary value for the volume
     """
-    volumes = [voxel_group.volume for voxel_group in voxel_group_dict.values() if voxel_group.volume is not None]
+    volumes = [
+        voxel_group.volume
+        for voxel_group in voxel_group_dict.values()
+        if voxel_group.volume is not None
+    ]
     if volumes:
         if summary_type == "total":
             return sum(volumes)
         elif summary_type == "max":
             return max(volumes)
         elif summary_type == "mean":
             return np.mean(volumes)
         else:
             print("Unsupported volume summary type")
 
     return 0.0
 
 
-def sort_voxelgroups_by_volume(voxelgroups: dict[int, VoxelGroup]) -> dict[int, VoxelGroup]:
+def sort_voxelgroups_by_volume(
+    voxelgroups: dict[int, VoxelGroup]
+) -> dict[int, VoxelGroup]:
     """
     Take a dictionary with indices as the keys and VoxelGroups as the values.
     Reassign the keys such that the VoxelGroups are sorted by volume.
     """
     return {
         i: voxelgroup
-        for i, voxelgroup in enumerate(sorted(voxelgroups.values(), key=lambda group: group.volume, reverse=True))
+        for i, voxelgroup in enumerate(
+            sorted(voxelgroups.values(), key=lambda group: group.volume, reverse=True)
+        )
     }
 
 
 def filter_voxelgroups_by_volume(
-    voxelgroups: dict[int, VoxelGroup], min_volume: Optional[float] = None, min_voxels: Optional[int] = None
+    voxelgroups: dict[int, VoxelGroup],
+    min_volume: Optional[float] = None,
+    min_voxels: Optional[int] = None,
 ) -> dict[int, VoxelGroup]:
     """
     Remove voxel groups based on min volumem and min number of voxels cutoff
     """
     if min_volume is not None:
         voxelgroups = {
-            i: voxelgroup for i, voxelgroup in enumerate(voxelgroups.values()) if voxelgroup.volume >= min_volume
+            i: voxelgroup
+            for i, voxelgroup in enumerate(voxelgroups.values())
+            if voxelgroup.volume >= min_volume
         }
     if min_voxels is not None:
         voxelgroups = {
-            i: voxelgroup for i, voxelgroup in enumerate(voxelgroups.values()) if voxelgroup.num_voxels >= min_voxels
+            i: voxelgroup
+            for i, voxelgroup in enumerate(voxelgroups.values())
+            if voxelgroup.num_voxels >= min_voxels
         }
 
     return voxelgroups
 
 
 def make_annotation_dataframe(annotation: Annotation) -> pd.DataFrame:
     """
```

### Comparing `volumizer-0.1.0/volumizer/volumizer.py` & `volumizer-0.1.1/volumizer/volumizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,84 @@
 """
 Entry-level functions to find pores and cavities.
 """
 
 
+from pathlib import Path
 from typing import Optional
 
 import biotite.structure as bts
+import pandas as pd
 
 from volumizer import utils, pdb, voxel, fib_sphere, align
 from volumizer.types import Annotation
 
 
-def annotate_pdb_structure(
-    structure: bts.AtomArray, min_voxels: Optional[int] = 2, min_volume: Optional[float] = None
+def annotate_structure_volumes(
+    structure: bts.AtomArray,
+    min_voxels: Optional[int] = 2,
+    min_volume: Optional[float] = None,
 ) -> tuple[Annotation, list[str]]:
     """
     Perform analysis of a prepared structure.
     """
     coords = pdb.get_structure_coords(structure)
     coords = fib_sphere.add_extra_points(coords, utils.VOXEL_SIZE)
 
     cloud = voxel.coords_to_point_cloud(coords)
     cloud, voxel_grid_id = voxel.add_voxel_grid(cloud)
     voxel_grid = voxel.get_voxel_grid(cloud, voxel_grid_id)
 
     protein_solvent_voxels = voxel.get_protein_solvent_voxel_array(voxel_grid)
-    protein_voxels, solvent_voxels = voxel.get_protein_and_solvent_voxels(protein_solvent_voxels, voxel_grid.x_y_z)
+    protein_voxels, solvent_voxels = voxel.get_protein_and_solvent_voxels(
+        protein_solvent_voxels, voxel_grid.x_y_z
+    )
 
     exposed_voxels, buried_voxels = voxel.get_exposed_and_buried_voxels(
         solvent_voxels, protein_voxels, voxel_grid.x_y_z
     )
 
     # get sub-selection of exposed voxels that are NEXT to a buried voxel
-    first_shell_exposed_voxels = voxel.get_first_shell_exposed_voxels(exposed_voxels, buried_voxels, voxel_grid)
+    first_shell_exposed_voxels = voxel.get_first_shell_exposed_voxels(
+        exposed_voxels, buried_voxels, voxel_grid
+    )
 
-    hubs, pores, pockets, cavities, occluded = voxel.get_pores_pockets_cavities_occluded(
+    (
+        hubs,
+        pores,
+        pockets,
+        cavities,
+        occluded,
+    ) = voxel.get_pores_pockets_cavities_occluded(
         buried_voxels, first_shell_exposed_voxels, voxel_grid
     )
     hubs = utils.sort_voxelgroups_by_volume(
-        utils.filter_voxelgroups_by_volume(hubs, min_voxels=min_voxels, min_volume=min_volume)
+        utils.filter_voxelgroups_by_volume(
+            hubs, min_voxels=min_voxels, min_volume=min_volume
+        )
     )
     pores = utils.sort_voxelgroups_by_volume(
-        utils.filter_voxelgroups_by_volume(pores, min_voxels=min_voxels, min_volume=min_volume)
+        utils.filter_voxelgroups_by_volume(
+            pores, min_voxels=min_voxels, min_volume=min_volume
+        )
     )
     pockets = utils.sort_voxelgroups_by_volume(
-        utils.filter_voxelgroups_by_volume(pockets, min_voxels=min_voxels, min_volume=min_volume)
+        utils.filter_voxelgroups_by_volume(
+            pockets, min_voxels=min_voxels, min_volume=min_volume
+        )
     )
     cavities = utils.sort_voxelgroups_by_volume(
-        utils.filter_voxelgroups_by_volume(cavities, min_voxels=min_voxels, min_volume=min_volume)
+        utils.filter_voxelgroups_by_volume(
+            cavities, min_voxels=min_voxels, min_volume=min_volume
+        )
     )
     occluded = utils.sort_voxelgroups_by_volume(
-        utils.filter_voxelgroups_by_volume(occluded, min_voxels=min_voxels, min_volume=min_volume)
+        utils.filter_voxelgroups_by_volume(
+            occluded, min_voxels=min_voxels, min_volume=min_volume
+        )
     )
 
     annotation = Annotation(
         total_hub_volume=utils.get_volume_summary(hubs, "total"),
         total_pore_volume=utils.get_volume_summary(pores, "total"),
         total_cavity_volume=utils.get_volume_summary(cavities, "total"),
         total_pocket_volume=utils.get_volume_summary(pockets, "total"),
@@ -71,30 +95,68 @@
         cavity_volumes={i: cavity.volume for i, cavity in cavities.items()},
         pocket_volumes={i: pocket.volume for i, pocket in pockets.items()},
         hub_dimensions={i: hub.axial_lengths for i, hub in hubs.items()},
         pore_dimensions={i: pore.axial_lengths for i, pore in pores.items()},
         cavity_dimensions={i: cavity.axial_lengths for i, cavity in cavities.items()},
         pocket_dimensions={i: pocket.axial_lengths for i, pocket in pockets.items()},
     )
+    annotation_df = utils.make_annotation_dataframe(annotation)
 
-    pdb_lines = pdb.points_to_pdb(voxel_grid, hubs, pores, pockets, cavities, occluded)
-    pdb_lines.extend(pdb.generate_resolution_remarks())
-    pdb_lines.extend(pdb.generate_volume_remarks(annotation))
+    annotation_structure = pdb.volumes_to_structure(
+        voxel_grid, hubs, pores, pockets, cavities, occluded
+    )
 
-    return (annotation, pdb_lines)
+    return (annotation_df, annotation_structure)
 
 
-def prepare_pdb_structure(structure: bts.AtomArray) -> tuple[bts.AtomArray, str]:
+def prepare_pdb_structure(structure: bts.AtomArray) -> bts.AtomArray:
     """
     Prepares a biotite AtomArray object for analysis by:
 
     1. Cleaning extraneous atoms
     2. Aligning along the principal axis
 
     Returns a biotite AtomArray
     """
-    structure = pdb.clean_structure(structure)
+    cleaned_structure = pdb.clean_structure(structure)
+    cleaned_aligned_structure = align.align_structure(cleaned_structure)
+
+    return cleaned_aligned_structure
+
+
+def volumize_structure(
+    structure: bts.AtomArray,
+) -> tuple[pd.DataFrame, bts.AtomArray, bts.AtomArray]:
+    """
+    Perform the volumizer pipeline on a biotite structure and return the:
+    annotation_df, pdb_structure, and annotated_structure
+    """
+    prepared_structure = prepare_pdb_structure(structure)
+
+    annotation_df, annotation_structure = annotate_structure_volumes(prepared_structure)
+
+    return annotation_df, prepared_structure, annotation_structure
 
-    structure, rotation, translation = align.align_structure(structure)
-    remarks = pdb.generate_rotation_translation_remarks(rotation, translation)
 
-    return (structure, remarks)
+def volumize_pdb(pdb_file: Path) -> tuple[pd.DataFrame, bts.AtomArray, bts.AtomArray]:
+    """
+    Convenience function to volumize a PDB file.
+    """
+    pdb_structure = pdb.load_structure(pdb_file)
+    return volumize_structure(pdb_structure)
+
+
+def volumize_pdb_and_save(
+    in_pdb_file: Path, out_pdb_file: Path, out_annotation_df: Path
+) -> None:
+    """
+    Convenience function to perform volumization and save the output.
+    """
+    annotation_df, prepared_pdb_structure, annotation_structure = volumize_pdb(
+        in_pdb_file
+    )
+    out_pdb_lines = pdb.make_volumized_pdb_lines(
+        [prepared_pdb_structure, annotation_structure]
+    )
+
+    annotation_df.to_json(out_annotation_df)
+    pdb.save_pdb_lines(out_pdb_lines, out_pdb_file)
```

### Comparing `volumizer-0.1.0/volumizer/voxel.py` & `volumizer-0.1.1/volumizer/voxel.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,37 +90,46 @@
             volume=compute_voxel_group_volume(len(solvent_voxel_indices)),
         ),
     )
 
 
 def get_occluded_dimensions(
     query_voxel: tuple[int, int, int],
-    possible_occluding_x: list[int],
-    possible_occluding_y: list[int],
-    possible_occluding_z: list[int],
+    occluding_x: list[int],
+    occluding_y: list[int],
+    occluding_z: list[int],
 ) -> list[int]:
     """
     Determine how many ordinal axes are occluded.
+
+    We simply compare our query voxel with the coordinates of the `occluding` voxels,
+    which are e.g. protein voxels.
+
+    For performance reasons rather than looking across ALL occluding voxels, we look at planar arrays
+    of coordinates.
     """
     occluded_dimensions = [0, 0, 0, 0, 0, 0]
 
-    if len(possible_occluding_z) != 0:
-        if min(possible_occluding_z) < query_voxel[2]:
+    # here we assume that e.g. occluding_z[0] is the min value and occluding_z[-1] is the max
+    #   if this becomes untrue we would need to explicitly take the min/max
+    #   this is less performant for large structures
+    if len(occluding_z) != 0:
+        if occluding_z[0] < query_voxel[2]:
             occluded_dimensions[4] = 1
-        if max(possible_occluding_z) > query_voxel[2]:
+        if occluding_z[-1] > query_voxel[2]:
             occluded_dimensions[5] = 1
-    if len(possible_occluding_y) != 0:
-        if min(possible_occluding_y) < query_voxel[1]:
+    if len(occluding_y) != 0:
+        if occluding_y[0] < query_voxel[1]:
             occluded_dimensions[2] = 1
-        if max(possible_occluding_y) > query_voxel[1]:
+        if occluding_y[-1] > query_voxel[1]:
             occluded_dimensions[3] = 1
-    if len(possible_occluding_x) != 0:
-        if min(possible_occluding_x) < query_voxel[0]:
+    if len(occluding_x) != 0:
+        if occluding_x[0] < query_voxel[0]:
             occluded_dimensions[0] = 1
-        if max(possible_occluding_x) > query_voxel[0]:
+        if occluding_x[-1] > query_voxel[0]:
             occluded_dimensions[1] = 1
 
     return occluded_dimensions
 
 
 def is_buried(occluded_dimensions: list[int]) -> bool:
     """
@@ -141,22 +150,30 @@
             return True
 
     return False
 
 
 def build_planar_voxel_coordinate_arrays(
     voxels: tuple[np.ndarray, ...], voxel_grid_dimensions: np.ndarray
-) -> tuple[list[list[list[int]]], list[list[list[int]]], list[list[list[int]]]]:
+) -> tuple[list[list[list[int]]], list[list[list[int]]], list[list[list[int]]],]:
     """
-    For each two-dimension pair, construct a list of coordinates in the 3rd dimension that match the first two dimensions.
+    For each two-dimension pair, construct a tuple of the min/max coordinates in the 3rd dimension.
     """
-    # TODO collapse down the final lists to min() and max() only as two different entries and use that for comparison in the downstream function
-    z_array = [[list() for y in range(voxel_grid_dimensions[1])] for x in range(voxel_grid_dimensions[0])]
-    y_array = [[list() for z in range(voxel_grid_dimensions[2])] for x in range(voxel_grid_dimensions[0])]
-    x_array = [[list() for z in range(voxel_grid_dimensions[2])] for y in range(voxel_grid_dimensions[1])]
+    z_array = [
+        [[] for y in range(voxel_grid_dimensions[1])]
+        for x in range(voxel_grid_dimensions[0])
+    ]
+    y_array = [
+        [[] for z in range(voxel_grid_dimensions[2])]
+        for x in range(voxel_grid_dimensions[0])
+    ]
+    x_array = [
+        [[] for z in range(voxel_grid_dimensions[2])]
+        for y in range(voxel_grid_dimensions[1])
+    ]
 
     for i in range(voxels[0].size):
         z_array[voxels[0][i]][voxels[1][i]].append(voxels[2][i])
         y_array[voxels[0][i]][voxels[2][i]].append(voxels[1][i])
         x_array[voxels[1][i]][voxels[2][i]].append(voxels[0][i])
 
     return z_array, y_array, x_array
@@ -169,18 +186,24 @@
 ) -> tuple[VoxelGroup, VoxelGroup]:
     """
     Use simple geometric heuristics to determine if a group of solvent voxels is buried or exposed.
     """
     buried_voxels = ([], [], [])
     exposed_voxels = ([], [], [])
 
-    z_array, y_array, x_array = build_planar_voxel_coordinate_arrays(protein_voxels.voxels, voxel_grid_dimensions)
+    z_array, y_array, x_array = build_planar_voxel_coordinate_arrays(
+        protein_voxels.voxels, voxel_grid_dimensions
+    )
 
     for i in range(solvent_voxels.voxels[0].size):
-        query_voxel = (solvent_voxels.voxels[0][i], solvent_voxels.voxels[1][i], solvent_voxels.voxels[2][i])
+        query_voxel = (
+            solvent_voxels.voxels[0][i],
+            solvent_voxels.voxels[1][i],
+            solvent_voxels.voxels[2][i],
+        )
 
         occluded_dimensions = get_occluded_dimensions(
             query_voxel,
             x_array[query_voxel[1]][query_voxel[2]],
             y_array[query_voxel[0]][query_voxel[2]],
             z_array[query_voxel[0]][query_voxel[1]],
         )
@@ -195,32 +218,41 @@
             exposed_voxels[2].append(query_voxel[2])
 
     buried_voxel_indices = compute_voxel_indices(buried_voxels, voxel_grid_dimensions)
     exposed_voxel_indices = compute_voxel_indices(exposed_voxels, voxel_grid_dimensions)
 
     return (
         VoxelGroup(
-            voxels=(np.array(exposed_voxels[0]), np.array(exposed_voxels[1]), np.array(exposed_voxels[2])),
+            voxels=(
+                np.array(exposed_voxels[0]),
+                np.array(exposed_voxels[1]),
+                np.array(exposed_voxels[2]),
+            ),
             indices=exposed_voxel_indices,
             num_voxels=len(exposed_voxel_indices),
             voxel_type="exposed",
             volume=compute_voxel_group_volume(len(exposed_voxel_indices)),
         ),
         VoxelGroup(
-            voxels=(np.array(buried_voxels[0]), np.array(buried_voxels[1]), np.array(buried_voxels[2])),
+            voxels=(
+                np.array(buried_voxels[0]),
+                np.array(buried_voxels[1]),
+                np.array(buried_voxels[2]),
+            ),
             indices=buried_voxel_indices,
             num_voxels=len(buried_voxel_indices),
             voxel_type="buried",
             volume=compute_voxel_group_volume(len(buried_voxel_indices)),
         ),
     )
 
 
 def get_neighbor_voxels_python(
-    query_voxels: tuple[np.ndarray, np.ndarray, np.ndarray], reference_voxels: tuple[np.ndarray, np.ndarray, np.ndarray]
+    query_voxels: tuple[np.ndarray, np.ndarray, np.ndarray],
+    reference_voxels: tuple[np.ndarray, np.ndarray, np.ndarray],
 ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Return the voxels from a query group that neighbor a reference group.
     """
     neighbor_indices = []
     for query_index in range(len(query_voxels[0])):
         query_voxel = get_single_voxel(query_voxels, query_index)
@@ -234,15 +266,16 @@
         np.array([query_voxels[0][i] for i in neighbor_indices]),
         np.array([query_voxels[1][i] for i in neighbor_indices]),
         np.array([query_voxels[2][i] for i in neighbor_indices]),
     )
 
 
 def get_neighbor_voxels_c(
-    query_voxels: tuple[np.ndarray, np.ndarray, np.ndarray], reference_voxels: tuple[np.ndarray, np.ndarray, np.ndarray]
+    query_voxels: tuple[np.ndarray, np.ndarray, np.ndarray],
+    reference_voxels: tuple[np.ndarray, np.ndarray, np.ndarray],
 ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Return the voxels from a query group that neighbor a reference group.
     """
     # make the voxels compatible with C
     num_query = len(query_voxels[0])
     query_x = (ctypes.c_int * num_query)(*query_voxels[0])
@@ -283,30 +316,40 @@
     voxel_grid: VoxelGrid,
     performant: bool = utils.using_performant(),
 ) -> VoxelGroup:
     """
     Subset exposed voxels into only those neighboring one or more buried voxels.
     """
     if performant:
-        first_shell_voxels = get_neighbor_voxels_c(exposed_voxels.voxels, buried_voxels.voxels)
+        first_shell_voxels = get_neighbor_voxels_c(
+            exposed_voxels.voxels, buried_voxels.voxels
+        )
     else:
-        first_shell_voxels = get_neighbor_voxels_python(exposed_voxels.voxels, buried_voxels.voxels)
+        first_shell_voxels = get_neighbor_voxels_python(
+            exposed_voxels.voxels, buried_voxels.voxels
+        )
 
     first_shell_indices = compute_voxel_indices(first_shell_voxels, voxel_grid.x_y_z)
 
     return VoxelGroup(
-        voxels=(np.array(first_shell_voxels[0]), np.array(first_shell_voxels[1]), np.array(first_shell_voxels[2])),
+        voxels=(
+            np.array(first_shell_voxels[0]),
+            np.array(first_shell_voxels[1]),
+            np.array(first_shell_voxels[2]),
+        ),
         indices=first_shell_indices,
         num_voxels=len(first_shell_indices),
         voxel_type="exposed",
         volume=compute_voxel_group_volume(len(first_shell_indices)),
     )
 
 
-def is_neighbor_voxel(voxel_one: tuple[np.int64, ...], voxel_two: tuple[np.int64, ...]) -> bool:
+def is_neighbor_voxel(
+    voxel_one: tuple[np.int64, ...], voxel_two: tuple[np.int64, ...]
+) -> bool:
     """
     Given two voxels return True if they are ordinal neighbors.
     """
     # below approach is ~2x faster than using a list comprehension, presumably because of early exit
     sum_differences = 0
     for dimension in range(3):
         difference = abs(voxel_one[dimension] - voxel_two[dimension])
@@ -319,44 +362,55 @@
     # a voxel is an ordinal neighbor when the sum of the absolute differences in axes indices is 1
     if sum_differences == 1:
         return True
 
     return False
 
 
-def get_single_voxel(voxels: tuple[np.ndarray, ...], index: int) -> tuple[np.int64, ...]:
+def get_single_voxel(
+    voxels: tuple[np.ndarray, ...], index: int
+) -> tuple[np.int64, ...]:
     """
     Given a set of voxels return just one voxel at index.
     """
     return (
         voxels[0][index],
         voxels[1][index],
         voxels[2][index],
     )
 
 
-def compute_voxel_indices(voxels: tuple[np.ndarray, ...], grid_dimensions: np.ndarray) -> set[int]:
+def compute_voxel_indices(
+    voxels: tuple[np.ndarray, ...], grid_dimensions: np.ndarray
+) -> set[int]:
     """
     Given a 3D array of voxels, compute the 1D set of their indices.
     """
-    # TODO: is this built-in easier and correct?: x, y, z = np.unravel_index(voxel, self.x_y_z)
+    grid_dimension_1_2 = grid_dimensions[1] * grid_dimensions[2]
+
     return {
-        (voxels[0][i] * grid_dimensions[1] * grid_dimensions[2] + voxels[1][i] * grid_dimensions[2] + voxels[2][i])
+        (
+            voxels[0][i] * grid_dimension_1_2
+            + voxels[1][i] * grid_dimensions[2]
+            + voxels[2][i]
+        )
         for i in range(len(voxels[0]))
     }
 
 
 def compute_voxel_group_volume(num_voxels: int) -> float:
     """
     Return the volume of a number of voxels
     """
     return num_voxels * utils.VOXEL_VOLUME
 
 
-def breadth_first_search_python(voxels: tuple[np.ndarray, ...], searchable_indices: set[int]) -> set[int]:
+def breadth_first_search_python(
+    voxels: tuple[np.ndarray, ...], searchable_indices: set[int]
+) -> set[int]:
     """
     Given a set of voxels and list of possible indices to add,
     add indices for all ordinal neighbors iteratively until no more such neighbors exist.
     """
     searchable_indices = deepcopy(searchable_indices)
     start_index = searchable_indices.pop()
     queue_indices = set([start_index])
@@ -371,29 +425,33 @@
                 queue_indices.add(searched_index)
                 neighbor_indices.add(searched_index)
         searchable_indices -= neighbor_indices
 
     return neighbor_indices
 
 
-def breadth_first_search_c(voxels: tuple[np.ndarray, ...], searchable_indices: set[int]) -> set[int]:
+def breadth_first_search_c(
+    voxels: tuple[np.ndarray, ...], searchable_indices: set[int]
+) -> set[int]:
     """
     Given a set of voxels and list of possible indices to add,
     add indices for all ordinal neighbors iteratively until no more such neighbors exist.
     """
     c_searchable_indices = list(deepcopy(searchable_indices))
 
     # make the voxels compatible with C
     num_voxels = len(voxels[0])
     voxels_x = (ctypes.c_int * num_voxels)(*voxels[0])
     voxels_y = (ctypes.c_int * num_voxels)(*voxels[1])
     voxels_z = (ctypes.c_int * num_voxels)(*voxels[2])
 
     # generate other inputs needed for C function
-    c_searchable_indices = (ctypes.c_int * len(c_searchable_indices))(*c_searchable_indices)
+    c_searchable_indices = (ctypes.c_int * len(c_searchable_indices))(
+        *c_searchable_indices
+    )
     initial_indices = (ctypes.c_int * num_voxels)(*([-1] * num_voxels))
 
     # run the breadth-first search
     VOXEL_C.breadth_first_search.restype = ctypes.POINTER(ctypes.c_int * num_voxels)
     neighbor_indices_c = VOXEL_C.breadth_first_search(
         ctypes.byref(voxels_x),
         ctypes.byref(voxels_y),
@@ -403,15 +461,17 @@
         ctypes.byref(initial_indices),
     )
 
     return set([i for i in neighbor_indices_c.contents if i != -1])
 
 
 def breadth_first_search(
-    voxels: tuple[np.ndarray, ...], searchable_indices: set[int], performant: bool = utils.using_performant()
+    voxels: tuple[np.ndarray, ...],
+    searchable_indices: set[int],
+    performant: bool = utils.using_performant(),
 ) -> set[int]:
     """
     Given a set of voxels and list of possible indices to add,
     add indices for all ordinal neighbors iteratively until no more such neighbors exist.
     """
     if performant:
         return breadth_first_search_c(voxels, searchable_indices)
@@ -430,16 +490,20 @@
     elif voxel[1] == voxel_grid_dimensions[1] - 1:
         return True
     elif voxel[2] == voxel_grid_dimensions[2] - 1:
         return True
 
     return False
 
+
 def get_agglomerated_type(
-    query_indices: set[int], buried_voxels: tuple[np.ndarray, ...], exposed_voxels: tuple[np.ndarray, ...], voxel_grid_dimensions: np.ndarray,
+    query_indices: set[int],
+    buried_voxels: tuple[np.ndarray, ...],
+    exposed_voxels: tuple[np.ndarray, ...],
+    voxel_grid_dimensions: np.ndarray,
 ) -> tuple[set[int], str]:
     """
     Find "surface" voxels, being buried voxel in direct contact with an exposed voxel. Four possibilites:
 
     a) there are no "surface" voxels -> this is a cavity
     b) all "surface" voxels can be agglomerated (BFS) into a single group -> this is a pocket
     c) the "surface" voxels can be agglomerated (BFS) into exactly two groups -> this is a pore
@@ -478,98 +542,136 @@
     # NOTE: we have to union the direct and neighbor surfaces, otherwise small discritization
     #   on the surface would look like a distinct surface
     surface_indices = direct_surface_indices.union(neighbor_surface_indices)
     single_surface_indices = breadth_first_search(buried_voxels, surface_indices)
     if len(single_surface_indices) < len(surface_indices):
         # run the agglomeration one more time on what's left
         remaining_surface_indices = surface_indices - single_surface_indices
-        single_surface_indices = breadth_first_search(buried_voxels, remaining_surface_indices)
+        single_surface_indices = breadth_first_search(
+            buried_voxels, remaining_surface_indices
+        )
 
         # if there are stil indices left, there were more than 2 surfaces, hence a hub
         if len(single_surface_indices) < len(remaining_surface_indices):
             return direct_surface_indices.union(neighbor_surface_indices), "hub"
 
         # othewise, exactly 2 and a pore
         return direct_surface_indices.union(neighbor_surface_indices), "pore"
 
     # if the first BFS went to completion and consumed all surfaces, there was only a single surface, hence pocket
     return direct_surface_indices.union(neighbor_surface_indices), "pocket"
 
 
-def get_voxel_group_center(voxel_indices: set[int], voxel_grid: VoxelGrid) -> np.ndarray:
+def get_voxel_group_center(
+    voxel_indices: set[int], voxel_grid: VoxelGrid
+) -> np.ndarray:
     """
     Compute the center of geometry for the voxel group.
     """
-    voxel_coords = np.array([voxel_grid.voxel_centers[voxel_index] for voxel_index in voxel_indices])
+    voxel_coords = np.array(
+        [voxel_grid.voxel_centers[voxel_index] for voxel_index in voxel_indices]
+    )
     return np.mean(voxel_coords, axis=0)
 
 
-def get_voxel_group_axial_lengths(voxel_indices: set[int], voxel_grid: VoxelGrid) -> list[float]:
+def get_voxel_group_axial_lengths(
+    voxel_indices: set[int], voxel_grid: VoxelGrid
+) -> list[float]:
     """
     Align the voxel group to it's principal axes, then compute the maximum length along each axis.
     """
-    voxel_coords = np.array([voxel_grid.voxel_centers[voxel_index] for voxel_index in voxel_indices])
+    voxel_coords = np.array(
+        [voxel_grid.voxel_centers[voxel_index] for voxel_index in voxel_indices]
+    )
     if len(voxel_coords) < 3:
         return [0, 0, 0]
 
-    #rotation, translation = align.get_principal_axis_alignment_translation_rotation(voxel_coords)
-    voxel_coords, _, _ = align.align_structure(voxel_coords)
+    # rotation, translation = align.get_principal_axis_alignment_translation_rotation(voxel_coords)
+    voxel_coords = align.align_structure(voxel_coords)
 
     # compute the maximum length across each axis
     xs = [voxel_coord[0] for voxel_coord in voxel_coords]
     ys = [voxel_coord[1] for voxel_coord in voxel_coords]
     zs = [voxel_coord[2] for voxel_coord in voxel_coords]
 
-    return sorted([max(xs) - min(xs), max(ys) - min(ys), max(zs) - min(zs)], reverse=True)
+    return sorted(
+        [
+            round(max(xs) - min(xs), 3),
+            round(max(ys) - min(ys), 3),
+            round(max(zs) - min(zs), 3),
+        ],
+        reverse=True,
+    )
 
 
 def get_pores_pockets_cavities_occluded(
     buried_voxels: VoxelGroup, exposed_voxels: VoxelGroup, voxel_grid: VoxelGrid
 ) -> tuple[
-    dict[int, VoxelGroup], dict[int, VoxelGroup], dict[int, VoxelGroup], dict[int, VoxelGroup], dict[int, VoxelGroup]
+    dict[int, VoxelGroup],
+    dict[int, VoxelGroup],
+    dict[int, VoxelGroup],
+    dict[int, VoxelGroup],
+    dict[int, VoxelGroup],
 ]:
     """
     Agglomerate buried solvent voxels into hubs, pores, pockets, cavities, and simply occluded.
     """
     buried_indices = set(range(buried_voxels.voxels[0].size))
     agglomerated_indices = set()
 
     hubs, pores, pockets, cavities, occluded = {}, {}, {}, {}, {}
     hub_id, pore_id, pocket_id, cavity_id, occluded_id = 0, 0, 0, 0, 0
 
     while len(agglomerated_indices) < len(buried_indices):
         remaining_indices = buried_indices - agglomerated_indices
 
         # perform BFS over the remaining indices
-        agglomerable_indices = breadth_first_search(buried_voxels.voxels, remaining_indices)
+        agglomerable_indices = breadth_first_search(
+            buried_voxels.voxels, remaining_indices
+        )
         # iterate our counter of finished indices
         agglomerated_indices = agglomerated_indices.union(agglomerable_indices)
 
         # if too small, don't assign direct surface indices and assign type "occluded"
         if len(agglomerable_indices) <= MIN_NUM_VOXELS:
             direct_surface_indices = set()
             agglomerated_type = "occluded"
         else:
             # identify what these agglomerated voxels are
             direct_surface_indices, agglomerated_type = get_agglomerated_type(
-                agglomerable_indices, buried_voxels.voxels, exposed_voxels.voxels, voxel_grid.x_y_z
+                agglomerable_indices,
+                buried_voxels.voxels,
+                exposed_voxels.voxels,
+                voxel_grid.x_y_z,
             )
 
         # get the surface voxels for use in getting their voxel-grid indices
         surface_voxels = (
-            np.array([buried_voxels.voxels[0][index] for index in direct_surface_indices]),
-            np.array([buried_voxels.voxels[1][index] for index in direct_surface_indices]),
-            np.array([buried_voxels.voxels[2][index] for index in direct_surface_indices]),
+            np.array(
+                [buried_voxels.voxels[0][index] for index in direct_surface_indices]
+            ),
+            np.array(
+                [buried_voxels.voxels[1][index] for index in direct_surface_indices]
+            ),
+            np.array(
+                [buried_voxels.voxels[2][index] for index in direct_surface_indices]
+            ),
         )
 
         # get the voxels
         volume_voxels = (
-            np.array([buried_voxels.voxels[0][index] for index in agglomerable_indices]),
-            np.array([buried_voxels.voxels[1][index] for index in agglomerable_indices]),
-            np.array([buried_voxels.voxels[2][index] for index in agglomerable_indices]),
+            np.array(
+                [buried_voxels.voxels[0][index] for index in agglomerable_indices]
+            ),
+            np.array(
+                [buried_voxels.voxels[1][index] for index in agglomerable_indices]
+            ),
+            np.array(
+                [buried_voxels.voxels[2][index] for index in agglomerable_indices]
+            ),
         )
         # get the voxel indices
         volume_indices = compute_voxel_indices(volume_voxels, voxel_grid.x_y_z)
         # create the voxelgroup
         voxel_group = VoxelGroup(
             voxels=volume_voxels,
             indices=volume_indices,
```

