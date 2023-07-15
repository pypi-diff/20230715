# Comparing `tmp/FRETpredict-0.1.3.tar.gz` & `tmp/FRETpredict-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FRETpredict-0.1.3.tar", last modified: Sat Jul 15 15:06:39 2023, max compression
+gzip compressed data, was "FRETpredict-0.1.4.tar", last modified: Sat Jul 15 16:30:19 2023, max compression
```

## Comparing `FRETpredict-0.1.3.tar` & `FRETpredict-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 15:06:39.784108 FRETpredict-0.1.3/
-drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 15:06:39.774966 FRETpredict-0.1.3/FRETpredict/
--rw-r--r--   0 vbr805     (501) staff       (20)    24607 2023-07-15 14:44:17.000000 FRETpredict-0.1.3/FRETpredict/FRET.py
--rw-r--r--   0 vbr805     (501) staff       (20)     3281 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/R0_calculation.py
--rw-r--r--   0 vbr805     (501) staff       (20)      222 2023-07-15 15:06:15.000000 FRETpredict-0.1.3/FRETpredict/__init__.py
--rw-r--r--   0 vbr805     (501) staff       (20)      542 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/lennardjones.py
--rw-r--r--   0 vbr805     (501) staff       (20)     4928 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/libraries.py
--rw-r--r--   0 vbr805     (501) staff       (20)    21351 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/FRETpredict/rotamer_libraries.py
--rw-r--r--   0 vbr805     (501) staff       (20)    18629 2023-07-15 14:40:07.000000 FRETpredict-0.1.3/FRETpredict/utils.py
-drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 15:06:39.782745 FRETpredict-0.1.3/FRETpredict.egg-info/
--rw-r--r--   0 vbr805     (501) staff       (20)     7697 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/PKG-INFO
--rw-r--r--   0 vbr805     (501) staff       (20)      381 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/SOURCES.txt
--rw-r--r--   0 vbr805     (501) staff       (20)        1 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/dependency_links.txt
--rw-r--r--   0 vbr805     (501) staff       (20)      161 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/requires.txt
--rw-r--r--   0 vbr805     (501) staff       (20)       12 2023-07-15 15:06:39.000000 FRETpredict-0.1.3/FRETpredict.egg-info/top_level.txt
--rw-r--r--   0 vbr805     (501) staff       (20)    35149 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/LICENSE
--rw-r--r--   0 vbr805     (501) staff       (20)     7697 2023-07-15 15:06:39.783331 FRETpredict-0.1.3/PKG-INFO
--rw-r--r--   0 vbr805     (501) staff       (20)     6739 2023-02-10 09:59:28.000000 FRETpredict-0.1.3/README.md
--rw-r--r--   0 vbr805     (501) staff       (20)       38 2023-07-15 15:06:39.784168 FRETpredict-0.1.3/setup.cfg
--rwxr-xr-x   0 vbr805     (501) staff       (20)     2228 2023-02-04 20:08:35.000000 FRETpredict-0.1.3/setup.py
+drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 16:30:19.222335 FRETpredict-0.1.4/
+drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 16:30:19.208712 FRETpredict-0.1.4/FRETpredict/
+-rw-r--r--   0 vbr805     (501) staff       (20)    26713 2023-07-15 15:23:51.000000 FRETpredict-0.1.4/FRETpredict/FRET.py
+-rw-r--r--   0 vbr805     (501) staff       (20)     3281 2023-07-15 15:17:30.000000 FRETpredict-0.1.4/FRETpredict/R0_calculation.py
+-rw-r--r--   0 vbr805     (501) staff       (20)      222 2023-07-15 15:28:43.000000 FRETpredict-0.1.4/FRETpredict/__init__.py
+-rw-r--r--   0 vbr805     (501) staff       (20)      542 2023-07-15 15:17:30.000000 FRETpredict-0.1.4/FRETpredict/lennardjones.py
+-rw-r--r--   0 vbr805     (501) staff       (20)     4928 2023-07-15 15:17:31.000000 FRETpredict-0.1.4/FRETpredict/libraries.py
+-rw-r--r--   0 vbr805     (501) staff       (20)    22882 2023-07-15 15:17:31.000000 FRETpredict-0.1.4/FRETpredict/rotamer_libraries.py
+-rw-r--r--   0 vbr805     (501) staff       (20)    18889 2023-07-15 15:21:36.000000 FRETpredict-0.1.4/FRETpredict/utils.py
+drwxr-xr-x   0 vbr805     (501) staff       (20)        0 2023-07-15 16:30:19.220990 FRETpredict-0.1.4/FRETpredict.egg-info/
+-rw-r--r--   0 vbr805     (501) staff       (20)     8384 2023-07-15 16:30:17.000000 FRETpredict-0.1.4/FRETpredict.egg-info/PKG-INFO
+-rw-r--r--   0 vbr805     (501) staff       (20)      381 2023-07-15 16:30:18.000000 FRETpredict-0.1.4/FRETpredict.egg-info/SOURCES.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)        1 2023-07-15 16:30:17.000000 FRETpredict-0.1.4/FRETpredict.egg-info/dependency_links.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)      161 2023-07-15 16:30:17.000000 FRETpredict-0.1.4/FRETpredict.egg-info/requires.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)       12 2023-07-15 16:30:17.000000 FRETpredict-0.1.4/FRETpredict.egg-info/top_level.txt
+-rw-r--r--   0 vbr805     (501) staff       (20)    35149 2023-07-15 15:17:31.000000 FRETpredict-0.1.4/LICENSE
+-rw-r--r--   0 vbr805     (501) staff       (20)     8384 2023-07-15 16:30:19.221690 FRETpredict-0.1.4/PKG-INFO
+-rw-r--r--   0 vbr805     (501) staff       (20)     7426 2023-07-15 15:17:31.000000 FRETpredict-0.1.4/README.md
+-rw-r--r--   0 vbr805     (501) staff       (20)       38 2023-07-15 16:30:19.222425 FRETpredict-0.1.4/setup.cfg
+-rwxr-xr-x   0 vbr805     (501) staff       (20)     2228 2023-07-15 15:17:31.000000 FRETpredict-0.1.4/setup.py
```

### Comparing `FRETpredict-0.1.3/FRETpredict/FRET.py` & `FRETpredict-0.1.4/FRETpredict/FRET.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,14 +75,17 @@
 
         load_file: Bool
             Load data from pre-existing file
 
         weights: numpy.array
             Boltzmann factors distribution
 
+        user_weights: numpy.array
+            User-provided per-frame weights
+
         stdev: float
             Standard deviation
 
 
     Methods
     =======
 
@@ -138,14 +141,15 @@
         self.rmin = -5
         self.rmax = kwargs.get('rmax', 20) * 2 - self.rmin
         self.nr = int(round((self.rmax - self.rmin) / self.dr, 0) + 1)
         self.rax = np.linspace(self.rmin, self.rmax, self.nr)
         self.output_prefix = kwargs.get('output_prefix', 'res')
         self.load_file = kwargs.get('load_file', False)
         self.weights = kwargs.get('weights', False)
+        self.user_weights = kwargs.get('user_weights', None)
         self.stdev = kwargs.get('filter_stdev', 0.02)
 
         # Logging set up
         logging.basicConfig(filename=kwargs.get('log_file', 'log'), level=logging.INFO)
 
         # Write the string for the placement residues selection
         for i in range(2):
@@ -155,15 +159,15 @@
             # If chains are specified, add them to the atom selection
             if type(self.chains[i]) == str:
                 residue_sel += " and segid {:s}".format(self.chains[i])
 
             # Logging information on the selected residues
             logging.info('{:s} = {:s}'.format(residue_sel, self.protein.select_atoms(residue_sel).atoms.resnames[0]))
 
-        # Raise error if the specified placement residues are different than two
+        # Raise error if the specified placement residues are different from two
         if len(residues) != 2:
             raise ValueError("The residue_list must contain exactly 2 "
                              "residue numbers: current value {0}.".format(residues))
 
     def compute_chromophore_vectors(self, rotamersSite1, rotamersSite2):
 
         """
@@ -275,15 +279,14 @@
         donor_producer = temp.match(self.donor).groups()[0]
         acceptor_producer = temp.match(self.acceptor).groups()[0]
 
         donor_number = temp.match(self.donor).groups()[1]
         acceptor_number = temp.match(self.acceptor).groups()[1]
 
         # Read donor spectrum from file and normalize max value to 1
-
         donor_spectrum = pd.read_csv(find_file(f'{donor_producer}{donor_number}.csv',pkglibdir=self.r0lib))
         donor_spectrum[['Emission', 'Excitation']] = donor_spectrum[['Emission', 'Excitation']] / 100
 
         # Read acceptor spectrum from file and normalize max value to 1
         acceptor_spectrum = pd.read_csv(find_file(f'{acceptor_producer}{acceptor_number}.csv',pkglibdir=self.r0lib))
         acceptor_spectrum[['Emission', 'Excitation']] = acceptor_spectrum[['Emission', 'Excitation']] / 100
 
@@ -476,50 +479,80 @@
         # Save <E>_dynamic2 distribution
         np.savetxt(self.output_prefix + '-Ed2-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]), edyn2_avg)
 
     def save(self, **kwargs):
 
         """
 
-        Calculate k2 distribution and k2, Static, Dynamic1, Dynamic2 averaging, with or without reweighting. Save data to file.
+        Calculate k2 distribution and k2, Static, Dynamic1, Dynamic2 averaging, with or without reweighting.    Save data to file.
 
         """
 
         output_reweight_prefix = kwargs.get('reweight_prefix', self.output_prefix)
 
         # Load <k2> distribution from file
         k2 = np.loadtxt(self.output_prefix + '-k2-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
 
-        # Check if weights is an array
-        if isinstance(self.weights, np.ndarray):
+        # Check if user provided per-frame weights
+        # If the user want the average to be unweighted
+        if self.user_weights is None:
 
-            # Check if every k2 instance is associated with one weight
-            if self.weights.size != k2.size:
-                # Warning log
-                logging.info('Weights array has size {} whereas the number of frames is {}'.
-                             format(self.weights.size, k2.size))
+            # Check if weights is an array
+            if isinstance(self.weights, np.ndarray):
 
-                # Raise error
-                raise ValueError('Weights array has size {} whereas the number of frames is {}'.
+                # Check if user_weights size corresponds to the total number of frames
+                if self.weights.size != k2.size:
+
+                    # Warning log
+                    logging.info('Weights array has size {} whereas the number of frames is {}'.
                                  format(self.weights.size, k2.size))
 
-        # If we want the average to be unweighted
-        elif self.weights == False:
+                    # Raise error
+                    raise ValueError('Weights array has size {} whereas the number of frames is {}'.
+                                     format(self.weights.size, k2.size))
 
-            # Associate every k2 instance with a unitary weight
-            self.weights = np.ones(k2.size)
+            # If we want the average to be unweighted
+            elif not self.weights:
 
-        # Other options will raise errors
-        else:
+                # Associate every k2 instance with a unitary weight
+                self.weights = np.ones(k2.size)
+
+        # If the user provided per-frame weights
+        elif self.user_weights is not None:
 
-            # Warning log
-            logging.info('Weights argument should be a numpy array')
+            # Check if user_weights is an array
+            if isinstance(self.user_weights, np.ndarray):
 
-            # Raise error
-            raise ValueError('Weights argument should be a numpy array')
+                # Check if user_weights size corresponds to the total number of frames
+                if self.user_weights.size != k2.size:
+
+                    # Warning log
+                    logging.info('User weights array has size {} whereas the number of frames is {}'.
+                                 format(self.user_weights.size, k2.size))
+
+                    # Raise error
+                    raise ValueError('User weights array has size {} whereas the number of frames is {}'.
+                                     format(self.user_weights.size, k2.size))
+
+                # Obtain dye-protein weights from FRETpredict calculations
+                dye_protein_weights = np.genfromtxt(
+                        self.output_prefix + '-w_s-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
+
+                # Combine dye-protein weights with user provided weights
+                self.weights = (dye_protein_weights * self.user_weights) / np.linalg.norm(
+                        dye_protein_weights * self.user_weights, ord=1)
+
+            # Other options will raise errors
+            else:
+
+                # Warning log
+                logging.info('User weights argument should be a numpy array')
+
+                # Raise error
+                raise ValueError('User weights argument should be a numpy array')
 
         # Read data from H5PY file
         f = h5py.File(self.output_prefix + '-{:d}-{:d}.hdf5'.format(self.residues[0], self.residues[1]), "r")
 
         # Read distribution data from H5PY file
         distributions = f.get('distributions')
 
@@ -554,47 +587,57 @@
 
             df = pd.DataFrame([self.weightedAvgSDSE(k2[np.isfinite(k2)], self.weights[np.isfinite(k2)]),
                                self.weightedAvgSDSE(estatic[np.isfinite(k2)], self.weights[np.isfinite(k2)]),
                                self.weightedAvgSDSE(edynamic1[np.isfinite(k2)], self.weights[np.isfinite(k2)]),
                                self.weightedAvgSDSE(edynamic2[np.isfinite(k2)], self.weights[np.isfinite(k2)])],
                               columns=['Average', 'SD', 'SE'], index=['k2', 'Estatic', 'Edynamic1', 'Edynamic2'])
 
+        print(f'Effective fraction of frames contributing to average: {self.fraction_frames()}')
+
         # Save DataFrame in pickle format
         df.to_pickle(output_reweight_prefix + '-data-{:d}-{:d}.pkl'.format(self.residues[0], self.residues[1]))
 
     def reweight(self, **kwargs):
 
         """
 
-        Alias for reweigthing calculations. Call save() function with weights for reweighting.
+        Alias for reweighting calculations. Call save() function with weights for reweighting.
 
         """
 
         output_reweight_prefix = kwargs.get('reweight_prefix', self.output_prefix)
 
-        self.weights = np.genfromtxt(
+        # User-provided per-frame weights
+        user_weights = kwargs.get('user_weights', None)
+
+        # Dye-protein weights from FRETpredict calculations
+        dye_protein_weights = np.genfromtxt(
                 self.output_prefix + '-w_s-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
 
-        print(f'Effective fraction of frames contributing to average: {self.fraction_frames()}')
+        # Normalized per-frame weights combining dye-protein and user provided weights
+        if user_weights is None:
 
-        self.save(reweight_prefix=output_reweight_prefix)
+            self.weights = dye_protein_weights
 
+        elif user_weights is not None:
 
-    def run(self, **kwargs):
+            self.weights = (dye_protein_weights * user_weights) / np.linalg.norm(dye_protein_weights * user_weights,
+                                                                                 ord=1)
+
+        self.save(reweight_prefix=output_reweight_prefix)
+
+    def run(self):
 
         """
 
         Run FRET Efficiency calculations by calling trajectoryAnalysis() and save data to file.
 
-
         """
 
         # Calculate distribution of <E> (i.e. one <E> for each protein trajectory frame) in Static, Dynamic1, and
         # Dynamic2 regimes.
         self.trajectoryAnalysis()
 
-        print(f'Effective fraction of frames contributing to average: {self.fraction_frames()}')
-
         # Calculate k2 distribution and k2, Static, Dynamic1, Dynamic2 averaging. Save data to file.
         self.save()
 
         print('\nDone.')
```

### Comparing `FRETpredict-0.1.3/FRETpredict/R0_calculation.py` & `FRETpredict-0.1.4/FRETpredict/R0_calculation.py`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.3/FRETpredict/lennardjones.py` & `FRETpredict-0.1.4/FRETpredict/lennardjones.py`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.3/FRETpredict/libraries.py` & `FRETpredict-0.1.4/FRETpredict/libraries.py`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.3/FRETpredict/rotamer_libraries.py` & `FRETpredict-0.1.4/FRETpredict/rotamer_libraries.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import seaborn as sns
 import itertools
 from scipy.signal import find_peaks
 from scipy.cluster.vq import kmeans2
 
 
 class RotamerClusters(object):
-
     """
 
     Calculation of a rotamer library starting from a dye+linker trajectory.
 
     Attributes
     ==========
 
@@ -74,23 +73,31 @@
     """
 
     def __init__(self, **kwargs):
 
         self.libpath = kwargs.get('libpath', 'lib/')
         self.path = kwargs.get('path', 'lib/genLIB2/')
         self.cutoff = kwargs.get('cutoff', [50])
-        self.dye = 'A48_C1R'
+        self.dye = kwargs.get('dye', 'A48_C1R')
         self.df = kwargs.get('df', pd.DataFrame({'indices': [], 'peaks': []}).T)
+        self.traj_extension = kwargs.get('traj_extension', 'xtc')
 
     def calcDihe(self):
 
         """ Calculate dihedral angles on the dye+linker trajectory. """
 
         # Load dye+linker trajectory
-        t = md.load_xtc(self.libpath + self.dye + '/traj.xtc', self.libpath + self.dye + '/conf_ed.gro')
+        if self.traj_extension == 'xtc':
+            t = md.load_xtc(self.libpath + self.dye + '/traj.xtc', self.libpath + self.dye + '/conf_ed.gro')
+
+        if self.traj_extension == 'dcd':
+            t = md.load_dcd(self.libpath + self.dye + '/traj.dcd', self.libpath + self.dye + '/conf_ed.gro')
+
+        elif self.traj_extension == 'pdb':
+            t = md.load_pdb(self.libpath + self.dye + '/traj.pdb')
 
         # Calculate dihedrals from atom indices
         dihe = md.compute_dihedrals(t, self.df.loc[self.dye, 'indices'], periodic=True, opt=True) / np.pi * 180
 
         # Save data to text file
         np.savetxt(self.path + 'dihedrals/' + self.dye + '.txt', dihe)
 
@@ -130,15 +137,16 @@
             # List of peak dihedral angles
             peaks.append(bins[p])
 
         # Do not display the plot
         plt.close(fig)
 
         # Append peak dihedral angles to the dye+linker dataframe
-        self.df.loc[self.dye, 'peaks'] = np.array(peaks)
+
+        self.df.loc[self.dye, 'peaks'] = peaks  # np.array(peaks)
 
     def genClusters(self):
 
         """
 
         1- Generate combinations of dihedral angles from the peaks (cluster centers C1).
 
@@ -252,28 +260,45 @@
         # -2-
         # Load dihedral data from file
         dihedrals = np.loadtxt(self.path + 'dihedrals/' + self.dye + '.txt')
 
         # Dihedral angle values of the remaining cluster centers
         sel_dihe = np.array(clusters.dihe.tolist())
 
-        # Iterate on every frame associated with the discarded cluster centers C2
-        for frame_index, frame_dihe in enumerate(dihedrals[discarded_frames]):
+        # If the number of filtered clusters is zero
+        if len(sel_dihe) == 0:
+
+            # Cannot create a rotamer library with zero clusters
+            print(f'\nNo cluster has population > {cutoff}, so the total number of clusters is 0!')
+
+            raise ValueError
+
+        # If there are no discarded frames
+        elif len(discarded_frames) == 0:
 
-            # Compute square distance of each frame dihedral angle with cluster center C3
-            sqdist = (frame_dihe - sel_dihe) ** 2
+            # Save cluster centers to pickle file
+            clusters.to_pickle(self.path + 'clusters_{:s}_{:d}_cutoff.pkl'.format(self.dye, cutoff))
 
-            # Compute sum of square distances of every dihedral angle for every peak combination
-            sumleastsq = np.sum(sqdist, axis=1)
+        # If there are discarded frames to reassign
+        else:
 
-            # Assign every frame of discarded cluster center to closest cluster center C3
-            clusters.iloc[sumleastsq.argmin()]['N'] += frequency[frame_index]
+            # Iterate on every frame associated with the discarded cluster centers C2
+            for frame_index, frame_dihe in enumerate(dihedrals[discarded_frames]):
 
-        # Save filtered cluster centers to pickle file
-        clusters.to_pickle(self.path + 'clusters_{:s}_{:d}_cutoff.pkl'.format(self.dye, cutoff))
+                # Compute square distance of each frame dihedral angle with cluster center C3
+                sqdist = (frame_dihe - sel_dihe) ** 2
+
+                # Compute sum of square distances of every dihedral angle for every peak combination
+                sumleastsq = np.sum(sqdist, axis=1)
+
+                # Assign every frame of discarded cluster center to closest cluster center C3
+                clusters.iloc[sumleastsq.argmin()]['N'] += frequency[frame_index]
+
+                # Save filtered cluster centers to pickle file
+                clusters.to_pickle(self.path + 'clusters_{:s}_{:d}_cutoff.pkl'.format(self.dye, cutoff))
 
     def genRotLib(self, cutoff):
 
         """
 
         Translate + Rotate C3 cluster centers conformations, and write data to file.
 
@@ -285,15 +310,22 @@
 
         """
 
         # Read C3 clusters data
         clusters = pd.read_pickle(self.path + 'clusters_{:s}_{:d}_cutoff.pkl'.format(self.dye, cutoff))
 
         # Create Universe for the dye+linker trajectory
-        u = MDAnalysis.Universe(self.libpath + self.dye + '/conf_ed.gro', self.libpath + self.dye + '/traj.xtc')
+        if self.traj_extension == 'xtc':
+            u = MDAnalysis.Universe(self.libpath + self.dye + '/conf_ed.gro', self.libpath + self.dye + '/traj.xtc')
+
+        if self.traj_extension == 'dcd':
+            u = MDAnalysis.Universe(self.libpath + self.dye + '/conf_ed.gro', self.libpath + self.dye + '/traj.dcd')
+
+        elif self.traj_extension == 'pdb':
+            u = MDAnalysis.Universe(self.libpath + self.dye + '/traj.pdb')
 
         # Select dye+linker atoms
         chromophore = u.select_atoms('all and not (resname ACE or resname NHE)')
 
         # Write PDB for first frame
         chromophore.write(self.path + 'rot_lib_{:s}.pdb'.format(self.dye))
 
@@ -404,15 +436,15 @@
 
         # Read C3 filtered data from pickle file
         clusters_cutoff = pd.read_pickle(self.path + 'clusters_{:s}_{:d}_cutoff.pkl'.format(self.dye, cutoff))
 
         # Plot
         sns.set_style('darkgrid')
 
-        fig, axes = plt.subplots(nrows=np.round(num_dihedrals/3).astype(int), ncols=3,
+        fig, axes = plt.subplots(nrows=np.round(num_dihedrals / 3).astype(int), ncols=3,
                                  sharex=True, sharey=True, figsize=(9, 6))
 
         for i, ax in enumerate(axes.flatten()):
 
             if i == num_dihedrals:
                 ax.set_visible(False)
                 continue
@@ -428,15 +460,15 @@
             # Vertical lines corresponding to the dihedral peaks
             ax.vlines(self.df.loc[self.dye, 'peaks'][i], ymin=0, ymax=1, color='k')
 
             ax.plot(bins, h, lw=2)
 
             ax.set_ylim(0, h.max() + 0.01)
 
-            ax.set_title("$\chi_" + '{' + f'{i+1}' +'}$')
+            ax.set_title("$\chi_" + '{' + f'{i + 1}' + '}$')
 
         # Set labels and titles
         for i in list(range(2, num_dihedrals, 3)) + list(range(0, num_dihedrals, 3)):
             axes.flatten()[i].set_ylabel(r'$P(\theta)$')
 
         for i in range(0, num_dihedrals):
             axes.flatten()[i].set_xlabel(r'$\theta$ / deg')
@@ -479,15 +511,15 @@
 
         # Read C3 filtered data from pickle file
         clusters_cutoff = pd.read_pickle(self.path + 'clusters_{:s}_{:d}_cutoff.pkl'.format(self.dye, cutoff))
 
         # Plot
         sns.set_style('darkgrid')
 
-        fig, axes = plt.subplots(np.round(num_dihedrals/3).astype(int), 3,
+        fig, axes = plt.subplots(np.round(num_dihedrals / 3).astype(int), 3,
                                  sharex=False, sharey=False, subplot_kw=dict(polar=True), figsize=(9, 7))
 
         for i, ax in enumerate(axes.flatten()):
 
             if i == num_dihedrals:
                 ax.set_visible(False)
                 continue
@@ -505,15 +537,15 @@
                       color='r', lw=0.5, ls=':')
 
             # Plot dihedral distribution in polar graph
             ax.plot((bins + 180) / 180 * np.pi, h, lw=2)
 
             # Plot settings
             ax.set_xticks(np.arange(0, 2 * np.pi, np.pi / 2))
-            ax.set_title("$\chi_" + '{' + f'{i+1}' +'}$')
+            ax.set_title("$\chi_" + '{' + f'{i + 1}' + '}$')
             ax.set_yticks([])
             ax.grid(False)
 
         Nrotamers = len(clusters_cutoff.index)
 
         fig.suptitle(self.dye.replace('_', ' ') + ' cutoff {:d}, {:d} rotamers'.format(cutoff, Nrotamers))
 
@@ -545,16 +577,20 @@
             print("\nGenerating cluster centers...")
             self.genClusters()
 
             # Filter C2 cluster centers for population, generate cluster centers C3,
             # save generated rotamer libraries.
             for _, co in enumerate(self.cutoff):
 
-                print(f"\nFiltering cluster centers...")
-                self.filterCluster(co)
+                try:
+
+                    print(f"\nFiltering cluster centers...")
+                    self.filterCluster(co)
 
-                print("\nGenerating rotamer library...")
-                self.genRotLib(co)
+                    print("\nGenerating rotamer library...")
+                    self.genRotLib(co)
 
-            print('Done.\n')
+                    print('Done.\n')
 
+                except ValueError:
 
+                    print(f'\nCould not generate rotamer library for cutoff {co}')
```

### Comparing `FRETpredict-0.1.3/FRETpredict/utils.py` & `FRETpredict-0.1.4/FRETpredict/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,20 +502,27 @@
 
     def fraction_frames(self):
 
         """ Compute effective fraction of frames contributing to the averages """
 
         if isinstance(self.weights, np.ndarray):
 
-        	w_s = self.weights
+            if np.array_equal(self.weights, np.ones(len(self.protein.trajectory))):
 
-        elif self.weights == False:
+                w_s = np.genfromtxt(
+                    self.output_prefix + '-w_s-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
 
-        	w_s = np.genfromtxt(
-        	self.output_prefix + '-w_s-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
+            else:
+
+                w_s = self.weights
+
+        elif not self.weights:
+
+            w_s = np.genfromtxt(
+                self.output_prefix + '-w_s-{:d}-{:d}.dat'.format(self.residues[0], self.residues[1]))
 
         ws_correct = w_s[w_s != 0]
         ws_0 = np.zeros(len(ws_correct))
         ws_0[:] = 1 / len(ws_correct)
 
         S = - np.sum(ws_correct * np.log(ws_correct / ws_0[ws_0 != 0]))
```

### Comparing `FRETpredict-0.1.3/FRETpredict.egg-info/PKG-INFO` & `FRETpredict-0.1.4/FRETpredict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRETpredict
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for FRET Efficiency prediction of protein structures and trajectories, based on the Rotamer Library Approach (RLA). Can be installed with pip.
 Home-page: https://github.com/KULL-Centre/FRETpredict
 Author: Daniele Montepietra, Giulio Tesei, João M Martins, Micha BA Kunze, Robert Best and Kresten Lindorff-Larsen
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,17 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/fretpredict/badge/?version=latest)](https://fretpredict.readthedocs.io/en/latest/?badge=latest)
 
-FRETpredict
-===========
+<br />
+<p align="left">
+  <img src="FRETpredict_logo.png" width="400" />
 
 Overview
 --------
 
 __[FRETpredict](https://doi.org/10.1101/2023.01.27.525885)__ is a Python package based on the Rotamer Library Approach (RLA) for calculating FRET efficiency based on protein conformational ensembles and MD trajectories.
 
 The FRETpredict class is initialized with (i) a protein structure or trajectory (provided as `MDAnalysis Universe` objects), (ii) the residue indices to which the fluorescent probes are attached, and (iii) the rotamer libraries for the fluorophores and linkers to be used in the calculation.
@@ -55,18 +56,22 @@
 - ATTO 465 C2R + L1R (`T46 C2R`, `T46 L1R`)
 - ATTO 495 C2R + L1R (`T49 C2R`, `T49 L1R`)
 - ATTO 520 C2R + L1R (`T52 C2R`, `T52 L1R`)
 - ATTO 610 C2R + L1R (`T61 C2R`, `T61 L1R`)
 - ATTO 488 C3R (`T48 C3R`)
 - ATTO Thio12 C3R (`Tth C3R`)
 
-- Lumiprobe Cy3 C2R (`C3N C2R`)
+- Lumiprobe Cy3 C2R (`C3N C2R`, `CY3 C2R` from __[HandyFRET](https://karri.anu.edu.au/handy/rl.html)__)
+- Lumiprobe Cy3b C2R (`Cy3b C2R` from __[Klose et al.](https://doi.org/10.1016/j.bpj.2021.09.021)__)
+- Lumiprobe Cy5 C2R (`CY5 C2R` from __[HandyFRET](https://karri.anu.edu.au/handy/rl.html)__)
 - Lumiprobe Cy5.5 C2R + L1R (`C55 C2R`, `C55 L1R`)
 - Lumiprobe Cy7.5 L1R (`C75 L1R`)
 
+- CF 660R C2R (`CF660 C2R` from __[Klose et al.](https://doi.org/10.1016/j.bpj.2021.09.021)__)
+
 In the absence of the exact probes, accurate trends can be predicted by (i) choosing rotamer libraries with similar structural characteristics (linker length, linker dihedrals, fluorophore structure) and (ii) manually setting the $R_0$ for the experimental pair of dyes.
 
 Installation
 ------------
 
 To install FRETpredict, use the [PyPI package](https://pypi.org/project/FRETpredict):
 
@@ -89,14 +94,16 @@
 -------
 
 ```bash
   pip install pytest
 
   python -m pytest
 ```
+The tests reproduce reference data for the following protein systems:
+- Hsp90
 
 Code Example
 ------------
 
 ```python
 
 import MDAnalysis
@@ -119,15 +126,21 @@
 Compute reweighted FRET efficiency based on protein-dye interactions
 
 ```python
 
 FRET.reweight(reweight_prefix='E_pp11_reweighted')
 
 ```
+and combine user-provided weights from previous calculations (e.g., Enhanced sampling simulations)
+
+```python
 
+FRET.reweight(reweight_prefix='E_pp11_reweighted', user_weights=user_weights_pp11)
+
+```
 
 Tutorials
 ---------
 
 - __[Tutorial_FRETpredict_pp11](https://github.com/Monte95/FRETpredict/blob/62ee39e82e82691a237da8e927d686378aff5fb1/tests/tutorials/Tutorial_FRETpredict_pp11.ipynb)__ : Jupyter Notebook with simple tutorials on how to compute the FRET efficiency from the trajectory of a Poliproline 11 (pp11) system.
 
 - __[Generate new rotamer libraries](https://github.com/Monte95/FRETpredict/blob/eef8bf0d219109ada605e943ecc4b1aa9dde86df/tests/tutorials/Tutorial_generate_new_rotamer_libraries.ipynb)__ : Jupyter Notebook on how to create and add new rotamer libraries.
```

### Comparing `FRETpredict-0.1.3/LICENSE` & `FRETpredict-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FRETpredict-0.1.3/PKG-INFO` & `FRETpredict-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRETpredict
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for FRET Efficiency prediction of protein structures and trajectories, based on the Rotamer Library Approach (RLA). Can be installed with pip.
 Home-page: https://github.com/KULL-Centre/FRETpredict
 Author: Daniele Montepietra, Giulio Tesei, João M Martins, Micha BA Kunze, Robert Best and Kresten Lindorff-Larsen
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,17 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/fretpredict/badge/?version=latest)](https://fretpredict.readthedocs.io/en/latest/?badge=latest)
 
-FRETpredict
-===========
+<br />
+<p align="left">
+  <img src="FRETpredict_logo.png" width="400" />
 
 Overview
 --------
 
 __[FRETpredict](https://doi.org/10.1101/2023.01.27.525885)__ is a Python package based on the Rotamer Library Approach (RLA) for calculating FRET efficiency based on protein conformational ensembles and MD trajectories.
 
 The FRETpredict class is initialized with (i) a protein structure or trajectory (provided as `MDAnalysis Universe` objects), (ii) the residue indices to which the fluorescent probes are attached, and (iii) the rotamer libraries for the fluorophores and linkers to be used in the calculation.
@@ -55,18 +56,22 @@
 - ATTO 465 C2R + L1R (`T46 C2R`, `T46 L1R`)
 - ATTO 495 C2R + L1R (`T49 C2R`, `T49 L1R`)
 - ATTO 520 C2R + L1R (`T52 C2R`, `T52 L1R`)
 - ATTO 610 C2R + L1R (`T61 C2R`, `T61 L1R`)
 - ATTO 488 C3R (`T48 C3R`)
 - ATTO Thio12 C3R (`Tth C3R`)
 
-- Lumiprobe Cy3 C2R (`C3N C2R`)
+- Lumiprobe Cy3 C2R (`C3N C2R`, `CY3 C2R` from __[HandyFRET](https://karri.anu.edu.au/handy/rl.html)__)
+- Lumiprobe Cy3b C2R (`Cy3b C2R` from __[Klose et al.](https://doi.org/10.1016/j.bpj.2021.09.021)__)
+- Lumiprobe Cy5 C2R (`CY5 C2R` from __[HandyFRET](https://karri.anu.edu.au/handy/rl.html)__)
 - Lumiprobe Cy5.5 C2R + L1R (`C55 C2R`, `C55 L1R`)
 - Lumiprobe Cy7.5 L1R (`C75 L1R`)
 
+- CF 660R C2R (`CF660 C2R` from __[Klose et al.](https://doi.org/10.1016/j.bpj.2021.09.021)__)
+
 In the absence of the exact probes, accurate trends can be predicted by (i) choosing rotamer libraries with similar structural characteristics (linker length, linker dihedrals, fluorophore structure) and (ii) manually setting the $R_0$ for the experimental pair of dyes.
 
 Installation
 ------------
 
 To install FRETpredict, use the [PyPI package](https://pypi.org/project/FRETpredict):
 
@@ -89,14 +94,16 @@
 -------
 
 ```bash
   pip install pytest
 
   python -m pytest
 ```
+The tests reproduce reference data for the following protein systems:
+- Hsp90
 
 Code Example
 ------------
 
 ```python
 
 import MDAnalysis
@@ -119,15 +126,21 @@
 Compute reweighted FRET efficiency based on protein-dye interactions
 
 ```python
 
 FRET.reweight(reweight_prefix='E_pp11_reweighted')
 
 ```
+and combine user-provided weights from previous calculations (e.g., Enhanced sampling simulations)
+
+```python
 
+FRET.reweight(reweight_prefix='E_pp11_reweighted', user_weights=user_weights_pp11)
+
+```
 
 Tutorials
 ---------
 
 - __[Tutorial_FRETpredict_pp11](https://github.com/Monte95/FRETpredict/blob/62ee39e82e82691a237da8e927d686378aff5fb1/tests/tutorials/Tutorial_FRETpredict_pp11.ipynb)__ : Jupyter Notebook with simple tutorials on how to compute the FRET efficiency from the trajectory of a Poliproline 11 (pp11) system.
 
 - __[Generate new rotamer libraries](https://github.com/Monte95/FRETpredict/blob/eef8bf0d219109ada605e943ecc4b1aa9dde86df/tests/tutorials/Tutorial_generate_new_rotamer_libraries.ipynb)__ : Jupyter Notebook on how to create and add new rotamer libraries.
```

### Comparing `FRETpredict-0.1.3/README.md` & `FRETpredict-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![Documentation Status](https://readthedocs.org/projects/fretpredict/badge/?version=latest)](https://fretpredict.readthedocs.io/en/latest/?badge=latest)
 
-FRETpredict
-===========
+<br />
+<p align="left">
+  <img src="FRETpredict_logo.png" width="400" />
 
 Overview
 --------
 
 __[FRETpredict](https://doi.org/10.1101/2023.01.27.525885)__ is a Python package based on the Rotamer Library Approach (RLA) for calculating FRET efficiency based on protein conformational ensembles and MD trajectories.
 
 The FRETpredict class is initialized with (i) a protein structure or trajectory (provided as `MDAnalysis Universe` objects), (ii) the residue indices to which the fluorescent probes are attached, and (iii) the rotamer libraries for the fluorophores and linkers to be used in the calculation.
@@ -35,18 +36,22 @@
 - ATTO 465 C2R + L1R (`T46 C2R`, `T46 L1R`)
 - ATTO 495 C2R + L1R (`T49 C2R`, `T49 L1R`)
 - ATTO 520 C2R + L1R (`T52 C2R`, `T52 L1R`)
 - ATTO 610 C2R + L1R (`T61 C2R`, `T61 L1R`)
 - ATTO 488 C3R (`T48 C3R`)
 - ATTO Thio12 C3R (`Tth C3R`)
 
-- Lumiprobe Cy3 C2R (`C3N C2R`)
+- Lumiprobe Cy3 C2R (`C3N C2R`, `CY3 C2R` from __[HandyFRET](https://karri.anu.edu.au/handy/rl.html)__)
+- Lumiprobe Cy3b C2R (`Cy3b C2R` from __[Klose et al.](https://doi.org/10.1016/j.bpj.2021.09.021)__)
+- Lumiprobe Cy5 C2R (`CY5 C2R` from __[HandyFRET](https://karri.anu.edu.au/handy/rl.html)__)
 - Lumiprobe Cy5.5 C2R + L1R (`C55 C2R`, `C55 L1R`)
 - Lumiprobe Cy7.5 L1R (`C75 L1R`)
 
+- CF 660R C2R (`CF660 C2R` from __[Klose et al.](https://doi.org/10.1016/j.bpj.2021.09.021)__)
+
 In the absence of the exact probes, accurate trends can be predicted by (i) choosing rotamer libraries with similar structural characteristics (linker length, linker dihedrals, fluorophore structure) and (ii) manually setting the $R_0$ for the experimental pair of dyes.
 
 Installation
 ------------
 
 To install FRETpredict, use the [PyPI package](https://pypi.org/project/FRETpredict):
 
@@ -69,14 +74,16 @@
 -------
 
 ```bash
   pip install pytest
 
   python -m pytest
 ```
+The tests reproduce reference data for the following protein systems:
+- Hsp90
 
 Code Example
 ------------
 
 ```python
 
 import MDAnalysis
@@ -99,15 +106,21 @@
 Compute reweighted FRET efficiency based on protein-dye interactions
 
 ```python
 
 FRET.reweight(reweight_prefix='E_pp11_reweighted')
 
 ```
+and combine user-provided weights from previous calculations (e.g., Enhanced sampling simulations)
+
+```python
 
+FRET.reweight(reweight_prefix='E_pp11_reweighted', user_weights=user_weights_pp11)
+
+```
 
 Tutorials
 ---------
 
 - __[Tutorial_FRETpredict_pp11](https://github.com/Monte95/FRETpredict/blob/62ee39e82e82691a237da8e927d686378aff5fb1/tests/tutorials/Tutorial_FRETpredict_pp11.ipynb)__ : Jupyter Notebook with simple tutorials on how to compute the FRET efficiency from the trajectory of a Poliproline 11 (pp11) system.
 
 - __[Generate new rotamer libraries](https://github.com/Monte95/FRETpredict/blob/eef8bf0d219109ada605e943ecc4b1aa9dde86df/tests/tutorials/Tutorial_generate_new_rotamer_libraries.ipynb)__ : Jupyter Notebook on how to create and add new rotamer libraries.
```

### Comparing `FRETpredict-0.1.3/setup.py` & `FRETpredict-0.1.4/setup.py`

 * *Files identical despite different names*

