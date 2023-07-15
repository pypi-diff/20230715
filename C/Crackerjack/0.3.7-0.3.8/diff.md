# Comparing `tmp/crackerjack-0.3.7.tar.gz` & `tmp/crackerjack-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.7.tar", last modified: Thu Jul 13 14:04:55 2023, max compression
+gzip compressed data, was "crackerjack-0.3.8.tar", last modified: Sat Jul 15 16:39:35 2023, max compression
```

## Comparing `crackerjack-0.3.7.tar` & `crackerjack-0.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.7/LICENSE
--rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.7/README.md
--rw-r--r--   0        0        0      243 2023-07-13 14:00:32.056242 crackerjack-0.3.7/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-07-13 14:00:32.094427 crackerjack-0.3.7/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2918 2023-07-13 14:00:32.078277 crackerjack-0.3.7/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.7/crackerjack/.pyanalyze-report.json
--rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.7/crackerjack/.pyanalyze-report.md
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.7/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.7/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.7/crackerjack/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.7/crackerjack/__main__.py
--rw-r--r--   0        0        0     6120 2023-07-09 13:10:21.246677 crackerjack-0.3.7/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1659 2023-07-13 14:00:32.992392 crackerjack-0.3.7/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2010 2023-07-13 14:04:55.130236 crackerjack-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.8/LICENSE
+-rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.8/README.md
+-rw-r--r--   0        0        0      233 2023-07-15 16:10:33.153833 crackerjack-0.3.8/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-07-15 16:10:33.184636 crackerjack-0.3.8/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2697 2023-07-15 16:10:33.169512 crackerjack-0.3.8/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.8/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.8/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.8/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.8/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.8/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.8/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6212 2023-07-15 16:04:48.965351 crackerjack-0.3.8/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1710 2023-07-15 16:10:33.923644 crackerjack-0.3.8/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2061 2023-07-15 16:39:35.644580 crackerjack-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.8/PKG-INFO
```

### Comparing `crackerjack-0.3.7/LICENSE` & `crackerjack-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.7/README.md` & `crackerjack-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.7/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.8/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.7/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.8/crackerjack/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pdm-project/pdm
-    rev: 2.8.0a2  # a PDM release exposing the hook
+    rev: 2.8.0  # a PDM release exposing the hook
     hooks:
       - id: pdm-lock-check
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
         name: trailing-whitspace
@@ -91,13 +91,7 @@
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: '23.7.0'
     hooks:
       - id: black
         language_version: python3.11
-  - repo: https://github.com/pdm-project/pdm
-    rev: 2.8.0a2 # a PDM release exposing the hook
-    hooks:
-      - id: pdm-export
-        args: [ '-o', 'requirements.txt', '--without-hashes' ]
-        files: ^pdm.lock$
```

### Comparing `crackerjack-0.3.7/crackerjack/.pyanalyze-report.json` & `crackerjack-0.3.8/crackerjack/.pyanalyze-report.json`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.7/crackerjack/.pyanalyze-report.md` & `crackerjack-0.3.8/crackerjack/.pyanalyze-report.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.7/crackerjack/__main__.py` & `crackerjack-0.3.8/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.7/crackerjack/crackerjack.py` & `crackerjack-0.3.8/crackerjack/crackerjack.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 from inflection import underscore
 from pydantic import BaseModel
 from pydantic import ConfigDict
 
 
 class Crakerjack(BaseModel):
     model_config: ConfigDict = ConfigDict(arbitrary_types_allowed=True)
-    our_path: AsyncPath = AsyncPath(__file__)
+    our_path: AsyncPath = AsyncPath(__file__).parent
     pkg_path: AsyncPath = AsyncPath.cwd()
     pkg_dir: t.Optional[AsyncPath] = None
     pkg_name: str = "crackerjack"
     our_toml: t.Optional[dict] = None
     pkg_toml: t.Optional[dict] = None
     our_toml_path: t.Optional[AsyncPath] = None
     pkg_toml_path: t.Optional[AsyncPath] = None
     poetry_pip_env: bool = False
 
     async def update_pyproject_configs(self) -> None:
         toml_file = "pyproject.toml"
-        self.our_toml_path = self.our_path.parent / toml_file
+        self.our_toml_path = self.our_path / toml_file
         self.pkg_toml_path = self.pkg_path / toml_file
         our_toml_config: t.Any = await load.toml(self.our_toml_path)  # type: ignore
         pkg_toml_config: t.Any = await load.toml(self.pkg_toml_path)  # type: ignore
         if self.poetry_pip_env:
             pkg_toml_config["tool"].pop("poetry")
         pkg_deps = pkg_toml_config["tool"]["pdm"]["dev-dependencies"]
         pkg_toml_config["tool"] = our_toml_config["tool"]
@@ -68,15 +68,15 @@
             ".gitignore",
             ".pre-commit-config.yaml",
             ".libcst.codemod.yaml",
             ".pyanalyze-report.json",
             ".pyanalyze-report.md",
         )
         for config in config_files:
-            config_path = self.our_path.parent / config
+            config_path = self.our_path / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
             if config in config_files[:-2]:
                 if self.pkg_path.stem == "crackerjack":
                     await config_path.write_text(await pkg_config_path.read_text())
                 # if poetry_pip_env:
                 #     await config_pkg_path.unlink()
@@ -108,14 +108,17 @@
         if not len([pkg for pkg in installed_pkgs if "pre-commit" in pkg]):
             run(["pdm", "self", "add", "keyring"])
             run(["pdm", "config", "python.use_venv", "false"])
             run(["git", "init"])
             run(["git", "branch", "-m", "main"])
             run(["git", "add", "pyproject.toml"])
             run(["pdm", "add", "-d", "pre_commit"])
+            run(["pdm", "add", "-d", "pytest"])
+            run(["pdm", "add", "-d", "pyanalyze"])
+            run(["pdm", "add", "-d", "autotyping"])
             run(["pre-commit", "install"])
             run(["git", "add", "pdm.lock"])
             run(["git", "config", "advice.addIgnoredFile", "false"])
         await self.update_pyproject_configs()
 
     async def process(self, options: t.Any) -> None:
         imp_dir = self.pkg_path / "__pypackages__"
@@ -134,15 +137,14 @@
         if options.interactive:
             for hook in ("refurb", "pyright"):
                 await self.run_interactive(hook)
         check_all = call(["pre-commit", "run", "--all-files"])
         if check_all > 0:
             call(["pre-commit", "run", "--all-files"])
         if options.publish:
-            run(["git", "add", "requirements.txt"])
             run(["pdm", "publish"])
         if options.commit:
             commit_msg = input("Commit message: ")
             call(["git", "commit", "-m", f"'{commit_msg}'", "--no-verify", "--", "."])
             call(["git", "push", "origin", "main"])
```

### Comparing `crackerjack-0.3.7/crackerjack/pyproject.toml` & `crackerjack-0.3.8/crackerjack/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.4.0",
     "icecream>=2.1.3",
     "pre-commit>=3.3.3",
+    "autotyping>=23.3.0",
+    "pyanalyze>=0.10.1",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -40,15 +42,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.7"
+version = "0.3.8"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -58,18 +60,18 @@
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "click>=8.1.4",
+    "click>=8.1.5",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
-    "pydantic>=2.0.2",
+    "pydantic>=2.0.3",
     "inflection>=0.5.1",
     "acb>=0.1.10",
     "tomli-w>=1.0.0",
     "pdm-bump>=0.7.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
```

### Comparing `crackerjack-0.3.7/pyproject.toml` & `crackerjack-0.3.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.4.0",
     "icecream>=2.1.3",
     "pre-commit>=3.3.3",
+    "autotyping>=23.3.0",
+    "pyanalyze>=0.10.1",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -59,15 +61,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.7"
+version = "0.3.8"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -77,18 +79,18 @@
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "click>=8.1.4",
+    "click>=8.1.5",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
-    "pydantic>=2.0.2",
+    "pydantic>=2.0.3",
     "inflection>=0.5.1",
     "acb>=0.1.10",
     "tomli-w>=1.0.0",
     "pdm-bump>=0.7.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
```

### Comparing `crackerjack-0.3.7/PKG-INFO` & `crackerjack-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.3.7
+Version: 0.3.8
 Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://github.com/lesleslie/crackerjack
 Project-URL: Documentation, https://github.com/lesleslie/crackerjack
 Project-URL: Repository, https://github.com/lesleslie/crackerjack
 Requires-Python: >=3.11
-Requires-Dist: click>=8.1.4
+Requires-Dist: click>=8.1.5
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: aioconsole>=0.6.1
-Requires-Dist: pydantic>=2.0.2
+Requires-Dist: pydantic>=2.0.3
 Requires-Dist: inflection>=0.5.1
 Requires-Dist: acb>=0.1.10
 Requires-Dist: tomli-w>=1.0.0
 Requires-Dist: pdm-bump>=0.7.1
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
```

