# Comparing `tmp/loco_hd-0.1.2.tar.gz` & `tmp/loco_hd-0.1.3.tar.gz`

## Comparing `loco_hd-0.1.2.tar` & `loco_hd-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 loco_hd-0.1.2/Cargo.toml
--rw-rw-r--   0     1000     1000     1462 2023-02-09 09:29:24.000000 loco_hd-0.1.2/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      725 2022-08-15 09:48:38.000000 loco_hd-0.1.2/.gitignore
--rw-r--r--   0     1000     1000     1070 2023-07-14 15:16:26.000000 loco_hd-0.1.2/LICENSE
--rw-rw-r--   0     1000     1000     2803 2023-07-14 15:32:40.000000 loco_hd-0.1.2/README.md
--rw-rw-r--   0     1000     1000      192 2023-07-05 07:38:55.000000 loco_hd-0.1.2/loco_hd/__init__.py
--rw-rw-r--   0     1000     1000     5859 2023-05-27 18:48:17.000000 loco_hd-0.1.2/loco_hd/atom_converter_utils.py
--rw-rw-r--   0     1000     1000    10262 2023-07-05 09:21:30.000000 loco_hd-0.1.2/loco_hd/loco_hd.pyi
--rw-rw-r--   0     1000     1000        0 2023-05-27 18:48:17.000000 loco_hd-0.1.2/loco_hd/py.typed
--rw-rw-r--   0     1000     1000    79633 2023-07-05 13:57:31.000000 loco_hd-0.1.2/locohd_logo.png
--rw-rw-r--   0     1000     1000      591 2023-07-14 15:32:37.000000 loco_hd-0.1.2/pyproject.toml
--rw-rw-r--   0     1000     1000     8445 2023-07-05 08:32:15.000000 loco_hd-0.1.2/python_codes/casp14_compare_structures.py
--rw-rw-r--   0     1000     1000     5089 2023-01-11 08:17:42.000000 loco_hd-0.1.2/python_codes/casp14_predictor_extractor.py
--rw-rw-r--   0     1000     1000    12075 2023-07-05 07:43:41.000000 loco_hd-0.1.2/python_codes/casp14_predictor_test.py
--rw-rw-r--   0     1000     1000    12707 2023-07-05 09:33:56.000000 loco_hd-0.1.2/python_codes/compare_ensembles.py
--rw-rw-r--   0     1000     1000     2709 2023-07-05 09:04:33.000000 loco_hd-0.1.2/python_codes/kras_scan.py
--rw-rw-r--   0     1000     1000     6629 2023-07-05 09:14:09.000000 loco_hd-0.1.2/python_codes/pisces_random_pairs.py
--rw-rw-r--   0     1000     1000    14302 2023-02-08 12:00:46.000000 loco_hd-0.1.2/python_codes/pisces_random_pairs_analyze.py
--rw-rw-r--   0     1000     1000     1665 2023-03-27 08:14:26.000000 loco_hd-0.1.2/python_codes/primitive_typings/all_atom.config.json
--rw-rw-r--   0     1000     1000     1718 2023-05-27 18:48:17.000000 loco_hd-0.1.2/python_codes/primitive_typings/all_atom_with_centroid.config.json
--rw-rw-r--   0     1000     1000     1031 2023-05-27 18:48:17.000000 loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained.config.json
--rw-rw-r--   0     1000     1000     1084 2023-05-27 18:48:17.000000 loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained_with_centroid.config.json
--rw-rw-r--   0     1000     1000     1611 2023-07-13 11:38:45.000000 loco_hd-0.1.2/python_codes/simple_test.py
--rw-rw-r--   0     1000     1000     1152 2023-06-25 17:06:17.000000 loco_hd-0.1.2/python_codes/test_integrators.py
--rw-rw-r--   0     1000     1000    13402 2023-07-05 09:54:31.000000 loco_hd-0.1.2/python_codes/trajectory_analyzer.py
--rw-rw-r--   0     1000     1000      333 2023-07-04 18:40:06.000000 loco_hd-0.1.2/src/lib.rs
--rw-rw-r--   0     1000     1000     1031 2023-07-05 09:28:40.000000 loco_hd-0.1.2/src/locohd/locohd_utests.rs
--rw-rw-r--   0     1000     1000     2610 2023-07-04 14:26:07.000000 loco_hd-0.1.2/src/locohd/pmf.rs
--rw-rw-r--   0     1000     1000     1358 2023-07-04 14:30:01.000000 loco_hd-0.1.2/src/locohd/pmf_utests.rs
--rw-rw-r--   0     1000     1000      633 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/primitive_atom.rs
--rw-r--r--   0     1000     1000     1691 2023-07-05 09:26:30.000000 loco_hd-0.1.2/src/locohd/tag_pairing_rule.rs
--rw-r--r--   0     1000     1000        0 2023-07-04 18:38:40.000000 loco_hd-0.1.2/src/locohd/tag_pairing_rule_utests.rs
--rw-rw-r--   0     1000     1000     1227 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/utils.rs
--rw-rw-r--   0     1000     1000     2106 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/weight_function/cdfs.rs
--rw-rw-r--   0     1000     1000     4253 2023-07-05 07:09:39.000000 loco_hd-0.1.2/src/locohd/weight_function.rs
--rw-rw-r--   0     1000     1000     6902 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/weight_function_utests.rs
--rw-rw-r--   0     1000     1000    13001 2023-07-05 09:29:39.000000 loco_hd-0.1.2/src/locohd.rs
--rw-rw-r--   0     1000     1000    10496 2023-05-27 18:48:17.000000 loco_hd-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 loco_hd-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 loco_hd-0.1.3/Cargo.toml
+-rw-rw-r--   0     1000     1000     1462 2023-02-09 09:29:24.000000 loco_hd-0.1.3/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      726 2023-07-15 09:10:55.000000 loco_hd-0.1.3/.gitignore
+-rw-r--r--   0     1000     1000     1070 2023-07-14 15:16:26.000000 loco_hd-0.1.3/LICENSE
+-rw-rw-r--   0     1000     1000     8634 2023-07-15 13:54:13.000000 loco_hd-0.1.3/README.md
+-rw-rw-r--   0     1000     1000      192 2023-07-05 07:38:55.000000 loco_hd-0.1.3/loco_hd/__init__.py
+-rw-rw-r--   0     1000     1000     5859 2023-05-27 18:48:17.000000 loco_hd-0.1.3/loco_hd/atom_converter_utils.py
+-rw-rw-r--   0     1000     1000    10423 2023-07-15 09:00:22.000000 loco_hd-0.1.3/loco_hd/loco_hd.pyi
+-rw-rw-r--   0     1000     1000        0 2023-05-27 18:48:17.000000 loco_hd-0.1.3/loco_hd/py.typed
+-rw-rw-r--   0     1000     1000    79633 2023-07-05 13:57:31.000000 loco_hd-0.1.3/locohd_logo.png
+-rw-rw-r--   0     1000     1000     1665 2023-03-27 08:14:26.000000 loco_hd-0.1.3/primitive_typings/all_atom.config.json
+-rw-rw-r--   0     1000     1000     1718 2023-05-27 18:48:17.000000 loco_hd-0.1.3/primitive_typings/all_atom_with_centroid.config.json
+-rw-rw-r--   0     1000     1000     1031 2023-05-27 18:48:17.000000 loco_hd-0.1.3/primitive_typings/coarse_grained.config.json
+-rw-rw-r--   0     1000     1000     1084 2023-05-27 18:48:17.000000 loco_hd-0.1.3/primitive_typings/coarse_grained_with_centroid.config.json
+-rw-rw-r--   0     1000     1000      591 2023-07-15 13:35:47.000000 loco_hd-0.1.3/pyproject.toml
+-rw-rw-r--   0     1000     1000     8683 2023-07-15 09:32:22.000000 loco_hd-0.1.3/python_codes/casp14_compare_structures.py
+-rw-rw-r--   0     1000     1000     5186 2023-07-15 09:15:16.000000 loco_hd-0.1.3/python_codes/casp14_predictor_extractor.py
+-rw-rw-r--   0     1000     1000    12068 2023-07-15 09:34:18.000000 loco_hd-0.1.3/python_codes/casp14_predictor_test.py
+-rw-rw-r--   0     1000     1000    12705 2023-07-15 09:42:10.000000 loco_hd-0.1.3/python_codes/compare_ensembles.py
+-rw-rw-r--   0     1000     1000     2719 2023-07-15 09:45:28.000000 loco_hd-0.1.3/python_codes/kras_scan.py
+-rw-rw-r--   0     1000     1000     6609 2023-07-15 09:47:45.000000 loco_hd-0.1.3/python_codes/pisces_random_pairs.py
+-rw-rw-r--   0     1000     1000    14357 2023-07-15 09:52:15.000000 loco_hd-0.1.3/python_codes/pisces_random_pairs_analyze.py
+-rw-rw-r--   0     1000     1000     1611 2023-07-13 11:38:45.000000 loco_hd-0.1.3/python_codes/simple_test.py
+-rw-rw-r--   0     1000     1000     1153 2023-07-15 09:52:28.000000 loco_hd-0.1.3/python_codes/test_integrators.py
+-rw-rw-r--   0     1000     1000    13447 2023-07-15 10:04:13.000000 loco_hd-0.1.3/python_codes/trajectory_analyzer.py
+-rw-rw-r--   0     1000     1000      333 2023-07-04 18:40:06.000000 loco_hd-0.1.3/src/lib.rs
+-rw-rw-r--   0     1000     1000     1078 2023-07-15 08:12:37.000000 loco_hd-0.1.3/src/locohd/locohd_utests.rs
+-rw-rw-r--   0     1000     1000     2610 2023-07-04 14:26:07.000000 loco_hd-0.1.3/src/locohd/pmf.rs
+-rw-rw-r--   0     1000     1000     1358 2023-07-04 14:30:01.000000 loco_hd-0.1.3/src/locohd/pmf_utests.rs
+-rw-rw-r--   0     1000     1000      633 2023-05-27 18:48:17.000000 loco_hd-0.1.3/src/locohd/primitive_atom.rs
+-rw-r--r--   0     1000     1000     1691 2023-07-05 09:26:30.000000 loco_hd-0.1.3/src/locohd/tag_pairing_rule.rs
+-rw-r--r--   0     1000     1000        0 2023-07-04 18:38:40.000000 loco_hd-0.1.3/src/locohd/tag_pairing_rule_utests.rs
+-rw-rw-r--   0     1000     1000     1227 2023-05-27 18:48:17.000000 loco_hd-0.1.3/src/locohd/utils.rs
+-rw-rw-r--   0     1000     1000     2106 2023-05-27 18:48:17.000000 loco_hd-0.1.3/src/locohd/weight_function/cdfs.rs
+-rw-rw-r--   0     1000     1000     4253 2023-07-05 07:09:39.000000 loco_hd-0.1.3/src/locohd/weight_function.rs
+-rw-rw-r--   0     1000     1000     6902 2023-05-27 18:48:17.000000 loco_hd-0.1.3/src/locohd/weight_function_utests.rs
+-rw-rw-r--   0     1000     1000    13214 2023-07-15 08:11:58.000000 loco_hd-0.1.3/src/locohd.rs
+-rw-rw-r--   0     1000     1000    10496 2023-05-27 18:48:17.000000 loco_hd-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     9206 1970-01-01 00:00:00.000000 loco_hd-0.1.3/PKG-INFO
```

### Comparing `loco_hd-0.1.2/Cargo.toml` & `loco_hd-0.1.3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/.github/workflows/CI.yml` & `loco_hd-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/.gitignore` & `loco_hd-0.1.3/.gitignore`

 * *Files 26% similar despite different names*

```diff
@@ -68,8 +68,9 @@
 # VSCode
 .vscode/
 
 # Pyenv
 .python-version
 
 # python workdir
-python_codes/workdir/
+workdir/
+data_sources/
```

### Comparing `loco_hd-0.1.2/LICENSE` & `loco_hd-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/loco_hd/atom_converter_utils.py` & `loco_hd-0.1.3/loco_hd/atom_converter_utils.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/loco_hd/loco_hd.pyi` & `loco_hd-0.1.3/loco_hd/loco_hd.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -129,25 +129,26 @@
     :param tag_pairing_rule: The ``TagPairingRule`` employed.
     """
 
     categories: List[str]
 
     def __init__(self, 
                 categories: List[str], 
-                w_func: WeightFunction, 
+                w_func: Optional[WeightFunction] = None, 
                 tag_pairing_rule: Optional[TagPairingRule] = None,
                 n_of_threads: Optional[int] = None) -> None:
         """
         The constructor of the ``LoCoHD`` class.
 
         :param categories: The full set of the primitive types that can occur during calculations. When a primitive
           type that is not part of this list is encountered, the software throws an error.
-        :param w_func: The weight function used inside the integral. It weights the cumulative contribution of the
-          different primitive atoms within certain distances from the anchor atom, i.e. the contribution of primitive
-          atoms within the anchor atom's environment.
+        :param w_func: Either ``None`` or a  ``WeightFunction`` instance. The weight function used inside the integral. 
+          It weights the cumulative contribution of the different primitive atoms within certain distances from 
+          the anchor atom, i.e. the contribution of primitive atoms within the anchor atom's environment.
+          When ``None``, it defaults to the ``WeightFunction("uniform", [3., 10.])`` case.
         :param tag_pairing_rule: Either ``None`` or a  ``TagPairingRule`` instance. See the description of the 
           ``TagPairingRule`` class for what it does. When ``None``, it defaults to the
           ``TagPairingRule({"accept_same": True})`` case.
         :param n_of_threads: Either ``None`` or an integer. The number of threads the instance is allowed to use.
           When ``None``, all the threads become available for the instance.
         """
```

### Comparing `loco_hd-0.1.2/locohd_logo.png` & `loco_hd-0.1.3/locohd_logo.png`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/pyproject.toml` & `loco_hd-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.13,<0.14"]
 build-backend = "maturin"
 
 [project]
 name = "loco_hd"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name = "Zsolt Fazekas", email = "zsolt.fazekas.9@gmail.com" }
 ]
 description = "Implementation of the LoCoHD metric for quantitative protein structure and substructure comparison"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `loco_hd-0.1.2/python_codes/casp14_compare_structures.py` & `loco_hd-0.1.3/python_codes/casp14_compare_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import numpy as np
 import tarfile
 import codecs
 import matplotlib.pyplot as plt
 from typing import Dict, List
 from Bio.PDB.PDBParser import PDBParser
 from Bio.PDB.Atom import Atom
@@ -18,21 +19,22 @@
 # - FEIG-R2:
 #     - T1074TS480_2 and _5
 #     - RESI_IDX_SHIFT = 0
 #     - MAX_LCHD = 0.5
 #   and
 #     - T1046s1_...
 
-LDDT_TARS_PATH = Path("/home/fazekaszs/CoreDir/PhD/PDB/casp14/lDDTs")
-PREDICTOR_NAME = "TS480"
-STRUCTURE_NAME = "T1074"
-PREDICTED_SUFFIX1 = "_2"
+LDDT_TARS_PATH = Path("../data_sources/casp14/lDDTs")
+TARGET_PATH = Path("../workdir/casp14")
+PREDICTOR_NAME = "TS427"
+STRUCTURE_NAME = "T1064"
+PREDICTED_SUFFIX1 = "_1"
 PREDICTED_SUFFIX2 = "_5"
-RESI_IDX_SHIFT = 0
-MAX_LCHD = 0.5
+RESI_IDX_SHIFT = 15
+MAX_LCHD = 0.4
 
 
 def lddt_from_text(text: str):
 
     text = text.split("\n")
     header_text = "Chain	ResName	ResNum	Asses.	Q.Prob.	Score"
     start_idx = next(idx for idx in range(len(text)) if text[idx].startswith(header_text))
@@ -63,18 +65,21 @@
 
     resi_id = prat.atom_source.source_residue
     resname = prat.atom_source.source_residue_name
     source = f"{resi_id[2]}/{resi_id[3][1]}-{resname}"
     return PrimitiveAtom(prat.primitive_type, source, prat.coordinates)
 
 
-def create_lchd_histograms(name: str,
-                           lchd_scores: np.ndarray,
-                           anchor_idxs: List[int],
-                           residues: List[PrimitiveAtomTemplate]):
+def create_lchd_histograms(
+        name: str,
+        lchd_scores: np.ndarray,
+        anchor_idxs: List[int],
+        residues: List[PrimitiveAtomTemplate],
+        output_path: Path
+):
 
     fig, ax = plt.subplots()
     first_idxs = np.argsort(lchd_scores)[::-1][:10]
     anchor_prats = [residues[anchor_idxs[idx]] for idx in first_idxs]
 
     # Set the y-axis tick labels to the residue names.
     labels = list()
@@ -90,132 +95,138 @@
     ax.barh(labels, lchd_scores[first_idxs])  # Horizontal barplot
     x_ticks = np.arange(0, MAX_LCHD, MAX_LCHD / 10)
     ax.set_xticks(x_ticks, labels=[f"{x:.0%}" for x in x_ticks])
     ax.set_xlabel("LoCoHD score")
     ax.set_ylabel("Residue name")
     fig.suptitle(f"Top 10 Largest per-Residue\nLoCoHD Values in {name}")
     plt.tight_layout()
-    fig.savefig(f"./workdir/{name}_top10lchd.png", dpi=300, bbox_inches="tight")
+    fig.savefig(output_path / f"{name}_top10lchd.png", dpi=300, bbox_inches="tight")
 
     plt.close(fig)
 
 
 def main():
 
     # Names of the predicted structures, like T1064TS427_1.
     pred1_name = f"{STRUCTURE_NAME}{PREDICTOR_NAME}{PREDICTED_SUFFIX1}"
     pred2_name = f"{STRUCTURE_NAME}{PREDICTOR_NAME}{PREDICTED_SUFFIX2}"
 
     # Source paths.
-    pdb_dir_path = Path(f"/home/fazekaszs/CoreDir/PhD/LoCoHD/CASP14_{STRUCTURE_NAME}/pdbs")
+    pdb_dir_path = Path(f"../data_sources/casp14_{STRUCTURE_NAME}/pdbs")
     pdb_true_path = pdb_dir_path / f"{STRUCTURE_NAME}.pdb"
     pdb_pred1_path = pdb_dir_path / f"{pred1_name}.pdb"
     pdb_pred2_path = pdb_dir_path / f"{pred2_name}.pdb"
 
+    # Target path.
+    output_path = TARGET_PATH / f"{STRUCTURE_NAME}{PREDICTOR_NAME}{PREDICTED_SUFFIX1}{PREDICTED_SUFFIX2}"
+    if not os.path.exists(output_path):
+        os.mkdir(output_path)
+
     # Reading the PDB files.
     protein_true = PDBParser(QUIET=True).get_structure("true", pdb_true_path)
     protein_pred1 = PDBParser(QUIET=True).get_structure("pred1", pdb_pred1_path)
     protein_pred2 = PDBParser(QUIET=True).get_structure("pred2", pdb_pred2_path)
 
     filter_atoms(protein_true, protein_pred1)
     filter_atoms(protein_true, protein_pred2)
 
     # Create the PrimitiveAssigner instance
-    primitive_assigner = PrimitiveAssigner(Path("primitive_typings/all_atom_with_centroid.config.json"))
+    primitive_assigner = PrimitiveAssigner(Path("../primitive_typings/all_atom_with_centroid.config.json"))
 
     # Initialize LoCoHD instance
     weight_function = WeightFunction("uniform", [3, 10])
     tag_pairing_rule = TagPairingRule({"accept_same": False})
     lchd = LoCoHD(primitive_assigner.all_primitive_types, weight_function, tag_pairing_rule)
 
     # Parse the structures
     pra_templates_true = primitive_assigner.assign_primitive_structure(protein_true)
     pra_templates_pred1 = primitive_assigner.assign_primitive_structure(protein_pred1)
     pra_templates_pred2 = primitive_assigner.assign_primitive_structure(protein_pred2)
 
     # Get the anchor indices
-    anchor_idxs = [
+    anchor_pairs = [
         (idx, idx)
         for idx, pra_template in enumerate(pra_templates_true)
         if pra_template.primitive_type == "Cent"
     ]
 
     # Create the PrimitiveAtom lists
     pra_true = list(map(prat_to_pra, pra_templates_true))
     pra_pred1 = list(map(prat_to_pra, pra_templates_pred1))
     pra_pred2 = list(map(prat_to_pra, pra_templates_pred2))
 
     # Calculate the LoCoHD values
-    lchd_values1 = lchd.from_primitives(pra_true, pra_pred1, anchor_idxs, 10.)
+    lchd_values1 = lchd.from_primitives(pra_true, pra_pred1, anchor_pairs, 10.)
     lchd_values1 = np.array(lchd_values1)
-    lchd_values2 = lchd.from_primitives(pra_true, pra_pred2, anchor_idxs, 10.)
+    lchd_values2 = lchd.from_primitives(pra_true, pra_pred2, anchor_pairs, 10.)
     lchd_values2 = np.array(lchd_values2)
 
     lchd_mean1 = np.mean(lchd_values1)
     print(f"Mean LoCoHD value for {pred1_name}: {lchd_mean1:.1%}")
     lchd_mean2 = np.mean(lchd_values2)
     print(f"Mean LoCoHD value for {pred2_name}: {lchd_mean2:.1%}")
 
     # Plot the histograms for the first five residues, based on the largest
     # LoCoHD order
-    create_lchd_histograms(pred1_name, lchd_values1, [x[0] for x in anchor_idxs], pra_templates_pred1)
-    create_lchd_histograms(pred2_name, lchd_values2, [x[0] for x in anchor_idxs], pra_templates_pred2)
+    anchor_idxs = [x[0] for x in anchor_pairs]
+    create_lchd_histograms(pred1_name, lchd_values1, anchor_idxs, pra_templates_pred1, output_path)
+    create_lchd_histograms(pred2_name, lchd_values2, anchor_idxs, pra_templates_pred2, output_path)
 
     # Save the primitive structures
     pdb_str_true = primitive_assigner.generate_primitive_pdb(pra_templates_true)
-    with open(pdb_dir_path / f"{STRUCTURE_NAME}{PREDICTOR_NAME}_true_primitiveStructure.pdb", "w") as f:
+    with open(output_path / f"{STRUCTURE_NAME}{PREDICTOR_NAME}_true_primitiveStructure.pdb", "w") as f:
         f.write(pdb_str_true)
 
     pdb_str_pred1 = primitive_assigner.generate_primitive_pdb(pra_templates_pred1)
-    with open(pdb_dir_path / f"{pred1_name}_primitiveStructure.pdb", "w") as f:
+    with open(output_path / f"{pred1_name}_primitiveStructure.pdb", "w") as f:
         f.write(pdb_str_pred1)
 
     pdb_str_pred2 = primitive_assigner.generate_primitive_pdb(pra_templates_pred2)
-    with open(pdb_dir_path / f"{pred2_name}_primitiveStructure.pdb", "w") as f:
+    with open(output_path / f"{pred2_name}_primitiveStructure.pdb", "w") as f:
         f.write(pdb_str_pred2)
 
     # Set B-factors to LoCoHD values
-    for idx, (anchor_idx, _) in enumerate(anchor_idxs):
+    for idx, (anchor_idx, _) in enumerate(anchor_pairs):
 
         resi_id = pra_templates_true[anchor_idx].atom_source.source_residue
 
         atom: Atom
         for atom in protein_pred1[resi_id[1]][resi_id[2]][resi_id[3]].get_atoms():
             atom.bfactor = lchd_values1[idx]
 
         for atom in protein_pred2[resi_id[1]][resi_id[2]][resi_id[3]].get_atoms():
             atom.bfactor = lchd_values2[idx]
 
     io = PDBIO()
 
     io.set_structure(protein_pred1)
-    io.save(str(pdb_dir_path / f"{pred1_name}_lchd_blabelled.pdb"))
+    io.save(str(output_path / f"{pred1_name}_lchd_blabelled.pdb"))
 
     io.set_structure(protein_pred2)
-    io.save(str(pdb_dir_path / f"{pred2_name}_lchd_blabelled.pdb"))
+    io.save(str(output_path / f"{pred2_name}_lchd_blabelled.pdb"))
 
     # Load lDDT values
     lddt_values = read_lddt_values()
 
     # Set B-factors to lDDT values
-    for idx, (anchor_idx, _) in enumerate(anchor_idxs):
+    for idx, (anchor_idx, _) in enumerate(anchor_pairs):
 
         resi_id = pra_templates_true[anchor_idx].atom_source.source_residue
         resi_name = pra_templates_true[anchor_idx].atom_source.source_residue_name
         lddt_key = f"{resi_id[2]}/{resi_id[3][1]}-{resi_name}"
 
         atom: Atom
         for atom in protein_pred1[resi_id[1]][resi_id[2]][resi_id[3]].get_atoms():
             atom.bfactor = lddt_values[pred1_name][lddt_key]
 
         for atom in protein_pred2[resi_id[1]][resi_id[2]][resi_id[3]].get_atoms():
             atom.bfactor = lddt_values[pred2_name][lddt_key]
 
     io.set_structure(protein_pred1)
-    io.save(str(pdb_dir_path / f"{pred1_name}_lddt_blabelled.pdb"))
+    io.save(str(output_path / f"{pred1_name}_lddt_blabelled.pdb"))
 
     io.set_structure(protein_pred2)
-    io.save(str(pdb_dir_path / f"{pred2_name}_lddt_blabelled.pdb"))
+    io.save(str(output_path / f"{pred2_name}_lddt_blabelled.pdb"))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `loco_hd-0.1.2/python_codes/casp14_predictor_extractor.py` & `loco_hd-0.1.3/python_codes/casp14_predictor_extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from Bio.PDB.Entity import Entity
 from Bio.PDB.Structure import Structure
 from Bio.PDB.Atom import Atom
 
 # Set the necessary constants. The available predictor keys are the following:
 # AF2: TS427, BAKER: TS473, BAKER-experimental: TS403, FEIG-R2: TS480, Zhang: TS129
 PREDICTOR_KEY = "TS427"
-TARFILE_ROOT = Path("/home/fazekaszs/CoreDir/PhD/PDB/casp14")
+TARFILE_ROOT = Path("../data_sources/casp14")
+TARGET_DIR = Path("../workdir/casp14")
 
 
 class InLinePDBParser(PDBParser):
 
     def from_str(self, pdb_id: str, pdb_content: str) -> Structure:
 
         with warnings.catch_warnings():
@@ -121,16 +122,18 @@
                 print(f"# of atoms: {n_of_atoms} (vs {n_of_atoms_true}),", end=" ")
                 print(f"# of structures in member: {len(all_structures[member_name])}")
 
                 f.close()
 
     all_structures = {key: value for key, value in all_structures.items() if len(value) > 1}
 
-    if not os.path.exists(f"./workdir/{PREDICTOR_KEY}_results"):
-        os.mkdir(f"./workdir/{PREDICTOR_KEY}_results")
+    predictor_target_dir = TARGET_DIR / f"{PREDICTOR_KEY}_results"
+    if not os.path.exists(predictor_target_dir):
+        os.mkdir(predictor_target_dir)
 
-    with open(f"./workdir/{PREDICTOR_KEY}_results/{PREDICTOR_KEY}_structures.pickle", "wb") as f:
+    predictor_target_file = predictor_target_dir / f"{PREDICTOR_KEY}_structures.pickle"
+    with open(predictor_target_file, "wb") as f:
         pickle.dump(all_structures, f)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `loco_hd-0.1.2/python_codes/casp14_predictor_test.py` & `loco_hd-0.1.3/python_codes/casp14_predictor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from scipy.stats import spearmanr
 
 from loco_hd import LoCoHD, PrimitiveAtom, WeightFunction, PrimitiveAssigner, PrimitiveAtomTemplate, TagPairingRule
 
 
 # Set the necessary paths. The available predictor keys are the following:
 # AF2: TS427, BAKER: TS473, BAKER-experimental: TS403, FEIG-R2: TS480, Zhang: TS129
-LDDT_TARS_PATH = Path("/home/fazekaszs/CoreDir/PhD/PDB/casp14/lDDTs")
+LDDT_TARS_PATH = Path("../data_sources/casp14/lDDTs")
 PREDICTOR_KEY = "TS129"
-WORKDIR = Path(f"./workdir/{PREDICTOR_KEY}_results")
+WORKDIR = Path(f"../workdir/casp14/{PREDICTOR_KEY}_results")
 
 ScoreStatType = Dict[str, Dict[str, Tuple[float, float, float]]]
 
 
 def prat_to_pra(prat: PrimitiveAtomTemplate) -> PrimitiveAtom:
 
     resi_id = prat.atom_source.source_residue
@@ -182,15 +182,15 @@
 
     plt.close(fig)
 
 
 def main():
 
     # Create the primitive assigner
-    primitive_assigner = PrimitiveAssigner(Path("./primitive_typings/all_atom_with_centroid.config.json"))
+    primitive_assigner = PrimitiveAssigner(Path("../primitive_typings/all_atom_with_centroid.config.json"))
 
     # Create the LoCoHD instance.
     w_func = WeightFunction("uniform", [3, 10])
     tag_pairing_rule = TagPairingRule({"accept_same": False})
     lchd = LoCoHD(primitive_assigner.all_primitive_types, w_func, tag_pairing_rule)
 
     # The values in the structures dict are also dicts. The first key refers to the
```

### Comparing `loco_hd-0.1.2/python_codes/compare_ensembles.py` & `loco_hd-0.1.3/python_codes/compare_ensembles.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
 
 def compare_structures(prot_root_path: Path, save_dir: Path, save_name: str) -> Dict[str, Any]:
 
     print(f"Starting {save_name}...")
 
     # Create the PrimitiveAssigner instance
-    primitive_assigner = PrimitiveAssigner(Path("primitive_typings/coarse_grained.config.json"))
+    primitive_assigner = PrimitiveAssigner(Path("../primitive_typings/coarse_grained.config.json"))
 
     # Initialize LoCoHD instance
     w_func = WeightFunction("uniform", [3., 10.])
     lchd = LoCoHD(primitive_assigner.all_primitive_types, w_func)
 
     # Collect all the filenames in the directory
     all_files: List[str] = os.listdir(prot_root_path)
@@ -299,24 +299,24 @@
     print(f"B-labelled primitive structure saved as {pdb_save_name} based on the template {all_files[0]}!")
 
     return {"rmsd_dmx": rmsd_dmx, "lchd_dmx": lchd_dmx, "lchd_by_atom": lchd_by_atom}
 
 
 def main():
 
-    save_dir = Path("./workdir/prot_batch_resuls")
+    save_dir = Path("../workdir/prot_batch_resuls")
     paths_and_names = [
-        # ("./workdir/pdb_files/h5", "h5_dummy"),
-        ("/home/fazekaszs/CoreDir/PhD/PDB/H5/277", "h5_277"),
-        ("/home/fazekaszs/CoreDir/PhD/PDB/H5/288", "h5_288"),
-        ("/home/fazekaszs/CoreDir/PhD/PDB/H5/299", "h5_299"),
-        ("/home/fazekaszs/CoreDir/PhD/PDB/H5/310", "h5_310"),
-        ("/home/fazekaszs/CoreDir/PhD/PDB/H5/321", "h5_321"),
-        # ("./workdir/pdb_files/PED00075e000", "PED00075e000"),
-        # ("./workdir/pdb_files/PED00072e000", "PED00072e000"),
+        # ("../data_sources/pdb_files/h5/dummy", "h5_dummy"),
+        ("../data_sources/pdb_files/h5/277", "h5_277"),
+        ("../data_sources/pdb_files/h5/288", "h5_288"),
+        ("../data_sources/pdb_files/h5/299", "h5_299"),
+        ("../data_sources/pdb_files/h5/310", "h5_310"),
+        ("../data_sources/pdb_files/h5/321", "h5_321"),
+        # ("../data_sources/pdb_files/PED00075e000", "PED00075e000"),
+        # ("../data_sources/pdb_files/PED00072e000", "PED00072e000"),
     ]
 
     rmsd_dmxs, lchd_dmxs, lchd_by_atom = list(), list(), list()
 
     for prot_root_path, prot_name in paths_and_names:
 
         out_dict = compare_structures(Path(prot_root_path), save_dir, prot_name)
```

### Comparing `loco_hd-0.1.2/python_codes/kras_scan.py` & `loco_hd-0.1.3/python_codes/kras_scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     resname = prat.atom_source.source_residue_name
     source = f"{resi_id[2]}/{resi_id[3][1]}-{resname}"
     return PrimitiveAtom(prat.primitive_type, source, prat.coordinates)
 
 
 def main():
 
-    protein: Chain = PDBParser(QUIET=True).get_structure("kras", "./workdir/kras_scan/4obe.pdb")[0]["A"]
-    pra_assigner = PrimitiveAssigner(Path("primitive_typings/all_atom.config.json"))
+    protein: Chain = PDBParser(QUIET=True).get_structure("kras", "../data_sources/kras_scan/4obe.pdb")[0]["A"]
+    pra_assigner = PrimitiveAssigner(Path("../primitive_typings/all_atom.config.json"))
 
     prat_list = pra_assigner.assign_primitive_structure(protein)
     pra_list = list(map(prat_to_pra, prat_list))
 
     scan_anchors: List[PrimitiveAtom] = list()
     atom: Atom
     for atom in protein.get_atoms():
@@ -69,13 +69,13 @@
         line += f"{scan_pra.coordinates[2]:8.3f}"  # z
         line += "      "  # occupancy
         line += f"{score:6.2f}"
         line += "\n"
 
         out += line
 
-    with open("./workdir/kras_scan/4obe_scan.pdb", "w") as f:
+    with open("../workdir/kras_scan/4obe_scan.pdb", "w") as f:
         f.write(out)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `loco_hd-0.1.2/python_codes/pisces_random_pairs.py` & `loco_hd-0.1.3/python_codes/pisces_random_pairs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 
 def main():
 
     # Parameters
     current_time = datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
     output_filename = "locohd_data.pisces"
-    workdir_target = Path("workdir/pisces")
-    assigner_config_path = Path("primitive_typings/coarse_grained_with_centroid.config.json")
-    pisces_path = Path("/home/fazekaszs/PycharmProjects/databases/pisces_220222")
+    workdir_target = Path("../workdir/pisces")
+    assigner_config_path = Path("../primitive_typings/coarse_grained_with_centroid.config.json")
+    pisces_path = Path("../../databases/pisces_220222")
     random_seed = 1994
     max_n_of_anchors = 1500
     weight_function = ("uniform", [3, 10, ])
     tag_pairing_rule = TagPairingRule({"accept_same": False})
     upper_cutoff = 10
 
     # Create working directory
```

### Comparing `loco_hd-0.1.2/python_codes/pisces_random_pairs_analyze.py` & `loco_hd-0.1.3/python_codes/pisces_random_pairs_analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -270,35 +270,35 @@
     fit_results = curve_fit(beta_cdf, x_values, y_values, p0=start_params, bounds=bound_params)
 
     return fit_results[0]
 
 
 def main():
 
-    workdir = Path("workdir/pisces")
+    data_source_dir = Path("../workdir/pisces")
     # data_source = "run_2023-01-10-11-52-33"
-    data_source = "run_2023-02-08-12-50-23"
+    data_source_name = "run_2023-02-08-12-50-23"
 
-    print(f"Opening directory: \"{data_source}\" at \"{workdir}\"")
+    print(f"Opening directory: \"{data_source_name}\" at \"{data_source_dir}\"")
 
-    with open(workdir / data_source / "locohd_data.pisces", "rb") as f:
+    with open(data_source_dir / data_source_name / "locohd_data.pisces", "rb") as f:
         data: List[Tuple[str, str, float]] = pickle.load(f)
 
     print(f"Number of samples: {len(data)}. Starting to generate statistics...")
 
     # Generating statistics for different property type pairs.
     statistics = generate_statistics(data)
 
     print("Statistics generated! Creating tsvs...")
     tsvs = stat_to_tsvs(statistics)
 
     # Saving the statistics.
 
     print("tsvs created! Saving tsv tables...")
-    analysis_dir_path = workdir / data_source / "analysis"
+    analysis_dir_path = data_source_dir / data_source_name / "analysis"
     if not os.path.exists(analysis_dir_path):
         os.mkdir(analysis_dir_path)
 
     for prop_name, tsv_data in zip(PROPERTY_NAMES, tsvs):
         with open(analysis_dir_path / f"{prop_name}_statistics.tsv", "w") as f:
             f.write(tsv_data)
```

### Comparing `loco_hd-0.1.2/python_codes/primitive_typings/all_atom.config.json` & `loco_hd-0.1.3/primitive_typings/all_atom.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/python_codes/primitive_typings/all_atom_with_centroid.config.json` & `loco_hd-0.1.3/primitive_typings/all_atom_with_centroid.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained.config.json` & `loco_hd-0.1.3/primitive_typings/coarse_grained.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained_with_centroid.config.json` & `loco_hd-0.1.3/primitive_typings/coarse_grained_with_centroid.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/python_codes/simple_test.py` & `loco_hd-0.1.3/python_codes/simple_test.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/python_codes/test_integrators.py` & `loco_hd-0.1.3/python_codes/test_integrators.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,12 +31,12 @@
 
         ax.plot(x_values, y_values)
         ax.plot(x_values[1:], y_prime_values)
 
         num_params_str = "p".join(map(lambda x: f"{x:.3f}", param_set[1]))
         test_name = f"{param_set[0]}_p{num_params_str}.png"
 
-        fig.savefig(f"./workdir/integrator_tests/{test_name}", dpi=300)
+        fig.savefig(f"../workdir/integrator_tests/{test_name}", dpi=300)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `loco_hd-0.1.2/python_codes/trajectory_analyzer.py` & `loco_hd-0.1.3/python_codes/trajectory_analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,17 +74,19 @@
     return PrimitiveAtom(prat.primitive_type, source, prat.coordinates)
 
 
 def arg_median(data: np.ndarray):
     return np.argsort(data)[len(data) // 2]
 
 
-def calculate_lchd_scores(universe: Universe,
-                          delta_frame: int,
-                          primitive_typing_scheme_path: Path) -> np.ndarray:
+def calculate_lchd_scores(
+        universe: Universe,
+        delta_frame: int,
+        primitive_typing_scheme_path: Path
+) -> np.ndarray:
 
     print("Calculating the time-dependency of residue LoCoHD scores!")
 
     # Define the primitive typing scheme
     primitive_assigner = MDPrimitiveAssigner(primitive_typing_scheme_path)
 
     # Define the LoCoHD instance
@@ -119,15 +121,15 @@
         eta *= (current_real_time - start_real_time) / (frame_idx + 1)  # current time / frame rate
         print(f"\r{frame_idx / full_trajectory_length:.1%} at time {frame.time:.0f} ps. ETA: {eta:.1f} s.", end="")
 
     print("\nCalculations done!")
     return np.array(all_points)
 
 
-def calculate_bimodality_coeff(universe: Universe, all_points: np.ndarray, workdir: Path):
+def calculate_bimodality_coeff(universe: Universe, all_points: np.ndarray, target_dir: Path):
 
     print("Calculating bimodalities!")
 
     lchd_skewnesses = skew(all_points, axis=0)
     lchd_kurtoses = kurtosis(all_points, axis=0, fisher=False)
 
     sarle_bimodality_coeff = (lchd_skewnesses ** 2 + 1) / lchd_kurtoses
@@ -137,23 +139,25 @@
     sarle_bimodality_coeff = sarle_bimodality_coeff[bimodality_order]
 
     out = ""
     for resname, coeff in zip(residues, sarle_bimodality_coeff):
         out += f"{resname}\t{coeff}\n"
     out = out[:-1]
 
-    with open(workdir / "resi_bimodalities.txt", "w") as f:
+    with open(target_dir / "resi_bimodalities.txt", "w") as f:
         f.write(out)
 
 
-def plot_time_dependencies(universe: Universe,
-                           x_values: np.ndarray,
-                           all_points: np.ndarray,
-                           delta_frame: int,
-                           workdir: Path):
+def plot_time_dependencies(
+        universe: Universe,
+        x_values: np.ndarray,
+        all_points: np.ndarray,
+        delta_frame: int,
+        target_dir: Path
+):
 
     print("Plotting LoCoHD score time dependencies!")
 
     fig, ax = plt.subplots()
     plt.tight_layout()
 
     max_lchd = np.max(all_points)
@@ -196,15 +200,15 @@
                   framealpha=0.7, handlelength=0, handletextpad=0)
         ax.plot(x_values, y_values, c="black")
         ax.set_xlabel("$t$ / ns")
         ax.set_ylabel("LoCoHD score")
         ax.set_title(plot_title)
         ax.set_yticks(y_axis_ticks, labels=[f"{tick:.1%}" for tick in y_axis_ticks])
         ax.set_ylim(0, max_lchd)
-        fig.savefig(str(workdir / f"{plot_title}.png"), dpi=200, bbox_inches="tight")
+        fig.savefig(str(target_dir / f"{plot_title}.png"), dpi=200, bbox_inches="tight")
 
     # Plotting of the mean (along residues) LoCoHD value's time dependency
     mean_lchd_t = np.mean(all_points, axis=1)
     ax.cla()
 
     max_lchd_idx = np.argmax(mean_lchd_t)
     max_lchd_time = max_lchd_idx * delta_frame * universe.trajectory.dt
@@ -233,20 +237,20 @@
               framealpha=0.7, handlelength=0, handletextpad=0)
     ax.plot(x_values, mean_lchd_t, c="black")
     ax.set_xlabel("$t$ / ns")
     ax.set_ylabel("LoCoHD score")
     ax.set_title("Mean LoCoHD values")
     ax.set_yticks(y_axis_ticks, labels=[f"{tick:.1%}" for tick in y_axis_ticks])
     ax.set_ylim(0, max_lchd)
-    fig.savefig(str(workdir / f"mean_locohd.png"), dpi=200, bbox_inches="tight")
+    fig.savefig(str(target_dir / f"mean_locohd.png"), dpi=200, bbox_inches="tight")
 
     print("\nPlotting for residues done!")
 
 
-def plot_pca(x_values: np.ndarray, all_points: np.ndarray, workdir: Path):
+def plot_pca(x_values: np.ndarray, all_points: np.ndarray, target_dir: Path):
 
     print("Calculating and plotting LoCoHD principal components...")
 
     fig, ax = plt.subplots()
     fig.tight_layout()
 
     # Skip the first frame, since it is an outlier (always 0)
@@ -255,95 +259,96 @@
 
     # Plotting the first principal component's time dependency
     ax.cla()
     ax.plot(x_values[1:], principal_comp[:, 0], c="black")
     ax.set_xlabel("$t$ / ns")
     ax.set_ylabel("PCA1")
     ax.set_title("Time Evolution of the First Principal Component")
-    fig.savefig(workdir / "pca.png", dpi=200, bbox_inches="tight")
+    fig.savefig(target_dir / "pca.png", dpi=200, bbox_inches="tight")
 
     # Plotting the first two principal component's time dependency
     ax.cla()
     ax.scatter(principal_comp[:, 0], principal_comp[:, 1], c=x_values[1:])
     ax.set_xlabel("PCA1")
     ax.set_ylabel("PCA2")
     ax.set_title("Time Evolution of the\nFirst Two Principal Components")
-    fig.savefig(workdir / "pca_2.png", dpi=200, bbox_inches="tight")
+    fig.savefig(target_dir / "pca_2.png", dpi=200, bbox_inches="tight")
 
     # Plotting the explained variance ratio of each component
     ax.cla()
     ax.set_xlabel("Rank of component")
     ax.set_ylabel("Cumulative explained variance")
     ax.set_title("Cumulative Explained Variance of\neach Principal Component")
 
     y_axis_ticks = np.arange(0, 1.1, 0.1)
     ax.set_yticks(y_axis_ticks, labels=[f"{tick:.1%}" for tick in y_axis_ticks])
     cumulative_expl_var = np.cumsum(pca.explained_variance_ratio_)
     cumulative_expl_var = np.append([0, ], cumulative_expl_var)
     ax.plot(np.arange(len(cumulative_expl_var)), cumulative_expl_var, c="black")
-    fig.savefig(workdir / "pca_explained_variance.png", dpi=200, bbox_inches="tight")
+    fig.savefig(target_dir / "pca_explained_variance.png", dpi=200, bbox_inches="tight")
 
     # Plotting the covariance matrix of the residues
     ax.cla()
     ax.imshow(pca.get_covariance())
     ax.set_title("Covariance Matrix between the\nLoCoHD Scores of Residues")
-    fig.savefig(workdir / "pca_cov.png", dpi=200, bbox_inches="tight")
+    fig.savefig(target_dir / "pca_cov.png", dpi=200, bbox_inches="tight")
 
     print("Principal components plotted!")
 
 
-def save_blabelled_pdb(universe: Universe, all_points: np.ndarray, workdir: Path):
+def save_blabelled_pdb(universe: Universe, all_points: np.ndarray, target_dir: Path):
 
     print("Creating and Saving b-factor labelled pdb file")
 
     universe.add_TopologyAttr("tempfactors")
     tempfactors = np.std(all_points[1:], axis=0) * 100
 
     print(f"Created {len(tempfactors)} number of temperature factors...")
 
     resi: mda.core.groups.Residue
     for resi, t_value in zip(universe.residues, tempfactors):
         resi.atoms.tempfactors += t_value
 
-    universe.select_atoms("protein").write(str(workdir / "b_labelled.pdb"))
+    universe.select_atoms("protein").write(str(target_dir / "b_labelled.pdb"))
 
 
 def main():
 
     # Establish working directory, data sources
-    workdir = Path("./workdir/trajectory_analysis/podocin_dimer")
-    trajectory_path = workdir / "podocin_wt_dimer_mcc_dt100.xtc"
-    structure_path = workdir / "podocin_wt_dimer_onlyProt.tpr"
-    primitive_typing_scheme_path = Path("./primitive_typings/coarse_grained_with_centroid.config.json")
+    source_dir = Path("../data_sources/trajectory_analysis/podocin_dimer")
+    target_dir = Path("../workdir/trajectory_analysis/podocin_dimer")
+    trajectory_path = source_dir / "podocin_wt_dimer_mcc_dt100.xtc"
+    structure_path = source_dir / "podocin_wt_dimer_onlyProt.tpr"
+    primitive_typing_scheme_path = Path("../primitive_typings/coarse_grained_with_centroid.config.json")
 
     # Read the structure file and the trajectory
     universe = mda.Universe(str(structure_path), str(trajectory_path))
 
     # Load in or calculate the LoCoHD data
     delta_frame = 25
-    scores_path = workdir / "LoCoHD_scores.npy"
+    scores_path = target_dir / "LoCoHD_scores.npy"
     if os.path.exists(scores_path):
         print("Already calculated scores found in the working directory! I will use them for the analysis!")
         all_points = np.load(str(scores_path))
     else:
         all_points = calculate_lchd_scores(universe, delta_frame, primitive_typing_scheme_path)
         np.save(str(scores_path), all_points)
 
     # Set the time points at which we made the analysis
     x_values = np.arange(len(all_points)) * delta_frame * universe.trajectory.dt / 1000
     x_values += universe.trajectory[0].time / 1000
 
     # Calculate the bimodality coefficient of the LoCoHD time dependence for every residue
-    calculate_bimodality_coeff(universe, all_points, workdir)
+    calculate_bimodality_coeff(universe, all_points, target_dir)
 
     # Plotting the first principal component's time dependency
-    plot_pca(x_values, all_points, workdir)
+    plot_pca(x_values, all_points, target_dir)
 
     # Saving a b-factor labelled structure
-    save_blabelled_pdb(universe, all_points, workdir)
+    save_blabelled_pdb(universe, all_points, target_dir)
 
     # Plotting of individual LoCoHD time dependencies
-    plot_time_dependencies(universe, x_values, all_points, delta_frame, workdir)
+    plot_time_dependencies(universe, x_values, all_points, delta_frame, target_dir)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `loco_hd-0.1.2/src/locohd/locohd_utests.rs` & `loco_hd-0.1.3/src/locohd/locohd_utests.rs`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 fn value_test1() -> PyResult<()> {
 
     let w_func = WeightFunction::build(
         "uniform".to_owned(), 
         vec![0., 4.]
     )?;
     let cats = vec!["O".to_owned(), "A".to_owned(), "B".to_owned(), "C".to_owned()];
-    let lchd = LoCoHD::build(cats, w_func, None, None)?;
+    let lchd = LoCoHD::build(
+        cats, 
+        Some(w_func), 
+        None, 
+        None
+    )?;
 
     let result = lchd.from_anchors(
         vec!["O".to_owned(), "A".to_owned(), "B".to_owned(), "C".to_owned()], 
         vec!["O".to_owned(), "A".to_owned(), "B".to_owned(), "C".to_owned()],
         vec![0., 1., 2., 3.],
         vec![0., 1., 1., 1.]
     )?;
```

### Comparing `loco_hd-0.1.2/src/locohd/pmf.rs` & `loco_hd-0.1.3/src/locohd/pmf.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd/pmf_utests.rs` & `loco_hd-0.1.3/src/locohd/pmf_utests.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd/primitive_atom.rs` & `loco_hd-0.1.3/src/locohd/primitive_atom.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd/tag_pairing_rule.rs` & `loco_hd-0.1.3/src/locohd/tag_pairing_rule.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd/utils.rs` & `loco_hd-0.1.3/src/locohd/utils.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd/weight_function/cdfs.rs` & `loco_hd-0.1.3/src/locohd/weight_function/cdfs.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd/weight_function.rs` & `loco_hd-0.1.3/src/locohd/weight_function.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd/weight_function_utests.rs` & `loco_hd-0.1.3/src/locohd/weight_function_utests.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.2/src/locohd.rs` & `loco_hd-0.1.3/src/locohd.rs`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,32 @@
 
 #[pymethods]
 impl LoCoHD {
 
     #[new]
     pub fn build(
         categories: Vec<String>, 
-        w_func: WeightFunction, 
+        w_func: Option<WeightFunction>, 
         tag_pairing_rule: Option<TagPairingRule>,
         n_of_threads: Option<usize>
     ) -> PyResult<Self> {
 
         // For faster lookup of the categories we use a HashMap instead of the supplied Vec.
         let categories: HashMap<_, _> = categories
             .into_iter()
             .enumerate()
             .map(|(a, b)| (b, a))
             .collect();
 
+        // Set default WeightFunction if necessary
+        let w_func = match w_func {
+            None => WeightFunction::build("uniform".to_owned(), vec![3., 10.])?,
+            Some(v) => v
+        };
+
         // Set default TagPairingRule options if necessary
         let tag_pairing_rule = match tag_pairing_rule {
             None => TagPairingRule::build(TagPairingRuleVariants::WithoutList { accept_same: true })?,
             Some(v) => v
         };
 
         // Set multithreading options
```

### Comparing `loco_hd-0.1.2/Cargo.lock` & `loco_hd-0.1.3/Cargo.lock`

 * *Files identical despite different names*

