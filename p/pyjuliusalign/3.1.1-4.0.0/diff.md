# Comparing `tmp/pyjuliusalign-3.1.1.tar.gz` & `tmp/pyjuliusalign-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjuliusalign-3.1.1.tar", last modified: Fri Sep  3 03:31:29 2021, max compression
+gzip compressed data, was "pyjuliusalign-4.0.0.tar", last modified: Sat Jul 15 14:28:29 2023, max compression
```

## Comparing `pyjuliusalign-3.1.1.tar` & `pyjuliusalign-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-09-03 03:31:29.801195 pyjuliusalign-3.1.1/
--rw-r--r--   0 tmahrt     (501) staff       (20)     1465 2020-10-11 10:44:02.000000 pyjuliusalign-3.1.1/LICENSE
--rw-r--r--   0 tmahrt     (501) staff       (20)       78 2019-01-09 14:18:58.000000 pyjuliusalign-3.1.1/MANIFEST.in
--rw-r--r--   0 tmahrt     (501) staff       (20)    10200 2021-09-03 03:31:29.801518 pyjuliusalign-3.1.1/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)     8512 2021-08-21 13:06:58.000000 pyjuliusalign-3.1.1/README.md
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-09-03 03:31:29.798620 pyjuliusalign-3.1.1/pyjuliusalign/
--rw-r--r--   0 tmahrt     (501) staff       (20)       48 2021-08-14 03:12:55.000000 pyjuliusalign-3.1.1/pyjuliusalign/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    17031 2021-08-21 12:38:02.000000 pyjuliusalign-3.1.1/pyjuliusalign/alignFromTextgrid.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     3906 2021-08-14 03:11:59.000000 pyjuliusalign-3.1.1/pyjuliusalign/audioScripts.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2571 2021-08-14 03:13:01.000000 pyjuliusalign-3.1.1/pyjuliusalign/convertKana.py
--rwxr-xr-x   0 tmahrt     (501) staff       (20)      685 2019-01-09 14:18:58.000000 pyjuliusalign-3.1.1/pyjuliusalign/hiraganaChart.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)     9897 2021-08-15 16:25:00.000000 pyjuliusalign-3.1.1/pyjuliusalign/jProcessingSnippet.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    12520 2021-09-03 03:18:09.000000 pyjuliusalign-3.1.1/pyjuliusalign/juliusAlignment.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      134 2021-08-14 03:12:13.000000 pyjuliusalign-3.1.1/pyjuliusalign/julius_to_p2fa.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      686 2019-01-09 14:18:58.000000 pyjuliusalign-3.1.1/pyjuliusalign/katakanaChart.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)     1095 2021-08-14 03:12:22.000000 pyjuliusalign-3.1.1/pyjuliusalign/unidic.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2470 2021-08-14 03:12:30.000000 pyjuliusalign-3.1.1/pyjuliusalign/utils.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     6685 2021-08-15 16:25:00.000000 pyjuliusalign-3.1.1/pyjuliusalign/yomi2voca.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-09-03 03:31:29.800860 pyjuliusalign-3.1.1/pyjuliusalign.egg-info/
--rw-r--r--   0 tmahrt     (501) staff       (20)    10200 2021-09-03 03:31:29.000000 pyjuliusalign-3.1.1/pyjuliusalign.egg-info/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)      591 2021-09-03 03:31:29.000000 pyjuliusalign-3.1.1/pyjuliusalign.egg-info/SOURCES.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        1 2021-09-03 03:31:29.000000 pyjuliusalign-3.1.1/pyjuliusalign.egg-info/dependency_links.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       38 2021-09-03 03:31:29.000000 pyjuliusalign-3.1.1/pyjuliusalign.egg-info/requires.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       14 2021-09-03 03:31:29.000000 pyjuliusalign-3.1.1/pyjuliusalign.egg-info/top_level.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       73 2021-09-03 03:31:29.802450 pyjuliusalign-3.1.1/setup.cfg
--rw-r--r--   0 tmahrt     (501) staff       (20)      772 2021-09-03 03:28:56.000000 pyjuliusalign-3.1.1/setup.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 14:28:29.829538 pyjuliusalign-4.0.0/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1465 2020-10-11 10:44:02.000000 pyjuliusalign-4.0.0/LICENSE
+-rw-r--r--   0 tmahrt     (501) staff       (20)       78 2019-01-09 14:18:58.000000 pyjuliusalign-4.0.0/MANIFEST.in
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8462 2023-07-15 14:28:29.829820 pyjuliusalign-4.0.0/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8099 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/README.md
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 14:28:29.823979 pyjuliusalign-4.0.0/pyjuliusalign/
+-rw-r--r--   0 tmahrt     (501) staff       (20)       48 2021-08-14 03:12:55.000000 pyjuliusalign-4.0.0/pyjuliusalign/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    17018 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/pyjuliusalign/alignFromTextgrid.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3903 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/pyjuliusalign/audioScripts.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2551 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/pyjuliusalign/convertKana.py
+-rwxr-xr-x   0 tmahrt     (501) staff       (20)      685 2019-01-09 14:18:58.000000 pyjuliusalign-4.0.0/pyjuliusalign/hiraganaChart.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)     9849 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/pyjuliusalign/jProcessingSnippet.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    12500 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/pyjuliusalign/juliusAlignment.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      134 2023-07-15 13:42:11.000000 pyjuliusalign-4.0.0/pyjuliusalign/julius_to_p2fa.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      686 2019-01-09 14:18:58.000000 pyjuliusalign-4.0.0/pyjuliusalign/katakanaChart.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1091 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/pyjuliusalign/unidic.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2469 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/pyjuliusalign/utils.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     6685 2023-07-15 13:42:45.000000 pyjuliusalign-4.0.0/pyjuliusalign/yomi2voca.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 14:28:29.827918 pyjuliusalign-4.0.0/pyjuliusalign.egg-info/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8462 2023-07-15 14:28:29.000000 pyjuliusalign-4.0.0/pyjuliusalign.egg-info/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)      591 2023-07-15 14:28:29.000000 pyjuliusalign-4.0.0/pyjuliusalign.egg-info/SOURCES.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        1 2023-07-15 14:28:29.000000 pyjuliusalign-4.0.0/pyjuliusalign.egg-info/dependency_links.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       56 2023-07-15 14:28:29.000000 pyjuliusalign-4.0.0/pyjuliusalign.egg-info/requires.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       14 2023-07-15 14:28:29.000000 pyjuliusalign-4.0.0/pyjuliusalign.egg-info/top_level.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       73 2023-07-15 14:28:29.830623 pyjuliusalign-4.0.0/setup.cfg
+-rw-r--r--   0 tmahrt     (501) staff       (20)      862 2023-07-15 14:19:07.000000 pyjuliusalign-4.0.0/setup.py
```

### Comparing `pyjuliusalign-3.1.1/LICENSE` & `pyjuliusalign-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjuliusalign-3.1.1/PKG-INFO` & `pyjuliusalign-4.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,181 +1,182 @@
 Metadata-Version: 2.1
 Name: pyjuliusalign
-Version: 3.1.1
+Version: 4.0.0
 Summary: A helper library for doing forced-alignment in Japanese with Julius.
 Home-page: https://github.com/timmahrt/pyJuliusAlign
 Author: Tim Mahrt
 Author-email: timmahrt@gmail.com
 License: LICENSE
-Description: 
-        # pyJuliusAlign
-        
-         [![](https://badges.gitter.im/pyJuliusAlign/Lobby.svg)](https://gitter.im/pyJuliusAlign/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://img.shields.io/badge/license-MIT-blue.svg?)](http://opensource.org/licenses/MIT) [![](https://img.shields.io/pypi/v/pyjuliusalign.svg)](https://pypi.org/project/pyjuliusalign/)
-        
-        *Questions?  Comments?  Feedback?  Chat with us on gitter!*
-        
-        -----
-        
-        Input and output of pyJuliusAlign:
-        
-        ![PyJuliusAlign example](./examples/files/pyjulius_example.png)
-        
-        録音音声とトランスクリプトはあるけど、どこにその単語またはその子音、母音があるのか正確に分からない時、それらを探すために「forced alignment」という機能を使います。「Julius」という音声認識システムは日本語で「forced alignment」を行うことができますが、音声内に発音を入れる必要があります。がしかし、基本的にはトランスクリプトは文字だけです。「cabocha」というソフトウェアは文章を元にそれぞれの単語からその発音まで変換することができます。「pyJuliusAlign」というライブラリは日本語を「forced alignment」する為に「Julius」と「cabocha」を一緒に使います。TextGridされた音声録音には、単語とその子音、母音を直接挿入することができます。
-        
-        When we have a speech recording and a text transcript but we don't know where the words, vowels, and consonants are, we can use a tool called "forced alignment" to find them. There is a speech recognition system called "Julius" that can do forced alignment in Japanese. However, it requires the pronunciation used in the recording. Usually, in the text transcript, there is only words. The "Cabocha" software can convert sentences to individual words and their pronunciations. The software library "pyJuliusAlign" uses "Julius" and "cabocha" together. In textgrid speech transcripts, words, vowels, and consonants can be directly inserted.
-        
-        ----
-        
-        英語やフランス語やスペイン語など「forced alignment」をしたいなら「SPPAS」と言うソフトウェアをお勧めします。
-        
-        If you want to do forced alignment in English, French, or Spanish, I recommend SPPAS.
-        
-        [http://www.sppas.org](http://www.sppas.org/)
-        
-        
-        ----
-        
-        To get started:
-        
-        */examples/align_example.py* should be sufficient for a large number of cases.
-        
-        */pyjuliusalign/alignFromTextgrid.py* provides a good example of building your own custom alignment code (with different inputs and outputs than textgrids).  
-        
-        
-        # Table of contents
-        1. [Major Revisions](#major-revisions)
-        2. [Requirements](#requirements)
-          * [Mac-specific Requirements Information](#mac-specific-requirements-information)
-          * [Windows-specific Requirements Information](#windows-specific-requirements-information)
-        3. [Installation](#installation)
-        4. [Testing Installation](#testing-installation)
-        5. [Example Usage](#example-usage)
-        6. [Troubleshooting](#troubleshooting)
-        
-        
-        ## Major Revisions
-        
-        Ver 3.1.0 (August 21, 2021)
-        - Added alignFromTextgrid.segmentPhrasesOnSmallPause for avoided problems with small pauses
-          - it is a very fuzzy process thats guesses and makes assumptions -- feedback is helpful!
-          - (see align_example.py and new test file introduction_one_line.TextGrid)
-        - Requires a new python library (pydub)
-        
-        Ver 3.0.0 (October 11, 2020)
-        - Fixed a bug preventing the use of triphone models.
-        - Requires a new python library (python-Levenshtein)
-        
-        Ver 2.0 (January 12, 2019)
-        - pyJuliusAlign now works with the latest version of Julius and the Julius Segmentation Kit.
-          - If you need to use the old segmentation kit (segment_julius4.pl), please use pyJuliusAlign ver 1.1 
-        - Quality of life improvements + documentation
-        
-        Ver 1.1 (August 12, 2018)
-        - Python 3.x support
-        
-        Ver 1.0 (September 2, 2014)
-        - Users can force-align words and phones for transcribed speech in Japanese
-        
-        
-        ## Requirements
-        
-        python - https://www.python.org/
-        
-        python-Levenshtein
-        - https://github.com/ztane/python-Levenshtein
-        
-        pyDub
-        - https://github.com/jiaaro/pydub
-        
-        praatIO - https://github.com/timmahrt/praatIO
-         - for textgrid manipulations
-        
-        Julius - https://github.com/julius-speech/julius
-         - the speech recognition engine
-         - pyJuliusAlign has been tested with Julius 4.5, released on January 2nd, 2019.
-        
-        Julius Segmentation Kit - https://github.com/julius-speech/segmentation-kit
-         - it's not a file you "install" but something you'll want to put in a stable folder where you can access it when needed
-         - Change line 33 to:
-          ```perl
-          ## data directory
-          $datadir = "./wav";
-          if (defined $ARGV[0]) {
-            $datadir = $ARGV[0];
-          }
-          ```
-          - Also in the configuration section, I recommend setting `$hmmdefs` to an absolute path e.g. `$hmmdefs="/Users/tmahrt/segmentation-kit/models/hmmdefs_monof_mix16_gid.binhmm"; # monophone model`
-          - Make sure to set silence appropriately.  If you have clearly marked the edges of speech, you'll want to turn off silence marking.  If you have not done so (for example, your recording only includes a single utterance) then you'll want to have the segmentation kit expect silence at the start and end of your recording.
-        
-        Sox - http://sox.sourceforge.net/
-         - Converts the sampling frequency of the audio if needed.
-         - Optional.  If you choose to not install sox, you'll need to make sure your audio files are at the same sampling frequency as the model data (the included data is 14khz)
-         - If you forced the script to run Julius on audio that has a different sampling frequency, the aligner would completely fail.
-        
-        Cabocha - http://taku910.github.io/cabocha/ 
-         - used to convert typical Japanese text into romaji/phones.
-         - (throw it into google translate if you need it in English)
-         - make a note of which encoding you use for the dictionary file--you'll need it in the code
-         - (you may need to configure cabocha post-install; see https://github.com/timmahrt/pyJuliusAlign/issues/7)
-        
-        Perl (for Julius)
-        
-        
-        ### Mac-specific Requirements Information
-        
-        I use a mac and was able to easily install many requirements using Homebrew.  Here are some guides that I found useful (they translate well enough from Japanese using google translate):
-         - Sox https://qiita.com/samurai20000@github/items/2af98b6c468af317bb09
-         - Cabocha https://qiita.com/musaprg/items/9a572ad5c4e28f79d2ae
-         - I manually built Julius using the configure and make scripts included in that project
-        
-        
-        ### Windows-specific Requirements Information
-        
-        I currently don't have access to a Windows machine. Earlier, I tested installation and got as far as running Julius. Perl tried to run gzip which I couldn't get to install.
-        
-        One user was able to get it working on Windows by installing cygwin and adding cygwin to the path in environment variables.  Also, they had to install MeCab before running Cabocha, otherwise, they would receive an exception saying there's something wrong with Cabocha.
-        
-        
-        ## Installation
-        
-        PyJuliusAlign is on pypi and can be installed or upgraded from the command-line shell with pip like so::
-        
-            python -m pip install pyjuliusalign --upgrade
-        
-        Otherwise, to manually install, after downloading the source from github, from a command-line shell, navigate to the directory containing setup.py and type::
-        
-            python setup.py install
-        
-        If python is not in your path, you'll need to enter the full path e.g.::
-        
-        	C:\Python36\python.exe setup.py install
-        
-        
-        ## Testing Installation
-        
-        In the folder 'examples' run the file 'align_example.py'.
-        
-        If sox, cabocha, julius, and perl are all in your path, you won't need to specify them in any of the arguments--leave them with your default values. Otherwise, you'll need to specify the full path of their bin/executable files.
-        
-        If you have difficulties running the code without specifying the full path, try using the full paths anyways.
-        
-        Also, you will need to configure "segment_julius.pl" which is a part of the Julius Segmentation Kit.
-        
-        
-        ## Example Usage
-        
-        Please see /examples for an example usage.
-        
-        There is pretty much only one way to use this library at the moment. Please contact me if you are having difficulties using this library.
-        
-        
-        ## Troubleshooting
-        
-        The scripts should catch any issues along the way with the exception of  issues stemming from Julius.  If you get bogus/null results, most likely Julius hasn't been set up correctly.
-        
-        The Julius Segmentation kit comes with an example.  If you can force align that, then you should be able to force align using this script as well.
-        
-        
-        
-        
 Platform: UNKNOWN
+Requires-Python: >3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# pyJuliusAlign
+
+ [![](https://badges.gitter.im/pyJuliusAlign/Lobby.svg)](https://gitter.im/pyJuliusAlign/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://img.shields.io/badge/license-MIT-blue.svg?)](http://opensource.org/licenses/MIT) [![](https://img.shields.io/pypi/v/pyjuliusalign.svg)](https://pypi.org/project/pyjuliusalign/)
+
+*Questions?  Comments?  Feedback?  Chat with us on gitter!*
+
+-----
+
+Input and output of pyJuliusAlign:
+
+![PyJuliusAlign example](./examples/files/pyjulius_example.png)
+
+録音音声とトランスクリプトはあるけど、どこにその単語またはその子音、母音があるのか正確に分からない時、それらを探すために「forced alignment」という機能を使います。「Julius」という音声認識システムは日本語で「forced alignment」を行うことができますが、音声内に発音を入れる必要があります。がしかし、基本的にはトランスクリプトは文字だけです。「cabocha」というソフトウェアは文章を元にそれぞれの単語からその発音まで変換することができます。「pyJuliusAlign」というライブラリは日本語を「forced alignment」する為に「Julius」と「cabocha」を一緒に使います。TextGridされた音声録音には、単語とその子音、母音を直接挿入することができます。
+
+When we have a speech recording and a text transcript but we don't know where the words, vowels, and consonants are, we can use a tool called "forced alignment" to find them. There is a speech recognition system called "Julius" that can do forced alignment in Japanese. However, it requires the pronunciation used in the recording. Usually, in the text transcript, there is only words. The "Cabocha" software can convert sentences to individual words and their pronunciations. The software library "pyJuliusAlign" uses "Julius" and "cabocha" together. In textgrid speech transcripts, words, vowels, and consonants can be directly inserted.
+
+----
+
+英語やフランス語やスペイン語など「forced alignment」をしたいなら「SPPAS」と言うソフトウェアをお勧めします。
+
+If you want to do forced alignment in English, French, or Spanish, I recommend SPPAS.
+
+[http://www.sppas.org](http://www.sppas.org/)
+
+
+----
+
+To get started:
+
+*/examples/align_example.py* should be sufficient for a large number of cases.
+
+*/pyjuliusalign/alignFromTextgrid.py* provides a good example of building your own custom alignment code (with different inputs and outputs than textgrids).  
+
+
+# Table of contents
+1. [Documentation](#documentation)
+2. [Major Revisions](#major-revisions)
+3. [Requirements](#requirements)
+  * [Mac-specific Requirements Information](#mac-specific-requirements-information)
+  * [Windows-specific Requirements Information](#windows-specific-requirements-information)
+4. [Installation](#installation)
+5. [Testing Installation](#testing-installation)
+6. [Example Usage](#example-usage)
+7. [Tests](#tests)
+8. [Troubleshooting](#troubleshooting)
+
+## Documentation
+
+Automatically generated pdocs can be found here:
+
+http://timmahrt.github.io/pyJuliusAlign/
+
+
+## Major Revisions
+
+*PyJuliusAlign uses semantic versioning (Major.Minor.Patch)*
+
+Please view [CHANGELOG.md](https://github.com/timmahrt/praatIO/blob/main/CHANGELOG.md) for version history.
+
+
+## Requirements
+
+python - https://www.python.org/
+
+python-Levenshtein
+- https://github.com/ztane/python-Levenshtein
+
+pyDub
+- https://github.com/jiaaro/pydub
+
+praatIO - https://github.com/timmahrt/praatIO
+ - for textgrid manipulations
+
+Julius - https://github.com/julius-speech/julius
+ - the speech recognition engine
+ - pyJuliusAlign has been tested with Julius 4.5, released on January 2nd, 2019.
+
+Julius Segmentation Kit - https://github.com/julius-speech/segmentation-kit
+ - it's not a file you "install" but something you'll want to put in a stable folder where you can access it when needed
+ - Change line 33 to:
+  ```perl
+  ## data directory
+  $datadir = "./wav";
+  if (defined $ARGV[0]) {
+    $datadir = $ARGV[0];
+  }
+  ```
+  - Also in the configuration section, I recommend setting `$hmmdefs` to an absolute path e.g. `$hmmdefs="/Users/tmahrt/segmentation-kit/models/hmmdefs_monof_mix16_gid.binhmm"; # monophone model`
+  - Make sure to set silence appropriately.  If you have clearly marked the edges of speech, you'll want to turn off silence marking.  If you have not done so (for example, your recording only includes a single utterance) then you'll want to have the segmentation kit expect silence at the start and end of your recording.
+
+Sox - http://sox.sourceforge.net/
+ - Converts the sampling frequency of the audio if needed.
+ - Optional.  If you choose to not install sox, you'll need to make sure your audio files are at the same sampling frequency as the model data (the included data is 14khz)
+ - If you forced the script to run Julius on audio that has a different sampling frequency, the aligner would completely fail.
+
+Cabocha - http://taku910.github.io/cabocha/ 
+ - used to convert typical Japanese text into romaji/phones.
+ - (throw it into google translate if you need it in English)
+ - make a note of which encoding you use for the dictionary file--you'll need it in the code
+ - (you may need to configure cabocha post-install; see https://github.com/timmahrt/pyJuliusAlign/issues/7)
+
+Perl (for Julius)
+
+
+### Mac-specific Requirements Information
+
+I use a mac and was able to easily install many requirements using Homebrew.  Here are some guides that I found useful (they translate well enough from Japanese using google translate):
+ - Sox https://qiita.com/samurai20000@github/items/2af98b6c468af317bb09
+ - Cabocha https://qiita.com/musaprg/items/9a572ad5c4e28f79d2ae
+ - I manually built Julius using the configure and make scripts included in that project
+
+
+### Windows-specific Requirements Information
+
+I currently don't have access to a Windows machine. Earlier, I tested installation and got as far as running Julius. Perl tried to run gzip which I couldn't get to install.
+
+One user was able to get it working on Windows by installing cygwin and adding cygwin to the path in environment variables.  Also, they had to install MeCab before running Cabocha, otherwise, they would receive an exception saying there's something wrong with Cabocha.
+
+## Installation
+
+PyJuliusAlign is on pypi and can be installed or upgraded from the command-line shell with pip like so::
+
+    python -m pip install pyjuliusalign --upgrade
+
+Otherwise, to manually install, after downloading the source from github, from a command-line shell, navigate to the directory containing setup.py and type::
+
+    python setup.py install
+
+If python is not in your path, you'll need to enter the full path e.g.::
+
+	C:\Python36\python.exe setup.py install
+
+
+## Testing Installation
+
+In the folder 'examples' run the file 'align_example.py'.
+
+If sox, cabocha, julius, and perl are all in your path, you won't need to specify them in any of the arguments--leave them with your default values. Otherwise, you'll need to specify the full path of their bin/executable files.
+
+If you have difficulties running the code without specifying the full path, try using the full paths anyways.
+
+Also, you will need to configure "segment_julius.pl" which is a part of the Julius Segmentation Kit.
+
+
+## Example Usage
+
+Please see /examples for an example usage.
+
+There is pretty much only one way to use this library at the moment. Please contact me if you are having difficulties using this library.
+
+
+## Tests
+
+I run tests with the following command (this requires pytest and pytest-cov to be installed):
+
+`pytest --cov=pyjuliusalign tests/`
+
+
+## Troubleshooting
+
+The scripts should catch any issues along the way with the exception of issues stemming from Julius.  If you get bogus/null results, most likely Julius hasn't been set up correctly.
+
+The Julius Segmentation kit comes with an example.  If you can force align that, then you should be able to force align using this script as well.
+
+
+
+
+
```

### Comparing `pyjuliusalign-3.1.1/README.md` & `pyjuliusalign-4.0.0/pyjuliusalign.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pyjuliusalign
+Version: 4.0.0
+Summary: A helper library for doing forced-alignment in Japanese with Julius.
+Home-page: https://github.com/timmahrt/pyJuliusAlign
+Author: Tim Mahrt
+Author-email: timmahrt@gmail.com
+License: LICENSE
+Platform: UNKNOWN
+Requires-Python: >3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # pyJuliusAlign
 
  [![](https://badges.gitter.im/pyJuliusAlign/Lobby.svg)](https://gitter.im/pyJuliusAlign/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://img.shields.io/badge/license-MIT-blue.svg?)](http://opensource.org/licenses/MIT) [![](https://img.shields.io/pypi/v/pyjuliusalign.svg)](https://pypi.org/project/pyjuliusalign/)
 
 *Questions?  Comments?  Feedback?  Chat with us on gitter!*
 
@@ -30,46 +43,37 @@
 
 */examples/align_example.py* should be sufficient for a large number of cases.
 
 */pyjuliusalign/alignFromTextgrid.py* provides a good example of building your own custom alignment code (with different inputs and outputs than textgrids).  
 
 
 # Table of contents
-1. [Major Revisions](#major-revisions)
-2. [Requirements](#requirements)
+1. [Documentation](#documentation)
+2. [Major Revisions](#major-revisions)
+3. [Requirements](#requirements)
   * [Mac-specific Requirements Information](#mac-specific-requirements-information)
   * [Windows-specific Requirements Information](#windows-specific-requirements-information)
-3. [Installation](#installation)
-4. [Testing Installation](#testing-installation)
-5. [Example Usage](#example-usage)
-6. [Troubleshooting](#troubleshooting)
+4. [Installation](#installation)
+5. [Testing Installation](#testing-installation)
+6. [Example Usage](#example-usage)
+7. [Tests](#tests)
+8. [Troubleshooting](#troubleshooting)
 
+## Documentation
 
-## Major Revisions
+Automatically generated pdocs can be found here:
+
+http://timmahrt.github.io/pyJuliusAlign/
 
-Ver 3.1.0 (August 21, 2021)
-- Added alignFromTextgrid.segmentPhrasesOnSmallPause for avoided problems with small pauses
-  - it is a very fuzzy process thats guesses and makes assumptions -- feedback is helpful!
-  - (see align_example.py and new test file introduction_one_line.TextGrid)
-- Requires a new python library (pydub)
-
-Ver 3.0.0 (October 11, 2020)
-- Fixed a bug preventing the use of triphone models.
-- Requires a new python library (python-Levenshtein)
-
-Ver 2.0 (January 12, 2019)
-- pyJuliusAlign now works with the latest version of Julius and the Julius Segmentation Kit.
-  - If you need to use the old segmentation kit (segment_julius4.pl), please use pyJuliusAlign ver 1.1 
-- Quality of life improvements + documentation
 
-Ver 1.1 (August 12, 2018)
-- Python 3.x support
+## Major Revisions
+
+*PyJuliusAlign uses semantic versioning (Major.Minor.Patch)*
 
-Ver 1.0 (September 2, 2014)
-- Users can force-align words and phones for transcribed speech in Japanese
+Please view [CHANGELOG.md](https://github.com/timmahrt/praatIO/blob/main/CHANGELOG.md) for version history.
 
 
 ## Requirements
 
 python - https://www.python.org/
 
 python-Levenshtein
@@ -122,15 +126,14 @@
 
 ### Windows-specific Requirements Information
 
 I currently don't have access to a Windows machine. Earlier, I tested installation and got as far as running Julius. Perl tried to run gzip which I couldn't get to install.
 
 One user was able to get it working on Windows by installing cygwin and adding cygwin to the path in environment variables.  Also, they had to install MeCab before running Cabocha, otherwise, they would receive an exception saying there's something wrong with Cabocha.
 
-
 ## Installation
 
 PyJuliusAlign is on pypi and can be installed or upgraded from the command-line shell with pip like so::
 
     python -m pip install pyjuliusalign --upgrade
 
 Otherwise, to manually install, after downloading the source from github, from a command-line shell, navigate to the directory containing setup.py and type::
@@ -156,15 +159,24 @@
 ## Example Usage
 
 Please see /examples for an example usage.
 
 There is pretty much only one way to use this library at the moment. Please contact me if you are having difficulties using this library.
 
 
+## Tests
+
+I run tests with the following command (this requires pytest and pytest-cov to be installed):
+
+`pytest --cov=pyjuliusalign tests/`
+
+
 ## Troubleshooting
 
-The scripts should catch any issues along the way with the exception of  issues stemming from Julius.  If you get bogus/null results, most likely Julius hasn't been set up correctly.
+The scripts should catch any issues along the way with the exception of issues stemming from Julius.  If you get bogus/null results, most likely Julius hasn't been set up correctly.
 
 The Julius Segmentation kit comes with an example.  If you can force align that, then you should be able to force align using this script as well.
 
 
 
+
+
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/alignFromTextgrid.py` & `pyjuliusalign-4.0.0/pyjuliusalign/alignFromTextgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import io
 import csv
 
 from pyjuliusalign import utils
 from pyjuliusalign import juliusAlignment
 from pyjuliusalign import audioScripts
 
-from praatio import tgio
+from praatio import textgrid
 from pydub import AudioSegment, silence
 
 
 def getSilencesInAudio(audioFN):
     # https://stackoverflow.com/questions/40896370/detecting-the-index-of-silence-from-a-given-audio-file-using-python
     audio = AudioSegment.from_wav(audioFN)
     silences = silence.detect_silence(
@@ -102,17 +102,14 @@
                 audio = AudioSegment.from_wav(tmpWavFN)
                 speechSegments = invertIntervalList(silences, 0, audio.duration_seconds)
                 speechSegments = [
                     (start + snippetStart, start + snippetEnd)
                     for snippetStart, snippetEnd in speechSegments
                 ]
                 speechSegments = removeUltrashortSegments(speechSegments, 0.2)
-                if len(speechSegments) == 0:
-                    print("This failed")
-
                 # speechSegments = bumpUltrashortSegments(speechSegments)
                 bucketDurations = [
                     snippetEnd - snippetStart
                     for snippetStart, snippetEnd in speechSegments
                 ]
                 speechDuration = sum(bucketDurations)
 
@@ -230,16 +227,15 @@
     7 chunks; 4 buckets
     [1, ...]
     [1 2, ...]
     [1 2 3, ...]
     [1 2 3 4, 5, 6, 7]
     7 - 4 + 1 -> 4 iterations
     """
-    # print((chunks, numBuckets))
-    # exit(0)
+
     gap = len(chunks) - numBuckets
 
     if numBuckets == 1:
         yield [chunks]  # [[4, 5, 6]]
 
     elif len(chunks) == numBuckets:
         yield [[chunk] for chunk in chunks]  # [[4], [5], [6]]
@@ -252,18 +248,18 @@
                 yield [chunks[:i]] + tailChunk  # [[1, 2, 3]] + [[4], [5], [6]]
 
 
 def textgridToCSV(inputPath, outputPath, outputExt=".csv", tierName="utterances"):
     utils.makeDir(outputPath)
 
     for fn in utils.findFiles(inputPath, filterExt=".TextGrid"):
-        tg = tgio.openTextgrid(join(inputPath, fn))
-        tier = tg.tierDict[tierName]
+        tg = textgrid.openTextgrid(join(inputPath, fn), includeEmptyIntervals=False)
+        tier = tg.getTier(tierName)
         outputList = []
-        for start, stop, label in tier.entryList:
+        for start, stop, label in tier.entries:
             outputList.append("%s,%s,%s" % (start, stop, label))
 
         name = os.path.splitext(fn)[0]
         outputTxt = "\n".join(outputList)
         outputFN = join(outputPath, "%s%s" % (name, outputExt))
         with io.open(outputFN, "w", encoding="utf-8") as fd:
             fd.write(outputTxt)
@@ -318,15 +314,15 @@
 
             numUnnamedEntities += unnamedEntity
             numUnidentifiedUtterances += unidentifiedUtterance
             numWordsProcessedWithNoError += tmpWordCount
 
             name = os.path.splitext(fn)[0]
             outputList = [
-                u"%s,%s,%s" % (name, startTime, stopTime),
+                "%s,%s,%s" % (name, startTime, stopTime),
                 origLine,
                 tmpWordList,
                 tmpKanaList,
                 tmpRomajiList,
             ]
             outputStr = ";".join(outputList)
 
@@ -434,29 +430,32 @@
         numIntervals += statList[3]
 
     # All durations should be the same
     inputWavFN = next(iter(wavNameDict.values()))
     maxDuration = audioScripts.getSoundFileDuration(join(wavPath, inputWavFN))
 
     # Create tiers and textgrids from the output of the alignment
-    tg = tgio.Textgrid()
+    tg = textgrid.Textgrid()
     for speaker in speakerList:
         for aspect in [
             juliusAlignment.UTTERANCE,
             juliusAlignment.WORD,
             juliusAlignment.PHONE,
         ]:
-
             tierName = "%s_%s" % (aspect, speaker)
-            tier = tgio.IntervalTier(
+            tier = textgrid.IntervalTier(
                 tierName, speakerEntryDict[speaker][aspect], minT=0, maxT=maxDuration
             )
             tg.addTier(tier)
 
-    tg.save(join(outputPath, outputWavName + ".TextGrid"))
+    tg.save(
+        join(outputPath, outputWavName + ".TextGrid"),
+        format="short_textgrid",
+        includeBlankSpaces=True,
+    )
 
     return (numPhonesFailedAlignment, numPhones, numFailedIntervals, numIntervals)
 
 
 def forceAlignCorpus(
     wavPath, txtPath, outputPath, juliusScriptPath=None, soxPath=None, perlPath=None
 ):
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/audioScripts.py` & `pyjuliusalign-4.0.0/pyjuliusalign/audioScripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     nframes = params[3]
 
     duration = float(nframes) / framerate
     return duration
 
 
 def extractSubwav(fn, outputFN, startT, endT, singleChannelFlag, soxPath=None):
-
     if soxPath is None:
         soxPath = "sox"  # Assumes it is in the user's path
 
     path, fnNoPath = os.path.split(fn)
     resampledAudioPath = join(path, "resampledAudio")
     resampledFN = join(resampledAudioPath, fnNoPath)
 
@@ -95,15 +94,14 @@
 
     outWave = wave.open(outputFN, "w")
     outWave.setparams(outParams)
     outWave.writeframes(audioFrames)
 
 
 def splitStereoAudio(path, fn, outputPath=None):
-
     if outputPath is None:
         outputPath = join(path, "split_audio")
 
     if not os.path.exists(outputPath):
         os.mkdir(outputPath)
 
     name = os.path.splitext(fn)[0]
@@ -119,15 +117,14 @@
     nframes = params[3]
     audioFrames = audiofile.readframes(nframes)
 
     for leftFactor, rightFactor, outputFN in (
         (1, 0, leftOutputFN),
         (0, 1, rightOutputFN),
     ):
-
         monoAudioFrames = audioop.tomono(
             audioFrames, sampwidth, leftFactor, rightFactor
         )
         params = tuple(
             [
                 1,
             ]
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/convertKana.py` & `pyjuliusalign-4.0.0/pyjuliusalign/convertKana.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,23 +48,23 @@
         retDict[value] = key
 
     return retDict
 
 
 def _getKataToKanaDict():
     retDict = {
-        u"ャ": u"ゃ",
-        u"ュ": u"ゅ",
-        u"ョ": u"ょ",
-        u"ッ": u"っ",
-        u"ァ": u"ぁ",
-        u"ィ": u"ぃ",
-        u"ゥ": u"ぅ",
-        u"ェ": u"ぇ",
-        u"ォ": u"ぉ",
+        "ャ": "ゃ",
+        "ュ": "ゅ",
+        "ョ": "ょ",
+        "ッ": "っ",
+        "ァ": "ぁ",
+        "ィ": "ぃ",
+        "ゥ": "ぅ",
+        "ェ": "ぇ",
+        "ォ": "ぉ",
     }
 
     for kata in kataToRomajiDict.keys():
         kana = romajiToKanaDict[kataToRomajiDict[kata]]
         retDict[kata] = kana
 
     return retDict
@@ -76,25 +76,25 @@
 romajiToKanaDict = _invertDict(kanaToRomajiDict)
 kataToKanaDict = _getKataToKanaDict()
 kanaToKataDict = _invertDict(kataToKanaDict)
 
 
 def convertKanaToKata(inputStr):
     """Input hiragana and return the corresponding string in katakana"""
-    retStr = u""
+    retStr = ""
     for char in inputStr:
         if char in kanaToKataDict.keys():
             char = kanaToKataDict[char]
         retStr += char
 
     return retStr
 
 
 def convertKataToKana(inputStr):
     """Input hiragana and return the corresponding string in katakana"""
-    retStr = u""
+    retStr = ""
     for char in inputStr:
         if char in kataToKanaDict.keys():
             char = kataToKanaDict[char]
         retStr += char
 
     return retStr
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/hiraganaChart.txt` & `pyjuliusalign-4.0.0/pyjuliusalign/hiraganaChart.txt`

 * *Files identical despite different names*

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/jProcessingSnippet.py` & `pyjuliusalign-4.0.0/pyjuliusalign/jProcessingSnippet.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,57 +28,57 @@
 class UnidentifiedJapaneseText(Exception):
     def __init__(self, sentence, word):
         super(UnidentifiedJapaneseText, self).__init__()
         self.sentence = sentence
         self.word = word
 
     def __str__(self):
-        return u"No match in dictionary for word '%s' in sentence: \n'%s'" % (
+        return "No match in dictionary for word '%s' in sentence: \n'%s'" % (
             self.word,
             self.sentence,
         )
 
 
 class ChunkingError(Exception):
     """Raised when a katakana string cannot be parsed correctly"""
 
     def __init__(self, txt):
         super(ChunkingError, self).__init__()
         self.textStr = txt
 
     def __str__(self):
-        return u"Chunking error for string: \n %s" % self.textStr
+        return "Chunking error for string: \n %s" % self.textStr
 
 
 class EmptyStrError(Exception):
     def __str__(self):
         return "Empty string passed in"
 
 
 class NonKatakanaError(Exception):
     def __init__(self, char, utterance):
         super(NonKatakanaError, self).__init__()
         self.char = char
         self.utterance = utterance
 
     def __str__(self):
-        return u"Wrongly interpreted character '%s' as kana in utterance:\n%s" % (
+        return "Wrongly interpreted character '%s' as kana in utterance:\n%s" % (
             unicode(self.char),
             unicode(self.utterance),
         )
 
 
 class CabochaNotRunError(Exception):
     def __init__(self, cabochaCmd):
         super(CabochaNotRunError, self).__init__()
         self.cabochaCmd = cabochaCmd
 
     def __str__(self):
         return (
-            u"Cabocha not installed or not in path.  "
+            "Cabocha not installed or not in path.  "
             "Attempted to run command:\n%s" % self.cabochaCmd
         )
 
 
 class CabochaOutputError(Exception):
     def __init__(self, outputStr):
         super(CabochaOutputError, self).__init__()
@@ -153,50 +153,48 @@
         except UnicodeDecodeError:
             raise TextDecodingError(cabochaEncoding)
 
     return retStr
 
 
 def jReads(target_sent, cabochaEncoding, cabochaPath):
-
     xmlStr = cabocha(target_sent, cabochaEncoding, cabochaPath).encode("utf-8")
     #     print(target_sent)
     #     print(xmlStr)
     try:
         sentence = etree.fromstring(xmlStr)
     except etree.ParseError:
         raise CabochaOutputError(xmlStr)
 
     retJReadsToks = []
     retWordList = []
 
     keyList = list(convertKana.kataToRomajiDict.keys())
     validKatakanaList = [
-        u"ャ",
-        u"ュ",
-        u"ョ",
-        u"ッ",
-        u"ァ",
-        u"ィ",
-        u"ゥ",
-        u"ェ",
-        u"ォ",
-        u"ー",
+        "ャ",
+        "ュ",
+        "ョ",
+        "ッ",
+        "ァ",
+        "ィ",
+        "ゥ",
+        "ェ",
+        "ォ",
+        "ー",
     ] + keyList
     #     validHiraganaList = [u"ゃ", u"ゅ", u"ょ", u"っ"] + convertKana.kanaToRomajiDict.keys()
     for chunk in sentence:
         jReadsToks = []
         wordList = []
         for tok in chunk.findall("tok"):
-
             # Determine if this word is punctuation (and if so, skip it)
             # Contains syntactic and morphological information
             featureStr = tok.get("feature")
             featureList = featureStr.split(",")
-            if featureList[0] == u"記号":
+            if featureList[0] == "記号":
                 continue
 
             # Don't process empty words (can happen a lot,
             # depending on the annotation scheme)
             word = tok.text.strip()
             if word == "":
                 continue
@@ -222,71 +220,68 @@
         retJReadsToks.append(jReadsToks)
         retWordList.append(wordList)
 
     return retJReadsToks, retWordList
 
 
 def getChunkedKana(string, cabochaEncoding, cabochaPath):
-
     if string == "":
         raise EmptyStrError()
 
     kanaList, wordList = jReads(string, cabochaEncoding, cabochaPath)
     kanaList = ["".join(subList) for subList in kanaList if len(subList) > 0]
     wordList = ["".join(subList) for subList in wordList if len(subList) > 0]
 
     # Special case - sometimes 'ー' ends up in its own word or at the start
     # of a word, but really it just makes the last vowel longer.  If its
     # by itself, attach it to the previous word
     def mergeTailingVowel(tmpList):
         retList = []
         for word in tmpList:
-            if word[0] == u"ー":
+            if word[0] == "ー":
                 retList[-1] += word
             else:
                 retList.append(word)
         return retList
 
     kanaList = mergeTailingVowel(kanaList)
     wordList = mergeTailingVowel(wordList)
 
-    vowelList = [u"ア", u"イ", u"ウ", u"エ", u"オ"]
-    vowelModifierDict = {u"ァ": u"a", u"ィ": u"i", u"ゥ": u"u", u"ェ": u"e", u"ォ": u"o"}
-    yModifierDict = {u"ャ": u"ya", u"ュ": u"yu", u"ョ": u"yo"}
+    vowelList = ["ア", "イ", "ウ", "エ", "オ"]
+    vowelModifierDict = {"ァ": "a", "ィ": "i", "ゥ": "u", "ェ": "e", "ォ": "o"}
+    yModifierDict = {"ャ": "ya", "ュ": "yu", "ョ": "yo"}
 
     romanjiedTextList = []
     for word in kanaList:
-
         # Sanitize kana
         try:
             kanaInputList = chunkKatakana(word)
         except IndexError:
             raise ChunkingError(word)
 
         # Convert kana to romanji
         romanjiList = []
         for kana in kanaInputList:
-
             # Over-write the previous vowel (foreign words)
             if kana in vowelModifierDict.keys():
                 romanjiList[-1] = romanjiList[-1][:-1] + vowelModifierDict[kana]
 
             # Last vowel is a long vowel
-            elif kana == u"ー":  # Long vowel
+            elif kana == "ー":  # Long vowel
                 # e.g. 'ホーー' becomes "ho::" or 'ふうんー' becomes "hu:n:"
                 #  -- both bad
                 if romanjiList[-1][-1] != ":" and romanjiList[-1][-1] != "N":
                     romanjiList[-1] += ":"
 
                 # Should get recognized as a single vowel by the forced aligner
 
             # Normal case
             else:
                 # Single-phone characters
-                if kana == u"ン" or kana in vowelList:
+                if kana == "ン" or kana in vowelList:
                     romanjiList.append(convertKana.kataToRomajiDict[kana])
                 else:
                     if kana in yModifierDict.keys():  # e.g. 'ィ' in 'ティム'
                         romanjiList.pop(-1)
                         syllable = yModifierDict[kana]
                     else:
                         try:
@@ -313,17 +308,17 @@
 
     returnList = []
     i = 0
     while i < len(kanaStr):
         kana = kanaList[i]
         # Some palatalized consonants are in our chart
         # (notably 'jy' and 'shy' are missing)
-        kanaFlag = kana in [u"ャ", u"ュ", u"ョ"]
+        kanaFlag = kana in ["ャ", "ュ", "ョ"]
         if kanaFlag and returnList[-1] + kana in convertKana.kataToRomajiDict.keys():
             returnList[-1] += kana
-        elif kana == u"ッ":  # Geminate consonant
+        elif kana == "ッ":  # Geminate consonant
             pass
         else:  # Normal case
             returnList.append(kana)
         i += 1
 
     return returnList
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/juliusAlignment.py` & `pyjuliusalign-4.0.0/pyjuliusalign/juliusAlignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
             "Here is the command that python attempted to run:\n"
         )
         cmdTxt = " ".join(self.cmdList)
         return errorStr + cmdTxt
 
 
 def runJuliusAlignment(resourcePath, juliusScriptPath, perlPath, loggerFd):
-
     if not os.path.exists(juliusScriptPath):
         raise JuliusRunError(juliusScriptPath)
 
     resourcePath = os.path.abspath(resourcePath)
 
     cmdList = [perlPath, juliusScriptPath, resourcePath]
     print(" ".join(cmdList))
@@ -268,15 +267,15 @@
                 # One phone occupies the whole interval
                 matchList = [(0.0, (intervalEnd - intervalStart) * 100)]
             else:
                 numPhonesFailedToAlign += numWords
                 numFailedIntervals += 1
                 print(
                     "Failed to align: %s - %f - %f"
-                    % ("".join(romajiList), intervalStart, intervalEnd)
+                    % ("".join(tmpRomajiList), intervalStart, intervalEnd)
                 )
                 continue
 
         adjustedPhonList = [
             [intervalStart + start, intervalStart + stop, label]
             for start, stop, label in matchList
         ]
@@ -332,58 +331,58 @@
     unnamedEntity = 0
 
     origLine = line
 
     # Clean up the line before it gets processed
     # Not sure what "・" is but cabocha doesn't like it
     for char in [
-        u"（",
-        u"）",
-        u" ",
-        u"．",
-        u"？",
-        u"「",
-        u"」",
-        u"［",
-        u"］",
-        u"＠Ｗ",
-        u"＠Ｓ",
-        u"＜",
-        u"＞",
-        u" ",
-        u"。",
+        "（",
+        "）",
+        " ",
+        "．",
+        "？",
+        "「",
+        "」",
+        "［",
+        "］",
+        "＠Ｗ",
+        "＠Ｓ",
+        "＜",
+        "＞",
+        " ",
+        "。",
     ]:
         line = line.replace(char, "")
 
     # Used to split names?
-    for char in [u"・", u"·"]:
+    for char in ["・", "·"]:
         line = line.replace(char, " ")
 
     line = line.strip()
 
     try:
         (tmpWordList, tmpKanaList, tmpRomajiList) = jProcessingSnippet.getChunkedKana(
             line, cabochaEncoding, cabochaPath
         )
     except (jProcessingSnippet.ChunkingError, jProcessingSnippet.NonKatakanaError) as e:
-        print(u"%s, %s" % (str(e), origLine))
+        print("%s, %s" % (str(e), origLine))
         unidentifiedUtterance = 1
     except jProcessingSnippet.UnidentifiedJapaneseText as e:
         # Maybe specific to my corpus?
-        if all([char == u"X" for char in e.word]):
+        if all([char == "X" for char in e.word]):
             unnamedEntity = 1
         else:
-            print(u"%s" % str(e))
+            print("%s" % str(e))
             unidentifiedUtterance = 1
     except jProcessingSnippet.EmptyStrError as e:
         pass
     except Exception:
         print(line)
         raise
-    line = line.replace(u",", u"")
+    line = line.replace(",", "")
 
     return (
         line,
         ",".join(tmpWordList),
         ",".join(tmpKanaList),
         ",".join(tmpRomajiList),
         unidentifiedUtterance,
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/katakanaChart.txt` & `pyjuliusalign-4.0.0/pyjuliusalign/katakanaChart.txt`

 * *Files identical despite different names*

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/unidic.py` & `pyjuliusalign-4.0.0/pyjuliusalign/unidic.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Created on Aug 19, 2014
 
 @author: tmahrt
 """
 
 from os.path import join
-import cPickle
+import pickle
 import io
 
 
 class UnidicTool(object):
     """
     A Japanese pronunciation dictionary developed by Ninjal
     """
@@ -27,19 +27,19 @@
             with io.open(self.unidicPath, "r", encoding="utf-8") as fd:
                 self.data = fd.read()
 
         startI = 0
         matchList = []
         while True:
             try:
-                matchI = self.data.index(u"\n" + word, startI) + 1
-                endI = self.data.index(u"\n", matchI)
+                matchI = self.data.index("\n" + word, startI) + 1
+                endI = self.data.index("\n", matchI)
             except ValueError:
                 break
 
             matchList.append(self.data[matchI + len(word) + 1 : endI].split(","))
             startI = matchI
 
         return matchList
 
     def saveCache(self):
-        cPickle.dump(self.cachedData, open(self.unidicCachePath, "w"))
+        pickle.dump(self.cachedData, open(self.unidicCachePath, "w"))
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/utils.py` & `pyjuliusalign-4.0.0/pyjuliusalign/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     path,
     filterPaths=False,
     filterExt=None,
     filterPattern=None,
     skipIfNameInList=None,
     stripExt=False,
 ):
-
     fnList = os.listdir(path)
 
     if filterPaths is True:
         fnList = [
             folderName
             for folderName in fnList
             if os.path.isdir(os.path.join(path, folderName))
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign/yomi2voca.py` & `pyjuliusalign-4.0.0/pyjuliusalign/yomi2voca.py`

 * *Files identical despite different names*

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign.egg-info/PKG-INFO` & `pyjuliusalign-4.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,167 @@
-Metadata-Version: 2.1
-Name: pyjuliusalign
-Version: 3.1.1
-Summary: A helper library for doing forced-alignment in Japanese with Julius.
-Home-page: https://github.com/timmahrt/pyJuliusAlign
-Author: Tim Mahrt
-Author-email: timmahrt@gmail.com
-License: LICENSE
-Description: 
-        # pyJuliusAlign
-        
-         [![](https://badges.gitter.im/pyJuliusAlign/Lobby.svg)](https://gitter.im/pyJuliusAlign/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://img.shields.io/badge/license-MIT-blue.svg?)](http://opensource.org/licenses/MIT) [![](https://img.shields.io/pypi/v/pyjuliusalign.svg)](https://pypi.org/project/pyjuliusalign/)
-        
-        *Questions?  Comments?  Feedback?  Chat with us on gitter!*
-        
-        -----
-        
-        Input and output of pyJuliusAlign:
-        
-        ![PyJuliusAlign example](./examples/files/pyjulius_example.png)
-        
-        録音音声とトランスクリプトはあるけど、どこにその単語またはその子音、母音があるのか正確に分からない時、それらを探すために「forced alignment」という機能を使います。「Julius」という音声認識システムは日本語で「forced alignment」を行うことができますが、音声内に発音を入れる必要があります。がしかし、基本的にはトランスクリプトは文字だけです。「cabocha」というソフトウェアは文章を元にそれぞれの単語からその発音まで変換することができます。「pyJuliusAlign」というライブラリは日本語を「forced alignment」する為に「Julius」と「cabocha」を一緒に使います。TextGridされた音声録音には、単語とその子音、母音を直接挿入することができます。
-        
-        When we have a speech recording and a text transcript but we don't know where the words, vowels, and consonants are, we can use a tool called "forced alignment" to find them. There is a speech recognition system called "Julius" that can do forced alignment in Japanese. However, it requires the pronunciation used in the recording. Usually, in the text transcript, there is only words. The "Cabocha" software can convert sentences to individual words and their pronunciations. The software library "pyJuliusAlign" uses "Julius" and "cabocha" together. In textgrid speech transcripts, words, vowels, and consonants can be directly inserted.
-        
-        ----
-        
-        英語やフランス語やスペイン語など「forced alignment」をしたいなら「SPPAS」と言うソフトウェアをお勧めします。
-        
-        If you want to do forced alignment in English, French, or Spanish, I recommend SPPAS.
-        
-        [http://www.sppas.org](http://www.sppas.org/)
-        
-        
-        ----
-        
-        To get started:
-        
-        */examples/align_example.py* should be sufficient for a large number of cases.
-        
-        */pyjuliusalign/alignFromTextgrid.py* provides a good example of building your own custom alignment code (with different inputs and outputs than textgrids).  
-        
-        
-        # Table of contents
-        1. [Major Revisions](#major-revisions)
-        2. [Requirements](#requirements)
-          * [Mac-specific Requirements Information](#mac-specific-requirements-information)
-          * [Windows-specific Requirements Information](#windows-specific-requirements-information)
-        3. [Installation](#installation)
-        4. [Testing Installation](#testing-installation)
-        5. [Example Usage](#example-usage)
-        6. [Troubleshooting](#troubleshooting)
-        
-        
-        ## Major Revisions
-        
-        Ver 3.1.0 (August 21, 2021)
-        - Added alignFromTextgrid.segmentPhrasesOnSmallPause for avoided problems with small pauses
-          - it is a very fuzzy process thats guesses and makes assumptions -- feedback is helpful!
-          - (see align_example.py and new test file introduction_one_line.TextGrid)
-        - Requires a new python library (pydub)
-        
-        Ver 3.0.0 (October 11, 2020)
-        - Fixed a bug preventing the use of triphone models.
-        - Requires a new python library (python-Levenshtein)
-        
-        Ver 2.0 (January 12, 2019)
-        - pyJuliusAlign now works with the latest version of Julius and the Julius Segmentation Kit.
-          - If you need to use the old segmentation kit (segment_julius4.pl), please use pyJuliusAlign ver 1.1 
-        - Quality of life improvements + documentation
-        
-        Ver 1.1 (August 12, 2018)
-        - Python 3.x support
-        
-        Ver 1.0 (September 2, 2014)
-        - Users can force-align words and phones for transcribed speech in Japanese
-        
-        
-        ## Requirements
-        
-        python - https://www.python.org/
-        
-        python-Levenshtein
-        - https://github.com/ztane/python-Levenshtein
-        
-        pyDub
-        - https://github.com/jiaaro/pydub
-        
-        praatIO - https://github.com/timmahrt/praatIO
-         - for textgrid manipulations
-        
-        Julius - https://github.com/julius-speech/julius
-         - the speech recognition engine
-         - pyJuliusAlign has been tested with Julius 4.5, released on January 2nd, 2019.
-        
-        Julius Segmentation Kit - https://github.com/julius-speech/segmentation-kit
-         - it's not a file you "install" but something you'll want to put in a stable folder where you can access it when needed
-         - Change line 33 to:
-          ```perl
-          ## data directory
-          $datadir = "./wav";
-          if (defined $ARGV[0]) {
-            $datadir = $ARGV[0];
-          }
-          ```
-          - Also in the configuration section, I recommend setting `$hmmdefs` to an absolute path e.g. `$hmmdefs="/Users/tmahrt/segmentation-kit/models/hmmdefs_monof_mix16_gid.binhmm"; # monophone model`
-          - Make sure to set silence appropriately.  If you have clearly marked the edges of speech, you'll want to turn off silence marking.  If you have not done so (for example, your recording only includes a single utterance) then you'll want to have the segmentation kit expect silence at the start and end of your recording.
-        
-        Sox - http://sox.sourceforge.net/
-         - Converts the sampling frequency of the audio if needed.
-         - Optional.  If you choose to not install sox, you'll need to make sure your audio files are at the same sampling frequency as the model data (the included data is 14khz)
-         - If you forced the script to run Julius on audio that has a different sampling frequency, the aligner would completely fail.
-        
-        Cabocha - http://taku910.github.io/cabocha/ 
-         - used to convert typical Japanese text into romaji/phones.
-         - (throw it into google translate if you need it in English)
-         - make a note of which encoding you use for the dictionary file--you'll need it in the code
-         - (you may need to configure cabocha post-install; see https://github.com/timmahrt/pyJuliusAlign/issues/7)
-        
-        Perl (for Julius)
-        
-        
-        ### Mac-specific Requirements Information
-        
-        I use a mac and was able to easily install many requirements using Homebrew.  Here are some guides that I found useful (they translate well enough from Japanese using google translate):
-         - Sox https://qiita.com/samurai20000@github/items/2af98b6c468af317bb09
-         - Cabocha https://qiita.com/musaprg/items/9a572ad5c4e28f79d2ae
-         - I manually built Julius using the configure and make scripts included in that project
-        
-        
-        ### Windows-specific Requirements Information
-        
-        I currently don't have access to a Windows machine. Earlier, I tested installation and got as far as running Julius. Perl tried to run gzip which I couldn't get to install.
-        
-        One user was able to get it working on Windows by installing cygwin and adding cygwin to the path in environment variables.  Also, they had to install MeCab before running Cabocha, otherwise, they would receive an exception saying there's something wrong with Cabocha.
-        
-        
-        ## Installation
-        
-        PyJuliusAlign is on pypi and can be installed or upgraded from the command-line shell with pip like so::
-        
-            python -m pip install pyjuliusalign --upgrade
-        
-        Otherwise, to manually install, after downloading the source from github, from a command-line shell, navigate to the directory containing setup.py and type::
-        
-            python setup.py install
-        
-        If python is not in your path, you'll need to enter the full path e.g.::
-        
-        	C:\Python36\python.exe setup.py install
-        
-        
-        ## Testing Installation
-        
-        In the folder 'examples' run the file 'align_example.py'.
-        
-        If sox, cabocha, julius, and perl are all in your path, you won't need to specify them in any of the arguments--leave them with your default values. Otherwise, you'll need to specify the full path of their bin/executable files.
-        
-        If you have difficulties running the code without specifying the full path, try using the full paths anyways.
-        
-        Also, you will need to configure "segment_julius.pl" which is a part of the Julius Segmentation Kit.
-        
-        
-        ## Example Usage
-        
-        Please see /examples for an example usage.
-        
-        There is pretty much only one way to use this library at the moment. Please contact me if you are having difficulties using this library.
-        
-        
-        ## Troubleshooting
-        
-        The scripts should catch any issues along the way with the exception of  issues stemming from Julius.  If you get bogus/null results, most likely Julius hasn't been set up correctly.
-        
-        The Julius Segmentation kit comes with an example.  If you can force align that, then you should be able to force align using this script as well.
-        
-        
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+
+# pyJuliusAlign
+
+ [![](https://badges.gitter.im/pyJuliusAlign/Lobby.svg)](https://gitter.im/pyJuliusAlign/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://img.shields.io/badge/license-MIT-blue.svg?)](http://opensource.org/licenses/MIT) [![](https://img.shields.io/pypi/v/pyjuliusalign.svg)](https://pypi.org/project/pyjuliusalign/)
+
+*Questions?  Comments?  Feedback?  Chat with us on gitter!*
+
+-----
+
+Input and output of pyJuliusAlign:
+
+![PyJuliusAlign example](./examples/files/pyjulius_example.png)
+
+録音音声とトランスクリプトはあるけど、どこにその単語またはその子音、母音があるのか正確に分からない時、それらを探すために「forced alignment」という機能を使います。「Julius」という音声認識システムは日本語で「forced alignment」を行うことができますが、音声内に発音を入れる必要があります。がしかし、基本的にはトランスクリプトは文字だけです。「cabocha」というソフトウェアは文章を元にそれぞれの単語からその発音まで変換することができます。「pyJuliusAlign」というライブラリは日本語を「forced alignment」する為に「Julius」と「cabocha」を一緒に使います。TextGridされた音声録音には、単語とその子音、母音を直接挿入することができます。
+
+When we have a speech recording and a text transcript but we don't know where the words, vowels, and consonants are, we can use a tool called "forced alignment" to find them. There is a speech recognition system called "Julius" that can do forced alignment in Japanese. However, it requires the pronunciation used in the recording. Usually, in the text transcript, there is only words. The "Cabocha" software can convert sentences to individual words and their pronunciations. The software library "pyJuliusAlign" uses "Julius" and "cabocha" together. In textgrid speech transcripts, words, vowels, and consonants can be directly inserted.
+
+----
+
+英語やフランス語やスペイン語など「forced alignment」をしたいなら「SPPAS」と言うソフトウェアをお勧めします。
+
+If you want to do forced alignment in English, French, or Spanish, I recommend SPPAS.
+
+[http://www.sppas.org](http://www.sppas.org/)
+
+
+----
+
+To get started:
+
+*/examples/align_example.py* should be sufficient for a large number of cases.
+
+*/pyjuliusalign/alignFromTextgrid.py* provides a good example of building your own custom alignment code (with different inputs and outputs than textgrids).  
+
+
+# Table of contents
+1. [Documentation](#documentation)
+2. [Major Revisions](#major-revisions)
+3. [Requirements](#requirements)
+  * [Mac-specific Requirements Information](#mac-specific-requirements-information)
+  * [Windows-specific Requirements Information](#windows-specific-requirements-information)
+4. [Installation](#installation)
+5. [Testing Installation](#testing-installation)
+6. [Example Usage](#example-usage)
+7. [Tests](#tests)
+8. [Troubleshooting](#troubleshooting)
+
+## Documentation
+
+Automatically generated pdocs can be found here:
+
+http://timmahrt.github.io/pyJuliusAlign/
+
+
+## Major Revisions
+
+*PyJuliusAlign uses semantic versioning (Major.Minor.Patch)*
+
+Please view [CHANGELOG.md](https://github.com/timmahrt/praatIO/blob/main/CHANGELOG.md) for version history.
+
+
+## Requirements
+
+python - https://www.python.org/
+
+python-Levenshtein
+- https://github.com/ztane/python-Levenshtein
+
+pyDub
+- https://github.com/jiaaro/pydub
+
+praatIO - https://github.com/timmahrt/praatIO
+ - for textgrid manipulations
+
+Julius - https://github.com/julius-speech/julius
+ - the speech recognition engine
+ - pyJuliusAlign has been tested with Julius 4.5, released on January 2nd, 2019.
+
+Julius Segmentation Kit - https://github.com/julius-speech/segmentation-kit
+ - it's not a file you "install" but something you'll want to put in a stable folder where you can access it when needed
+ - Change line 33 to:
+  ```perl
+  ## data directory
+  $datadir = "./wav";
+  if (defined $ARGV[0]) {
+    $datadir = $ARGV[0];
+  }
+  ```
+  - Also in the configuration section, I recommend setting `$hmmdefs` to an absolute path e.g. `$hmmdefs="/Users/tmahrt/segmentation-kit/models/hmmdefs_monof_mix16_gid.binhmm"; # monophone model`
+  - Make sure to set silence appropriately.  If you have clearly marked the edges of speech, you'll want to turn off silence marking.  If you have not done so (for example, your recording only includes a single utterance) then you'll want to have the segmentation kit expect silence at the start and end of your recording.
+
+Sox - http://sox.sourceforge.net/
+ - Converts the sampling frequency of the audio if needed.
+ - Optional.  If you choose to not install sox, you'll need to make sure your audio files are at the same sampling frequency as the model data (the included data is 14khz)
+ - If you forced the script to run Julius on audio that has a different sampling frequency, the aligner would completely fail.
+
+Cabocha - http://taku910.github.io/cabocha/ 
+ - used to convert typical Japanese text into romaji/phones.
+ - (throw it into google translate if you need it in English)
+ - make a note of which encoding you use for the dictionary file--you'll need it in the code
+ - (you may need to configure cabocha post-install; see https://github.com/timmahrt/pyJuliusAlign/issues/7)
+
+Perl (for Julius)
+
+
+### Mac-specific Requirements Information
+
+I use a mac and was able to easily install many requirements using Homebrew.  Here are some guides that I found useful (they translate well enough from Japanese using google translate):
+ - Sox https://qiita.com/samurai20000@github/items/2af98b6c468af317bb09
+ - Cabocha https://qiita.com/musaprg/items/9a572ad5c4e28f79d2ae
+ - I manually built Julius using the configure and make scripts included in that project
+
+
+### Windows-specific Requirements Information
+
+I currently don't have access to a Windows machine. Earlier, I tested installation and got as far as running Julius. Perl tried to run gzip which I couldn't get to install.
+
+One user was able to get it working on Windows by installing cygwin and adding cygwin to the path in environment variables.  Also, they had to install MeCab before running Cabocha, otherwise, they would receive an exception saying there's something wrong with Cabocha.
+
+## Installation
+
+PyJuliusAlign is on pypi and can be installed or upgraded from the command-line shell with pip like so::
+
+    python -m pip install pyjuliusalign --upgrade
+
+Otherwise, to manually install, after downloading the source from github, from a command-line shell, navigate to the directory containing setup.py and type::
+
+    python setup.py install
+
+If python is not in your path, you'll need to enter the full path e.g.::
+
+	C:\Python36\python.exe setup.py install
+
+
+## Testing Installation
+
+In the folder 'examples' run the file 'align_example.py'.
+
+If sox, cabocha, julius, and perl are all in your path, you won't need to specify them in any of the arguments--leave them with your default values. Otherwise, you'll need to specify the full path of their bin/executable files.
+
+If you have difficulties running the code without specifying the full path, try using the full paths anyways.
+
+Also, you will need to configure "segment_julius.pl" which is a part of the Julius Segmentation Kit.
+
+
+## Example Usage
+
+Please see /examples for an example usage.
+
+There is pretty much only one way to use this library at the moment. Please contact me if you are having difficulties using this library.
+
+
+## Tests
+
+I run tests with the following command (this requires pytest and pytest-cov to be installed):
+
+`pytest --cov=pyjuliusalign tests/`
+
+
+## Troubleshooting
+
+The scripts should catch any issues along the way with the exception of issues stemming from Julius.  If you get bogus/null results, most likely Julius hasn't been set up correctly.
+
+The Julius Segmentation kit comes with an example.  If you can force align that, then you should be able to force align using this script as well.
+
+
+
```

### Comparing `pyjuliusalign-3.1.1/pyjuliusalign.egg-info/SOURCES.txt` & `pyjuliusalign-4.0.0/pyjuliusalign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjuliusalign-3.1.1/setup.py` & `pyjuliusalign-4.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,26 @@
 @author: tmahrt
 """
 from setuptools import setup
 import io
 
 setup(
     name="pyjuliusalign",
-    version="3.1.1",
+    python_requires=">3.6.0",
+    version="4.0.0",
     author="Tim Mahrt",
     author_email="timmahrt@gmail.com",
     url="https://github.com/timmahrt/pyJuliusAlign",
     package_dir={"pyjuliusalign": "pyjuliusalign"},
     packages=["pyjuliusalign"],
     package_data={"pyjuliusalign": ["hiraganaChart.txt", "katakanaChart.txt"]},
     license="LICENSE",
     description="A helper library for doing forced-alignment in Japanese with Julius.",
-    install_requires=["praatio ~= 4.1", "python-Levenshtein", "pydub"],
+    install_requires=[
+        "praatio ~= 6.0",
+        "python-Levenshtein",
+        "pydub",
+        "typing_extensions",
+    ],
     long_description=io.open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
 )
```

