# Comparing `tmp/conda_lock-2.1.0.tar.gz` & `tmp/conda_lock-2.1.1.tar.gz`

## Comparing `conda_lock-2.1.0.tar` & `conda_lock-2.1.1.tar`

### file list

```diff
@@ -1,556 +1,557 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.flake8
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.gitattributes
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 conda_lock-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 conda_lock-2.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.0/Dockerfile
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 conda_lock-2.1.0/DockerfileTest
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 conda_lock-2.1.0/codecov.yml
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 conda_lock-2.1.0/mkdocs.yml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 conda_lock-2.1.0/mypy.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 conda_lock-2.1.0/pyrightconfig.json
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 conda_lock-2.1.0/renovate.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 conda_lock-2.1.0/requirements-dev.txt
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.github/workflows/update-lockfile.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/__main__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/click_helpers.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/common.py
--rw-r--r--   0        0        0    50277 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/conda_lock.py
--rw-r--r--   0        0        0    20088 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/conda_solver.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/errors.py
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/invoke_conda.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/lookup.py
--rw-r--r--   0        0        0    13921 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/pypi_solver.py
--rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/virtual_package.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/LICENSES.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/cleo.LICENSE
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/cleo.pyi
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda.pyi
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry-core.LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry.LICENSE
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry.pyi
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/vendor.txt
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/cleo/LICENSE
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/cleo/io/io_mixin.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/.version
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/LICENSE
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/LICENSE.txt
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/__main__.py
--rw-r--r--   0        0        0    47200 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/activate.py
--rw-r--r--   0        0        0    17270 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/api.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/appdirs.LICENSE.txt
--rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/distro.LICENSE.txt
--rw-r--r--   0        0        0    53998 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/exceptions.py
--rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/exports.py
--rw-r--r--   0        0        0    15475 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/history.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/instructions.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/lock.py
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/misc.py
--rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/plan.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/py-cpuinfo.LICENSE
--rw-r--r--   0        0        0    66502 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/resolve.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/six.LICENSE
--rw-r--r--   0        0        0    19343 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/utils.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/__init__.py
--rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/appdirs.py
--rw-r--r--   0        0        0    39759 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/distro.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/six.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/boltons/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/boltons/__init__.py
--rw-r--r--   0        0        0    33620 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/boltons/setutils.py
--rw-r--r--   0        0        0    20478 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/cpuinfo/__init__.py
--rw-r--r--   0        0        0    83718 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py
--rw-r--r--   0        0        0    25343 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/recipes.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/utils.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/__main__.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/_main.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/_tqdm.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/auto.py
--rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/cli.py
--rw-r--r--   0        0        0    57572 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/std.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/utils.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/version.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/LICENSE
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/__init__.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/collection.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/compat.py
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/decorators.py
--rw-r--r--   0        0        0    33324 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/entity.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/exceptions.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/ish.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/logz.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/packaging.py
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/type_coercion.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/base/__init__.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/base/constants.py
--rw-r--r--   0        0        0    75564 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/base/context.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/base/exceptions.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/__init__.py
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/common.py
--rw-r--r--   0        0        0    59153 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/conda_argparse.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/find_commands.py
--rw-r--r--   0        0        0    16609 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/install.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main.py
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_clean.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_compare.py
--rw-r--r--   0        0        0    16627 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_config.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_create.py
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_info.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_init.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_install.py
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_list.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_notices.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_package.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_pip.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_remove.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_rename.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_run.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_search.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_update.py
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/cli/python_api.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/__init__.py
--rw-r--r--   0        0        0    26678 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/_logic.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/compat.py
--rw-r--r--   0        0        0    58130 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/configuration.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/constants.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/cuda.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/decorators.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/disk.py
--rw-r--r--   0        0        0    21968 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/io.py
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/logic.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/path.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/serialize.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/signals.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/toposort.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/url.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/_os/__init__.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/_os/linux.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/_os/unix.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/_os/windows.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/pkg_formats/__init__.py
--rw-r--r--   0        0        0    45704 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/common/pkg_formats/python.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/__init__.py
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/envs_manager.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/index.py
--rw-r--r--   0        0        0    61517 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/initialize.py
--rw-r--r--   0        0        0    58045 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/link.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/package_cache.py
--rw-r--r--   0        0        0    32215 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/package_cache_data.py
--rw-r--r--   0        0        0    57240 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/path_actions.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/portability.py
--rw-r--r--   0        0        0    16680 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/prefix_data.py
--rw-r--r--   0        0        0    71861 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/solve.py
--rw-r--r--   0        0        0    30211 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/core/subdir_data.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/__init__.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/anaconda_client.py
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/logging.py
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/subprocess.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/__init__.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/download.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/session.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/adapters/__init__.py
--rw-r--r--   0        0        0    11297 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/__init__.py
--rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/create.py
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/delete.py
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/link.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/permissions.py
--rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/read.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/test.py
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/update.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/__init__.py
--rw-r--r--   0        0        0    18571 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/channel.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/dist.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/enums.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/leased_path_entry.py
--rw-r--r--   0        0        0    35276 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/match_spec.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/package_info.py
--rw-r--r--   0        0        0    16650 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/prefix_graph.py
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/records.py
--rw-r--r--   0        0        0    24971 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/models/version.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/notices/__init__.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/notices/cache.py
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/notices/core.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/notices/http.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/notices/types.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/notices/views.py
--rw-r--r--   0        0        0    40960 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/cli-32.exe
--rw-r--r--   0        0        0    41984 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/cli-64.exe
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/conda.xsh
--rw-r--r--   0        0        0   126355 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/conda_icon.ico
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/Library/bin/conda.bat
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/Scripts/activate.bat
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/bin/activate
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/bin/conda
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/bin/deactivate
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/Conda.psm1
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/activate.bat
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/conda-hook.ps1
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/conda.bat
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/deactivate.bat
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/rename_tmp.bat
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/cases.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/decorators.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/fixtures.py
--rw-r--r--   0        0        0    29666 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/helpers.py
--rw-r--r--   0        0        0    16761 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/integration.py
--rw-r--r--   0        0        0    46730 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/solver_helpers.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/gateways/__init__.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/gateways/fixtures.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/notices/__init__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/notices/fixtures.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/testing/notices/helpers.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/trust/__init__.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/trust/constants.py
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/conda/trust/signature_verification.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/LICENSE
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/__version__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/exceptions.py
--rwxr-xr-x   0        0        0     5366 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/factory.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/locations.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/poetry.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/_vendor/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/config/__init__.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/config/config.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/config/config_source.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/config/dict_config_source.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/config/file_config_source.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/__init__.py
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/factory.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/poetry.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/_pyrsistent_version.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE
--rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/vendor.txt
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py
--rw-r--r--   0        0        0    88313 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/py.typed
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__main__.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py
--rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py
--rw-r--r--   0        0        0    29400 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/__init__.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/common.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py
--rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py
--rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py
--rw-r--r--   0        0        0    35346 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py
--rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py
--rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/__init__.py
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py
--rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py
--rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tools/__init__.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py
--rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py
--rw-r--r--   0        0        0    14643 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py
--rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/py.typed
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py
--rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py
--rw-r--r--   0        0        0    33853 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py
--rw-r--r--   0        0        0    42075 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_document.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/exceptions/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/exceptions/base.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/json/__init__.py
--rw-r--r--   0        0        0    20976 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/api.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builder.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/metadata.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builders/__init__.py
--rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builders/builder.py
--rw-r--r--   0        0        0    14530 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py
--rw-r--r--   0        0        0    13483 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/include.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/module.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/__init__.py
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/dependency.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/directory_dependency.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/file_dependency.py
--rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/package.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/project_package.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/specification.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/url_dependency.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/utils/__init__.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/utils/link.py
--rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/utils/utils.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/pyproject/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/pyproject/exceptions.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/pyproject/tables.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/pyproject/toml.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/__init__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/empty_constraint.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/exceptions.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/patterns.py
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version_constraint.py
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version_range.py
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version_union.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/__init__.py
--rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/license.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/updater.py
--rw-r--r--   0        0        0    30162 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/data/licenses.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/toml/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/toml/exceptions.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/toml/file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/_compat.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/helpers.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/patterns.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/toml_file.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/vcs/__init__.py
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/vcs/git.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/base.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/exceptions.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/helpers.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/legacy_version.py
--rw-r--r--   0        0        0    22972 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/markers.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/requirements.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/utils.py
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/grammars/__init__.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/grammars/markers.lark
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/inspection/__init__.py
--rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/inspection/info.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/__init__.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/authenticator.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/base_installer.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/chef.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/chooser.py
--rw-r--r--   0        0        0    24842 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/executor.py
--rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/installer.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/noop_installer.py
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/pip_installer.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/install.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/operation.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/uninstall.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/update.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/io/__init__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/io/null_io.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/json/__init__.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/layouts/__init__.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/layouts/layout.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/layouts/src.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/layouts/standard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/masonry/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/masonry/api.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/masonry/builders/__init__.py
--rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/masonry/builders/editable.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/__init__.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/assignment.py
--rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/failure.py
--rw-r--r--   0        0        0    16149 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/incompatibility.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py
--rwxr-xr-x   0        0        0     7506 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/partial_solution.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/result.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/set_relation.py
--rwxr-xr-x   0        0        0     6132 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/term.py
--rwxr-xr-x   0        0        0    18984 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/version_solver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/solutions/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/packages/__init__.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/packages/dependency_package.py
--rw-r--r--   0        0        0    22709 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/packages/locker.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/packages/package_collection.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/puzzle/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/puzzle/exceptions.py
--rwxr-xr-x   0        0        0    29291 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/puzzle/provider.py
--rw-r--r--   0        0        0    16301 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/puzzle/solver.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/__init__.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/base_repository.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/exceptions.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/installed_repository.py
--rwxr-xr-x   0        0        0    12943 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/legacy_repository.py
--rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/pool.py
--rwxr-xr-x   0        0        0    16575 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/pypi_repository.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/remote_repository.py
--rwxr-xr-x   0        0        0     3408 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/__init__.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/_compat.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/appdirs.py
--rw-r--r--   0        0        0    54820 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/env.py
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/exporter.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/extras.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/helpers.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/password_manager.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/patterns.py
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/setup_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/version/__init__.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/_vendor/poetry/version/version_selector.py
--rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/lockfile/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/lockfile/v1/models.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/lockfile/v2prelim/models.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/models/__init__.py
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/models/channel.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/models/lock_spec.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/README.md
--rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/migration.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/requirements.txt
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/vendor_helpers.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/patches/poetry.patch
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/src_parser/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/src_parser/aggregation.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/src_parser/conda_common.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/src_parser/environment_yaml.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/src_parser/meta_yaml.py
--rw-r--r--   0        0        0    20022 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/src_parser/pyproject_toml.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 conda_lock-2.1.0/conda_lock/src_parser/selectors.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/authenticated_channels.md
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/docker.md
--rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/flags.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/getting_started.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/index.md
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/output.md
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/pip.md
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/src_environment_yml.md
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/src_meta_yaml.md
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/src_pyproject.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/cli/gen.md
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.0/docs/flags/strip-auth.md
--rw-r--r--   0        0        0   305465 2020-02-02 00:00:00.000000 conda_lock-2.1.0/environments/conda-lock.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 conda_lock-2.1.0/environments/dev-environment.yaml
--rw-r--r--   0        0        0   324897 2020-02-02 00:00:00.000000 conda_lock-2.1.0/example/pangeo/conda-lock.yml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 conda_lock-2.1.0/example/pangeo/environment.yml
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 conda_lock-2.1.0/example/zlib/conda-lock.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 conda_lock-2.1.0/example/zlib/environment.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 conda_lock-2.1.0/.gitignore
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 conda_lock-2.1.0/LICENSE
--rw-r--r--   0        0        0    15287 2020-02-02 00:00:00.000000 conda_lock-2.1.0/README.md
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 conda_lock-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 conda_lock-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.flake8
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.gitattributes
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 conda_lock-2.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 conda_lock-2.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.1/Dockerfile
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 conda_lock-2.1.1/DockerfileTest
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 conda_lock-2.1.1/codecov.yml
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 conda_lock-2.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 conda_lock-2.1.1/mypy.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 conda_lock-2.1.1/pyrightconfig.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 conda_lock-2.1.1/renovate.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 conda_lock-2.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.github/workflows/update-lockfile.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/__main__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/click_helpers.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/common.py
+-rw-r--r--   0        0        0    50388 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/conda_lock.py
+-rw-r--r--   0        0        0    20109 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/conda_solver.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/errors.py
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/invoke_conda.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lookup.py
+-rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/pypi_solver.py
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/virtual_package.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/LICENSES.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo.LICENSE
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo.pyi
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda.pyi
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry-core.LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry.LICENSE
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry.pyi
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/vendor.txt
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo/LICENSE
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/cleo/io/io_mixin.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/.version
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE.txt
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/__main__.py
+-rw-r--r--   0        0        0    47200 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/activate.py
+-rw-r--r--   0        0        0    17270 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/api.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/appdirs.LICENSE.txt
+-rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/distro.LICENSE.txt
+-rw-r--r--   0        0        0    53998 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/exceptions.py
+-rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/exports.py
+-rw-r--r--   0        0        0    15475 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/history.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/instructions.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/lock.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/misc.py
+-rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/plan.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/py-cpuinfo.LICENSE
+-rw-r--r--   0        0        0    66502 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/resolve.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/six.LICENSE
+-rw-r--r--   0        0        0    19343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/utils.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/__init__.py
+-rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/appdirs.py
+-rw-r--r--   0        0        0    39759 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/distro.py
+-rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/six.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/__init__.py
+-rw-r--r--   0        0        0    33620 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/setutils.py
+-rw-r--r--   0        0        0    20478 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/cpuinfo/__init__.py
+-rw-r--r--   0        0        0    83718 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py
+-rw-r--r--   0        0        0    25343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/recipes.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/utils.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/__main__.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_main.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_tqdm.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/auto.py
+-rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/cli.py
+-rw-r--r--   0        0        0    57572 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/std.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/utils.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/version.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/LICENSE
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/__init__.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/collection.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/compat.py
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/decorators.py
+-rw-r--r--   0        0        0    33324 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/entity.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/exceptions.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/ish.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/logz.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/packaging.py
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/type_coercion.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/__init__.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/constants.py
+-rw-r--r--   0        0        0    75564 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/context.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/base/exceptions.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/__init__.py
+-rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/common.py
+-rw-r--r--   0        0        0    59153 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/conda_argparse.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/find_commands.py
+-rw-r--r--   0        0        0    16609 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/install.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main.py
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_clean.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_compare.py
+-rw-r--r--   0        0        0    16627 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_config.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_create.py
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_info.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_init.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_install.py
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_notices.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_package.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_pip.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_remove.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_rename.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_run.py
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_search.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_update.py
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/cli/python_api.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/__init__.py
+-rw-r--r--   0        0        0    26678 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_logic.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/compat.py
+-rw-r--r--   0        0        0    58130 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/configuration.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/constants.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/cuda.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/decorators.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/disk.py
+-rw-r--r--   0        0        0    21968 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/io.py
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/logic.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/path.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/serialize.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/signals.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/toposort.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/url.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/__init__.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/linux.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/unix.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/windows.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/pkg_formats/__init__.py
+-rw-r--r--   0        0        0    45704 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/common/pkg_formats/python.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/__init__.py
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/envs_manager.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/index.py
+-rw-r--r--   0        0        0    61517 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/initialize.py
+-rw-r--r--   0        0        0    58045 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/link.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/package_cache.py
+-rw-r--r--   0        0        0    32215 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/package_cache_data.py
+-rw-r--r--   0        0        0    57240 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/path_actions.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/portability.py
+-rw-r--r--   0        0        0    16680 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/prefix_data.py
+-rw-r--r--   0        0        0    71861 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/solve.py
+-rw-r--r--   0        0        0    30211 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/core/subdir_data.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/__init__.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/anaconda_client.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/logging.py
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/subprocess.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/__init__.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/download.py
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/session.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/__init__.py
+-rw-r--r--   0        0        0    11297 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/__init__.py
+-rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/create.py
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/delete.py
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/link.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/permissions.py
+-rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/read.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/test.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/update.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/__init__.py
+-rw-r--r--   0        0        0    18571 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/channel.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/dist.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/enums.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/leased_path_entry.py
+-rw-r--r--   0        0        0    35276 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/match_spec.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/package_info.py
+-rw-r--r--   0        0        0    16650 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/prefix_graph.py
+-rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/records.py
+-rw-r--r--   0        0        0    24971 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/models/version.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/__init__.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/cache.py
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/core.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/http.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/types.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/notices/views.py
+-rw-r--r--   0        0        0    40960 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-32.exe
+-rw-r--r--   0        0        0    41984 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-64.exe
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda.xsh
+-rw-r--r--   0        0        0   126355 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda_icon.ico
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/Library/bin/conda.bat
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/Scripts/activate.bat
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/bin/activate
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/bin/conda
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/bin/deactivate
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/Conda.psm1
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/activate.bat
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda-hook.ps1
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda.bat
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/deactivate.bat
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/rename_tmp.bat
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/cases.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/decorators.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/fixtures.py
+-rw-r--r--   0        0        0    29666 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/helpers.py
+-rw-r--r--   0        0        0    16761 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/integration.py
+-rw-r--r--   0        0        0    46730 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/solver_helpers.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/gateways/__init__.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/gateways/fixtures.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/__init__.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/fixtures.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/helpers.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/trust/__init__.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/trust/constants.py
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/conda/trust/signature_verification.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/LICENSE
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/__version__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/exceptions.py
+-rwxr-xr-x   0        0        0     5366 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/factory.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/locations.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/poetry.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/_vendor/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/__init__.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/config.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/config_source.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/dict_config_source.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/config/file_config_source.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/__init__.py
+-rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/factory.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/poetry.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/_pyrsistent_version.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE
+-rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/vendor.txt
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py
+-rw-r--r--   0        0        0    88313 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/py.typed
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__main__.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py
+-rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py
+-rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py
+-rw-r--r--   0        0        0    29400 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__init__.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/common.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py
+-rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py
+-rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py
+-rw-r--r--   0        0        0    35346 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py
+-rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py
+-rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/__init__.py
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py
+-rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/__init__.py
+-rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py
+-rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py
+-rw-r--r--   0        0        0    14643 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py
+-rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/py.typed
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py
+-rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py
+-rw-r--r--   0        0        0    33853 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py
+-rw-r--r--   0        0        0    42075 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_document.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/exceptions/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/exceptions/base.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/__init__.py
+-rw-r--r--   0        0        0    20976 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/api.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builder.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/metadata.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/__init__.py
+-rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/builder.py
+-rw-r--r--   0        0        0    14530 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py
+-rw-r--r--   0        0        0    13483 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/include.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/module.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/__init__.py
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/dependency.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/directory_dependency.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/file_dependency.py
+-rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/package.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/project_package.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/specification.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/url_dependency.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/__init__.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/link.py
+-rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/utils.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/exceptions.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/tables.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/toml.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/__init__.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/empty_constraint.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/exceptions.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/patterns.py
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_constraint.py
+-rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_range.py
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_union.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/__init__.py
+-rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/license.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/updater.py
+-rw-r--r--   0        0        0    30162 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/data/licenses.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/exceptions.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/_compat.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/helpers.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/patterns.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/toml_file.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/__init__.py
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/git.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/base.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/exceptions.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/helpers.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/legacy_version.py
+-rw-r--r--   0        0        0    22972 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/markers.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/requirements.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/utils.py
+-rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/__init__.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/markers.lark
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/inspection/__init__.py
+-rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/inspection/info.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/__init__.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/authenticator.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/base_installer.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chef.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chooser.py
+-rw-r--r--   0        0        0    24842 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/executor.py
+-rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/installer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/noop_installer.py
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/pip_installer.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/install.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/operation.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/uninstall.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/update.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/io/__init__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/io/null_io.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/json/__init__.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/__init__.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/layout.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/src.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/api.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/builders/__init__.py
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/builders/editable.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/__init__.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/assignment.py
+-rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/failure.py
+-rw-r--r--   0        0        0    16149 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py
+-rwxr-xr-x   0        0        0     7506 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/partial_solution.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/result.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/set_relation.py
+-rwxr-xr-x   0        0        0     6132 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/term.py
+-rwxr-xr-x   0        0        0    18984 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/version_solver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/__init__.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/dependency_package.py
+-rw-r--r--   0        0        0    22709 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/locker.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/package_collection.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/exceptions.py
+-rwxr-xr-x   0        0        0    29291 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/provider.py
+-rw-r--r--   0        0        0    16301 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/solver.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/__init__.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/base_repository.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/exceptions.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/installed_repository.py
+-rwxr-xr-x   0        0        0    12943 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/legacy_repository.py
+-rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pool.py
+-rwxr-xr-x   0        0        0    16575 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pypi_repository.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/remote_repository.py
+-rwxr-xr-x   0        0        0     3408 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/__init__.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/_compat.py
+-rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/appdirs.py
+-rw-r--r--   0        0        0    54820 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/env.py
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/exporter.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/extras.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/helpers.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/password_manager.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/patterns.py
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/setup_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/version/__init__.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/_vendor/poetry/version/version_selector.py
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lockfile/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lockfile/v1/models.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/lockfile/v2prelim/models.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/models/__init__.py
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/models/channel.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/models/lock_spec.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/README.md
+-rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/migration.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/requirements.txt
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/vendor_helpers.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry.patch
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/aggregation.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/conda_common.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/environment_yaml.py
+-rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/meta_yaml.py
+-rw-r--r--   0        0        0    20022 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/pyproject_toml.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 conda_lock-2.1.1/conda_lock/src_parser/selectors.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/authenticated_channels.md
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/docker.md
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/flags.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/getting_started.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/index.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/output.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/pip.md
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/scipy-2023.md
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/src_environment_yml.md
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/src_meta_yaml.md
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/src_pyproject.md
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/cli/gen.md
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 conda_lock-2.1.1/docs/flags/strip-auth.md
+-rw-r--r--   0        0        0   305465 2020-02-02 00:00:00.000000 conda_lock-2.1.1/environments/conda-lock.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 conda_lock-2.1.1/environments/dev-environment.yaml
+-rw-r--r--   0        0        0   324897 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/pangeo/conda-lock.yml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/pangeo/environment.yml
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/zlib/conda-lock.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 conda_lock-2.1.1/example/zlib/environment.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 conda_lock-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 conda_lock-2.1.1/LICENSE
+-rw-r--r--   0        0        0    15293 2020-02-02 00:00:00.000000 conda_lock-2.1.1/README.md
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 conda_lock-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17290 2020-02-02 00:00:00.000000 conda_lock-2.1.1/PKG-INFO
```

### Comparing `conda_lock-2.1.0/CODE_OF_CONDUCT.md` & `conda_lock-2.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/CONTRIBUTING.md` & `conda_lock-2.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/mkdocs.yml` & `conda_lock-2.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/mypy.ini` & `conda_lock-2.1.1/mypy.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 [mypy]
 plugins = pydantic.mypy
-disallow_untyped_defs = true
 # disallow_untyped_calls = true
 # disallow_untyped_decorators = false
-disallow_incomplete_defs = true
+disallow_untyped_defs = false
+disallow_untyped_calls = false
+disallow_untyped_decorators = false
+disallow_incomplete_defs = false
 check_untyped_defs = true
 exclude = (?x)(
     tests/test-local-pip/setup.py
   )
 
+[mypy-conda_lock.*]
+disallow_untyped_defs = true
+# disallow_untyped_calls = true
+# disallow_untyped_decorators = true
+disallow_incomplete_defs = true
+
 [pydantic-mypy]
 init_forbid_extra = True
 init_typed = True
 warn_required_dynamic_aliases = True
 warn_untyped_fields = True
 
 [mypy-conda_lock._vendor.*]
@@ -32,12 +40,8 @@
 
 [mypy-flaky.*]
 ignore_missing_imports = True
 
 [mypy-click_default_group.*]
 ignore_missing_imports = True
 
-[mypy-test_conda_lock]
-disallow_untyped_defs = false
-disallow_untyped_calls = false
-disallow_untyped_decorators = false
-disallow_incomplete_defs = false
+[mypy-tests.*]
```

### Comparing `conda_lock-2.1.0/.github/workflows/mkdocs.yml` & `conda_lock-2.1.1/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/.github/workflows/release.yaml` & `conda_lock-2.1.1/.github/workflows/release.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -33,11 +33,11 @@
     - name: Test wheels
       run: |
         python -m twine check dist/*
       shell: bash
 
     - name: Publish a Python distribution to PyPI
       if: ${{ github.event_name == 'release' }}
-      uses: pypa/gh-action-pypi-publish@v1.8.6
+      uses: pypa/gh-action-pypi-publish@v1.8.8
       with:
         user: __token__
         password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `conda_lock-2.1.0/.github/workflows/test.yml` & `conda_lock-2.1.1/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   # concurrency group while a previous build is running it will be canceled.
   # Repeated pushes to a PR will cancel all previous builds, while multiple
   # merges to main will not cancel.
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 env:
-  MICROMAMBA_VERSION: '1.4.2-2'
+  MICROMAMBA_VERSION: 'latest'
 
 jobs:
   test-windows:
     env:
       PYTHONUNBUFFERED: "1"
       FORCE_COLOR: "1"
     runs-on: windows-latest
@@ -84,41 +84,42 @@
             python=${{ matrix.python-version }}
             mamba
             pip
             pytest-cov
             pytest-xdist
 
       - name: Install dev deps
+        shell: bash -eo pipefail -l {0}
         run: |
           set -x
           echo "${PATH}"
           which pip
           which python
           python -m pip install -r requirements-dev.txt
 
       - name: install conda-lock
-        shell: bash -l {0}
+        shell: bash -eo pipefail -l {0}
         run: |
           which pip
           pip install -e . --force-reinstall
 
       - name: run-test
-        shell: bash -l {0}
+        shell: bash -eo pipefail -l {0}
         run: |
           cp pyproject.toml "${RUNNER_TEMP}/"
           cp -a tests "${RUNNER_TEMP}/"
           pushd "${RUNNER_TEMP}"
           export TMPDIR="${RUNNER_TEMP}"
           ls -lah
           set -x
           which pytest
           pytest --cov=conda_lock --cov-branch --cov-report=xml --cov-report=term tests
           cp coverage.xml "${GITHUB_WORKSPACE}"
       - uses: codecov/codecov-action@v3
 
       - name: test-gdal
-        shell: bash -l {0}
+        shell: bash -eo pipefail -l {0}
         run: |
           pushd "${RUNNER_TEMP}/tests/gdal"
           export TMPDIR="${RUNNER_TEMP}"
           ls -lah
           conda-lock --mamba  -f environment.yml -p linux-64
```

### Comparing `conda_lock-2.1.0/.github/workflows/update-lockfile.yaml` & `conda_lock-2.1.1/.github/workflows/update-lockfile.yaml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/click_helpers.py` & `conda_lock-2.1.1/conda_lock/click_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/common.py` & `conda_lock-2.1.1/conda_lock/common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/conda_lock.py` & `conda_lock-2.1.1/conda_lock/conda_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -975,15 +975,15 @@
     with temporary_file_with_contents("\n".join(content) + "\n") as path:
         yield path
 
 
 def run_lock(
     environment_files: List[pathlib.Path],
     *,
-    conda_exe: Optional[str],
+    conda_exe: Optional[PathLike],
     platforms: Optional[List[str]] = None,
     mamba: bool = False,
     micromamba: bool = False,
     include_dev_dependencies: bool = True,
     channel_overrides: Optional[Sequence[str]] = None,
     filename_template: Optional[str] = None,
     kinds: Optional[Sequence[TKindAll]] = None,
@@ -1235,15 +1235,18 @@
     with_cuda: Optional[str] = None,
     update: Optional[List[str]] = None,
     metadata_choices: Sequence[str] = (),
     metadata_yamls: Sequence[pathlib.Path] = (),
 ) -> None:
     """Generate fully reproducible lock files for conda environments.
 
-    By default, the lock files are written to conda-{platform}.lock. These filenames can be customized using the
+    By default, a multi-platform lock file is written to conda-lock.yml.
+
+    When choosing the "explicit" or "env" kind, lock files are written to
+    conda-{platform}.lock. These filenames can be customized using the
     --filename-template argument. The following tokens are available:
 
     \b
         platform: The platform this lock file was generated for (conda subdir).
         dev-dependencies: Whether or not dev dependencies are included in this lock file.
         input-hash: A sha256 hash of the lock file input specification.
         version: The version of conda-lock used to generate this lock file.
```

### Comparing `conda_lock-2.1.0/conda_lock/conda_solver.py` & `conda_lock-2.1.1/conda_lock/conda_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,15 +488,15 @@
                 proc.check_returncode()
             except subprocess.CalledProcessError as exc:
                 err_json = json.loads(proc.stdout)
                 raise RuntimeError(
                     f"Could not lock the environment for platform {platform}: {err_json.get('message')}"
                 ) from exc
 
-            dryrun_install: DryRunInstall = json.loads(proc.stdout)
+            dryrun_install: DryRunInstall = json.loads(extract_json_object(proc.stdout))
         else:
             dryrun_install = {"actions": {"LINK": [], "FETCH": []}}
 
         if "actions" not in dryrun_install:
             dryrun_install["actions"] = {"LINK": [], "FETCH": []}
 
         updated = {entry["name"]: entry for entry in dryrun_install["actions"]["LINK"]}
```

### Comparing `conda_lock-2.1.0/conda_lock/invoke_conda.py` & `conda_lock-2.1.1/conda_lock/invoke_conda.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,26 @@
 
     if _conda_exe is None:
         return None
     return pathlib.Path(_conda_exe)
 
 
 def _determine_conda_executable(
-    conda_executable: Optional[str], mamba: bool, micromamba: bool
+    conda_executable: Optional[PathLike], mamba: bool, micromamba: bool
 ) -> Iterator[Optional[PathLike]]:
     if conda_executable:
         if pathlib.Path(conda_executable).exists():
             yield conda_executable
         yield shutil.which(conda_executable)
 
     yield _ensureconda(mamba=mamba, micromamba=micromamba, conda=True, conda_exe=True)
 
 
 def determine_conda_executable(
-    conda_executable: Optional[str], mamba: bool, micromamba: bool
+    conda_executable: Optional[PathLike], mamba: bool, micromamba: bool
 ) -> PathLike:
     for candidate in _determine_conda_executable(conda_executable, mamba, micromamba):
         if candidate is not None:
             if is_micromamba(candidate):
                 if determine_micromamba_version(str(candidate)) < LooseVersion("0.17"):
                     mamba_root_prefix()
             return candidate
```

### Comparing `conda_lock-2.1.0/conda_lock/lookup.py` & `conda_lock-2.1.1/conda_lock/lookup.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/pypi_solver.py` & `conda_lock-2.1.1/conda_lock/pypi_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional
 from urllib.parse import urldefrag
 
 from clikit.api.io.flags import VERY_VERBOSE
 from clikit.io import ConsoleIO, NullIO
-from packaging.tags import compatible_tags, cpython_tags
+from packaging.tags import compatible_tags, cpython_tags, mac_platforms
 
 from conda_lock._vendor.poetry.core.packages import Dependency as PoetryDependency
 from conda_lock._vendor.poetry.core.packages import Package as PoetryPackage
 from conda_lock._vendor.poetry.core.packages import (
     ProjectPackage as PoetryProjectPackage,
 )
 from conda_lock._vendor.poetry.core.packages import URLDependency as PoetryURLDependency
@@ -36,57 +36,51 @@
 
 if TYPE_CHECKING:
     from packaging.tags import Tag
 
 
 # NB: in principle these depend on the glibc in the conda env
 MANYLINUX_TAGS = ["1", "2010", "2014", "_2_17"]
+# This needs to be updated periodically as new macOS versions are released.
+MACOS_VERSION = (13, 4)
 
 
 class PlatformEnv(Env):
     """
     Fake poetry Env to match PyPI distributions to the target conda environment
     """
 
     def __init__(self, python_version: str, platform: str):
         super().__init__(path=Path(sys.prefix))
-        if platform.startswith("linux-"):
-            arch = platform.split("-")[-1]
-            if arch == "64":
-                arch = "x86_64"
+        system, arch = platform.split("-")
+        if arch == "64":
+            arch = "x86_64"
+
+        if system == "linux":
             self._platforms = [
                 f"manylinux{tag}_{arch}" for tag in reversed(MANYLINUX_TAGS)
             ]
             self._platforms.append(f"linux_{arch}")
-        elif platform == "osx-64":
-            self._platforms = [
-                "macosx_10_9_x86_64",
-                *(f"macosx_10_{version}_universal2" for version in range(16, 3, -1)),
-                *(f"macosx_10_{version}_universal" for version in range(16, 3, -1)),
-            ]
-        elif platform == "osx-arm64":
-            self._platforms = [
-                "macosx_11_0_arm64",
-                *(f"macosx_10_{version}_universal2" for version in range(16, 3, -1)),
-            ]
+        elif system == "osx":
+            self._platforms = list(mac_platforms(MACOS_VERSION, arch))
         elif platform == "win-64":
             self._platforms = ["win_amd64"]
         else:
             raise ValueError(f"Unsupported platform '{platform}'")
         self._python_version = tuple(map(int, python_version.split(".")))
 
-        if platform.startswith("osx-"):
+        if system == "osx":
             self._sys_platform = "darwin"
             self._platform_system = "Darwin"
             self._os_name = "posix"
-        elif platform.startswith("linux-"):
+        elif system == "linux":
             self._sys_platform = "linux"
             self._platform_system = "Linux"
             self._os_name = "posix"
-        elif platform.startswith("win-"):
+        elif system == "win":
             self._sys_platform = "win32"
             self._platform_system = "Windows"
             self._os_name = "nt"
         else:
             raise ValueError(f"Unsupported platform '{platform}'")
 
     def get_supported_tags(self) -> List["Tag"]:
```

### Comparing `conda_lock-2.1.0/conda_lock/virtual_package.py` & `conda_lock-2.1.1/conda_lock/virtual_package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/LICENSES.md` & `conda_lock-2.1.1/conda_lock/_vendor/LICENSES.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/cleo.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/cleo.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry-core.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry-core.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/cleo/LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/cleo/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/cleo/io/io_mixin.py` & `conda_lock-2.1.1/conda_lock/_vendor/cleo/io/io_mixin.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/LICENSE.txt` & `conda_lock-2.1.1/conda_lock/_vendor/conda/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/activate.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/activate.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/api.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/appdirs.LICENSE.txt` & `conda_lock-2.1.1/conda_lock/_vendor/conda/appdirs.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/distro.LICENSE.txt` & `conda_lock-2.1.1/conda_lock/_vendor/conda/distro.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/exceptions.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/exports.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/exports.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/history.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/history.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/instructions.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/instructions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/lock.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/lock.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/misc.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/misc.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/plan.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/plan.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/py-cpuinfo.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/conda/py-cpuinfo.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/resolve.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/resolve.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/six.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/conda/six.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/appdirs.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/distro.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/six.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/boltons/LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/boltons/setutils.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/setutils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/boltons/timeutils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/cpuinfo/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/frozendict/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/toolz/recipes.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/asyncio.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/cli.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/cli.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/std.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/_vendor/tqdm/utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/_vendor/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/collection.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/collection.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/decorators.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/decorators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/entity.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/entity.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/exceptions.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/ish.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/ish.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/logz.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/logz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/packaging.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/packaging.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/auxlib/type_coercion.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/auxlib/type_coercion.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/base/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/base/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/base/constants.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/base/constants.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/base/context.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/base/context.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/common.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/conda_argparse.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/conda_argparse.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/find_commands.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/find_commands.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/install.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/install.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_clean.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_clean.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_compare.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_compare.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_config.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_config.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_create.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_create.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_info.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_init.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_init.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_install.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_install.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_list.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_list.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_package.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_pip.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_pip.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_remove.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_remove.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_rename.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_rename.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_run.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_search.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_search.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/main_update.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/main_update.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/cli/python_api.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/cli/python_api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/_logic.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_logic.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/configuration.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/configuration.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/constants.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/constants.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/cuda.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/cuda.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/decorators.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/decorators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/disk.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/disk.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/io.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/io.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/logic.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/logic.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/path.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/path.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/serialize.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/serialize.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/signals.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/signals.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/toposort.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/toposort.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/url.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/url.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/_os/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/_os/linux.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/linux.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/_os/windows.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/_os/windows.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/common/pkg_formats/python.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/common/pkg_formats/python.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/envs_manager.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/envs_manager.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/index.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/index.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/initialize.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/initialize.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/link.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/link.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/package_cache_data.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/package_cache_data.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/path_actions.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/path_actions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/portability.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/portability.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/prefix_data.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/prefix_data.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/solve.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/solve.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/core/subdir_data.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/core/subdir_data.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/anaconda_client.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/anaconda_client.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/logging.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/logging.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/subprocess.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/subprocess.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/download.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/download.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/session.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/session.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/ftp.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/localfs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/connection/adapters/s3.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/create.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/create.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/delete.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/delete.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/link.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/link.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/permissions.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/permissions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/read.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/read.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/test.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/test.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/gateways/disk/update.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/gateways/disk/update.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/channel.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/channel.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/dist.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/dist.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/enums.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/enums.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/leased_path_entry.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/leased_path_entry.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/match_spec.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/match_spec.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/package_info.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/package_info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/prefix_graph.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/prefix_graph.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/records.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/records.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/models/version.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/models/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/notices/cache.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/cache.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/notices/core.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/core.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/notices/http.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/http.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/notices/types.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/types.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/notices/views.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/notices/views.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/cli-32.exe` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-32.exe`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/cli-64.exe` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/cli-64.exe`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/conda.xsh` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda.xsh`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/conda_icon.ico` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/conda_icon.ico`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/Scripts/activate.bat` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/Conda.psm1` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/Conda.psm1`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/_conda_activate.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/conda.bat` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_auto_activate.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/condabin/conda_hook.bat`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/fish/conf.d/conda.fish`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.csh`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh` & `conda_lock-2.1.1/conda_lock/_vendor/conda/shell/etc/profile.d/conda.sh`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/decorators.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/fixtures.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/integration.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/integration.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/solver_helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/solver_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/gateways/fixtures.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/gateways/fixtures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/notices/fixtures.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/fixtures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/testing/notices/helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/testing/notices/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/trust/constants.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/trust/constants.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/conda/trust/signature_verification.py` & `conda_lock-2.1.1/conda_lock/_vendor/conda/trust/signature_verification.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/factory.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/factory.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/locations.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/locations.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/poetry.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/poetry.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/config/config.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/config/config.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/config/dict_config_source.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/config/dict_config_source.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/config/file_config_source.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/config/file_config_source.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/factory.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/factory.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/poetry.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/poetry.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attrs.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark-parser.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/vendor.txt` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/vendor.txt`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_config.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_make.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_next_gen.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/converters.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/filters.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/setters.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/attr/validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/COPYING`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_format.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_legacy_validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_reflect.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_types.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/cli.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/validators.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/benchmarks/issue232.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft3.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft4.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft6.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/jsonschema/schemas/draft7.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/common.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammar.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/indenter.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lark.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/lexer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/load_grammar.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parse_tree_builder.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parser_frontends.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/reconstruct2.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tree.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/visitors.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/grammars/common.lark`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/cyk.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/earley_forest.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/grammar_analysis.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_analysis.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_parser.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/lalr_puppet.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/parsers/xearley.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/nearley.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/serialize.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/lark/tools/standalone.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_checked_types.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_field_common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_immutable.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pbag.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pclass.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pdeque.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_plist.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pmap.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_precord.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pset.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_pvector.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_toolz.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/_transformations.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/pyrsistent/typing.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/_utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/container.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/items.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/parser.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/source.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_char.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/_vendor/tomlkit/toml_file.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/json/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/json/schemas/poetry-schema.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/api.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builder.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builder.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/metadata.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/metadata.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builders/builder.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/builder.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/include.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/include.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/module.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/module.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/masonry/utils/package_include.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/dependency.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/directory_dependency.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/directory_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/file_dependency.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/file_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/package.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/project_package.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/project_package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/specification.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/specification.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/url_dependency.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/url_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/vcs_dependency.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/any_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/base_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/multi_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/constraints/union_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/utils/link.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/link.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/packages/utils/utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/packages/utils/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/pyproject/tables.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/tables.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/pyproject/toml.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/pyproject/toml.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/empty_constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/patterns.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/patterns.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version_constraint.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_constraint.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version_range.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_range.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/semver/version_union.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/semver/version_union.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/license.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/license.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/updater.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/updater.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/spdx/data/licenses.json` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/spdx/data/licenses.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/toml/file.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/toml/file.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/_compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/utils/toml_file.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/utils/toml_file.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/vcs/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/vcs/git.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/vcs/git.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/base.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/base.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/legacy_version.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/legacy_version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/markers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/markers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/requirements.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/requirements.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/utils.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/utils.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/version.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/version.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/grammars/markers.lark` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/markers.lark`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/core/version/grammars/pep508.lark`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/inspection/info.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/inspection/info.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/authenticator.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/authenticator.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/chef.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chef.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/chooser.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/chooser.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/executor.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/executor.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/installer.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/installer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/noop_installer.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/noop_installer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/pip_installer.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/pip_installer.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/install.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/install.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/operation.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/operation.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/uninstall.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/uninstall.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/installation/operations/update.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/installation/operations/update.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/json/__init__.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/json/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/json/schemas/poetry-schema.json`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/layouts/layout.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/layouts/layout.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/masonry/api.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/api.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/masonry/builders/editable.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/masonry/builders/editable.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/assignment.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/failure.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/incompatibility.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/partial_solution.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/term.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/term.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/version_solver.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/version_solver.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/providers/python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/mixology/solutions/solutions/python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/packages/dependency_package.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/dependency_package.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/packages/locker.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/locker.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/packages/package_collection.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/packages/package_collection.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/puzzle/provider.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/provider.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/puzzle/solver.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/puzzle/solver.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/installed_repository.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/installed_repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/legacy_repository.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/legacy_repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/pool.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pool.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/pypi_repository.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/pypi_repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/repositories/repository.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/_compat.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/appdirs.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/env.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/env.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/exporter.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/exporter.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/extras.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/extras.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/helpers.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/password_manager.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/password_manager.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/utils/setup_reader.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/utils/setup_reader.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/_vendor/poetry/version/version_selector.py` & `conda_lock-2.1.1/conda_lock/_vendor/poetry/version/version_selector.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/lockfile/__init__.py` & `conda_lock-2.1.1/conda_lock/lockfile/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/lockfile/v1/models.py` & `conda_lock-2.1.1/conda_lock/lockfile/v1/models.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/lockfile/v2prelim/models.py` & `conda_lock-2.1.1/conda_lock/lockfile/v2prelim/models.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/models/channel.py` & `conda_lock-2.1.1/conda_lock/models/channel.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/models/lock_spec.py` & `conda_lock-2.1.1/conda_lock/models/lock_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
 class _BaseDependency(StrictModel):
     name: str
     manager: Literal["conda", "pip"] = "conda"
     category: str = "main"
     extras: List[str] = []
 
+    @validator("extras")
+    def sorted_extras(cls, v: List[str]) -> List[str]:
+        return sorted(v)
+
 
 class VersionedDependency(_BaseDependency):
     version: str
     build: Optional[str] = None
     conda_channel: Optional[str] = None
```

### Comparing `conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/migration.py` & `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/migration.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/vendor_helpers.py` & `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/vendor_helpers.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch` & `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry-core.patch`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/scripts/vendor_poetry/patches/poetry.patch` & `conda_lock-2.1.1/conda_lock/scripts/vendor_poetry/patches/poetry.patch`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/src_parser/__init__.py` & `conda_lock-2.1.1/conda_lock/src_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/src_parser/aggregation.py` & `conda_lock-2.1.1/conda_lock/src_parser/aggregation.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/src_parser/conda_common.py` & `conda_lock-2.1.1/conda_lock/src_parser/conda_common.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/src_parser/environment_yaml.py` & `conda_lock-2.1.1/conda_lock/src_parser/environment_yaml.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/src_parser/meta_yaml.py` & `conda_lock-2.1.1/conda_lock/src_parser/meta_yaml.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/src_parser/pyproject_toml.py` & `conda_lock-2.1.1/conda_lock/src_parser/pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/conda_lock/src_parser/selectors.py` & `conda_lock-2.1.1/conda_lock/src_parser/selectors.py`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/authenticated_channels.md` & `conda_lock-2.1.1/docs/authenticated_channels.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/docker.md` & `conda_lock-2.1.1/docs/docker.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/flags.md` & `conda_lock-2.1.1/docs/flags.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,19 +141,19 @@
 
 If you want to override which virtual packages are injected you can create a virtual package spec file
 
 ```{.yaml title="virtual-packages.yml"}
 subdirs:
   linux-64:
     packages:
-      __glibc: 2.17
-      __cuda: 11.4
+      __glibc: "2.17"
+      __cuda: "11.4"
   win-64:
     packages:
-      __cuda: 11.4
+      __cuda: "11.4"
 ```
 
 conda-lock will automatically use a `virtual-packages.yml` it finds in the the current working directory.  Alternatively one can be specified
 explicitly via the flag.
 
 ```bash
 conda lock --virtual-package-spec virtual-packages-cuda.yml --platform linux-64
```

### Comparing `conda_lock-2.1.0/docs/index.md` & `conda_lock-2.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/output.md` & `conda_lock-2.1.1/docs/output.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/pip.md` & `conda_lock-2.1.1/docs/pip.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/src_environment_yml.md` & `conda_lock-2.1.1/docs/src_environment_yml.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/src_meta_yaml.md` & `conda_lock-2.1.1/docs/src_meta_yaml.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/src_pyproject.md` & `conda_lock-2.1.1/docs/src_pyproject.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/docs/flags/strip-auth.md` & `conda_lock-2.1.1/docs/flags/strip-auth.md`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/environments/conda-lock.yml` & `conda_lock-2.1.1/environments/conda-lock.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/example/pangeo/conda-lock.yml` & `conda_lock-2.1.1/example/pangeo/conda-lock.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/example/zlib/conda-lock.yml` & `conda_lock-2.1.1/example/zlib/conda-lock.yml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/LICENSE` & `conda_lock-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/README.md` & `conda_lock-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -223,19 +223,19 @@
 If you want to override which virtual packages are injected you can create a file like
 
 ```yaml
 # virtual-packages.yml
 subdirs:
   linux-64:
     packages:
-      __glibc: 2.17
-      __cuda: 11.4
+      __glibc: "2.17"
+      __cuda: "11.4"
   win-64:
     packages:
-      __cuda: 11.4
+      __cuda: "11.4"
 ```
 
 conda-lock will automatically use a `virtual-packages.yml` it finds in the the current working directory.  Alternatively one can be specified
 explicitly via the flag.
 
 ```bash
 conda lock --virtual-package-spec virtual-packages-cuda.yml -p linux-64
```

### Comparing `conda_lock-2.1.0/pyproject.toml` & `conda_lock-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conda_lock-2.1.0/PKG-INFO` & `conda_lock-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda_lock
-Version: 2.1.0
+Version: 2.1.1
 Summary: Lockfiles for conda
 Project-URL: Homepage, https://github.com/conda/conda-lock
 Project-URL: Repository, https://github.com/conda/conda-lock
 Project-URL: Documentation, https://conda.github.io/conda-lock/
 Project-URL: Issue Tracker, https://github.com/conda/conda-lock/issues
 Project-URL: Conda-Forge Feedstock, https://github.com/conda-forge/conda-lock-feedstock
 Project-URL: Anaconda.org, https://anaconda.org/conda-forge/conda-lock
@@ -274,19 +274,19 @@
 If you want to override which virtual packages are injected you can create a file like
 
 ```yaml
 # virtual-packages.yml
 subdirs:
   linux-64:
     packages:
-      __glibc: 2.17
-      __cuda: 11.4
+      __glibc: "2.17"
+      __cuda: "11.4"
   win-64:
     packages:
-      __cuda: 11.4
+      __cuda: "11.4"
 ```
 
 conda-lock will automatically use a `virtual-packages.yml` it finds in the the current working directory.  Alternatively one can be specified
 explicitly via the flag.
 
 ```bash
 conda lock --virtual-package-spec virtual-packages-cuda.yml -p linux-64
```

