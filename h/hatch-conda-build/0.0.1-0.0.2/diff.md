# Comparing `tmp/hatch_conda_build-0.0.1.tar.gz` & `tmp/hatch_conda_build-0.0.2.tar.gz`

## Comparing `hatch_conda_build-0.0.1.tar` & `hatch_conda_build-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/hatch_conda_build/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/hatch_conda_build/__version__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/hatch_conda_build/config.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/hatch_conda_build/hooks.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/hatch_conda_build/plugin.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/tests/package-a/README.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/tests/package-a/pyproject.toml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/tests/package-a/package_a/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/README.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/__version__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/config.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/hooks.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/plugin.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/tests/test_hatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/PKG-INFO
```

### Comparing `hatch_conda_build-0.0.1/.github/workflows/release.yaml` & `hatch_conda_build-0.0.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

