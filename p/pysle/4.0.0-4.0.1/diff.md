# Comparing `tmp/pysle-4.0.0.tar.gz` & `tmp/pysle-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysle-4.0.0.tar", last modified: Mon Jan  3 13:52:01 2022, max compression
+gzip compressed data, was "pysle-4.0.1.tar", last modified: Sat Jul 15 15:16:19 2023, max compression
```

## Comparing `pysle-4.0.0.tar` & `pysle-4.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2022-01-03 13:52:01.537586 pysle-4.0.0/
--rw-r--r--   0 tmahrt     (501) staff       (20)     1366 2022-01-03 13:51:00.000000 pysle-4.0.0/LICENSE
--rw-r--r--   0 tmahrt     (501) staff       (20)     6796 2022-01-03 13:52:01.537712 pysle-4.0.0/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)     6416 2022-01-03 13:51:04.000000 pysle-4.0.0/README.md
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2022-01-03 13:52:01.498940 pysle-4.0.0/pysle/
--rw-r--r--   0 tmahrt     (501) staff       (20)     1279 2022-01-03 13:51:00.000000 pysle-4.0.0/pysle/__init__.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2022-01-03 13:52:01.501519 pysle-4.0.0/pysle/data/
--rw-r--r--   0 tmahrt     (501) staff       (20) 13662144 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/data/ISLEdict.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)    14932 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/isletool.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    27168 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/phonetics.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    15570 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/praattools.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     3187 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/pronunciationtools.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2022-01-03 13:52:01.537340 pysle-4.0.0/pysle/utilities/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/utilities/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      681 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/utilities/constants.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     5094 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/utilities/errors.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2224 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/utilities/isle_io.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1672 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/utilities/phonetic_constants.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     8793 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/utilities/search.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1861 2022-01-03 13:51:04.000000 pysle-4.0.0/pysle/utilities/utils.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2022-01-03 13:52:01.501111 pysle-4.0.0/pysle.egg-info/
--rw-r--r--   0 tmahrt     (501) staff       (20)     6796 2022-01-03 13:52:00.000000 pysle-4.0.0/pysle.egg-info/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)      506 2022-01-03 13:52:00.000000 pysle-4.0.0/pysle.egg-info/SOURCES.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        1 2022-01-03 13:52:00.000000 pysle-4.0.0/pysle.egg-info/dependency_links.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       31 2022-01-03 13:52:00.000000 pysle-4.0.0/pysle.egg-info/requires.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        6 2022-01-03 13:52:00.000000 pysle-4.0.0/pysle.egg-info/top_level.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       73 2022-01-03 13:52:01.538233 pysle-4.0.0/setup.cfg
--rw-r--r--   0 tmahrt     (501) staff       (20)      862 2022-01-03 13:51:04.000000 pysle-4.0.0/setup.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 15:16:19.062258 pysle-4.0.1/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1366 2022-01-03 13:51:00.000000 pysle-4.0.1/LICENSE
+-rw-r--r--   0 tmahrt     (501) staff       (20)     6397 2023-07-15 15:16:19.062560 pysle-4.0.1/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)     6017 2023-07-15 15:13:35.000000 pysle-4.0.1/README.md
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 15:16:18.862996 pysle-4.0.1/pysle/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1279 2022-01-03 13:51:00.000000 pysle-4.0.1/pysle/__init__.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 15:16:18.867125 pysle-4.0.1/pysle/data/
+-rw-r--r--   0 tmahrt     (501) staff       (20) 13662144 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/data/ISLEdict.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)    14920 2023-07-15 15:13:35.000000 pysle-4.0.1/pysle/isletool.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    27168 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/phonetics.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    15449 2023-07-15 15:13:35.000000 pysle-4.0.1/pysle/praattools.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3187 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/pronunciationtools.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 15:16:19.061380 pysle-4.0.1/pysle/utilities/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/utilities/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      681 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/utilities/constants.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     5094 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/utilities/errors.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2224 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/utilities/isle_io.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1672 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/utilities/phonetic_constants.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8793 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/utilities/search.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1861 2022-01-03 13:51:04.000000 pysle-4.0.1/pysle/utilities/utils.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 15:16:18.866266 pysle-4.0.1/pysle.egg-info/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     6397 2023-07-15 15:16:11.000000 pysle-4.0.1/pysle.egg-info/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)      506 2023-07-15 15:16:11.000000 pysle-4.0.1/pysle.egg-info/SOURCES.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        1 2023-07-15 15:16:11.000000 pysle-4.0.1/pysle.egg-info/dependency_links.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       31 2023-07-15 15:16:11.000000 pysle-4.0.1/pysle.egg-info/requires.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        6 2023-07-15 15:16:11.000000 pysle-4.0.1/pysle.egg-info/top_level.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       73 2023-07-15 15:16:19.064575 pysle-4.0.1/setup.cfg
+-rw-r--r--   0 tmahrt     (501) staff       (20)      862 2023-07-15 15:13:35.000000 pysle-4.0.1/setup.py
```

### Comparing `pysle-4.0.0/LICENSE` & `pysle-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/PKG-INFO` & `pysle-4.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysle
-Version: 4.0.0
+Version: 4.0.1
 Summary: An interface to ISLEX, an IPA pronunciation dictionary for English with stress and syllable markings.
 Home-page: https://github.com/timmahrt/pysle
 Author: Tim Mahrt
 Author-email: timmahrt@gmail.com
 License: LICENSE
 Platform: UNKNOWN
 Requires-Python: >3.6.0
@@ -32,41 +32,40 @@
 # Table of contents
 1. [Documentation](#documentation)
 2. [Tutorials](#tutorials)
 3. [Version History](#version-history)
 4. [Requirements](#requirements)
 5. [ISLE Dictionary](#isle-dictionary)
 6. [Installation](#installation)
-7. [Version 3 to 4 Migration](#version-3-to-4-migration)
+7. [Upgrading](#upgrading)
 8. [Usage](#usage)
 9. [Common Use Cases](#common-use-cases)
 10. [Tests](#tests)
 11. [Citing psyle](#citing-pysle)
 12. [Acknowledgements](#acknowledgements)
 
 
 ## Documentation
 
 Automatically generated pdocs can be found here:
 
 http://timmahrt.github.io/pysle/
 
-The documentation is generated with the following command:
-`pdoc ./pysle -d google -o docs`
-
 ## Tutorials
 
 There are tutorials available for learning how to use Pysle.  These
 are in the form of IPython Notebooks which can be found in the /tutorials/
 folder distributed with Pysle.
 
 You can view them online using the external website Jupyter:
 
 [Tutorial 1: Introduction to Pysle](<https://nbviewer.jupyter.org/github/timmahrt/pysle/blob/main/tutorials/tutorial1_intro_to_pysle.ipynb>)
 
+[Tutorial 2: Pronunciationtools](<https://nbviewer.jupyter.org/github/timmahrt/pysle/blob/main/tutorials/tutorial2_pronunciationtools.ipynb>)
+
 ## Version History
 
 *Pysle uses semantic versioning (Major.Minor.Patch)*
 
 Please view [CHANGELOG.md](https://github.com/timmahrt/pysle/blob/main/CHANGELOG.md) for version history.
 
 
@@ -109,24 +108,17 @@
 
     python setup.py install
 
 If python is not in your path, you'll need to enter the full path e.g.
 
     C:\Python36\python.exe setup.py install
 
-## Version 3 to 4 Migration
-
-The iterface to isle dictionaries, praattools, and pronunciationtools haven't changed so
-much except for a bit of renaming.
-
-The expected return types have completely changed however--shifting to datatypes now defined
-in `phonetics.py`. If you are struggling with migrating to version 4, please let me know.
+## Upgrading
 
-Looking over changes to the example files may help show the changes that need to be made
-to get the same results.
+Please view [UPGRADING.md](https://github.com/timmahrt/pysle/blob/main/UPGRADING.md) for detailed information about how to upgrade from earlier versions.
 
 ## Usage
 
 Here is a typical usage
 
 ```python
 from pysle import isletool
@@ -174,21 +166,14 @@
 
 - automatically syllabify a praat textgrid (see [praatIO](<https://github.com/timmahrt/praatIO>))
    containing words and phones (e.g. force-aligned text)
     ```python
     pysle.syllabifyTextgrid(isleDict, praatioTextgrid, "words", "phones")
     ```
 
-## Tests
-
-I run tests with the following command (this requires pytest and pytest-cov to be installed):
-
-`pytest --cov=pysle tests/`
-
-
 ## Citing pysle
 
 
 Pysle is general purpose coding and doesn't need to be cited
 (you should cite the
 [ISLEX project](<http://www.isle.illinois.edu/speech_web_lg/data/g2ps/>)
 instead) but if you would like to, it can be cited like so:
```

### Comparing `pysle-4.0.0/README.md` & `pysle-4.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,41 +19,40 @@
 # Table of contents
 1. [Documentation](#documentation)
 2. [Tutorials](#tutorials)
 3. [Version History](#version-history)
 4. [Requirements](#requirements)
 5. [ISLE Dictionary](#isle-dictionary)
 6. [Installation](#installation)
-7. [Version 3 to 4 Migration](#version-3-to-4-migration)
+7. [Upgrading](#upgrading)
 8. [Usage](#usage)
 9. [Common Use Cases](#common-use-cases)
 10. [Tests](#tests)
 11. [Citing psyle](#citing-pysle)
 12. [Acknowledgements](#acknowledgements)
 
 
 ## Documentation
 
 Automatically generated pdocs can be found here:
 
 http://timmahrt.github.io/pysle/
 
-The documentation is generated with the following command:
-`pdoc ./pysle -d google -o docs`
-
 ## Tutorials
 
 There are tutorials available for learning how to use Pysle.  These
 are in the form of IPython Notebooks which can be found in the /tutorials/
 folder distributed with Pysle.
 
 You can view them online using the external website Jupyter:
 
 [Tutorial 1: Introduction to Pysle](<https://nbviewer.jupyter.org/github/timmahrt/pysle/blob/main/tutorials/tutorial1_intro_to_pysle.ipynb>)
 
+[Tutorial 2: Pronunciationtools](<https://nbviewer.jupyter.org/github/timmahrt/pysle/blob/main/tutorials/tutorial2_pronunciationtools.ipynb>)
+
 ## Version History
 
 *Pysle uses semantic versioning (Major.Minor.Patch)*
 
 Please view [CHANGELOG.md](https://github.com/timmahrt/pysle/blob/main/CHANGELOG.md) for version history.
 
 
@@ -96,24 +95,17 @@
 
     python setup.py install
 
 If python is not in your path, you'll need to enter the full path e.g.
 
     C:\Python36\python.exe setup.py install
 
-## Version 3 to 4 Migration
-
-The iterface to isle dictionaries, praattools, and pronunciationtools haven't changed so
-much except for a bit of renaming.
-
-The expected return types have completely changed however--shifting to datatypes now defined
-in `phonetics.py`. If you are struggling with migrating to version 4, please let me know.
+## Upgrading
 
-Looking over changes to the example files may help show the changes that need to be made
-to get the same results.
+Please view [UPGRADING.md](https://github.com/timmahrt/pysle/blob/main/UPGRADING.md) for detailed information about how to upgrade from earlier versions.
 
 ## Usage
 
 Here is a typical usage
 
 ```python
 from pysle import isletool
@@ -161,21 +153,14 @@
 
 - automatically syllabify a praat textgrid (see [praatIO](<https://github.com/timmahrt/praatIO>))
    containing words and phones (e.g. force-aligned text)
     ```python
     pysle.syllabifyTextgrid(isleDict, praatioTextgrid, "words", "phones")
     ```
 
-## Tests
-
-I run tests with the following command (this requires pytest and pytest-cov to be installed):
-
-`pytest --cov=pysle tests/`
-
-
 ## Citing pysle
 
 
 Pysle is general purpose coding and doesn't need to be cited
 (you should cite the
 [ISLEX project](<http://www.isle.illinois.edu/speech_web_lg/data/g2ps/>)
 instead) but if you would like to, it can be cited like so:
```

### Comparing `pysle-4.0.0/pysle/__init__.py` & `pysle-4.0.1/pysle/__init__.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/data/ISLEdict.txt` & `pysle-4.0.1/pysle/data/ISLEdict.txt`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/isletool.py` & `pysle-4.0.1/pysle/isletool.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
         """
         phoneCount = 0.0
         syllableCount = 0.0
 
         syllableCountList = []
         phoneCountList = []
 
-        entryList = self.lookup(word)
-        for entry in entryList:
+        entries = self.lookup(word)
+        for entry in entries:
             syllableList = []
             phoneList = []
             for syllabification in entry.syllabificationList:
                 syllableList.extend(syllabification.syllables)
                 phoneList.extend(syllabification.desyllabify().phonemes)
 
             syllableCountList.append(len(syllableList))
@@ -249,34 +249,34 @@
 
         if preference:
             utils.validateOption("preference", preference, constants.LengthOptions)
 
         transcribedWordsList: List[phonetics.PhonemeList] = []
         wordList = sentenceTxt.split(" ")
         for word in wordList:
-            entryList = self.lookup(word)
+            entries = self.lookup(word)
 
             phoneListsOrderedByEntry = [
                 syllabification.desyllabify()
-                for entry in entryList
+                for entry in entries
                 for syllabification in entry.syllabificationList
             ]
             numPhones = [len(phoneList) for phoneList in phoneListsOrderedByEntry]
 
             i = 0
             if preference == constants.LengthOptions.SHORTEST:
                 i = numPhones.index(min(numPhones))
             elif preference == constants.LengthOptions.LONGEST:
                 i = numPhones.index(max(numPhones))
 
             transcribedWordsList.append(phoneListsOrderedByEntry[i])
 
         def cleanPron(pron):
-            for val in [u"ˈ", u"ˌ", u" "]:
-                pron = pron.replace(val, u"")
+            for val in ["ˈ", "ˌ", " "]:
+                pron = pron.replace(val, "")
             return pron
 
         words: List[str] = [
             " ".join(phoneList.phonemes) for phoneList in transcribedWordsList
         ]
         words = [cleanPron(phones) for phones in words]
```

### Comparing `pysle-4.0.0/pysle/phonetics.py` & `pysle-4.0.1/pysle/phonetics.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/praattools.py` & `pysle-4.0.1/pysle/praattools.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,33 +80,33 @@
 
     Returns:
         a modified version of the input textgrid with the word segmented
 
     Raises:
         WordNotInIsleError: The word was not in the Isle dictionary
     """
-    utteranceTier = tg.tierDict[utteranceTierName]
+    utteranceTier = tg.getTier(utteranceTierName)
 
     wordTier = None
-    if wordTierName in tg.tierNameList:
-        wordTier = tg.tierDict[wordTierName]
+    if wordTierName in tg.tierNames:
+        wordTier = tg.getTier(wordTierName)
 
     # Load in the word tier, if it exists:
-    wordEntryList = []
-    phoneEntryList = []
+    wordEntries = []
+    phoneEntries = []
     if wordTier is not None:
         if removeOverlappingSegments:
-            for start, stop, _ in utteranceTier.entryList:
+            for start, stop, _ in utteranceTier.entries:
                 wordTier = wordTier.eraseRegion(
                     start, stop, praatioConstants.EraseCollision.TRUNCATE, False
                 )
-        wordEntryList = wordTier.entryList
+        wordEntries = wordTier.entries
 
     # Do the naive alignment
-    for start, stop, label in utteranceTier.entryList:
+    for start, stop, label in utteranceTier.entries:
         wordList = label.split()
 
         # Get the list of phones in each word
         superPhoneList: List[List[str]] = []
         numPhones = 0
         i = 0
         while i < len(wordList):
@@ -118,50 +118,50 @@
                 continue
             superPhoneList.append(entry.phonemeList.phonemes)
             numPhones += len(entry.phonemeList.phonemes)
             i += 1
 
         # Get the naive alignment for words, if alignment doesn't
         # already exist for words
-        subWordEntryList = []
-        subPhoneEntryList = []
+        subWordEntries = []
+        subPhoneEntries = []
         if wordTier is not None:
-            subWordEntryList = wordTier.crop(
+            subWordEntries = wordTier.crop(
                 start, stop, praatioConstants.CropCollision.TRUNCATED, False
-            ).entryList
+            ).entries
 
-        if len(subWordEntryList) == 0:
+        if len(subWordEntries) == 0:
             wordStart = start
             phoneDur = (stop - start) / float(numPhones)
             for i, word in enumerate(wordList):
                 phoneListTxt = " ".join(superPhoneList[i])
                 wordEnd = wordStart + (phoneDur * len(superPhoneList[i]))
-                subWordEntryList.append((wordStart, wordEnd, word))
-                subPhoneEntryList.append((wordStart, wordEnd, phoneListTxt))
+                subWordEntries.append((wordStart, wordEnd, word))
+                subPhoneEntries.append((wordStart, wordEnd, phoneListTxt))
                 wordStart = wordEnd
 
-        wordEntryList.extend(subWordEntryList)
-        phoneEntryList.extend(subPhoneEntryList)
+        wordEntries.extend(subWordEntries)
+        phoneEntries.extend(subPhoneEntries)
 
     # Replace or add the word tier
     newWordTier = textgrid.IntervalTier(
-        wordTierName, wordEntryList, tg.minTimestamp, tg.maxTimestamp
+        wordTierName, wordEntries, tg.minTimestamp, tg.maxTimestamp
     )
     if wordTier is not None:
         tg.replaceTier(wordTierName, newWordTier)
     else:
         tg.addTier(newWordTier)
 
     # Add the phone tier
     # This is mainly used as an annotation tier
-    if phoneHelperTierName is not None and len(phoneEntryList) > 0:
+    if phoneHelperTierName is not None and len(phoneEntries) > 0:
         newPhoneTier = textgrid.IntervalTier(
-            phoneHelperTierName, phoneEntryList, tg.minTimestamp, tg.maxTimestamp
+            phoneHelperTierName, phoneEntries, tg.minTimestamp, tg.maxTimestamp
         )
-        if phoneHelperTierName in tg.tierNameList:
+        if phoneHelperTierName in tg.tierNames:
             tg.replaceTier(phoneHelperTierName, newPhoneTier)
         else:
             tg.addTier(newPhoneTier)
 
     return tg
 
 
@@ -188,68 +188,66 @@
 
     Returns:
         a modified version of the input textgrid with the word segmented
 
     Raises:
         WordNotInIsleError: The word was not in the Isle dictionary
     """
-    wordTier = tg.tierDict[wordTierName]
+    wordTier = tg.getTier(wordTierName)
 
     phoneTier = None
-    if phoneTierName in tg.tierNameList:
-        phoneTier = tg.tierDict[phoneTierName]
+    if phoneTierName in tg.tierNames:
+        phoneTier = tg.getTier(phoneTierName)
 
     # Load in the phone tier, if it exists:
-    phoneEntryList = []
+    phoneEntries = []
     if phoneTier is not None:
         if removeOverlappingSegments:
-            for startT, stopT, _ in wordTier.entryList:
+            for startT, stopT, _ in wordTier.entries:
                 phoneTier = phoneTier.eraseRegion(
                     startT, stopT, praatioConstants.EraseCollision.TRUNCATE, False
                 )
-        phoneEntryList = phoneTier.entryList
+        phoneEntries = phoneTier.entries
 
     # Do the naive alignment
-    for wordStartT, wordEndT, word in wordTier.entryList:
-
+    for wordStartT, wordEndT, word in wordTier.entries:
         # Get the list of phones in this word
         try:
             entry = isle.lookup(word)[0]
         except errors.WordNotInIsleError:
             continue
 
         phones = entry.phonemeList.stripDiacritics().phonemes
 
         # Get the naive alignment for phones, if alignment doesn't
         # already exist for phones
-        subPhoneEntryList = []
+        subPhoneEntries = []
         if phoneTier is not None:
-            subPhoneEntryList = phoneTier.crop(
+            subPhoneEntries = phoneTier.crop(
                 wordStartT, wordEndT, praatioConstants.CropCollision.TRUNCATED, False
-            ).entryList
+            ).entries
 
-        if len(subPhoneEntryList) == 0:
+        if len(subPhoneEntries) == 0:
             phoneDur = (wordEndT - wordStartT) / len(phones)
 
             phoneStartT = wordStartT
             for phone in phones:
                 phoneEndT = phoneStartT + phoneDur
-                subPhoneEntryList.append((phoneStartT, phoneEndT, phone))
+                subPhoneEntries.append((phoneStartT, phoneEndT, phone))
                 phoneStartT = phoneEndT
 
-        phoneEntryList.extend(subPhoneEntryList)
+        phoneEntries.extend(subPhoneEntries)
 
     # Replace or add the phone tier
     newPhoneTier = textgrid.IntervalTier(
-        phoneTierName, phoneEntryList, tg.minTimestamp, tg.maxTimestamp
+        phoneTierName, phoneEntries, tg.minTimestamp, tg.maxTimestamp
     )
     if phoneTier is not None:
         tg.replaceTier(phoneTierName, newPhoneTier)
     else:
-
         tg.addTier(newPhoneTier)
 
     return tg
 
 
 def syllabifyTextgrid(
     isle: isletool.Isle,
@@ -302,49 +300,48 @@
 
     stressErrorReporter = utils.getErrorReporter(stressDetectionErrorMode)
     syllabificationErrorReporter = utils.getErrorReporter(syllabificationErrorMode)
 
     minT = tg.minTimestamp
     maxT = tg.maxTimestamp
 
-    wordTier = tg.tierDict[wordTierName]
-    phoneTier = tg.tierDict[phoneTierName]
+    wordTier = tg.getTier(wordTierName)
+    phoneTier = tg.getTier(phoneTierName)
 
     if not isinstance(wordTier, textgrid.IntervalTier):
         raise AttributeError(f"Tier '{wordTierName}' must be an interval tier")
     if not isinstance(phoneTier, textgrid.IntervalTier):
         raise AttributeError(f"Tier '{phoneTierName}' must be an interval tier")
 
     if skipLabelList is None:
         skipLabelList = []
 
-    syllableEntryList = []
-    tonicSEntryList = []
-    tonicPEntryList = []
+    syllableEntries = []
+    tonicSEntries = []
+    tonicPEntries = []
 
     if start is not None or stop is not None:
         if start is None:
             start = minT
         if stop is None:
             stop = maxT
 
         wordTier = wordTier.crop(
             start, stop, praatioConstants.CropCollision.TRUNCATED, False
         )
 
-    for entryStart, entryStop, word in wordTier.entryList:
-
+    for entryStart, entryStop, word in wordTier.entries:
         if word in skipLabelList:
             continue
 
         subPhoneTier = phoneTier.crop(
             entryStart, entryStop, praatioConstants.CropCollision.STRICT, False
         )
 
-        phoneList = [entry[2] for entry in subPhoneTier.entryList if entry[2] != ""]
+        phoneList = [entry[2] for entry in subPhoneTier.entries if entry[2] != ""]
 
         try:
             sylTmp = isle.findBestSyllabification(word, phoneList)
         except errors.WordNotInIsleError:
             print(
                 f"Not is isle -- skipping syllabification; Word '{word}' at {entryStart:.2f}"
             )
@@ -365,47 +362,46 @@
         islesAdjustedSyllableList = syllableList
 
         if len(stressI) > 0 and len(stressJ) > 0:
             syllableList[stressI[0]].phonemes[stressJ[0]] += "ˈ"
 
         i = 0
         for k, syllable in enumerate(syllableList):
-
             # Create the syllable tier entry
             j = len(syllable)
-            stubEntryList = subPhoneTier.entryList[i : i + j]
+            stubEntries = subPhoneTier.entries[i : i + j]
             i += j
 
             # The whole syllable was deleted
-            if len(stubEntryList) == 0:
+            if len(stubEntries) == 0:
                 continue
 
-            syllableStart = stubEntryList[0][0]
-            syllableEnd = stubEntryList[-1][1]
-            label = "-".join([entry[2] for entry in stubEntryList])
+            syllableStart = stubEntries[0][0]
+            syllableEnd = stubEntries[-1][1]
+            label = "-".join([entry[2] for entry in stubEntries])
 
-            syllableEntryList.append((syllableStart, syllableEnd, label))
+            syllableEntries.append((syllableStart, syllableEnd, label))
 
             # Create the tonic syllable tier entry
             if k == stressI:
-                tonicSEntryList.append(
+                tonicSEntries.append(
                     (syllableStart, syllableEnd, phonetic_constants.TONIC)
                 )
 
             # Create the tonic phone tier entry
             if k == stressI:
                 syllablePhoneTier = phoneTier.crop(
                     syllableStart,
                     syllableEnd,
                     praatioConstants.CropCollision.STRICT,
                     False,
                 )
 
                 tonicSyllableEntries: List[textgrid.constants.Interval] = [
-                    entry for entry in syllablePhoneTier.entryList if entry[2] != ""
+                    entry for entry in syllablePhoneTier.entries if entry[2] != ""
                 ]
                 tonicSyllable = phonetics.Syllable(
                     [phone for _, _, phone in tonicSyllableEntries]
                 )
                 cvList = tonicSyllable.simplify().phonemes
 
                 tmpStressJ = None
@@ -423,20 +419,20 @@
                         f"No stressed syllable; word: '{word}' at {syllableStart:.2f}, "
                         f"actual mapped pronunciation: {syllableList}, "
                         f"ISLE's mapped pronunciation: {islesAdjustedSyllableList}",
                     )
                     continue
 
                 phoneStart, phoneEnd = tonicSyllableEntries[tmpStressJ][:2]
-                tonicPEntryList.append((phoneStart, phoneEnd, phonetic_constants.TONIC))
+                tonicPEntries.append((phoneStart, phoneEnd, phonetic_constants.TONIC))
 
     # Create a textgrid with the two syllable-level tiers
-    syllableTier = textgrid.IntervalTier("syllable", syllableEntryList, minT, maxT)
-    tonicSTier = textgrid.IntervalTier("tonicSyllable", tonicSEntryList, minT, maxT)
-    tonicPTier = textgrid.IntervalTier("tonicVowel", tonicPEntryList, minT, maxT)
+    syllableTier = textgrid.IntervalTier("syllable", syllableEntries, minT, maxT)
+    tonicSTier = textgrid.IntervalTier("tonicSyllable", tonicSEntries, minT, maxT)
+    tonicPTier = textgrid.IntervalTier("tonicVowel", tonicPEntries, minT, maxT)
 
     syllableTG = textgrid.Textgrid()
     syllableTG.addTier(syllableTier)
     syllableTG.addTier(tonicSTier)
     syllableTG.addTier(tonicPTier)
 
     return syllableTG
```

### Comparing `pysle-4.0.0/pysle/pronunciationtools.py` & `pysle-4.0.1/pysle/pronunciationtools.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/utilities/constants.py` & `pysle-4.0.1/pysle/utilities/constants.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/utilities/errors.py` & `pysle-4.0.1/pysle/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/utilities/isle_io.py` & `pysle-4.0.1/pysle/utilities/isle_io.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/utilities/phonetic_constants.py` & `pysle-4.0.1/pysle/utilities/phonetic_constants.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/utilities/search.py` & `pysle-4.0.1/pysle/utilities/search.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle/utilities/utils.py` & `pysle-4.0.1/pysle/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pysle-4.0.0/pysle.egg-info/PKG-INFO` & `pysle-4.0.1/pysle.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysle
-Version: 4.0.0
+Version: 4.0.1
 Summary: An interface to ISLEX, an IPA pronunciation dictionary for English with stress and syllable markings.
 Home-page: https://github.com/timmahrt/pysle
 Author: Tim Mahrt
 Author-email: timmahrt@gmail.com
 License: LICENSE
 Platform: UNKNOWN
 Requires-Python: >3.6.0
@@ -32,41 +32,40 @@
 # Table of contents
 1. [Documentation](#documentation)
 2. [Tutorials](#tutorials)
 3. [Version History](#version-history)
 4. [Requirements](#requirements)
 5. [ISLE Dictionary](#isle-dictionary)
 6. [Installation](#installation)
-7. [Version 3 to 4 Migration](#version-3-to-4-migration)
+7. [Upgrading](#upgrading)
 8. [Usage](#usage)
 9. [Common Use Cases](#common-use-cases)
 10. [Tests](#tests)
 11. [Citing psyle](#citing-pysle)
 12. [Acknowledgements](#acknowledgements)
 
 
 ## Documentation
 
 Automatically generated pdocs can be found here:
 
 http://timmahrt.github.io/pysle/
 
-The documentation is generated with the following command:
-`pdoc ./pysle -d google -o docs`
-
 ## Tutorials
 
 There are tutorials available for learning how to use Pysle.  These
 are in the form of IPython Notebooks which can be found in the /tutorials/
 folder distributed with Pysle.
 
 You can view them online using the external website Jupyter:
 
 [Tutorial 1: Introduction to Pysle](<https://nbviewer.jupyter.org/github/timmahrt/pysle/blob/main/tutorials/tutorial1_intro_to_pysle.ipynb>)
 
+[Tutorial 2: Pronunciationtools](<https://nbviewer.jupyter.org/github/timmahrt/pysle/blob/main/tutorials/tutorial2_pronunciationtools.ipynb>)
+
 ## Version History
 
 *Pysle uses semantic versioning (Major.Minor.Patch)*
 
 Please view [CHANGELOG.md](https://github.com/timmahrt/pysle/blob/main/CHANGELOG.md) for version history.
 
 
@@ -109,24 +108,17 @@
 
     python setup.py install
 
 If python is not in your path, you'll need to enter the full path e.g.
 
     C:\Python36\python.exe setup.py install
 
-## Version 3 to 4 Migration
-
-The iterface to isle dictionaries, praattools, and pronunciationtools haven't changed so
-much except for a bit of renaming.
-
-The expected return types have completely changed however--shifting to datatypes now defined
-in `phonetics.py`. If you are struggling with migrating to version 4, please let me know.
+## Upgrading
 
-Looking over changes to the example files may help show the changes that need to be made
-to get the same results.
+Please view [UPGRADING.md](https://github.com/timmahrt/pysle/blob/main/UPGRADING.md) for detailed information about how to upgrade from earlier versions.
 
 ## Usage
 
 Here is a typical usage
 
 ```python
 from pysle import isletool
@@ -174,21 +166,14 @@
 
 - automatically syllabify a praat textgrid (see [praatIO](<https://github.com/timmahrt/praatIO>))
    containing words and phones (e.g. force-aligned text)
     ```python
     pysle.syllabifyTextgrid(isleDict, praatioTextgrid, "words", "phones")
     ```
 
-## Tests
-
-I run tests with the following command (this requires pytest and pytest-cov to be installed):
-
-`pytest --cov=pysle tests/`
-
-
 ## Citing pysle
 
 
 Pysle is general purpose coding and doesn't need to be cited
 (you should cite the
 [ISLEX project](<http://www.isle.illinois.edu/speech_web_lg/data/g2ps/>)
 instead) but if you would like to, it can be cited like so:
```

### Comparing `pysle-4.0.0/setup.py` & `pysle-4.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 """
 import io
 from setuptools import setup
 
 setup(
     name="pysle",
     python_requires=">3.6.0",
-    version="4.0.0",
+    version="4.0.1",
     author="Tim Mahrt",
     author_email="timmahrt@gmail.com",
     url="https://github.com/timmahrt/pysle",
     package_dir={"pysle": "pysle"},
     packages=["pysle", "pysle.utilities"],
     package_data={
         "pysle": [
             "data/ISLEdict.txt",
         ]
     },
     install_requires=[
-        "praatio >= 5.0",
+        "praatio ~= 6.0",
         "typing_extensions",
     ],
     license="LICENSE",
     description=(
         "An interface to ISLEX, an IPA pronunciation dictionary "
         "for English with stress and syllable markings."
     ),
```

