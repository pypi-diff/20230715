# Comparing `tmp/mtg_scryfall_grabber-0.1.3.tar.gz` & `tmp/mtg_scryfall_grabber-1.0.0.tar.gz`

## Comparing `mtg_scryfall_grabber-0.1.3.tar` & `mtg_scryfall_grabber-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/license.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/mtg_scryfall_grabber.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/requirements.txt
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/setup.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/example/msfg.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/.gitignore
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/environment.yaml
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/license.md
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/mtg_scryfall_grabber.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/requirements.txt
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/example/msfg.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/.gitignore
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/README.md
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 mtg_scryfall_grabber-1.0.0/PKG-INFO
```

### Comparing `mtg_scryfall_grabber-0.1.3/license.md` & `mtg_scryfall_grabber-1.0.0/license.md`

 * *Files identical despite different names*

### Comparing `mtg_scryfall_grabber-0.1.3/.github/workflows/pylint.yml` & `mtg_scryfall_grabber-1.0.0/.github/workflows/pylint.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Pylint
+name: pylint
 
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
```

### Comparing `mtg_scryfall_grabber-0.1.3/example/msfg.py` & `mtg_scryfall_grabber-1.0.0/example/msfg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 #/opt/homebrew/bin/python3
 # pylint: disable=C0301
-
+# pylint: disable=C0303
+# pylint: disable=R0913
+# pylint: disable=R0914
+# pylint: disable=R0133
+# pylint: disable=R0124
 """
-Module for scraping usefull info off of the scryfall 
-REST API when invoked as a module, versus a library
+Example implementation of the mtg_scryfall_grabber module from @contrastellar
+https://pypi.org/project/mtg-scryfall-grabber/
 
 Author: Contrastellar (Gabriella Agathon)
 2023
 """
 
 import os
 import json
@@ -23,14 +27,29 @@
 def json_parse(obj) -> str:
     """
     Return a string object of the json passed in via obj
     """
     text = json.dumps(obj, sort_keys=True, indent=3)
     return text
 
+def file_name_creation(user_set, pull_card_info, pull_price_info) -> str:
+    """
+    Create a filename to be used during the output process
+    """
+    file_name = ""
+    file_name += user_set
+    if pull_card_info :
+        file_name += "_name"
+    if pull_price_info :
+        file_name += "_price"
+    file_name += "_"
+    file_name += str(int(time.time()))
+
+    return file_name
+
 # Consts
 PAGENUM = 1
 MODULE_DESCRIPTION = "Script to pull card info from api.scryfall.com based on specific set"
 
 def main():
     """
     main, allowing this to be invoked as a module from the command line.
@@ -116,21 +135,15 @@
 
     path = "output"
     does_exist = os.path.exists(path=path)
     if not does_exist:
         os.makedirs(path)
 
     # Create Filename based on arguments
-    file_name = ""
-    file_name += user_set
-    if pull_card_info :
-        file_name += "_name"
-    if pull_price_info :
-        file_name += "_price"
-    file_name += str(int(time.time()))
+    file_name = file_name_creation(user_set=user_set, pull_card_info=pull_card_info, pull_price_info=pull_price_info)
 
     # Writing to sample.json
     with open("output/" + file_name + ".json", "w", encoding="UTF8") as outfile:
         outfile.write(output_object)
 
 if __name__ == "__main__":
     main()
```

### Comparing `mtg_scryfall_grabber-0.1.3/.gitignore` & `mtg_scryfall_grabber-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_scryfall_grabber-0.1.3/pyproject.toml` & `mtg_scryfall_grabber-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mtg_scryfall_grabber"
-version = "0.1.3"
+version = "1.0.0"
 authors = [
   { name="Gabriella Agathon", email="gjstimac@gmail.com" },
 ]
 description = "MTG_Scryfall_Grabber (MSG) is a Python library/repository for scraping and organizing data from the Scryfall Rest-API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Contrastellar/mtg_scryfall_grabber"
 "Bug Tracker" = "https://github.com/Contrastellar/mtg_scryfall_grabber/issues"
+
+[tool.pytest.ini_options]
```

### Comparing `mtg_scryfall_grabber-0.1.3/PKG-INFO` & `mtg_scryfall_grabber-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,91 @@
-Metadata-Version: 2.1
-Name: mtg_scryfall_grabber
-Version: 0.1.3
-Summary: MTG_Scryfall_Grabber (MSG) is a Python library/repository for scraping and organizing data from the Scryfall Rest-API.
-Project-URL: Homepage, https://github.com/Contrastellar/mtg_scryfall_grabber
-Project-URL: Bug Tracker, https://github.com/Contrastellar/mtg_scryfall_grabber/issues
-Author-email: Gabriella Agathon <gjstimac@gmail.com>
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# mtg_scryfall_grabber
+[![Pylint](https://github.com/Contrastellar/mtg_scryfall_grabber/actions/workflows/pylint.yml/badge.svg?branch=main)](https://github.com/Contrastellar/mtg_scryfall_grabber/actions/workflows/pylint.yml)
+[![pytest](https://github.com/Contrastellar/mtg_scryfall_grabber/actions/workflows/pytest.yml/badge.svg)](https://github.com/Contrastellar/mtg_scryfall_grabber/actions/workflows/pytest.yml)
 
-# mtg-scryfall-grabber
+mtg_scryfall_grabber (MSG) is a Python library and module for scraping and organizing data from the Scryfall Rest-API.
 
-MTG-Scryfall-Grabber (MSG) is a Python library and module for scraping and organizing data from the Scryfall Rest-API.
+`conda` is not _needed_ but a sample `environment.yaml` is provided for the bare minimums you need to run in your own conda enviornment.
 
 ## Installation
 
 Please go to [Releases](https://github.com/Contrastellar/mtg-scryfall-grabber/releases) for the latest directories.
 
 Additionally, this can be installed from pip using
 
 ```bash
-python3 -m pip install mtg-scryfall-grabber
+python3 -m pip install mtg_scryfall_grabber
 ```
 
 
 ## Usage
 
 After installing via pip using 
 ```bash
-python3 -m pip install --upgrade mtg-scryfall-grabber
+python3 -m pip install --upgrade mtg_scryfall_grabber
 ```
 
 The functions from `mtg_scryfall_grabber.py` can be invoked using
 ```python
 import mtg_scryfall_grabber
 ```
 
-## Quickstart
+
+## Quickstart (/w conda)
+
+
+### conda install
+
+`conda` can be installed from [here](https://docs.conda.io/projects/conda/en/stable/user-guide/install/index.html)
+
+### Once conda is installed
+
+1. Clone the following repo
+```
+https://github.com/Contrastellar/mtg_scryfall_grabber
+```
+
+2. Navigate to the repo
+```sh
+cd ./mtg_scryfall_grabber/
+```
+
+3. Install the environment, where `$NAME_OF_ENVIRONMENT` is any name, or is omitted altogether, as one is given in the file.
+```sh
+conda env create --file ./environment.yaml --name $NAME_OF_ENVIRONMENT
+```
+
+4. Activate the environment
+```sh
+conda activate $NAME_OF_ENVIRONMENT
+```
+
+5. Navigate to the `./example/` directory
+```sh
+cd ./example/
+```
+
+6. Run the following OS dependant command to download the information for the set "Phyrexia, All Will Be One"
+### PowerShell
+```bash
+py msfg.py ONE -c -p
+```
+
+### Unix 
+```bash
+python3 msfg.py ONE -c -p
+```
+
+
+## Quickstart w/o conda
 To get started quickly, one must install Python 3 (version 3.8 or greater).
 
 Once having completed Python 3 installation for your Operating System, running the following command
 
-### WINDOWS PowerShell ---
+### PowerShell ---
 ```bash
 py -m pip install --upgrade mtg-scryfall-grabber
 ```
 
 ### MacOS/UNIX Terminal/bash ---
 ```bash
 python3 -m pip install --upgrade mtg-scryfall-grabber
@@ -55,35 +94,38 @@
 This will install mtg-scryfall-grabber's `mtg_scryfall_grabber` library, to be imported and used in your own Python Module if so desired.
 From here, downloading (either from releases, or from [cloning](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) this repository) the `example/msfg.py` file. Once this is done, the following steps can be taken to 'quickstart' downloading information from the Scryfall API.
 
 1. In your commandline (henceforth the CLI), navigate to the directory.
 ```bash
 cd $MTG_SCRYFALL_GRABBER_DOWNLOAD_LOCATION/example/
 ```
-2. Run the following command to download the information for "Phyrexia, All Will Be One"
-### WINDOWS PowerShell
+
+2. Run the following command to download the information for the set "Phyrexia, All Will Be One"
+### PowerShell
 ```bash
 py msfg.py ONE -c -p
 ```
 
 ### MacOS/UNIX Terminal/Bash
 ```bash
 python3 msfg.py ONE -c -p
 ```
 
-In `./example/`, this will create a directory named "output", which will contain a `.json` file named `Phyrexia: All Will Be One_card_name_price_$UNIX_TIME_OF_RUN.json` where `$UNIX_TIME_OF_RUN` is a time like `1679966043`.
+In `./example/`, this will create a directory named "output", which will contain a `.json` file named like `ONE_name_price_$(TIME).json` -- where it is compiled by set code + unix time.
+
 
 ## TODO
 
 Nothing else major needs to be done at this point, however polishing and code testing will be implemented to this library before this is considered a full, ready-to-be-used in production v.1 release.
 
-Additional functions need to be implimented, however -- an example implementation of this library is given in `./example/` under `msfg.py`. This implementation can also be treated as the "primary" method of using this library, in order to generate JSON to be used inside Excel spreadsheets.
+Additional functions need to be implimented, however -- an example implementation of this library is given in `./example/` under `msfg.py`. This implementation can also be treated as the "primary" method of using this library, in order to generate JSON to be used inside Excel spreadsheets or another spreadsheet program.
+
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 ## License
 The license is covered under the file [license.md](https://github.com/Contrastellar/mtg-scryfall-grabber/blob/main/license.md).
 
-In essence, please do not use this software for commercial (for profit) means. This library is provided as is, modifications to the source code are allowed. This is to follow the Wizards of the Coast's Fan Content Policy.
+In essence, please do not use this software for commercial (for profit) means. This library is provided as is, modifications to the source code are allowed. This is to follow the Wizards of the Coast's (WotC) Fan Content Policy. All modifications should be done in accordance with the WotC Fan Content Policy.
```

