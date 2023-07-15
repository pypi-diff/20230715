# Comparing `tmp/promo-1.3.3.tar.gz` & `tmp/promo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promo-1.3.3.tar", last modified: Sat Aug  7 13:58:08 2021, max compression
+gzip compressed data, was "promo-2.0.0.tar", last modified: Sat Jul 15 11:46:49 2023, max compression
```

## Comparing `promo-1.3.3.tar` & `promo-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-07 13:58:08.858016 promo-1.3.3/
--rw-r--r--   0 tmahrt     (501) staff       (20)    12697 2021-08-07 13:58:08.857772 promo-1.3.3/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)    10161 2019-12-08 10:43:56.000000 promo-1.3.3/README.rst
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-07 13:58:08.852050 promo-1.3.3/promo/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:42:48.000000 promo-1.3.3/promo/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    13101 2019-04-30 15:42:48.000000 promo-1.3.3/promo/duration_morph.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     6113 2019-04-30 15:42:48.000000 promo-1.3.3/promo/f0_morph.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-07 13:58:08.857176 promo-1.3.3/promo/morph_utils/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:42:48.000000 promo-1.3.3/promo/morph_utils/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      354 2019-04-30 15:42:48.000000 promo-1.3.3/promo/morph_utils/audio_scripts.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1191 2019-04-30 15:42:48.000000 promo-1.3.3/promo/morph_utils/interpolation.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     5505 2019-04-30 15:42:48.000000 promo-1.3.3/promo/morph_utils/modify_pitch_accent.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    10161 2019-04-30 15:42:48.000000 promo-1.3.3/promo/morph_utils/morph_sequence.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     6769 2020-10-26 14:53:06.000000 promo-1.3.3/promo/morph_utils/plot_morphed_data.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      947 2019-04-30 15:42:48.000000 promo-1.3.3/promo/morph_utils/utils.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-07 13:58:08.854222 promo-1.3.3/promo.egg-info/
--rw-r--r--   0 tmahrt     (501) staff       (20)    12697 2021-08-07 13:58:08.000000 promo-1.3.3/promo.egg-info/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)      466 2021-08-07 13:58:08.000000 promo-1.3.3/promo.egg-info/SOURCES.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        1 2021-08-07 13:58:08.000000 promo-1.3.3/promo.egg-info/dependency_links.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       13 2021-08-07 13:58:08.000000 promo-1.3.3/promo.egg-info/requires.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        6 2021-08-07 13:58:08.000000 promo-1.3.3/promo.egg-info/top_level.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       38 2021-08-07 13:58:08.858101 promo-1.3.3/setup.cfg
--rw-r--r--   0 tmahrt     (501) staff       (20)      737 2021-08-07 13:51:02.000000 promo-1.3.3/setup.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 11:46:49.217203 promo-2.0.0/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1076 2019-04-30 15:42:48.000000 promo-2.0.0/LICENSE
+-rw-r--r--   0 tmahrt     (501) staff       (20)    10114 2023-07-15 11:46:49.216789 promo-2.0.0/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)     9803 2023-07-15 11:42:36.000000 promo-2.0.0/README.rst
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 11:46:49.210251 promo-2.0.0/promo/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:42:48.000000 promo-2.0.0/promo/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    12589 2023-07-15 11:42:36.000000 promo-2.0.0/promo/duration_morph.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     5800 2023-07-15 11:42:36.000000 promo-2.0.0/promo/f0_morph.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 11:46:49.216198 promo-2.0.0/promo/morph_utils/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:42:48.000000 promo-2.0.0/promo/morph_utils/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      346 2023-07-15 11:42:36.000000 promo-2.0.0/promo/morph_utils/audio_scripts.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1143 2023-07-15 11:42:36.000000 promo-2.0.0/promo/morph_utils/interpolation.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     5100 2023-07-15 11:42:36.000000 promo-2.0.0/promo/morph_utils/modify_pitch_accent.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    10134 2023-07-15 11:42:36.000000 promo-2.0.0/promo/morph_utils/morph_sequence.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     7005 2023-07-15 11:42:36.000000 promo-2.0.0/promo/morph_utils/plot_morphed_data.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      851 2023-07-15 11:42:36.000000 promo-2.0.0/promo/morph_utils/utils.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 11:46:49.212809 promo-2.0.0/promo.egg-info/
+-rw-r--r--   0 tmahrt     (501) staff       (20)    10114 2023-07-15 11:46:49.000000 promo-2.0.0/promo.egg-info/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)      474 2023-07-15 11:46:49.000000 promo-2.0.0/promo.egg-info/SOURCES.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        1 2023-07-15 11:46:49.000000 promo-2.0.0/promo.egg-info/dependency_links.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       31 2023-07-15 11:46:49.000000 promo-2.0.0/promo.egg-info/requires.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        6 2023-07-15 11:46:49.000000 promo-2.0.0/promo.egg-info/top_level.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       38 2023-07-15 11:46:49.217391 promo-2.0.0/setup.cfg
+-rw-r--r--   0 tmahrt     (501) staff       (20)      788 2023-07-15 11:42:36.000000 promo-2.0.0/setup.py
```

### Comparing `promo-1.3.3/README.rst` & `promo-2.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 -----------------------
 ProMo (Prosody Morph)
 -----------------------
 
-.. image:: https://travis-ci.org/timmahrt/ProMo.svg?branch=master
+.. image:: https://travis-ci.org/timmahrt/ProMo.svg?branch=main
     :target: https://travis-ci.org/timmahrt/ProMo
 
-.. image:: https://coveralls.io/repos/github/timmahrt/ProMo/badge.svg?branch=master
-    :target: https://coveralls.io/github/timmahrt/ProMo?branch=master
+.. image:: https://coveralls.io/repos/github/timmahrt/ProMo/badge.svg?branch=main
+    :target: https://coveralls.io/github/timmahrt/ProMo?branch=main
     
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg?
    :target: http://opensource.org/licenses/MIT
    
 *Questions?  Comments?  Feedback?  Chat with us on gitter!*
 
 .. image:: https://badges.gitter.im/pythonProMo/Lobby.svg?
@@ -153,61 +153,39 @@
 
 
 Tutorials
 ================
 
 Tutorials for learning about prosody manipulation and how to use ProMo are available.
 
-`Tutorial 1.1: Intro to ProMo <https://nbviewer.jupyter.org/github/timmahrt/ProMo/blob/master/tutorials/tutorial1_1_intro_to_promo.ipynb>`_
+`Tutorial 1.1: Intro to ProMo <https://nbviewer.jupyter.org/github/timmahrt/ProMo/blob/main/tutorials/tutorial1_1_intro_to_promo.ipynb>`_
 
-`Tutorial 1.2: Pitch manipulation tutorial <https://nbviewer.jupyter.org/github/timmahrt/ProMo/blob/master/tutorials/tutorial1_2_pitch_manipulations.ipynb>`_
+`Tutorial 1.2: Pitch manipulation tutorial <https://nbviewer.jupyter.org/github/timmahrt/ProMo/blob/main/tutorials/tutorial1_2_pitch_manipulations.ipynb>`_
 
 
-Major revisions
+Version History
 ================
 
-Ver 1.3 (May 29, 2017)
+*ProMo uses semantic versioning (Major.Minor.Patch)*
 
-- added tutorials
-
-- f0Morph() can now exclude certain regions from the morph process if desired
-
-Ver 1.2 (January 27, 2017)
-
-- added code for reshaping pitch accents (shift alignment, add plateau, or change height)
-
-Ver 1.1 (February 22, 2016)
-
-- f0 morph code for modifying speaker pitch range and average pitch
-
-- (October 20, 2016) Added integration tests with travis CI and coveralls support.
-
-Ver 1.0 (January 19, 2016)
-
-- first public release.
-
-Beta (July 1, 2013)
-
-- first version which was utilized in my dissertation work
+Please view `CHANGELOG.md <https://github.com/timmahrt/promo/blob/main/CHANGELOG.md>` for version history.
 
 
 Requirements
 ==============
 
-``Python 2.7.*`` or above
-
 ``Python 3.3.*`` or above (or below, probably)
 
-My praatIO library is used extensively and can be downloaded 
+My praatIO library is required and can be downloaded
 `here <https://github.com/timmahrt/praatIO>`_
 
-Matplotlib is needed if you want to plot graphs.
+Matplotlib is required if you want to plot graphs.
 `Matplotlib website <http://matplotlib.org/>`_
 
-Scipy is needed if you want to use interpolation--typically if you have stylized
+Scipy is required if you want to use interpolation--typically if you have stylized
 pitch contours (in praat PitchTier format, for example) that you want to use in
 your morphing).
 `Scipy website <http://scipy.org/>`_
 
 Matplotlib and SciPy are non-trivial to install, as they depends on several large
 packages.  You can
 visit their websites for more information.  **I recommend the following instructions to
@@ -232,14 +210,16 @@
 
     python setup.py install
 
 If python is not in your path, you'll need to enter the full path e.g.::
 
 	C:\Python27\python.exe setup.py install
 
+If you are using ``Python 2.x`` or ``Python < 3.7``, you can use `Promo 1.x`.
+
 Usage
 =========
 
 See /examples for example usages
 
 
 Installation
```

### Comparing `promo-1.3.3/promo/duration_morph.py` & `promo-2.0.0/promo/duration_morph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,156 +1,167 @@
-'''
+"""
 Created on Jun 5, 2013
 
 @author: timmahrt
-'''
+"""
 
 import os
 from os.path import join
 import copy
 
-from praatio import tgio
+from praatio import textgrid
 from praatio import praat_scripts
-from praatio import dataio
+from praatio import data_points
+from praatio.utilities import constants
 
 from promo.morph_utils import utils
 from promo.morph_utils import audio_scripts
 from promo.morph_utils import plot_morphed_data
 
 # This value is used to differentiate a praat interval boundary that marks
 # the start of one region and the end of another.
 PRAAT_TIME_DIFF = 0.000001
 
 
 class NoLabeledRegionFoundException(Exception):
-
     def __init__(self, tgFN):
         super(NoLabeledRegionFoundException, self).__init__()
         self.tgFN = tgFN
 
     def __str__(self):
-        return "No labeled region fitting the specified criteria for tg: " + \
-            self.tgFN
+        return "No labeled region fitting the specified criteria for tg: " + self.tgFN
 
 
-def changeDuration(fromWavFN, durationParameters, stepList, outputName,
-                   outputMinPitch, outputMaxPitch, praatEXE):
-    '''
+def changeDuration(
+    fromWavFN,
+    durationParameters,
+    stepList,
+    outputName,
+    outputMinPitch,
+    outputMaxPitch,
+    praatEXE,
+):
+    """
     Uses praat to morph duration in one file to duration in another
 
     Praat uses the PSOLA algorithm
-    '''
+    """
 
     rootPath = os.path.split(fromWavFN)[0]
 
     # Prep output directories
     outputPath = join(rootPath, "duration_resynthesized_wavs")
     utils.makeDir(outputPath)
-    
+
     durationTierPath = join(rootPath, "duration_tiers")
     utils.makeDir(durationTierPath)
 
     fromWavDuration = audio_scripts.getSoundFileDuration(fromWavFN)
 
     durationParameters = copy.deepcopy(durationParameters)
     # Pad any gaps with values of 1 (no change in duration)
-    
+
     # No need to stretch out any pauses at the beginning
     if durationParameters[0][0] != 0:
         tmpVar = (0, durationParameters[0][0] - PRAAT_TIME_DIFF, 1)
         durationParameters.insert(0, tmpVar)
 
     # Or the end
     if durationParameters[-1][1] < fromWavDuration:
-        durationParameters.append((durationParameters[-1][1] + PRAAT_TIME_DIFF,
-                                   fromWavDuration, 1))
+        durationParameters.append(
+            (durationParameters[-1][1] + PRAAT_TIME_DIFF, fromWavDuration, 1)
+        )
 
     # Create the praat script for doing duration manipulation
     for stepAmount in stepList:
         durationPointList = []
         for start, end, ratio in durationParameters:
             percentChange = 1 + (ratio - 1) * stepAmount
             durationPointList.append((start, percentChange))
             durationPointList.append((end, percentChange))
-        
+
         outputPrefix = "%s_%0.3g" % (outputName, stepAmount)
-        durationTierFN = join(durationTierPath,
-                              "%s.DurationTier" % outputPrefix)
+        durationTierFN = join(durationTierPath, "%s.DurationTier" % outputPrefix)
         outputWavFN = join(outputPath, "%s.wav" % outputPrefix)
-        durationTier = dataio.PointObject2D(durationPointList, dataio.DURATION,
-                                            0, fromWavDuration)
+        durationTier = data_points.PointObject2D(
+            durationPointList, constants.DataPointTypes.DURATION, 0, fromWavDuration
+        )
         durationTier.save(durationTierFN)
-        
-        praat_scripts.resynthesizeDuration(praatEXE,
-                                           fromWavFN,
-                                           durationTierFN,
-                                           outputWavFN,
-                                           outputMinPitch, outputMaxPitch)
+
+        praat_scripts.resynthesizeDuration(
+            praatEXE,
+            fromWavFN,
+            durationTierFN,
+            outputWavFN,
+            outputMinPitch,
+            outputMaxPitch,
+        )
 
 
 def getBareParameters(wavFN):
     wavDuration = audio_scripts.getSoundFileDuration(wavFN)
-    return [(0, wavDuration, ''), ]
+    return [
+        (0, wavDuration, ""),
+    ]
 
 
-def getMorphParameters(fromTGFN, toTGFN, tierName,
-                       filterFunc=None, useBlanks=False):
-    '''
+def getMorphParameters(fromTGFN, toTGFN, tierName, filterFunc=None, useBlanks=False):
+    """
     Get intervals for source and target audio files
-    
+
     Use this information to find out how much to stretch/shrink each source
     interval.
-    
+
     The target values are based on the contents of toTGFN.
-    '''
-    
+    """
+
     if filterFunc is None:
         filterFunc = lambda entry: True  # Everything is accepted
-    
-    fromEntryList = utils.getIntervals(fromTGFN, tierName,
-                                       includeUnlabeledRegions=useBlanks)
-    toEntryList = utils.getIntervals(toTGFN, tierName,
-                                     includeUnlabeledRegions=useBlanks)
+
+    fromEntryList = utils.getIntervals(
+        fromTGFN, tierName, includeUnlabeledRegions=useBlanks
+    )
+    toEntryList = utils.getIntervals(
+        toTGFN, tierName, includeUnlabeledRegions=useBlanks
+    )
 
     fromEntryList = [entry for entry in fromEntryList if filterFunc(entry)]
     toEntryList = [entry for entry in toEntryList if filterFunc(entry)]
 
-    assert(len(fromEntryList) == len(toEntryList))
+    assert len(fromEntryList) == len(toEntryList)
 
     durationParameters = []
     for fromEntry, toEntry in zip(fromEntryList, toEntryList):
         fromStart, fromEnd = fromEntry[:2]
         toStart, toEnd = toEntry[:2]
 
         # Praat will ignore a second value appearing at the same time as
         # another so we give each start a tiny offset to distinguish intervals
         # that start and end at the same point
         toStart += PRAAT_TIME_DIFF
         fromStart += PRAAT_TIME_DIFF
-        
+
         ratio = (toEnd - toStart) / float((fromEnd - fromStart))
         durationParameters.append((fromStart, fromEnd, ratio))
-    
+
     return durationParameters
 
 
-def getManipulatedParamaters(tgFN, tierName, modFunc,
-                             filterFunc=None, useBlanks=False):
-    '''
+def getManipulatedParamaters(tgFN, tierName, modFunc, filterFunc=None, useBlanks=False):
+    """
     Get intervals for source and target audio files
-    
+
     Use this information to find out how much to stretch/shrink each source
     interval.
-    
+
     The target values are based on modfunc.
-    '''
-    
-    fromExtractInfo = utils.getIntervals(tgFN, tierName, filterFunc,
-                                         useBlanks)
-    
+    """
+
+    fromExtractInfo = utils.getIntervals(tgFN, tierName, filterFunc, useBlanks)
+
     durationParameters = []
     for fromInfoTuple in fromExtractInfo:
         fromStart, fromEnd = fromInfoTuple[:2]
         toStart, toEnd = modFunc(fromStart), modFunc(fromEnd)
 
         # Praat will ignore a second value appearing at the same time as
         # another so we give each start a tiny offset to distinguish intervals
@@ -162,212 +173,220 @@
 
         ratioTuple = (fromStart, fromEnd, ratio)
         durationParameters.append(ratioTuple)
 
     return durationParameters
 
 
-def outputMorphTextgrids(fromTGFN, durationParameters, stepList,
-                         outputTGName):
-
+def outputMorphTextgrids(fromTGFN, durationParameters, stepList, outputTGName):
     if outputTGName is not None:
         utils.makeDir(os.path.split(outputTGName)[0])
 
     # Create the adjusted textgrids
     if outputTGName is not None:
-        
         for stepFactor in stepList:
-            
-            stepDurationParameters = [(start,
-                                       end,
-                                       1 + (ratio - 1) * stepFactor)
-                                      for start, end, ratio
-                                      in durationParameters]
-            adjustedTG = textgridManipulateDuration(fromTGFN,
-                                                    stepDurationParameters)
-            
+            stepDurationParameters = [
+                (start, end, 1 + (ratio - 1) * stepFactor)
+                for start, end, ratio in durationParameters
+            ]
+            adjustedTG = textgridManipulateDuration(fromTGFN, stepDurationParameters)
+
             outputTGFN = "%s_%0.3g.TextGrid" % (outputTGName, stepFactor)
-            adjustedTG.save(outputTGFN)
+            adjustedTG.save(
+                outputTGFN, format="short_textgrid", includeBlankSpaces=True
+            )
 
 
-def outputMorphPlot(fromTGFN, toTGFN, tierName, durationParameters, stepList,
-                    outputImageFN):
-    
+def outputMorphPlot(
+    fromTGFN, toTGFN, tierName, durationParameters, stepList, outputImageFN
+):
     if outputImageFN is not None:
         utils.makeDir(os.path.split(outputImageFN)[0])
-        
+
     # Create the plot of the morph
     if outputImageFN is not None:
-        _plotResults(durationParameters, fromTGFN, toTGFN,
-                     tierName, stepList, outputImageFN,
-                     None, False)
-
-
-def _plotResults(durationParameters, fromTGFN, toTGFN, tierName,
-                 stepList, outputPNGFN, filterFunc,
-                 includeUnlabeledRegions):
-
+        _plotResults(
+            durationParameters,
+            fromTGFN,
+            toTGFN,
+            tierName,
+            stepList,
+            outputImageFN,
+            None,
+            False,
+        )
+
+
+def _plotResults(
+    durationParameters,
+    fromTGFN,
+    toTGFN,
+    tierName,
+    stepList,
+    outputPNGFN,
+    filterFunc,
+    includeUnlabeledRegions,
+):
     # Containers
     fromDurList = []
     toDurList = []
     actDurList = []
     labelList = []
 
-    fromExtractInfo = utils.getIntervals(fromTGFN, tierName, filterFunc,
-                                         includeUnlabeledRegions)
-    toExtractInfo = utils.getIntervals(toTGFN, tierName, filterFunc,
-                                       includeUnlabeledRegions)
+    fromExtractInfo = utils.getIntervals(
+        fromTGFN, tierName, filterFunc, includeUnlabeledRegions
+    )
+    toExtractInfo = utils.getIntervals(
+        toTGFN, tierName, filterFunc, includeUnlabeledRegions
+    )
 
     # Get durations
     for fromInfoTuple, toInfoTuple in zip(fromExtractInfo, toExtractInfo):
         fromStart, fromEnd = fromInfoTuple[:2]
         toStart, toEnd = toInfoTuple[:2]
 
         labelList.append(fromInfoTuple[2])
         fromDurList.append(fromEnd - fromStart)
         toDurList.append(toEnd - toStart)
 
     # Get iterpolated values
     for stepAmount in stepList:
         tmpDurList = []
         for fromStart, fromEnd, ratio in durationParameters:
-            dur = (fromEnd - fromStart)
+            dur = fromEnd - fromStart
             percentChange = 1 + (ratio - 1) * stepAmount
             tmpDurList.append(dur * percentChange)
 
         actDurList.append(tmpDurList)
 
     # Plot data
-    plot_morphed_data.plotDuration(fromDurList, toDurList, actDurList,
-                                   labelList, outputPNGFN)
+    plot_morphed_data.plotDuration(
+        fromDurList, toDurList, actDurList, labelList, outputPNGFN
+    )
 
 
 def textgridMorphDuration(fromTGFN, toTGFN):
-    '''
+    """
     A convenience function.  Morphs interval durations of one tg to another.
-    
+
     This assumes the two textgrids have the same number of segments.
-    '''
-    fromTG = tgio.openTextgrid(fromTGFN)
-    toTG = tgio.openTextgrid(toTGFN)
-    adjustedTG = tgio.Textgrid()
-
-    for tierName in fromTG.tierNameList:
-        fromTier = fromTG.tierDict[tierName]
-        toTier = toTG.tierDict[tierName]
+    """
+    fromTG = textgrid.openTextgrid(fromTGFN, includeEmptyIntervals=False)
+    toTG = textgrid.openTextgrid(toTGFN, includeEmptyIntervals=False)
+    adjustedTG = textgrid.Textgrid()
+
+    for tierName in fromTG.tierNames:
+        fromTier = fromTG.getTier(tierName)
+        toTier = toTG.getTier(tierName)
         adjustedTier = fromTier.morph(toTier)
         adjustedTG.addTier(adjustedTier)
 
     return adjustedTG
 
 
 def textgridManipulateDuration(tgFN, ratioList):
+    tg = textgrid.openTextgrid(tgFN, includeEmptyIntervals=False)
 
-    tg = tgio.openTextgrid(tgFN)
+    adjustedTG = textgrid.Textgrid()
 
-    adjustedTG = tgio.Textgrid()
+    for tierName in tg.tierNames:
+        fromTier = tg.getTier(tierName)
 
-    for tierName in tg.tierNameList:
-        fromTier = tg.tierDict[tierName]
-        
         adjustedTier = None
-        if isinstance(fromTier, tgio.IntervalTier):
+        if isinstance(fromTier, textgrid.IntervalTier):
             adjustedTier = _morphIntervalTier(fromTier, ratioList)
-        elif isinstance(fromTier, tgio.PointTier):
+        elif isinstance(fromTier, textgrid.PointTier):
             adjustedTier = _morphPointTier(fromTier, ratioList)
-        
-        assert(adjustedTier is not None)
+
+        assert adjustedTier is not None
         adjustedTG.addTier(adjustedTier)
 
     return adjustedTG
 
 
 def _getTimeDiff(start, stop, ratio):
-    '''Returns the time difference between interval and interval*ratio'''
+    """Returns the time difference between interval and interval*ratio"""
     return (ratio - 1) * (stop - start)
 
 
 def _morphPointTier(tier, ratioList):
-    
     cumulativeAdjustAmount = 0
     i = 0
     newEntryList = []
-    for timestamp, label in tier.entryList:
-        
+    for timestamp, label in tier.entries:
         # Advance to the manipulation interval that coincides with the
         # current point or appears after it
         while i < len(ratioList) and timestamp > ratioList[i][1]:
             rStart, rStop, ratio = ratioList[i]
             cumulativeAdjustAmount += _getTimeDiff(rStart, rStop, ratio)
             i += 1
-        
+
         newTime = timestamp + cumulativeAdjustAmount
-        
+
         # Alter the time if the point is within a manipulation interval
         if i < len(ratioList):
             rStart, rStop, ratio = ratioList[i]
             if timestamp > rStart and timestamp <= rStop:
                 newTime += _getTimeDiff(rStart, timestamp, ratio)
-        
+
         newEntryList.append((newTime, label))
-    
+
     maxT = tier.maxTimestamp + cumulativeAdjustAmount
-    return tier.new(entryList=newEntryList, maxTimestamp=maxT)
+    return tier.new(entries=newEntryList, maxTimestamp=maxT)
 
 
 def _morphIntervalTier(tier, ratioList):
-    
     cumulativeAdjustAmount = 0
     i = 0
     newEntryList = []
-    for start, stop, label in tier.entryList:
-        
+    for start, stop, label in tier.entries:
         # Syncronize the manipulation and data intervals so that they
         # are either overlapping or the manipulation interval is farther
         # in the future.  This accumulates the effect of past
         # manipulations so we know how much to offset timestamps
         # for the current interval.
-        while (i < len(ratioList) and start > ratioList[i][0] and
-               start >= ratioList[i][1]):
+        while (
+            i < len(ratioList) and start > ratioList[i][0] and start >= ratioList[i][1]
+        ):
             rStart, rStop, ratio = ratioList[i]
             cumulativeAdjustAmount = _getTimeDiff(rStart, rStop, ratio)
             i += 1
-        
+
         newStart = start + cumulativeAdjustAmount
         newStop = stop + cumulativeAdjustAmount
-        
+
         # Manipulate the interval further if there is overlap with a
         # manipulation interval
         while i < len(ratioList):
             rStart, rStop, ratio = ratioList[i]
-            
+
             # currAdjustAmount is the ratio modified by percent change
             # e.g. if the ratio is a boost of 1.2 but percent change is
             # 0.5, ratio = 1.1 (it loses half of its effect)
-            
+
             # Adjusting the start position based on overlap with the
             # current adjust interval
             if start <= rStart:
                 pass
             elif start > rStart and start <= rStop:
                 newStart += _getTimeDiff(rStart, start, ratio)
-                
+
             # Adjusting the stop position based on overlap with the
             # current adjust interval
             if stop >= rStop:
                 newStop += _getTimeDiff(rStart, rStop, ratio)
             elif stop < rStop and stop >= rStart:
                 newStop += _getTimeDiff(rStart, stop, ratio)
-            
+
             # If we are beyond the current manipulation interval,
             # then we need to move to the next one
             if stop >= rStop:
                 cumulativeAdjustAmount += _getTimeDiff(rStart, rStop, ratio)
                 i += 1
             # Otherwise, we are done manipulating the current interval
             elif stop < rStop:
                 break
-        
+
         newEntryList.append((newStart, newStop, label))
-    
+
     newMax = tier.maxTimestamp + cumulativeAdjustAmount
-    return tier.new(entryList=newEntryList, maxTimestamp=newMax)
+    return tier.new(entries=newEntryList, maxTimestamp=newMax)
```

### Comparing `promo-1.3.3/promo/f0_morph.py` & `promo-2.0.0/promo/f0_morph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,156 +1,177 @@
-'''
+"""
 Created on May 31, 2013
 
 @author: timmahrt
 
 Contains utilities for extracting, creating, and manipulating pitch files in
 praat.
-'''
+"""
 
 from os.path import join
 
-from praatio import tgio
-from praatio import dataio
+from praatio import textgrid
+from praatio import data_points
 from praatio import praat_scripts
 from praatio.utilities import utils as praatio_utils
+from praatio.utilities import constants
 
 from promo.morph_utils import utils
 from promo.morph_utils import audio_scripts
 from promo.morph_utils import plot_morphed_data
 from promo.morph_utils import morph_sequence
 
 
 class MissingPitchDataException(Exception):
-        
     def __str__(self):
-        txt = ("\n\nNo data points available in a region for morphing.\n"
-               "Two data points are needed in each region to do the morph\n"
-               "Regions with fewer than two samples are skipped, which "
-               "should be fine for some cases (e.g. unvoiced segments).\n"
-               "If you need more data points, see "
-               "promo.morph_utils.interpolation")
+        txt = (
+            "\n\nNo data points available in a region for morphing.\n"
+            "Two data points are needed in each region to do the morph\n"
+            "Regions with fewer than two samples are skipped, which "
+            "should be fine for some cases (e.g. unvoiced segments).\n"
+            "If you need more data points, see "
+            "promo.morph_utils.interpolation"
+        )
         return txt
 
 
 def getPitchForIntervals(data, tgFN, tierName):
-    '''
+    """
     Preps data for use in f0Morph
-    '''
-    tg = tgio.openTextgrid(tgFN)
-    data = tg.tierDict[tierName].getValuesInIntervals(data)
+    """
+    tg = textgrid.openTextgrid(tgFN, includeEmptyIntervals=False)
+    data = tg.getTier(tierName).getValuesInIntervals(data)
     data = [dataList for _, dataList in data]
 
     return data
 
 
-def f0Morph(fromWavFN, pitchPath, stepList,
-            outputName, doPlotPitchSteps, fromPitchData, toPitchData,
-            outputMinPitch, outputMaxPitch, praatEXE, keepPitchRange=False,
-            keepAveragePitch=False, sourcePitchDataList=None,
-            minIntervalLength=0.3):
-    '''
+def f0Morph(
+    fromWavFN,
+    pitchPath,
+    stepList,
+    outputName,
+    doPlotPitchSteps,
+    fromPitchData,
+    toPitchData,
+    outputMinPitch,
+    outputMaxPitch,
+    praatEXE,
+    keepPitchRange=False,
+    keepAveragePitch=False,
+    sourcePitchDataList=None,
+    minIntervalLength=0.3,
+):
+    """
     Resynthesizes the pitch track from a source to a target wav file
 
     fromPitchData and toPitchData should be segmented according to the
     portions that you want to morph.  The two lists must have the same
     number of sublists.
 
     Occurs over a three-step process.
 
     This function can act as a template for how to use the function
     morph_sequence.morphChunkedDataLists to morph pitch contours or
     other data.
-    
+
     By default, everything is morphed, but it is possible to maintain elements
     of the original speaker's pitch (average pitch and pitch range) by setting
     the appropriate flag)
-    
+
     sourcePitchDataList: if passed in, any regions unspecified by
                          fromPitchData will be sampled from this list.  In
                          essence, this allows one to leave segments of
                          the original pitch contour untouched by the
                          morph process.
-    '''
+    """
 
     fromDuration = audio_scripts.getSoundFileDuration(fromWavFN)
 
     # Find source pitch samples that will be mixed in with the target
     # pitch samples later
     nonMorphPitchData = []
     if sourcePitchDataList is not None:
         timeList = sorted(fromPitchData)
         timeList = [(row[0][0], row[-1][0]) for row in timeList]
         endTime = sourcePitchDataList[-1][0]
         invertedTimeList = praatio_utils.invertIntervalList(timeList, endTime)
-        invertedTimeList = [(start, stop) for start, stop in invertedTimeList
-                            if stop - start > minIntervalLength]
-        
+        invertedTimeList = [
+            (start, stop)
+            for start, stop in invertedTimeList
+            if stop - start > minIntervalLength
+        ]
+
         for start, stop in invertedTimeList:
-            pitchList = praatio_utils.getValuesInInterval(sourcePitchDataList,
-                                                          start,
-                                                          stop)
+            pitchList = praatio_utils.getValuesInInterval(
+                sourcePitchDataList, start, stop
+            )
             nonMorphPitchData.extend(pitchList)
 
     # Iterative pitch tier data path
     pitchTierPath = join(pitchPath, "pitchTiers")
     resynthesizedPath = join(pitchPath, "f0_resynthesized_wavs")
     for tmpPath in [pitchTierPath, resynthesizedPath]:
         utils.makeDir(tmpPath)
 
     # 1. Prepare the data for morphing - acquire the segments to merge
     # (Done elsewhere, with the input fed into this function)
-    
+
     # 2. Morph the fromData to the toData
     try:
-        finalOutputList = morph_sequence.morphChunkedDataLists(fromPitchData,
-                                                               toPitchData,
-                                                               stepList)
+        finalOutputList = morph_sequence.morphChunkedDataLists(
+            fromPitchData, toPitchData, stepList
+        )
     except IndexError:
         raise MissingPitchDataException()
 
     fromPitchData = [row for subList in fromPitchData for row in subList]
     toPitchData = [row for subList in toPitchData for row in subList]
 
     # 3. Save the pitch data and resynthesize the pitch
     mergedDataList = []
     for i in range(0, len(finalOutputList)):
-        
         outputDataList = finalOutputList[i]
-        
+
         if keepPitchRange is True:
-            outputDataList = morph_sequence.morphRange(outputDataList,
-                                                       fromPitchData)
-            
+            outputDataList = morph_sequence.morphRange(outputDataList, fromPitchData)
+
         if keepAveragePitch is True:
-            outputDataList = morph_sequence.morphAveragePitch(outputDataList,
-                                                              fromPitchData)
-        
+            outputDataList = morph_sequence.morphAveragePitch(
+                outputDataList, fromPitchData
+            )
+
         if sourcePitchDataList is not None:
             outputDataList.extend(nonMorphPitchData)
             outputDataList.sort()
-        
+
         stepOutputName = "%s_%0.3g" % (outputName, stepList[i])
         pitchFNFullPath = join(pitchTierPath, "%s.PitchTier" % stepOutputName)
         outputFN = join(resynthesizedPath, "%s.wav" % stepOutputName)
-        pointObj = dataio.PointObject2D(outputDataList, dataio.PITCH,
-                                        0, fromDuration)
+        pointObj = data_points.PointObject2D(
+            outputDataList, constants.DataPointTypes.PITCH, 0, fromDuration
+        )
         pointObj.save(pitchFNFullPath)
 
         outputTime, outputVals = zip(*outputDataList)
         mergedDataList.append((outputTime, outputVals))
-        
-        praat_scripts.resynthesizePitch(praatEXE, fromWavFN, pitchFNFullPath,
-                                        outputFN, outputMinPitch,
-                                        outputMaxPitch)
+
+        praat_scripts.resynthesizePitch(
+            praatEXE,
+            fromWavFN,
+            pitchFNFullPath,
+            outputFN,
+            outputMinPitch,
+            outputMaxPitch,
+        )
 
     # 4. (Optional) Plot the generated contours
     if doPlotPitchSteps:
-
         fromTime, fromVals = zip(*fromPitchData)
         toTime, toVals = zip(*toPitchData)
 
-        plot_morphed_data.plotF0((fromTime, fromVals),
-                                 (toTime, toVals),
-                                 mergedDataList,
-                                 join(pitchTierPath,
-                                      "%s.png" % outputName))
+        plot_morphed_data.plotF0(
+            (fromTime, fromVals),
+            (toTime, toVals),
+            mergedDataList,
+            join(pitchTierPath, "%s.png" % outputName),
+        )
```

### Comparing `promo-1.3.3/promo/morph_utils/interpolation.py` & `promo-2.0.0/promo/morph_utils/interpolation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-'''
+"""
 Created on Jun 29, 2016
 
 @author: Tim
-'''
+"""
 
 try:
     import numpy as np
 except ImportError:
     hasNumpy = False
 else:
     hasNumpy = True
 
- 
+
 def _numpyCheck():
     if not hasNumpy:
-        raise ImportError("Numpy required to do data interpolation. "
-                          "Install numpy or don't use data interpolation")
+        raise ImportError(
+            "Numpy required to do data interpolation. "
+            "Install numpy or don't use data interpolation"
+        )
 
 
-def quadraticInterpolation(valueList2d, numDegrees, n,
-                           startTime=None, endTime=None):
-    '''
+def quadraticInterpolation(valueList2d, numDegrees, n, startTime=None, endTime=None):
+    """
     Generates a series of points on a smooth curve that cross the given points
-    
+
     numDegrees - the degrees of the fitted polynomial
                - the curve gets weird if this value is too high for the input
     n - number of points to output
     startTime/endTime/n - n points will be generated at evenly spaced
                           intervals between startTime and endTime
-    '''
+    """
     _numpyCheck()
-    
+
     x, y = zip(*valueList2d)
-    
+
     if startTime is None:
         startTime = x[0]
     if endTime is None:
         endTime = x[-1]
-    
+
     polyFunc = np.poly1d(np.polyfit(x, y, numDegrees))
-    
+
     newX = np.linspace(startTime, endTime, n)
-    
+
     retList = [(n, polyFunc(n)) for n in newX]
-    
+
     return retList
```

### Comparing `promo-1.3.3/promo/morph_utils/modify_pitch_accent.py` & `promo-2.0.0/promo/morph_utils/modify_pitch_accent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 Created on Jan 26, 2017
 
 This convenience code that makes it easy to manipulate
 characteristics of a pitch accent.  It is flexible in how
 it is used (on a stylized pitch contour or raw values and
 as a single step or in a piecewise manner).
 
@@ -11,153 +11,150 @@
 NOTE: By pitch accent, I mean a single hill or peak, surrounded
 by less intense values to the left and right.  Some of the
 functions make reference to the max value in the dataset, so if you
 have multiple peaks or a downward slope, etc. you may get strange
 results.
 
 @author: Tim
-'''
+"""
 import copy
-    
-    
+
+
 def _deletePoints(f0List, start, end):
-    return [(timeV, f0V) for timeV, f0V in f0List
-            if timeV < start or timeV > end]
+    return [(timeV, f0V) for timeV, f0V in f0List if timeV < start or timeV > end]
 
 
 class PitchAccent(object):
-    
     def __init__(self, pointList):
-        
+
         self.pointList = copy.deepcopy(pointList)
-        
+
         self.netLeftShift = 0
         self.netRightShift = 0
-        
+
         pitchList = [f0V for _, f0V in self.pointList]
         minV = min(pitchList)
         maxV = max(pitchList)
-        
+
         self.peakI = pitchList.index(maxV)
-    
+
         timeList = [timeV for timeV, _ in self.pointList]
         self.minT = min(timeList)
         self.maxT = max(timeList)
-    
-    
+
     def adjustPeakHeight(self, heightAmount):
-        '''
+        """
         Adjust peak height
-        
+
         The foot of the accent is left unchanged and intermediate
         values are linearly scaled
-        '''
+        """
         if heightAmount == 0:
             return
-        
+
         pitchList = [f0V for _, f0V in self.pointList]
         minV = min(pitchList)
         maxV = max(pitchList)
         scale = lambda x, y: x + y * (x - minV) / float(maxV - minV)
-        
-        self.pointList = [(timeV, scale(f0V, heightAmount))
-                          for timeV, f0V in self.pointList]
-    
+
+        self.pointList = [
+            (timeV, scale(f0V, heightAmount)) for timeV, f0V in self.pointList
+        ]
+
     def addPlateau(self, plateauAmount, pitchSampFreq=None):
-        '''
+        """
         Add a plateau
-        
+
         A negative plateauAmount will move the peak backwards.
         A positive plateauAmount will move the peak forwards.
-        
+
         All points on the side of the peak growth will also get moved.
         i.e. the slope of the peak does not change.  The accent gets
         wider instead.
-        
+
         If pitchSampFreq=None, the plateau will only be specified by
         the start and end points of the plateau
-        '''
+        """
         if plateauAmount == 0:
             return
-        
+
         maxPoint = self.pointList[self.peakI]
-        
+
         # Define the plateau
         if pitchSampFreq is not None:
             numSteps = abs(int(plateauAmount / pitchSampFreq))
-            timeChangeList = [stepV * pitchSampFreq
-                              for stepV in
-                              range(0, numSteps + 1)]
+            timeChangeList = [stepV * pitchSampFreq for stepV in range(0, numSteps + 1)]
         else:
-            timeChangeList = [plateauAmount, ]
-            
+            timeChangeList = [
+                plateauAmount,
+            ]
+
         # Shift the side being pushed by the plateau
         if plateauAmount < 0:  # Plateau moves left of the peak
-            leftSide = self.pointList[:self.peakI]
-            rightSide = self.pointList[self.peakI:]
-            
-            plateauPoints = [(maxPoint[0] + timeChange, maxPoint[1])
-                             for timeChange in timeChangeList]
-            leftSide = [(timeV + plateauAmount, f0V)
-                        for timeV, f0V in leftSide]
+            leftSide = self.pointList[: self.peakI]
+            rightSide = self.pointList[self.peakI :]
+
+            plateauPoints = [
+                (maxPoint[0] + timeChange, maxPoint[1]) for timeChange in timeChangeList
+            ]
+            leftSide = [(timeV + plateauAmount, f0V) for timeV, f0V in leftSide]
             self.netLeftShift += plateauAmount
-            
+
         elif plateauAmount > 0:  # Plateau moves right of the peak
-            leftSide = self.pointList[:self.peakI + 1]
-            rightSide = self.pointList[self.peakI + 1:]
-            
-            plateauPoints = [(maxPoint[0] + timeChange, maxPoint[1])
-                             for timeChange in timeChangeList]
-            rightSide = [(timeV + plateauAmount, f0V)
-                         for timeV, f0V in rightSide]
+            leftSide = self.pointList[: self.peakI + 1]
+            rightSide = self.pointList[self.peakI + 1 :]
+
+            plateauPoints = [
+                (maxPoint[0] + timeChange, maxPoint[1]) for timeChange in timeChangeList
+            ]
+            rightSide = [(timeV + plateauAmount, f0V) for timeV, f0V in rightSide]
             self.netRightShift += plateauAmount
-        
+
         self.pointList = leftSide + plateauPoints + rightSide
-                   
+
     def shiftAccent(self, shiftAmount):
-        '''
+        """
         Move the whole accent earlier or later
-        '''
+        """
         if shiftAmount == 0:
             return
-        
-        self.pointList = [(time + shiftAmount, pitch)
-                          for time, pitch in self.pointList]
-        
+
+        self.pointList = [(time + shiftAmount, pitch) for time, pitch in self.pointList]
+
         # Update shift amounts
         if shiftAmount < 0:
             self.netLeftShift += shiftAmount
         elif shiftAmount >= 0:
             self.netRightShift += shiftAmount
-    
+
     def deleteOverlapping(self, targetList):
-        '''
+        """
         Erase points from another list that overlap with points in this list
-        '''
+        """
         start = self.pointList[0][0]
         stop = self.pointList[-1][0]
-        
+
         if self.netLeftShift < 0:
             start += self.netLeftShift
-            
+
         if self.netRightShift > 0:
             stop += self.netRightShift
-            
+
         targetList = _deletePoints(targetList, start, stop)
-        
+
         return targetList
-    
+
     def reintegrate(self, fullPointList):
-        '''
+        """
         Integrates the pitch values of the accent into a larger pitch contour
-        '''
+        """
         # Erase the original region of the accent
         fullPointList = _deletePoints(fullPointList, self.minT, self.maxT)
-        
+
         # Erase the new region of the accent
         fullPointList = self.deleteOverlapping(fullPointList)
-        
+
         # Add the accent into the full pitch list
         outputPointList = fullPointList + self.pointList
         outputPointList.sort()
-        
+
         return outputPointList
```

### Comparing `promo-1.3.3/promo/morph_utils/morph_sequence.py` & `promo-2.0.0/promo/morph_utils/morph_sequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 Created on Sep 18, 2013
 
 @author: timmahrt
 
 Given two lists of tuples of the form [(value, time), (value, time)], morph
 can iteratively transform the values in one list to the values in the other
 while maintaining the times in the first list.
@@ -12,153 +12,168 @@
 occur at the same relative location (half way through, at the end, etc.).
 
 Both dynamic time warping and morph, align two data lists in time.  However,
 dynamic time warping does this by analyzing the event structure and aligning
 events in the two signals as best it can
 (i.e. it changes when events happen in relative time while morph preserves
 when events happen in relative time).
-'''
+"""
 
 
 class RelativizeSequenceException(Exception):
-
     def __init__(self, dist):
         super(RelativizeSequenceException, self).__init__()
         self.dist = dist
 
     def __str__(self):
-        return "You need at least two unique values to make " + \
-            "a sequence relative. Input: %s" % repr(self.dist)
+        return (
+            "You need at least two unique values to make "
+            + "a sequence relative. Input: %s" % repr(self.dist)
+        )
 
 
 def makeSequenceRelative(absVSequence):
-    '''
+    """
     Puts every value in a list on a continuum between 0 and 1
 
     Also returns the min and max values (to reverse the process)
-    '''
+    """
 
     if len(absVSequence) < 2 or len(set(absVSequence)) == 1:
         raise RelativizeSequenceException(absVSequence)
 
     minV = min(absVSequence)
     maxV = max(absVSequence)
     relativeSeq = [(value - minV) / (maxV - minV) for value in absVSequence]
 
     return relativeSeq, minV, maxV
 
 
 def makeSequenceAbsolute(relVSequence, minV, maxV):
-    '''
+    """
     Makes every value in a sequence absolute
-    '''
+    """
 
     return [(value * (maxV - minV)) + minV for value in relVSequence]
 
 
 def _makeTimingRelative(absoluteDataList):
-    '''
+    """
     Given normal pitch tier data, puts the times on a scale from 0 to 1
 
     Input is a list of tuples of the form
     ([(time1, pitch1), (time2, pitch2),...]
 
     Also returns the start and end time so that the process can be reversed
-    '''
+    """
 
     timingSeq = [row[0] for row in absoluteDataList]
     valueSeq = [list(row[1:]) for row in absoluteDataList]
 
     relTimingSeq, startTime, endTime = makeSequenceRelative(timingSeq)
-    
-    relDataList = [tuple([time, ] + row) for time, row
-                   in zip(relTimingSeq, valueSeq)]
+
+    relDataList = [
+        tuple(
+            [
+                time,
+            ]
+            + row
+        )
+        for time, row in zip(relTimingSeq, valueSeq)
+    ]
 
     return relDataList, startTime, endTime
 
 
 def _makeTimingAbsolute(relativeDataList, startTime, endTime):
-    '''
+    """
     Maps values from 0 to 1 to the provided start and end time
 
     Input is a list of tuples of the form
     ([(time1, pitch1), (time2, pitch2),...]
-    '''
+    """
 
     timingSeq = [row[0] for row in relativeDataList]
     valueSeq = [list(row[1:]) for row in relativeDataList]
-    
+
     absTimingSeq = makeSequenceAbsolute(timingSeq, startTime, endTime)
 
-    absDataList = [tuple([time, ] + row) for time, row
-                   in zip(absTimingSeq, valueSeq)]
+    absDataList = [
+        tuple(
+            [
+                time,
+            ]
+            + row
+        )
+        for time, row in zip(absTimingSeq, valueSeq)
+    ]
 
     return absDataList
 
 
 def _getSmallestDifference(inputList, targetVal):
-    '''
+    """
     Returns the value in inputList that is closest to targetVal
-    
+
     Iteratively splits the dataset in two, so it should be pretty fast
-    '''
+    """
     targetList = inputList[:]
     retVal = None
     while True:
         # If we're down to one value, stop iterating
         if len(targetList) == 1:
             retVal = targetList[0]
             break
         halfPoint = int(len(targetList) / 2.0) - 1
         a = targetList[halfPoint]
         b = targetList[halfPoint + 1]
-        
+
         leftDiff = abs(targetVal - a)
         rightDiff = abs(targetVal - b)
-        
+
         # If the distance is 0, stop iterating, the targetVal is present
         # in the inputList
         if leftDiff == 0 or rightDiff == 0:
             retVal = targetVal
             break
-        
+
         # Look at left half or right half
         if leftDiff < rightDiff:
-            targetList = targetList[:halfPoint + 1]
+            targetList = targetList[: halfPoint + 1]
         else:
-            targetList = targetList[halfPoint + 1:]
-         
+            targetList = targetList[halfPoint + 1 :]
+
     return retVal
-        
-    
+
+
 def _getNearestMappingIndexList(fromValList, toValList):
-    '''
+    """
     Finds the indicies for data points that are closest to each other.
 
     The inputs should be in relative time, scaled from 0 to 1
     e.g. if you have [0, .1, .5., .9] and [0, .1, .2, 1]
     will output [0, 1, 1, 2]
-    '''
+    """
 
     indexList = []
     for fromTimestamp in fromValList:
         smallestDiff = _getSmallestDifference(toValList, fromTimestamp)
         i = toValList.index(smallestDiff)
         indexList.append(i)
 
     return indexList
 
 
 def morphDataLists(fromList, toList, stepList):
-    '''
+    """
     Iteratively morph fromList into toList using the values 0 to 1 in stepList
-    
+
     stepList: a value of 0 means no change and a value of 1 means a complete
     change to the other value
-    '''
+    """
 
     # If there are more than 1 pitch value, then we align the data in
     # relative time.
     # Each data point comes with a timestamp.  The earliest timestamp is 0
     # and the latest timestamp is 1.  Using this method, for each relative
     # timestamp in the source list, we find the closest relative timestamp
     # in the target list.  Just because two pitch values have the same index
@@ -184,118 +199,120 @@
 
             # i + 1 b/c i_0 = 0 = no change
             newValue = fromValue + (stepAmount * (toValue - fromValue))
             newTime = fromTime + (stepAmount * (toTime - fromTime))
 
             newPitchList.append((newTime, newValue))
 
-        newPitchList = _makeTimingAbsolute(newPitchList, fromStartTime,
-                                           fromEndTime)
+        newPitchList = _makeTimingAbsolute(newPitchList, fromStartTime, fromEndTime)
 
         yield stepAmount, newPitchList
 
 
 def morphChunkedDataLists(fromDataList, toDataList, stepList):
-    '''
+    """
     Morph one set of data into another, in a stepwise fashion
 
     A convenience function.  Given a set of paired data lists,
     this will morph each one individually.
 
     Returns a single list with all data combined together.
-    '''
+    """
 
-    assert(len(fromDataList) == len(toDataList))
+    assert len(fromDataList) == len(toDataList)
 
     # Morph the fromDataList into the toDataList
     outputList = []
     for x, y in zip(fromDataList, toDataList):
 
         # We cannot morph a region if there is no data or only
         # a single data point for either side
         if (len(x) < 2) or (len(y) < 2):
             continue
 
-        tmpList = [outputPitchList for _, outputPitchList
-                   in morphDataLists(x, y, stepList)]
+        tmpList = [
+            outputPitchList for _, outputPitchList in morphDataLists(x, y, stepList)
+        ]
         outputList.append(tmpList)
 
     # Transpose list
     finalOutputList = outputList.pop(0)
     for subList in outputList:
         for i, subsubList in enumerate(subList):
             finalOutputList[i].extend(subsubList)
 
     return finalOutputList
 
 
 def morphAveragePitch(fromDataList, toDataList):
-    '''
+    """
     Adjusts the values in fromPitchList to have the same average as toPitchList
-    
+
     Because other manipulations can alter the average pitch, morphing the pitch
     is the last pitch manipulation that should be done
-    
+
     After the morphing, the code removes any values below zero, thus the
     final average might not match the target average.
-    '''
-    
+    """
+
     timeList, fromPitchList = zip(*fromDataList)
     toPitchList = [pitchVal for _, pitchVal in toDataList]
-    
+
     # Zero pitch values aren't meaningful, so filter them out if they are
     # in the dataset
     fromListNoZeroes = [val for val in fromPitchList if val > 0]
     fromAverage = sum(fromListNoZeroes) / float(len(fromListNoZeroes))
-    
+
     toListNoZeroes = [val for val in toPitchList if val > 0]
     toAverage = sum(toListNoZeroes) / float(len(toListNoZeroes))
-    
+
     newPitchList = [val - fromAverage + toAverage for val in fromPitchList]
-    
-#     finalAverage = sum(newPitchList) / float(len(newPitchList))
-    
+
+    #     finalAverage = sum(newPitchList) / float(len(newPitchList))
+
     # Removing zeroes and negative pitch values
-    retDataList = [(time, pitchVal) for time, pitchVal
-                   in zip(timeList, newPitchList)
-                   if pitchVal > 0]
-    
+    retDataList = [
+        (time, pitchVal)
+        for time, pitchVal in zip(timeList, newPitchList)
+        if pitchVal > 0
+    ]
+
     return retDataList
 
 
 def morphRange(fromDataList, toDataList):
-    '''
+    """
     Changes the scale of values in one distribution to that of another
-    
+
     ie The maximum value in fromDataList will be set to the maximum value in
     toDataList.  The 75% largest value in fromDataList will be set to the
     75% largest value in toDataList, etc.
-    
+
     Small sample sizes will yield results that are not very meaningful
-    '''
-    
+    """
+
     # Isolate and sort pitch values
     fromPitchList = [dataTuple[1] for dataTuple in fromDataList]
     toPitchList = [dataTuple[1] for dataTuple in toDataList]
-    
+
     fromPitchListSorted = sorted(fromPitchList)
     toPitchListSorted = sorted(toPitchList)
-    
+
     # Bin pitch values between 0 and 1
     fromListRel = makeSequenceRelative(fromPitchListSorted)[0]
     toListRel = makeSequenceRelative(toPitchListSorted)[0]
-    
+
     # Find each values closest equivalent in the other list
     indexList = _getNearestMappingIndexList(fromListRel, toListRel)
-    
+
     # Map the source pitch to the target pitch value
     # Pitch value -> get sorted position -> get corresponding position in
     # target list -> get corresponding pitch value = the new pitch value
     retList = []
     for time, pitch in fromDataList:
         fromI = fromPitchListSorted.index(pitch)
         toI = indexList[fromI]
         newPitch = toPitchListSorted[toI]
-        
+
         retList.append((time, newPitch))
-    
+
     return retList
```

### Comparing `promo-1.3.3/promo/morph_utils/plot_morphed_data.py` & `promo-2.0.0/promo/morph_utils/plot_morphed_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,133 @@
-'''
+"""
 Created on Sep 18, 2013
 
 @author: timmahrt
-'''
+"""
 
 import math
 
 try:
     import matplotlib.pyplot as plt
     import matplotlib.cm as cm
 except ImportError:
     hasMatplotlib = False
 else:
     hasMatplotlib = True
 
- 
+
 def _matplotlibCheck():
     if not hasMatplotlib:
-        raise ImportError("Matplotlib required to generate plots. "
-                          "Install matplotlib or disable plotting")
+        raise ImportError(
+            "Matplotlib required to generate plots. "
+            "Install matplotlib or disable plotting"
+        )
 
 
 def plotSinglePitchTrack(fromTuple, fnFullPath):
     _matplotlibCheck()
 
     fig, (ax0) = plt.subplots(nrows=1)
 
     # Old data
-    plot1 = ax0.plot(fromTuple, color='red', linewidth=2,
-                     )
+    plot1 = ax0.plot(
+        fromTuple,
+        color="red",
+        linewidth=2,
+    )
 
-    plt.ylabel('Pitch (Hz)')
-    plt.xlabel('Sample number')
+    plt.ylabel("Pitch (Hz)")
+    plt.xlabel("Sample number")
 
-    plt.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
-#     plt.legend([plot1, plot2, plot3], ["From", "To", "Merged line"])
+    plt.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.0)
+    #     plt.legend([plot1, plot2, plot3], ["From", "To", "Merged line"])
 
-    plt.savefig(fnFullPath, dpi=300, bbox_inches='tight')
+    plt.savefig(fnFullPath, dpi=300, bbox_inches="tight")
     plt.close(fig)
 
 
 def plotTwoPitchTracks(fromTuple, toTuple, fnFullPath):
     _matplotlibCheck()
 
     fig, (ax0, ax1) = plt.subplots(nrows=2)
 
     # Old data
-    plot1 = ax0.plot(fromTuple, color='red', linewidth=2,
-                     # label="From"
-                     )
+    plot1 = ax0.plot(
+        fromTuple,
+        color="red",
+        linewidth=2,
+        # label="From"
+    )
     ax0.set_title("Mary is going to the mall (statement)")
 
-    plot2 = ax1.plot(toTuple, color='red', linewidth=2,
-                     # label="From"
-                     )
+    plot2 = ax1.plot(
+        toTuple,
+        color="red",
+        linewidth=2,
+        # label="From"
+    )
 
     ax1.set_title("Mary is going to the mall (question)")
 
-    plt.ylabel('Pitch (Hz)')
-    plt.xlabel('Sample number')
+    plt.ylabel("Pitch (Hz)")
+    plt.xlabel("Sample number")
 
-    plt.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
-#     plt.legend([plot1, plot2, plot3], ["From", "To", "Merged line"])
+    plt.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.0)
+    #     plt.legend([plot1, plot2, plot3], ["From", "To", "Merged line"])
 
-    plt.savefig(fnFullPath, dpi=300, bbox_inches='tight')
+    plt.savefig(fnFullPath, dpi=300, bbox_inches="tight")
     plt.close(fig)
 
 
 def plotF0(fromTuple, toTuple, mergeTupleList, fnFullPath):
-    '''
+    """
     Plots the original data in a graph above the plot of the dtw'ed data
-    '''
+    """
     _matplotlibCheck()
 
     fig, (ax0) = plt.subplots(nrows=1)
 
     # Old data
-    plot1 = ax0.plot(fromTuple[0], fromTuple[1], color='red',
-                     linewidth=2, label="From")
-    plot2 = ax0.plot(toTuple[0], toTuple[1], color='blue',
-                     linewidth=2, label="To")
+    plot1 = ax0.plot(fromTuple[0], fromTuple[1], color="red", linewidth=2, label="From")
+    plot2 = ax0.plot(toTuple[0], toTuple[1], color="blue", linewidth=2, label="To")
     ax0.set_title("Plot of F0 Morph")
-    plt.ylabel('Pitch (hz)')
-    plt.xlabel('Time (s)')
+    plt.ylabel("Pitch (hz)")
+    plt.xlabel("Time (s)")
 
     # Merge data
     colorValue = 0
     colorStep = 255.0 / len(mergeTupleList)
     for timeList, valueList in mergeTupleList:
         colorValue += colorStep
         hexValue = "#%02x0000" % int(255 - colorValue)
         if int(colorValue) == 255:
-            ax0.plot(timeList, valueList, color=hexValue, linewidth=1,
-                     label="Merged line, final iteration")
+            ax0.plot(
+                timeList,
+                valueList,
+                color=hexValue,
+                linewidth=1,
+                label="Merged line, final iteration",
+            )
         else:
             ax0.plot(timeList, valueList, color=hexValue, linewidth=1)
 
-    plt.legend(loc=1, borderaxespad=0.)
-#     plt.legend([plot1, plot2, plot3], ["From", "To", "Merged line"])
+    plt.legend(loc=1, borderaxespad=0.0)
+    #     plt.legend([plot1, plot2, plot3], ["From", "To", "Merged line"])
 
-    plt.savefig(fnFullPath, dpi=300, bbox_inches='tight')
+    plt.savefig(fnFullPath, dpi=300, bbox_inches="tight")
     plt.close(fig)
 
 
-def plotIntensity(fromDataList, toDataList, mergeTupleList,
-                  controlPoints, fnFullPath):
-
+def plotIntensity(fromDataList, toDataList, mergeTupleList, controlPoints, fnFullPath):
     def mag2DB(valueList):
         stepSize = 500
 
         returnList = []
         for i in range(int(math.ceil(len(valueList) / float(stepSize)))):
-            subList = valueList[i * stepSize:(i + 1) * stepSize]
+            subList = valueList[i * stepSize : (i + 1) * stepSize]
             value = math.sqrt(sum([val ** 2 for val in subList]))
 
             returnList.append(20.0 * math.log10(value))
 
         return returnList
 
     _matplotlibCheck()
@@ -123,26 +135,26 @@
     fromDataList = mag2DB(fromDataList)
     toDataList = mag2DB(toDataList)
 
     print(max(fromDataList))
     print(max(toDataList))
 
     fig, ax0 = plt.subplots(nrows=1)
-#     fig, (ax0, ax1, ax2) = plt.subplots(nrows=3)
+    #     fig, (ax0, ax1, ax2) = plt.subplots(nrows=3)
 
     # Old data
-    plot1 = ax0.plot(fromDataList, color='red', linewidth=2, label="From")
-#     plot1.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
+    plot1 = ax0.plot(fromDataList, color="red", linewidth=2, label="From")
+    #     plot1.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
 
-    plot2 = ax0.plot(toDataList, color='blue', linewidth=2, label="To")
-#     plot2.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
+    plot2 = ax0.plot(toDataList, color="blue", linewidth=2, label="To")
+    #     plot2.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
 
     ax0.set_title("Plot of Intensity Morph")
-    plt.ylabel('RMS intensity (db)')
-    plt.xlabel('Time (s)')
+    plt.ylabel("RMS intensity (db)")
+    plt.xlabel("Time (s)")
 
     # Merge data
 
     colorValue = 0
     colorStep = 255.0 / len(mergeTupleList)
     for valueList in mergeTupleList:
 
@@ -150,86 +162,111 @@
 
         print(max(valueList))
 
         colorValue += colorStep
         hexValue = "#%02x0000" % int(255 - colorValue)
         xValues = [i for i in range(len(valueList))]
         if colorValue == 255.0:
-            plot3 = ax0.plot(xValues, valueList, color=hexValue, linewidth=1,
-                             label="Merged line")
+            plot3 = ax0.plot(
+                xValues, valueList, color=hexValue, linewidth=1, label="Merged line"
+            )
         else:
             plot3 = ax0.plot(xValues, valueList, color=hexValue, linewidth=1)
 
     controlPoints = mag2DB(controlPoints)
     xValues = [i for i in range(len(controlPoints))]
-    ax0.scatter(xValues, controlPoints, color='pink', label="Control points")
+    ax0.scatter(xValues, controlPoints, color="pink", label="Control points")
 
-    plt.legend(loc=1,
-               # bbox_to_anchor=(1.05, 1), loc=2,
-               borderaxespad=0.)
+    plt.legend(
+        loc=1,
+        # bbox_to_anchor=(1.05, 1), loc=2,
+        borderaxespad=0.0,
+    )
 
-    plt.savefig(fnFullPath, dpi=300, bbox_inches='tight')
+    plt.savefig(fnFullPath, dpi=300, bbox_inches="tight")
     plt.close(fig)
 
 
-def plotDuration(fromDurationList, toDurationList, resultDataList,
-                 labelList, fnFullPath):
+def plotDuration(
+    fromDurationList, toDurationList, resultDataList, labelList, fnFullPath
+):
 
     _matplotlibCheck()
 
-    dataList = [fromDurationList, ] + resultDataList + [toDurationList, ]
+    dataList = (
+        [
+            fromDurationList,
+        ]
+        + resultDataList
+        + [
+            toDurationList,
+        ]
+    )
 
     # Sanity check
     for subList in dataList:
-        assert(len(subList) == len(fromDurationList))
+        assert len(subList) == len(fromDurationList)
 
     # Constants
-    colorTuple = ['red', 'yellow', 'blue']
+    colorTuple = ["red", "yellow", "blue"]
     width = 0.2
     n = len(dataList)
     iterN = range(n)
 
     # Pre-plotting work
     fig, ax0 = plt.subplots(nrows=1)
 
     # Labels
     ax0.set_title("Plot of Duration Morph")
-    plt.ylabel('Duration (s)')
-    plt.xlabel('Iterations')
-    plt.title('Duration morph')
+    plt.ylabel("Duration (s)")
+    plt.xlabel("Iterations")
+    plt.title("Duration morph")
 
     # Draw x ticks (iteration numbers)
     xLabelList = []
     for i in range(len(resultDataList)):
         xLabelList.append(str(i + 1))  # 1 based
 
-    xLabelList = ["From", ] + xLabelList + ["To", ]
+    xLabelList = (
+        [
+            "From",
+        ]
+        + xLabelList
+        + [
+            "To",
+        ]
+    )
     iterN2 = [val + width / 2.0 for val in iterN]
     plt.xticks(iterN2, xLabelList)
 
     # Plot the data
     transposedList = zip(*dataList)
     bottom = [0 for i in iterN]
     for i, row in enumerate(transposedList):
 
         # Horizontal line that sits on the tallest column
         ax0.axhline(bottom[0], color="black")
 
         # Word label that appears after the final column
         bottomAppend = max(row)
-        ax0.text(n - 1.0 + 0.5, (bottom[0] + (bottomAppend / 3.0)),
-                 labelList[i])
+        ax0.text(n - 1.0 + 0.5, (bottom[0] + (bottomAppend / 3.0)), labelList[i])
 
         # The column data
-        ax0.bar(x=iterN, height=row, bottom=bottom, width=width,
-                alpha=0.6, color=colorTuple[i % 3])
+        ax0.bar(
+            x=iterN,
+            height=row,
+            bottom=bottom,
+            width=width,
+            alpha=0.6,
+            color=colorTuple[i % 3],
+        )
 
         # Update the start positions for the next iteration
 
         bottom = [origBottom + bottomAppend for origBottom in bottom]
 
     # Draw a final horizontal line over the highest column
     ax0.axhline(bottom[0], color="black")
 
     # Save and cleanup
-    plt.savefig(fnFullPath, dpi=300, bbox_inches='tight')
+    plt.savefig(fnFullPath, dpi=300, bbox_inches="tight")
     plt.close(fig)
```

### Comparing `promo-1.3.3/promo/morph_utils/utils.py` & `promo-2.0.0/promo/morph_utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-'''
+"""
 Created on Apr 2, 2015
 
 @author: tmahrt
-'''
+"""
 
 import os
 
-from praatio import tgio
+from praatio import textgrid
 
 
-def getIntervals(fn, tierName, filterFunc=None,
-                 includeUnlabeledRegions=False):
-    '''
+def getIntervals(fn, tierName, filterFunc=None, includeUnlabeledRegions=False):
+    """
     Get information about the 'extract' tier, used by several merge scripts
-    '''
+    """
 
-    tg = tgio.openTextgrid(fn)
-    
-    tier = tg.tierDict[tierName]
-    if includeUnlabeledRegions is True:
-        tier = tgio._fillInBlanks(tier)
+    tg = textgrid.openTextgrid(fn, includeEmptyIntervals=includeUnlabeledRegions)
 
-    entryList = tier.entryList
+    tier = tg.getTier(tierName)
+
+    entries = tier.entries
     if filterFunc is not None:
-        entryList = [entry for entry in entryList if filterFunc(entry)]
+        entries = [entry for entry in entries if filterFunc(entry)]
 
-    return entryList
+    return entries
 
 
 def makeDir(path):
-    
     if not os.path.exists(path):
         os.mkdir(path)
-        
+
 
 def generateStepList(numSteps, includeZero=False):
-    
-    assert(numSteps > 0)
-    
+    assert numSteps > 0
+
     stepList = []
     if includeZero:
         stepList.append(0)
-        
+
     for i in range(numSteps):
         stepList.append((i + 1) / float((numSteps)))
-        
+
     return stepList
```

### Comparing `promo-1.3.3/setup.py` & `promo-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 @author: tmahrt
 """
 from setuptools import setup
 import io
 
 setup(
     name="promo",
-    version="1.3.3",
+    python_requires=">3.6.0",
+    version="2.0.0",
     author="Tim Mahrt",
     author_email="timmahrt@gmail.com",
     url="https://github.com/timmahrt/ProMo",
     package_dir={"promo": "promo"},
     packages=["promo", "promo.morph_utils"],
     license="LICENSE",
-    install_requires=["praatio ~= 4.1"],
+    install_requires=["praatio ~= 6.0", "typing_extensions"],
     description=(
         "Library for manipulating pitch and duration in an "
         "algorithmic way, for resynthesizing speech"
     ),
     long_description=io.open("README.rst", "r", encoding="utf-8").read(),
     #       install_requires=[], # No requirements! # requires 'from setuptools import setup'
 )
```

