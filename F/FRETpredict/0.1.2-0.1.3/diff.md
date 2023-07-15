# Comparing `tmp/FRETpredict-0.1.2.tar.gz` & `tmp/FRETpredict-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FRETpredict-0.1.2.tar", last modified: Fri Feb 10 10:13:25 2023, max compression
+gzip compressed data, was "FRETpredict-0.1.3.tar", last modified: Sat Jul 15 15:06:39 2023, max compression
```

## Comparing `FRETpredict-0.1.2.tar` & `FRETpredict-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-02-10 10:13:25.494417 FRETpredict-0.1.2/
-drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-02-10 10:13:25.488549 FRETpredict-0.1.2/FRETpredict/
--rw-r--r--   0 vbr805     (501) staff       (20)    24633 2023-02-10 09:56:53.000000 FRETpredict-0.1.2/FRETpredict/FRET.py
--rw-r--r--   0 vbr805     (501) staff       (20)     3281 2023-02-04 20:08:35.000000 FRETpredict-0.1.2/FRETpredict/R0_calculation.py
--rw-r--r--   0 vbr805     (501) staff       (20)      222 2023-02-10 10:00:49.000000 FRETpredict-0.1.2/FRETpredict/__init__.py
--rw-r--r--   0 vbr805     (501) staff       (20)      542 2023-02-04 20:08:35.000000 FRETpredict-0.1.2/FRETpredict/lennardjones.py
--rw-r--r--   0 vbr805     (501) staff       (20)     4928 2023-02-04 20:08:35.000000 FRETpredict-0.1.2/FRETpredict/libraries.py
--rw-r--r--   0 vbr805     (501) staff       (20)    21351 2023-02-04 20:08:35.000000 FRETpredict-0.1.2/FRETpredict/rotamer_libraries.py
--rw-r--r--   0 vbr805     (501) staff       (20)    18647 2023-02-10 09:56:53.000000 FRETpredict-0.1.2/FRETpredict/utils.py
-drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-02-10 10:13:25.493218 FRETpredict-0.1.2/FRETpredict.egg-info/
--rw-r--r--   0 vbr805     (501) staff       (20)     7697 2023-02-10 10:13:24.000000 FRETpredict-0.1.2/FRETpredict.egg-info/PKG-INFO
--rw-r--r--   0 vbr805     (501) staff       (20)      381 2023-02-10 10:13:24.000000 FRETpredict-0.1.2/FRETpredict.egg-info/SOURCES.txt
--rw-r--r--   0 vbr805     (501) staff       (20)        1 2023-02-10 10:13:24.000000 FRETpredict-0.1.2/FRETpredict.egg-info/dependency_links.txt
--rw-r--r--   0 vbr805     (501) staff       (20)      161 2023-02-10 10:13:24.000000 FRETpredict-0.1.2/FRETpredict.egg-info/requires.txt
--rw-r--r--   0 vbr805     (501) staff       (20)       12 2023-02-10 10:13:24.000000 FRETpredict-0.1.2/FRETpredict.egg-info/top_level.txt
--rw-r--r--   0 vbr805     (501) staff       (20)    35149 2023-02-04 20:08:35.000000 FRETpredict-0.1.2/LICENSE
--rw-r--r--   0 vbr805     (501) staff       (20)     7697 2023-02-10 10:13:25.494029 FRETpredict-0.1.2/PKG-INFO
--rw-r--r--   0 vbr805     (501) staff       (20)     6739 2023-02-10 09:59:28.000000 FRETpredict-0.1.2/README.md
--rw-r--r--   0 vbr805     (501) staff       (20)       38 2023-02-10 10:13:25.494463 FRETpredict-0.1.2/setup.cfg
--rwxr-xr-x   0 vbr805     (501) staff       (20)     2228 2023-02-04 20:08:35.000000 FRETpredict-0.1.2/setup.py
+drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 15:06:39.784108 FRETpredict-0.1.3/
+drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 15:06:39.774966 FRETpredict-0.1.3/FRETpredict/
+-rw-r--r--   0 vbr805     (501) staff       (20)    24607 2023-07-15 14:44:17.000000 FRETpredict-0.1.3/FRETpredict/FRET.py
+-rw-r--r--   0 vbr805     (501) staff       (20)     3281 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/R0_calculation.py
+-rw-r--r--   0 vbr805     (501) staff       (20)      222 2023-07-15 15:06:15.000000 FRETpredict-0.1.3/FRETpredict/__init__.py
+-rw-r--r--   0 vbr805     (501) staff       (20)      542 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/lennardjones.py
+-rw-r--r--   0 vbr805     (501) staff       (20)     4928 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/libraries.py
+-rw-r--r--   0 vbr805     (501) staff       (20)    21351 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/rotamer_libraries.py
+-rw-r--r--   0 vbr805     (501) staff       (20)    18629 2023-07-15 14:40:07.000000 FRETpredict-0.1.3/FRETpredict/utils.py
+drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 15:06:39.782745 FRETpredict-0.1.3/FRETpredict.egg-info/
+-rw-r--r--   0 vbr805     (501) staff       (20)     7697 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/PKG-INFO
+-rw-r--r--   0 vbr805     (501) staff       (20)      381 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/SOURCES.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)        1 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/dependency_links.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)      161 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/requires.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)       12 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/top_level.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)    35149 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/LICENSE
+-rw-r--r--   0 vbr805     (501) staff       (20)     7697 2023-07-15 15:06:39.783331 FRETpredict-0.1.3/PKG-INFO
+-rw-r--r--   0 vbr805     (501) staff       (20)     6739 2023-02-10 09:59:28.000000 FRETpredict-0.1.3/README.md
+-rw-r--r--   0 vbr805     (501) staff       (20)       38 2023-07-15 15:06:39.784168 FRETpredict-0.1.3/setup.cfg
+-rwxr-xr-x   0 vbr805     (501) staff       (20)     2228 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/setup.py
```

### Comparing `FRETpredict-0.1.2/FRETpredict/FRET.py` & `FRETpredict-0.1.3/FRETpredict/FRET.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import h5py
 import logging
 import MDAnalysis
 import re
 
 # Inner imports
 from .utils import Operations
-
+from .libraries import *
 
 class FRETpredict(Operations):
     """
 
     Calculation of FRET signal between two chromophores.
 
     Attributes
@@ -95,15 +95,15 @@
 
         trajectoryAnalysis:
             Calculate distribution of <E> (i.e. one <E> for each protein trajectory frame) in static, dynamic1, and
             dynamic2 regimes.
 
         save:
             Calculate k2 distribution and k2, Static, Dynamic1, Dynamic2 averaging, with or without reweighting. Save data to file.
-            
+
         reweight:
             Alias for reweigthing calculations. Call save() function with weights for reweighting.
 
         run:
             Run FRET Efficiency calculations by calling trajectoryAnalysis() and save data to file.
 
     """
@@ -275,24 +275,25 @@
         donor_producer = temp.match(self.donor).groups()[0]
         acceptor_producer = temp.match(self.acceptor).groups()[0]
 
         donor_number = temp.match(self.donor).groups()[1]
         acceptor_number = temp.match(self.acceptor).groups()[1]
 
         # Read donor spectrum from file and normalize max value to 1
-        donor_spectrum = pd.read_csv(f'{self.r0lib}/{donor_producer}{donor_number}.csv')
+
+        donor_spectrum = pd.read_csv(find_file(f'{donor_producer}{donor_number}.csv',pkglibdir=self.r0lib))
         donor_spectrum[['Emission', 'Excitation']] = donor_spectrum[['Emission', 'Excitation']] / 100
 
         # Read acceptor spectrum from file and normalize max value to 1
-        acceptor_spectrum = pd.read_csv(f'{self.r0lib}/{acceptor_producer}{acceptor_number}.csv')
+        acceptor_spectrum = pd.read_csv(find_file(f'{acceptor_producer}{acceptor_number}.csv',pkglibdir=self.r0lib))
         acceptor_spectrum[['Emission', 'Excitation']] = acceptor_spectrum[['Emission', 'Excitation']] / 100
 
         # Quantum yield and extinction coefficient data for the chromophores
-        chromophore_data = pd.read_csv(f'{self.r0lib}/Dyes_extinction_QD.csv', delimiter=',', on_bad_lines='skip',
-                                       names=['Type', 'Chromophore', 'Ext_coeff', 'QD'])
+        chromophore_data = pd.read_csv(find_file('Dyes_extinction_QD.csv',pkglibdir=self.r0lib),delimiter=',',
+                                       on_bad_lines='skip',names=['Type', 'Chromophore', 'Ext_coeff', 'QD'])
 
         # R0 calculation parameters
         # Initial factor, for R0 expressed in nm
         factor = 0.02108
 
         # 4th-power of the medium refractive index (water)
         n4 = 1.4 ** 4
@@ -353,15 +354,15 @@
         edyn1_avg = np.full(self.protein.trajectory.n_frames, np.nan)
         edyn2_avg = np.full(self.protein.trajectory.n_frames, np.nan)
         allk2 = np.empty(0)
         allZ = np.empty(0)
 
         for frame_ndx, _ in enumerate(self.protein.trajectory):
 
-            print(f'\nFrame {frame_ndx + 1}/{len(self.protein.trajectory)}')
+            print(f'{frame_ndx + 1}/{len(self.protein.trajectory)}',end='-')
 
             # Fit the rotamers onto the protein
             # Each protein structure (i.e. trajectory frame) has m conformations for chromophore 1 and l conformations
             # for chromophore 2
             rotamersSite1 = self.rotamer_placement(rotamer1, prot_atoms1, self.lib_1)
             rotamersSite2 = self.rotamer_placement(rotamer2, prot_atoms2, self.lib_2)
 
@@ -555,45 +556,45 @@
                                self.weightedAvgSDSE(estatic[np.isfinite(k2)], self.weights[np.isfinite(k2)]),
                                self.weightedAvgSDSE(edynamic1[np.isfinite(k2)], self.weights[np.isfinite(k2)]),
                                self.weightedAvgSDSE(edynamic2[np.isfinite(k2)], self.weights[np.isfinite(k2)])],
                               columns=['Average', 'SD', 'SE'], index=['k2', 'Estatic', 'Edynamic1', 'Edynamic2'])
 
         # Save DataFrame in pickle format
         df.to_pickle(output_reweight_prefix + '-data-{:d}-{:d}.pkl'.format(self.residues[0], self.residues[1]))
-        
+
     def reweight(self, **kwargs):
-        
-        """ 
-        
+
+        """
+
         Alias for reweigthing calculations. Call save() function with weights for reweighting.
-        
+
         """
-        
+
         output_reweight_prefix = kwargs.get('reweight_prefix', self.output_prefix)
-        
+
         self.weights = np.genfromtxt(
                 self.output_prefix + '-w_s-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
 
         print(f'Effective fraction of frames contributing to average: {self.fraction_frames()}')
-        
+
         self.save(reweight_prefix=output_reweight_prefix)
-        
-        
+
+
     def run(self, **kwargs):
 
         """
 
         Run FRET Efficiency calculations by calling trajectoryAnalysis() and save data to file.
-        
+
 
         """
 
         # Calculate distribution of <E> (i.e. one <E> for each protein trajectory frame) in Static, Dynamic1, and
         # Dynamic2 regimes.
         self.trajectoryAnalysis()
-            
+
         print(f'Effective fraction of frames contributing to average: {self.fraction_frames()}')
 
         # Calculate k2 distribution and k2, Static, Dynamic1, Dynamic2 averaging. Save data to file.
         self.save()
 
         print('\nDone.')
```

### Comparing `FRETpredict-0.1.2/FRETpredict/R0_calculation.py` & `FRETpredict-0.1.3/FRETpredict/R0_calculation.py`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.2/FRETpredict/lennardjones.py` & `FRETpredict-0.1.3/FRETpredict/lennardjones.py`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.2/FRETpredict/libraries.py` & `FRETpredict-0.1.3/FRETpredict/libraries.py`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.2/FRETpredict/rotamer_libraries.py` & `FRETpredict-0.1.3/FRETpredict/rotamer_libraries.py`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.2/FRETpredict/utils.py` & `FRETpredict-0.1.3/FRETpredict/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,31 +489,31 @@
     def calculate_ws(self):
 
         """ Calculate per-frame weights for reweighting """
 
         Z = np.genfromtxt(self.output_prefix + '-Z-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]),
                           skip_header=-1,
                           skip_footer=0,
-                          delimiter=' ')
+                          delimiter=' ').reshape(-1,2)
 
         Z_s = Z[:, 0] * Z[:, 1]
         w_s = Z_s / np.sum(Z_s)
 
         return w_s
 
     def fraction_frames(self):
 
         """ Compute effective fraction of frames contributing to the averages """
-        
+
         if isinstance(self.weights, np.ndarray):
-        
+
         	w_s = self.weights
-        
+
         elif self.weights == False:
-        
+
         	w_s = np.genfromtxt(
         	self.output_prefix + '-w_s-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
 
         ws_correct = w_s[w_s != 0]
         ws_0 = np.zeros(len(ws_correct))
         ws_0[:] = 1 / len(ws_correct)
```

### Comparing `FRETpredict-0.1.2/FRETpredict.egg-info/PKG-INFO` & `FRETpredict-0.1.3/FRETpredict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRETpredict
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for FRET Efficiency prediction of protein structures and trajectories, based on the Rotamer Library Approach (RLA). Can be installed with pip.
 Home-page: https://github.com/KULL-Centre/FRETpredict
 Author: Daniele Montepietra, Giulio Tesei, João M Martins, Micha BA Kunze, Robert Best and Kresten Lindorff-Larsen
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FRETpredict-0.1.2/LICENSE` & `FRETpredict-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.2/PKG-INFO` & `FRETpredict-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRETpredict
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for FRET Efficiency prediction of protein structures and trajectories, based on the Rotamer Library Approach (RLA). Can be installed with pip.
 Home-page: https://github.com/KULL-Centre/FRETpredict
 Author: Daniele Montepietra, Giulio Tesei, João M Martins, Micha BA Kunze, Robert Best and Kresten Lindorff-Larsen
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FRETpredict-0.1.2/README.md` & `FRETpredict-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.2/setup.py` & `FRETpredict-0.1.3/setup.py`

 * *Files identical despite different names*

