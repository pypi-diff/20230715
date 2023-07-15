# Comparing `tmp/aesara_nightly-2.9.0.post4.tar.gz` & `tmp/aesara_nightly-2.9.1.post2.tar.gz`

## Comparing `aesara_nightly-2.9.0.post4.tar` & `aesara_nightly-2.9.1.post2.tar`

### file list

```diff
@@ -1,608 +1,609 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/.gitattributes
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/README.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/conftest.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/requirements-rtd.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/requirements.txt
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/_version.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/assert_op.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/breakpoint.py
--rw-r--r--   0        0        0    46225 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/configdefaults.py
--rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/configparser.py
--rw-r--r--   0        0        0    86751 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/gradient.py
--rw-r--r--   0        0        0    29067 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/ifelse.py
--rw-r--r--   0        0        0    67046 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/printing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/py.typed
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/raise_op.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/updates.py
--rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/utils.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/bin/__init__.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/bin/aesara_cache.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/__init__.py
--rw-r--r--   0        0        0    41442 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/builders.py
--rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/compiledir.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/compilelock.py
--rw-r--r--   0        0        0    85654 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/debugmode.py
--rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/io.py
--rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/mode.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/monitormode.py
--rw-r--r--   0        0        0     8326 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/nanguardmode.py
--rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/ops.py
--rw-r--r--   0        0        0    59770 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/profiling.py
--rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/sharedvalue.py
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/function/__init__.py
--rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/function/pfunc.py
--rw-r--r--   0        0        0    73889 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/compile/function/types.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/__init__.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/d3viz.py
--rw-r--r--   0        0        0    11843 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/formatting.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/css/d3-context-menu.css
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/css/d3viz.css
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/html/template.html
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/js/d3-context-menu.js
--rw-r--r--   0        0        0   151143 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/js/d3.v3.min.js
--rw-r--r--   0        0        0    23208 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/js/d3viz.js
--rw-r--r--   0        0        0    47566 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/js/dagre-d3.min.js
--rw-r--r--   0        0        0   115617 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/d3viz/js/graphlib-dot.min.js
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/__init__.py
--rw-r--r--   0        0        0    59773 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/basic.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/destroyhandler.py
--rw-r--r--   0        0        0    24835 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/features.py
--rw-r--r--   0        0        0    36232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/fg.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/kanren.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/null_type.py
--rw-r--r--   0        0        0    25036 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/op.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/opt.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/opt_utils.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/optdb.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/sched.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/toolbox.py
--rw-r--r--   0        0        0     9527 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/type.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/unify.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/rewriting/__init__.py
--rw-r--r--   0        0        0   114199 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/rewriting/basic.py
--rw-r--r--   0        0        0    19934 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/rewriting/db.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/rewriting/kanren.py
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/rewriting/unify.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/graph/rewriting/utils.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/__init__.py
--rw-r--r--   0        0        0    23890 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/basic.py
--rw-r--r--   0        0        0    28716 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/utils.py
--rw-r--r--   0        0        0    50565 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/vm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/__init__.py
--rw-r--r--   0        0        0    72572 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/basic.py
--rw-r--r--   0        0        0   112844 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/cmodule.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/cutils.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/cvm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/exceptions.py
--rw-r--r--   0        0        0    19955 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/interface.py
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/lazylinker_c.py
--rw-r--r--   0        0        0    24724 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/op.py
--rw-r--r--   0        0        0    31544 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/params_type.py
--rw-r--r--   0        0        0    26540 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/type.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/c_code/aesara_mod_helper.h
--rw-r--r--   0        0        0    35583 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/c/c_code/lazylinker_c.c
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/jax_dispatch.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/jax_linker.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/linker.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/__init__.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/basic.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/elemwise.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/extra_ops.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/nlinalg.py
--rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/random.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/scalar.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/scan.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/shape.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/slinalg.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/subtensor.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/tensor_basic.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/linker.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/__init__.py
--rw-r--r--   0        0        0    25903 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/basic.py
--rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/elemwise.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/extra_ops.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/nlinalg.py
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/random.py
--rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/scalar.py
--rw-r--r--   0        0        0    14203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/scan.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/sparse.py
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/tensor_basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/__init__.py
--rw-r--r--   0        0        0     9672 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/check_blas.py
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/check_blas_many.sh
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/check_duplicate_key.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/elemwise_openmp_speedup.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/elemwise_time_test.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/frozendict.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/latence_gpu_transfert.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/may_share_memory.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/ordered_set.py
--rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/pkl_utils.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/misc/safe_asarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/__init__.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/fourier.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/minimal.py
--rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/multinomial.py
--rw-r--r--   0        0        0    48271 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/rng_mrg.py
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/samples_MRG31k3p_12_7_5.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/solve.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/linalg/__init__.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sandbox/linalg/ops.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/__init__.py
--rw-r--r--   0        0        0   143432 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/basic.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/basic_scipy.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/basic_sympy.py
--rw-r--r--   0        0        0    46142 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/math.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/sharedvar.py
--rw-r--r--   0        0        0   126227 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/c_code/Faddeeva.cc
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/c_code/Faddeeva.hh
--rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scalar/c_code/gamma.c
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/__init__.py
--rw-r--r--   0        0        0    50095 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/basic.py
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/checkpoints.py
--rw-r--r--   0        0        0   140522 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/op.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/opt.py
--rw-r--r--   0        0        0    95587 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/rewriting.py
--rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/scan_perform.pyx
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/scan_perform_ext.py
--rw-r--r--   0        0        0    38052 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/utils.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/views.py
--rw-r--r--   0        0        0  1114748 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/scan/c_code/scan_perform.c
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/__init__.py
--rw-r--r--   0        0        0   118008 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/basic.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/opt.py
--rw-r--r--   0        0        0    76905 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/rewriting.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/sharedvar.py
--rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/type.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/sandbox/__init__.py
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/sandbox/sp.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/sparse/sandbox/sp2.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/__init__.py
--rw-r--r--   0        0        0   135685 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/basic.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/basic_opt.py
--rw-r--r--   0        0        0    98819 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/blas.py
--rw-r--r--   0        0        0    26486 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/blas_c.py
--rw-r--r--   0        0        0    68050 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/blas_headers.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/blas_scipy.py
--rw-r--r--   0        0        0    66675 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/elemwise.py
--rw-r--r--   0        0        0    20860 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/elemwise_cgen.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/exceptions.py
--rw-r--r--   0        0        0    57997 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/extra_ops.py
--rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/fft.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/fourier.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/inplace.py
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/io.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/linalg.py
--rw-r--r--   0        0        0    96168 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/math.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/math_opt.py
--rw-r--r--   0        0        0    22498 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nlinalg.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/opt_uncanonicalize.py
--rw-r--r--   0        0        0    33298 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/shape.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/sharedvar.py
--rw-r--r--   0        0        0    24997 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/slinalg.py
--rw-r--r--   0        0        0    17849 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/sort.py
--rw-r--r--   0        0        0    27385 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/special.py
--rw-r--r--   0        0        0    91231 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/subtensor.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/subtensor_opt.py
--rw-r--r--   0        0        0    41188 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/type.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/type_other.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/utils.py
--rw-r--r--   0        0        0    37592 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/var.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/xlogx.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/c_code/alt_blas_common.h
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/c_code/alt_blas_template.c
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/c_code/dimshuffle.c
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/__init__.py
--rw-r--r--   0        0        0   138965 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/abstract_conv.py
--rw-r--r--   0        0        0    75765 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/basic.py
--rw-r--r--   0        0        0    35376 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/batchnorm.py
--rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/blocksparse.py
--rw-r--r--   0        0        0    94523 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/conv.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/conv3d2d.py
--rw-r--r--   0        0        0    40356 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/corr.py
--rw-r--r--   0        0        0    36145 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/corr3d.py
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/ctc.py
--rw-r--r--   0        0        0    35353 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/neighbours.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/opt.py
--rw-r--r--   0        0        0    17297 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/rewriting.py
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/sigm.py
--rw-r--r--   0        0        0    18972 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/c_code/corr3d_gemm.c
--rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/c_code/corr_gemm.c
--rw-r--r--   0        0        0     8195 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/nnet/c_code/ctc_wrapper.c
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/__init__.py
--rw-r--r--   0        0        0    64232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/basic.py
--rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/op.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/opt.py
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/type.py
--rw-r--r--   0        0        0     9024 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/utils.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/var.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/rewriting/__init__.py
--rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/rewriting/basic.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/random/rewriting/jax.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/__init__.py
--rw-r--r--   0        0        0    42723 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/basic.py
--rw-r--r--   0        0        0    39439 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/elemwise.py
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/extra_ops.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/jax.py
--rw-r--r--   0        0        0   124250 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/math.py
--rw-r--r--   0        0        0    43264 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/shape.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/special.py
--rw-r--r--   0        0        0    63199 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/subtensor.py
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/uncanonicalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/signal/__init__.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/signal/conv.py
--rwxr-xr-x   0        0        0    97524 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/tensor/signal/pool.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/typed_list/__init__.py
--rw-r--r--   0        0        0    18222 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/typed_list/basic.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/typed_list/rewriting.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/aesara/typed_list/type.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/bin/__init__.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/bin/aesara-cache
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/bin/aesara_cache.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/acknowledgement.rst
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/conf.py
--rw-r--r--   0        0        0    30688 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/config.rst
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/core_development_guide.rst
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/css.inc
--rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/dev_start_guide.rst
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/generate_dtype_tensor_table.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/glossary.rst
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/help.rst
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/how_to_think_in_aesara.rst
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/index.rst
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/install.rst
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/introduction.rst
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/mission.rst
--rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/pylintrc
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/.build/PLACEHOLDER
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/.static/PLACEHOLDER
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/.static/fix_rtd.css
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/.static/version_switch.js
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/.templates/PLACEHOLDER
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/.templates/layout.html
--rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/debugmode.rst
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/function.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/index.rst
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/io.rst
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/mode.rst
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/modes.rst
--rwxr-xr-x   0        0        0     1881 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/modes_solution_1.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/nanguardmode.rst
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/opfromgraph.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/ops.rst
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/profilemode.rst
--rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/shared.rst
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/compile/rewrites/index.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/rewrite.rst
--rw-r--r--   0        0        0    46604 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/backend/creating_a_c_op.rst
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/backend/creating_a_numba_jax_op.rst
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/backend/ctype.rst
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/backend/index.rst
--rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/op/apply.png
--rw-r--r--   0        0        0    20340 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/op/apply.svg
--rw-r--r--   0        0        0    32078 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/op/apply2.svg
--rw-r--r--   0        0        0    32787 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/op/creating_an_op.rst
--rw-r--r--   0        0        0    17336 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/op/how_to_make_ops.rst
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/op/index.rst
--rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/extend/op/inplace.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/compilation/index.rst
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/compilation/pipeline.rst
--rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/apply.png
--rw-r--r--   0        0        0    20340 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/apply.svg
--rw-r--r--   0        0        0    32078 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/apply2.svg
--rw-r--r--   0        0        0    13712 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graphstructures.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/index.rst
--rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/op.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/other_ops.rst
--rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/symbolic_graph_opt.png
--rw-r--r--   0        0        0    62062 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/symbolic_graph_unopt.png
--rw-r--r--   0        0        0    19679 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/type.rst
--rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/using_params.rst
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/features.rst
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/fgraph.rst
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/graph.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/index.rst
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/op.rst
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/type.rst
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/utils.rst
--rw-r--r--   0        0        0    55613 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/rewrites/graph_rewriting.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/rewrites/index.rst
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/fundamentals/rewrites/optimizations.rst
--rw-r--r--   0        0        0    94102 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/Elman_srnn.png
--rw-r--r--   0        0        0    15088 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/aesara_logo_200.png
--rw-r--r--   0        0        0   116646 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/aesara_logo_2400.png
--rw-r--r--   0        0        0   198151 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/aesara_overview_diagram.png
--rw-r--r--   0        0        0   102018 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/blocksparse.png
--rw-r--r--   0        0        0    13780 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/lstm.png
--rw-r--r--   0        0        0    14362 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/lstm_memorycell.png
--rw-r--r--   0        0        0   273555 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/talk2010.gif
--rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/images/talk2010.png
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/conditionals.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/index.rst
--rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/gradient/dlogistic.png
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/gradient/gradient_api.rst
--rw-r--r--   0        0        0    10641 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/gradient/gradient_tutorial.rst
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/gradient/index.rst
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/loops/index.rst
--rwxr-xr-x   0        0        0     2517 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/loops/loop_solution_1.py
--rw-r--r--   0        0        0    26346 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/loops/loops_api.rst
--rw-r--r--   0        0        0    12565 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/loops/loops_tutorial.rst
--rw-r--r--   0        0        0    17090 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/loops/scan_extend.rst
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/random/index.rst
--rw-r--r--   0        0        0    25804 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/bcast.png
--rw-r--r--   0        0        0    14117 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/bcast.svg
--rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/create.rst
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/index.rst
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.binary_operations.rst
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.discrete_fourier.rst
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.indexing.rst
--rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.linalg.rst
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.logic.rst
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.mathematical_functions.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.padding.rst
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.rst
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.sorting.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.statistics.rst
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.tensor_creation.rst
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.tensor_manipulation.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.window_functions.rst
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/shapes.rst
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/tensor.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/utils.rst
--rw-r--r--   0        0        0    11485 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/shared/aliasing.rst
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/shared/index.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/shared/shared.rst
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/sparse/index.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/sparse/sandbox.rst
--rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/reference/tensor/sparse/sparse_api.rst
--rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/ccodegen.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/compilation.rst
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/debugging_with_stepmode.rst
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/elemwise_compiler.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/function.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/functional.rst
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/index.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/index2.rst
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/interactive_debugger.rst
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/logistic_regression_example.rst
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/performance.rst
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/randomnumbers.rst
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/rethinkccodegen.rst
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/sandbox.rst
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/software.rst
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/sparse.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/sandbox/tensoroptools.rst
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/scripts/docgen.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/serializing/index.rst
--rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/serializing/loading_and_saving.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/serializing/pkl_utils.rst
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/breakpoints.rst
--rw-r--r--   0        0        0    55147 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz.png
--rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/debug_faq.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/index.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/interacting_with_graph.rst
--rw-r--r--   0        0        0   106142 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/logreg_pydotprint_predict.png
--rw-r--r--   0        0        0   148860 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/logreg_pydotprint_prediction.png
--rw-r--r--   0        0        0   473403 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/logreg_pydotprint_train.png
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/nan_tutorial.rst
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/optimisations.rst
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/printing.rst
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/printing_drawing.rst
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/profiling.rst
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/profiling_example_out.prof
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/troubleshooting.rst
--rw-r--r--   0        0        0   216157 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index.ipynb
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index.rst
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp.html
--rw-r--r--   0        0        0    84140 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp.png
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp2.html
--rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp2.pdf
--rw-r--r--   0        0        0    46699 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp2.png
--rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/ofg.html
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/ofg2.html
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/css/d3-context-menu.css
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/css/d3viz.css
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/d3-context-menu.js
--rw-r--r--   0        0        0   151143 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/d3.v3.min.js
--rw-r--r--   0        0        0    23339 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/d3viz.js
--rw-r--r--   0        0        0    47566 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/dagre-d3.min.js
--rw-r--r--   0        0        0   115617 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/graphlib-dot.min.js
--rw-r--r--   0        0        0    93049 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_10_0.png
--rw-r--r--   0        0        0    93049 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_11_0.png
--rw-r--r--   0        0        0    46699 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_24_0.png
--rw-r--r--   0        0        0    46699 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_25_0.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/__init__.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_breakpoint.py
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_config.py
--rw-r--r--   0        0        0    34472 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_gradient.py
--rw-r--r--   0        0        0    25050 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_ifelse.py
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_printing.py
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_raise_op.py
--rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_rop.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/test_updates.py
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/unittest_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/__init__.py
--rw-r--r--   0        0        0    24285 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_builders.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_compilelock.py
--rw-r--r--   0        0        0    25864 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_debugmode.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_misc.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_mode.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_monitormode.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_nanguardmode.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_ops.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_profiling.py
--rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/test_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/function/__init__.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/function/test_function.py
--rw-r--r--   0        0        0    36404 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/function/test_pfunc.py
--rw-r--r--   0        0        0    42215 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/compile/function/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/d3viz/__init__.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/d3viz/models.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/d3viz/test_d3viz.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/d3viz/test_formatting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/__init__.py
--rw-r--r--   0        0        0    23703 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_basic.py
--rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_compute_test_value.py
--rw-r--r--   0        0        0    14846 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_destroyhandler.py
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_features.py
--rw-r--r--   0        0        0    22433 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_fg.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_op.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_sched.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_types.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/test_utils.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/rewriting/__init__.py
--rw-r--r--   0        0        0    28891 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_basic.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_db.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_kanren.py
--rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_unify.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/__init__.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/test_link.py
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/test_utils.py
--rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/test_vm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/__init__.py
--rw-r--r--   0        0        0    13074 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/test_basic.py
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/test_cmodule.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/test_op.py
--rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/test_params_type.py
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/test_type.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/c_code/test_cenum.h
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/c/c_code/test_quadratic_function.c
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_basic.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_elemwise.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_extra_ops.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_nlinalg.py
--rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_random.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_scalar.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_scan.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_shape.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_slinalg.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_subtensor.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/jax/test_tensor_basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/__init__.py
--rw-r--r--   0        0        0    30411 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_basic.py
--rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_elemwise.py
--rw-r--r--   0        0        0    13197 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_extra_ops.py
--rw-r--r--   0        0        0    12589 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_nlinalg.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_performance.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_random.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_scalar.py
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_scan.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_sparse.py
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/link/numba/test_tensor_basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/misc/__init__.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/misc/test_may_share_memory.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/misc/test_pkl_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sandbox/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sandbox/test_minimal.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sandbox/test_multinomial.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sandbox/test_multinomial_wo_replacement.py
--rw-r--r--   0        0        0    34649 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sandbox/test_rng_mrg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sandbox/linalg/__init__.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sandbox/linalg/test_linalg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scalar/__init__.py
--rw-r--r--   0        0        0    16995 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scalar/test_basic.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scalar/test_basic_sympy.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scalar/test_math.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scalar/test_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scan/__init__.py
--rw-r--r--   0        0        0   133995 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scan/test_basic.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scan/test_checkpoints.py
--rw-r--r--   0        0        0    25319 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scan/test_printing.py
--rw-r--r--   0        0        0    56551 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scan/test_rewriting.py
--rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scan/test_utils.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/scan/test_views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/__init__.py
--rw-r--r--   0        0        0   116949 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/test_basic.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/test_rewriting.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/test_sharedvar.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/test_sp2.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/test_type.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/test_utils.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/test_var.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/sandbox/__init__.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/sparse/sandbox/test_sp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/__init__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/_test_mpi_roundtrip.py
--rw-r--r--   0        0        0   148595 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_basic.py
--rw-r--r--   0        0        0    99618 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_blas.py
--rw-r--r--   0        0        0    14554 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_blas_c.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_blas_scipy.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_casting.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_complex.py
--rw-r--r--   0        0        0    34431 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_elemwise.py
--rw-r--r--   0        0        0    47330 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_extra_ops.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_fft.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_fourier.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_gc.py
--rw-r--r--   0        0        0    11957 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_inplace.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_io.py
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_keepdims.py
--rw-r--r--   0        0        0   123957 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_math.py
--rw-r--r--   0        0        0    29972 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_math_scipy.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_merge.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_misc.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_mpi.py
--rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_nlinalg.py
--rw-r--r--   0        0        0    22601 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_shape.py
--rw-r--r--   0        0        0    27332 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_sharedvar.py
--rw-r--r--   0        0        0    18787 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_slinalg.py
--rw-r--r--   0        0        0    18538 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_sort.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_special.py
--rw-r--r--   0        0        0    91185 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_subtensor.py
--rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_type.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_type_other.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_utils.py
--rw-r--r--   0        0        0    12727 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_var.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/test_xlogx.py
--rw-r--r--   0        0        0    38712 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/__init__.py
--rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/speed_test_conv.py
--rw-r--r--   0        0        0   103862 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_abstract_conv.py
--rw-r--r--   0        0        0    42020 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_basic.py
--rw-r--r--   0        0        0    25674 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_batchnorm.py
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_blocksparse.py
--rw-r--r--   0        0        0    28956 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_conv.py
--rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_conv3d2d.py
--rw-r--r--   0        0        0    21906 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_corr.py
--rw-r--r--   0        0        0    21818 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_corr3d.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_ctc.py
--rw-r--r--   0        0        0    25410 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_neighbours.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_rewriting.py
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_sigm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/random/__init__.py
--rw-r--r--   0        0        0    41556 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/random/test_basic.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/random/test_op.py
--rw-r--r--   0        0        0    17712 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/random/test_rewriting.py
--rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/random/test_type.py
--rw-r--r--   0        0        0    10653 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/random/test_utils.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/random/test_var.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/__init__.py
--rw-r--r--   0        0        0    63207 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_basic.py
--rw-r--r--   0        0        0    41140 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_elemwise.py
--rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_extra_ops.py
--rw-r--r--   0        0        0   166414 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_math.py
--rw-r--r--   0        0        0    18170 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_shape.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_special.py
--rw-r--r--   0        0        0    80378 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_subtensor.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_uncanonicalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/signal/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/signal/test_conv.py
--rw-r--r--   0        0        0    51694 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/tensor/signal/test_pool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/typed_list/__init__.py
--rw-r--r--   0        0        0    17535 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/typed_list/test_basic.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/typed_list/test_rewriting.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/tests/typed_list/test_type.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/.gitignore
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/DESCRIPTION.txt
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/LICENSE.txt
--rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/pyproject.toml
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 aesara_nightly-2.9.0.post4/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/.gitattributes
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/CITATION.cff
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/README.md
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/conftest.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/requirements-rtd.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/requirements.txt
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/_version.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/assert_op.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/breakpoint.py
+-rw-r--r--   0        0        0    46225 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/configdefaults.py
+-rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/configparser.py
+-rw-r--r--   0        0        0    86751 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/gradient.py
+-rw-r--r--   0        0        0    29067 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/ifelse.py
+-rw-r--r--   0        0        0    67046 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/printing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/py.typed
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/raise_op.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/updates.py
+-rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/utils.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/bin/__init__.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/bin/aesara_cache.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/__init__.py
+-rw-r--r--   0        0        0    41442 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/builders.py
+-rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/compiledir.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/compilelock.py
+-rw-r--r--   0        0        0    85654 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/debugmode.py
+-rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/io.py
+-rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/mode.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/monitormode.py
+-rw-r--r--   0        0        0     8326 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/nanguardmode.py
+-rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/ops.py
+-rw-r--r--   0        0        0    59770 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/profiling.py
+-rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/sharedvalue.py
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/function/__init__.py
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/function/pfunc.py
+-rw-r--r--   0        0        0    73889 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/compile/function/types.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/__init__.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/d3viz.py
+-rw-r--r--   0        0        0    11843 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/formatting.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/css/d3-context-menu.css
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/css/d3viz.css
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/html/template.html
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/js/d3-context-menu.js
+-rw-r--r--   0        0        0   151143 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/js/d3.v3.min.js
+-rw-r--r--   0        0        0    23208 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/js/d3viz.js
+-rw-r--r--   0        0        0    47566 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/js/dagre-d3.min.js
+-rw-r--r--   0        0        0   115617 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/d3viz/js/graphlib-dot.min.js
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/__init__.py
+-rw-r--r--   0        0        0    59773 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/basic.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/destroyhandler.py
+-rw-r--r--   0        0        0    24835 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/features.py
+-rw-r--r--   0        0        0    36232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/fg.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/kanren.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/null_type.py
+-rw-r--r--   0        0        0    25036 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/op.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/opt.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/opt_utils.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/optdb.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/sched.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/toolbox.py
+-rw-r--r--   0        0        0     9527 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/type.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/unify.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/rewriting/__init__.py
+-rw-r--r--   0        0        0   114199 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/rewriting/basic.py
+-rw-r--r--   0        0        0    19934 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/rewriting/db.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/rewriting/kanren.py
+-rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/rewriting/unify.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/graph/rewriting/utils.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/__init__.py
+-rw-r--r--   0        0        0    23890 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/basic.py
+-rw-r--r--   0        0        0    28716 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/utils.py
+-rw-r--r--   0        0        0    50565 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/vm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/__init__.py
+-rw-r--r--   0        0        0    72572 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/basic.py
+-rw-r--r--   0        0        0   112844 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/cmodule.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/cutils.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/cvm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/exceptions.py
+-rw-r--r--   0        0        0    19955 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/interface.py
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/lazylinker_c.py
+-rw-r--r--   0        0        0    24724 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/op.py
+-rw-r--r--   0        0        0    31544 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/params_type.py
+-rw-r--r--   0        0        0    26540 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/type.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/c_code/aesara_mod_helper.h
+-rw-r--r--   0        0        0    35583 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/c/c_code/lazylinker_c.c
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/jax_dispatch.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/jax_linker.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/linker.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/__init__.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/basic.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/elemwise.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/extra_ops.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/nlinalg.py
+-rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/random.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/scalar.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/scan.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/shape.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/slinalg.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/subtensor.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/tensor_basic.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/linker.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/__init__.py
+-rw-r--r--   0        0        0    25903 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/basic.py
+-rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/elemwise.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/extra_ops.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/nlinalg.py
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/random.py
+-rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/scalar.py
+-rw-r--r--   0        0        0    14203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/scan.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/sparse.py
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/tensor_basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/__init__.py
+-rw-r--r--   0        0        0     9672 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/check_blas.py
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/check_blas_many.sh
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/check_duplicate_key.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/elemwise_openmp_speedup.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/elemwise_time_test.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/frozendict.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/latence_gpu_transfert.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/may_share_memory.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/ordered_set.py
+-rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/pkl_utils.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/misc/safe_asarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/__init__.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/fourier.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/minimal.py
+-rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/multinomial.py
+-rw-r--r--   0        0        0    48271 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/rng_mrg.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/samples_MRG31k3p_12_7_5.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/solve.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/linalg/__init__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sandbox/linalg/ops.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/__init__.py
+-rw-r--r--   0        0        0   143432 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/basic.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/basic_scipy.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/basic_sympy.py
+-rw-r--r--   0        0        0    46142 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/math.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/sharedvar.py
+-rw-r--r--   0        0        0   126227 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/c_code/Faddeeva.cc
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/c_code/Faddeeva.hh
+-rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scalar/c_code/gamma.c
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/__init__.py
+-rw-r--r--   0        0        0    50095 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/basic.py
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/checkpoints.py
+-rw-r--r--   0        0        0   140522 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/op.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/opt.py
+-rw-r--r--   0        0        0    95587 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/rewriting.py
+-rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/scan_perform.pyx
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/scan_perform_ext.py
+-rw-r--r--   0        0        0    38052 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/utils.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/views.py
+-rw-r--r--   0        0        0  1114748 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/scan/c_code/scan_perform.c
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/__init__.py
+-rw-r--r--   0        0        0   118008 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/basic.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/opt.py
+-rw-r--r--   0        0        0    76905 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/rewriting.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/sharedvar.py
+-rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/type.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/sandbox/__init__.py
+-rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/sandbox/sp.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/sparse/sandbox/sp2.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/__init__.py
+-rw-r--r--   0        0        0   135685 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/basic.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/basic_opt.py
+-rw-r--r--   0        0        0    98819 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/blas.py
+-rw-r--r--   0        0        0    26486 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/blas_c.py
+-rw-r--r--   0        0        0    68050 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/blas_headers.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/blas_scipy.py
+-rw-r--r--   0        0        0    66675 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/elemwise.py
+-rw-r--r--   0        0        0    20860 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/elemwise_cgen.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/exceptions.py
+-rw-r--r--   0        0        0    57997 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/extra_ops.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/fft.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/fourier.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/inplace.py
+-rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/io.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/linalg.py
+-rw-r--r--   0        0        0    96168 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/math.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/math_opt.py
+-rw-r--r--   0        0        0    22498 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nlinalg.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/opt_uncanonicalize.py
+-rw-r--r--   0        0        0    33298 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/shape.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/sharedvar.py
+-rw-r--r--   0        0        0    24997 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/slinalg.py
+-rw-r--r--   0        0        0    17849 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/sort.py
+-rw-r--r--   0        0        0    27385 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/special.py
+-rw-r--r--   0        0        0    91231 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/subtensor.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/subtensor_opt.py
+-rw-r--r--   0        0        0    41188 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/type.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/type_other.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/utils.py
+-rw-r--r--   0        0        0    37592 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/var.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/xlogx.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/c_code/alt_blas_common.h
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/c_code/alt_blas_template.c
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/c_code/dimshuffle.c
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/__init__.py
+-rw-r--r--   0        0        0   138965 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/abstract_conv.py
+-rw-r--r--   0        0        0    75765 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/basic.py
+-rw-r--r--   0        0        0    35376 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/batchnorm.py
+-rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/blocksparse.py
+-rw-r--r--   0        0        0    94523 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/conv.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/conv3d2d.py
+-rw-r--r--   0        0        0    40356 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/corr.py
+-rw-r--r--   0        0        0    36145 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/corr3d.py
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/ctc.py
+-rw-r--r--   0        0        0    35353 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/neighbours.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/opt.py
+-rw-r--r--   0        0        0    17297 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/rewriting.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/sigm.py
+-rw-r--r--   0        0        0    18972 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/c_code/corr3d_gemm.c
+-rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/c_code/corr_gemm.c
+-rw-r--r--   0        0        0     8195 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/nnet/c_code/ctc_wrapper.c
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/__init__.py
+-rw-r--r--   0        0        0    64232 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/basic.py
+-rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/op.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/opt.py
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/type.py
+-rw-r--r--   0        0        0     9024 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/utils.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/var.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/rewriting/__init__.py
+-rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/rewriting/basic.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/random/rewriting/jax.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/__init__.py
+-rw-r--r--   0        0        0    42723 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/basic.py
+-rw-r--r--   0        0        0    39439 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/elemwise.py
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/extra_ops.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/jax.py
+-rw-r--r--   0        0        0   124250 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/math.py
+-rw-r--r--   0        0        0    43264 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/shape.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/special.py
+-rw-r--r--   0        0        0    63199 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/subtensor.py
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/uncanonicalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/signal/__init__.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/signal/conv.py
+-rwxr-xr-x   0        0        0    97524 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/tensor/signal/pool.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/typed_list/__init__.py
+-rw-r--r--   0        0        0    18222 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/typed_list/basic.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/typed_list/rewriting.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/aesara/typed_list/type.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/bin/__init__.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/bin/aesara-cache
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/bin/aesara_cache.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/acknowledgement.rst
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/conf.py
+-rw-r--r--   0        0        0    30688 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/config.rst
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/core_development_guide.rst
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/css.inc
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/dev_start_guide.rst
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/generate_dtype_tensor_table.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/glossary.rst
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/help.rst
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/how_to_think_in_aesara.rst
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/index.rst
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/install.rst
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/introduction.rst
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/mission.rst
+-rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/pylintrc
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/.build/PLACEHOLDER
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/.static/PLACEHOLDER
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/.static/fix_rtd.css
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/.static/version_switch.js
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/.templates/PLACEHOLDER
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/.templates/layout.html
+-rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/debugmode.rst
+-rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/function.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/index.rst
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/io.rst
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/mode.rst
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/modes.rst
+-rwxr-xr-x   0        0        0     1881 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/modes_solution_1.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/nanguardmode.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/opfromgraph.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/ops.rst
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/profilemode.rst
+-rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/shared.rst
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/compile/rewrites/index.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/rewrite.rst
+-rw-r--r--   0        0        0    46604 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/backend/creating_a_c_op.rst
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/backend/creating_a_numba_jax_op.rst
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/backend/ctype.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/backend/index.rst
+-rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/op/apply.png
+-rw-r--r--   0        0        0    20340 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/op/apply.svg
+-rw-r--r--   0        0        0    32078 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/op/apply2.svg
+-rw-r--r--   0        0        0    32787 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/op/creating_an_op.rst
+-rw-r--r--   0        0        0    17336 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/op/how_to_make_ops.rst
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/op/index.rst
+-rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/extend/op/inplace.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/compilation/index.rst
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/compilation/pipeline.rst
+-rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/apply.png
+-rw-r--r--   0        0        0    20340 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/apply.svg
+-rw-r--r--   0        0        0    32078 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/apply2.svg
+-rw-r--r--   0        0        0    13712 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graphstructures.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/index.rst
+-rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/op.rst
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/other_ops.rst
+-rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/symbolic_graph_opt.png
+-rw-r--r--   0        0        0    62062 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/symbolic_graph_unopt.png
+-rw-r--r--   0        0        0    19679 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/type.rst
+-rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/using_params.rst
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/features.rst
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/fgraph.rst
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/graph.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/index.rst
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/op.rst
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/type.rst
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/utils.rst
+-rw-r--r--   0        0        0    55613 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/rewrites/graph_rewriting.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/rewrites/index.rst
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/fundamentals/rewrites/optimizations.rst
+-rw-r--r--   0        0        0    94102 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/Elman_srnn.png
+-rw-r--r--   0        0        0    15088 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/aesara_logo_200.png
+-rw-r--r--   0        0        0   116646 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/aesara_logo_2400.png
+-rw-r--r--   0        0        0   198151 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/aesara_overview_diagram.png
+-rw-r--r--   0        0        0   102018 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/blocksparse.png
+-rw-r--r--   0        0        0    13780 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/lstm.png
+-rw-r--r--   0        0        0    14362 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/lstm_memorycell.png
+-rw-r--r--   0        0        0   273555 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/talk2010.gif
+-rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/images/talk2010.png
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/conditionals.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/index.rst
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/gradient/dlogistic.png
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/gradient/gradient_api.rst
+-rw-r--r--   0        0        0    10641 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/gradient/gradient_tutorial.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/gradient/index.rst
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/loops/index.rst
+-rwxr-xr-x   0        0        0     2517 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/loops/loop_solution_1.py
+-rw-r--r--   0        0        0    26346 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/loops/loops_api.rst
+-rw-r--r--   0        0        0    12565 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/loops/loops_tutorial.rst
+-rw-r--r--   0        0        0    17090 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/loops/scan_extend.rst
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/random/index.rst
+-rw-r--r--   0        0        0    25804 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/bcast.png
+-rw-r--r--   0        0        0    14117 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/bcast.svg
+-rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/create.rst
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/index.rst
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.binary_operations.rst
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.discrete_fourier.rst
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.indexing.rst
+-rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.linalg.rst
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.logic.rst
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.mathematical_functions.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.padding.rst
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.rst
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.sorting.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.statistics.rst
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.tensor_creation.rst
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.tensor_manipulation.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.window_functions.rst
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/shapes.rst
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/tensor.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/utils.rst
+-rw-r--r--   0        0        0    11485 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/shared/aliasing.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/shared/index.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/shared/shared.rst
+-rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/sparse/index.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/sparse/sandbox.rst
+-rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/reference/tensor/sparse/sparse_api.rst
+-rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/ccodegen.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/compilation.rst
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/debugging_with_stepmode.rst
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/elemwise_compiler.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/function.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/functional.rst
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/index.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/index2.rst
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/interactive_debugger.rst
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/logistic_regression_example.rst
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/performance.rst
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/randomnumbers.rst
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/rethinkccodegen.rst
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/sandbox.rst
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/software.rst
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/sparse.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/sandbox/tensoroptools.rst
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/scripts/docgen.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/serializing/index.rst
+-rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/serializing/loading_and_saving.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/serializing/pkl_utils.rst
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/breakpoints.rst
+-rw-r--r--   0        0        0    55147 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz.png
+-rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/debug_faq.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/index.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/interacting_with_graph.rst
+-rw-r--r--   0        0        0   106142 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/logreg_pydotprint_predict.png
+-rw-r--r--   0        0        0   148860 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/logreg_pydotprint_prediction.png
+-rw-r--r--   0        0        0   473403 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/logreg_pydotprint_train.png
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/nan_tutorial.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/optimisations.rst
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/printing.rst
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/printing_drawing.rst
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/profiling.rst
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/profiling_example_out.prof
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/troubleshooting.rst
+-rw-r--r--   0        0        0   216157 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index.ipynb
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index.rst
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp.html
+-rw-r--r--   0        0        0    84140 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp.png
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp2.html
+-rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp2.pdf
+-rw-r--r--   0        0        0    46699 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp2.png
+-rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/ofg.html
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/ofg2.html
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/css/d3-context-menu.css
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/css/d3viz.css
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/d3-context-menu.js
+-rw-r--r--   0        0        0   151143 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/d3.v3.min.js
+-rw-r--r--   0        0        0    23339 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/d3viz.js
+-rw-r--r--   0        0        0    47566 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/dagre-d3.min.js
+-rw-r--r--   0        0        0   115617 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/graphlib-dot.min.js
+-rw-r--r--   0        0        0    93049 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_10_0.png
+-rw-r--r--   0        0        0    93049 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_11_0.png
+-rw-r--r--   0        0        0    46699 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_24_0.png
+-rw-r--r--   0        0        0    46699 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_25_0.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/__init__.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_breakpoint.py
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_config.py
+-rw-r--r--   0        0        0    34472 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_gradient.py
+-rw-r--r--   0        0        0    25050 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_ifelse.py
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_printing.py
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_raise_op.py
+-rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_rop.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/test_updates.py
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/unittest_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/__init__.py
+-rw-r--r--   0        0        0    24285 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_builders.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_compilelock.py
+-rw-r--r--   0        0        0    25864 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_debugmode.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_misc.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_mode.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_monitormode.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_nanguardmode.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_ops.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_profiling.py
+-rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/test_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/function/__init__.py
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/function/test_function.py
+-rw-r--r--   0        0        0    36404 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/function/test_pfunc.py
+-rw-r--r--   0        0        0    42215 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/compile/function/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/d3viz/__init__.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/d3viz/models.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/d3viz/test_d3viz.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/d3viz/test_formatting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/__init__.py
+-rw-r--r--   0        0        0    23703 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_basic.py
+-rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_compute_test_value.py
+-rw-r--r--   0        0        0    14846 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_destroyhandler.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_features.py
+-rw-r--r--   0        0        0    22433 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_fg.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_op.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_sched.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_types.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/test_utils.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/rewriting/__init__.py
+-rw-r--r--   0        0        0    28891 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_basic.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_db.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_kanren.py
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_unify.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/__init__.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/test_link.py
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/test_utils.py
+-rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/test_vm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/__init__.py
+-rw-r--r--   0        0        0    13074 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/test_basic.py
+-rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/test_cmodule.py
+-rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/test_op.py
+-rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/test_params_type.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/test_type.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/c_code/test_cenum.h
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/c/c_code/test_quadratic_function.c
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_basic.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_elemwise.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_extra_ops.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_nlinalg.py
+-rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_random.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_scalar.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_scan.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_shape.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_slinalg.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_subtensor.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/jax/test_tensor_basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/__init__.py
+-rw-r--r--   0        0        0    30411 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_basic.py
+-rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_elemwise.py
+-rw-r--r--   0        0        0    13197 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_extra_ops.py
+-rw-r--r--   0        0        0    12589 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_nlinalg.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_performance.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_random.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_scalar.py
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_scan.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_sparse.py
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/link/numba/test_tensor_basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/misc/__init__.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/misc/test_may_share_memory.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/misc/test_pkl_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sandbox/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sandbox/test_minimal.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sandbox/test_multinomial.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sandbox/test_multinomial_wo_replacement.py
+-rw-r--r--   0        0        0    34649 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sandbox/test_rng_mrg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sandbox/linalg/__init__.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sandbox/linalg/test_linalg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scalar/__init__.py
+-rw-r--r--   0        0        0    16995 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scalar/test_basic.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scalar/test_basic_sympy.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scalar/test_math.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scalar/test_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scan/__init__.py
+-rw-r--r--   0        0        0   133995 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scan/test_basic.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scan/test_checkpoints.py
+-rw-r--r--   0        0        0    25319 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scan/test_printing.py
+-rw-r--r--   0        0        0    56551 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scan/test_rewriting.py
+-rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scan/test_utils.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/scan/test_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/__init__.py
+-rw-r--r--   0        0        0   116949 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/test_basic.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/test_rewriting.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/test_sharedvar.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/test_sp2.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/test_type.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/test_utils.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/test_var.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/sandbox/__init__.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/sparse/sandbox/test_sp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/_test_mpi_roundtrip.py
+-rw-r--r--   0        0        0   148595 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_basic.py
+-rw-r--r--   0        0        0    99618 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_blas.py
+-rw-r--r--   0        0        0    14554 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_blas_c.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_blas_scipy.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_casting.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_complex.py
+-rw-r--r--   0        0        0    34431 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_elemwise.py
+-rw-r--r--   0        0        0    47330 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_extra_ops.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_fft.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_fourier.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_gc.py
+-rw-r--r--   0        0        0    11957 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_inplace.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_io.py
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_keepdims.py
+-rw-r--r--   0        0        0   123957 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_math.py
+-rw-r--r--   0        0        0    29972 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_math_scipy.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_merge.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_misc.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_mpi.py
+-rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_nlinalg.py
+-rw-r--r--   0        0        0    22601 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_shape.py
+-rw-r--r--   0        0        0    27332 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_sharedvar.py
+-rw-r--r--   0        0        0    18787 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_slinalg.py
+-rw-r--r--   0        0        0    18538 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_sort.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_special.py
+-rw-r--r--   0        0        0    91185 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_subtensor.py
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_type.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_type_other.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_utils.py
+-rw-r--r--   0        0        0    12727 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_var.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/test_xlogx.py
+-rw-r--r--   0        0        0    38712 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/__init__.py
+-rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/speed_test_conv.py
+-rw-r--r--   0        0        0   103862 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_abstract_conv.py
+-rw-r--r--   0        0        0    42020 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_basic.py
+-rw-r--r--   0        0        0    25674 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_batchnorm.py
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_blocksparse.py
+-rw-r--r--   0        0        0    28956 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_conv.py
+-rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_conv3d2d.py
+-rw-r--r--   0        0        0    21906 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_corr.py
+-rw-r--r--   0        0        0    21818 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_corr3d.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_ctc.py
+-rw-r--r--   0        0        0    25410 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_neighbours.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_rewriting.py
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_sigm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/random/__init__.py
+-rw-r--r--   0        0        0    41556 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/random/test_basic.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/random/test_op.py
+-rw-r--r--   0        0        0    17712 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/random/test_rewriting.py
+-rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/random/test_type.py
+-rw-r--r--   0        0        0    10653 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/random/test_utils.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/random/test_var.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/__init__.py
+-rw-r--r--   0        0        0    63207 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_basic.py
+-rw-r--r--   0        0        0    41140 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_elemwise.py
+-rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_extra_ops.py
+-rw-r--r--   0        0        0   166414 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_math.py
+-rw-r--r--   0        0        0    18170 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_shape.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_special.py
+-rw-r--r--   0        0        0    80378 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_subtensor.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_uncanonicalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/signal/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/signal/test_conv.py
+-rw-r--r--   0        0        0    51694 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/tensor/signal/test_pool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/typed_list/__init__.py
+-rw-r--r--   0        0        0    17535 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/typed_list/test_basic.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/typed_list/test_rewriting.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/tests/typed_list/test_type.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/.gitignore
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/DESCRIPTION.txt
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/LICENSE.txt
+-rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/pyproject.toml
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 aesara_nightly-2.9.1.post2/PKG-INFO
```

### Comparing `aesara_nightly-2.9.0.post4/README.md` & `aesara_nightly-2.9.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/conftest.py` & `aesara_nightly-2.9.1.post2/conftest.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/breakpoint.py` & `aesara_nightly-2.9.1.post2/aesara/breakpoint.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/configdefaults.py` & `aesara_nightly-2.9.1.post2/aesara/configdefaults.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/configparser.py` & `aesara_nightly-2.9.1.post2/aesara/configparser.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/gradient.py` & `aesara_nightly-2.9.1.post2/aesara/gradient.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/ifelse.py` & `aesara_nightly-2.9.1.post2/aesara/ifelse.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/printing.py` & `aesara_nightly-2.9.1.post2/aesara/printing.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/raise_op.py` & `aesara_nightly-2.9.1.post2/aesara/raise_op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/updates.py` & `aesara_nightly-2.9.1.post2/aesara/updates.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/utils.py` & `aesara_nightly-2.9.1.post2/aesara/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/version.py` & `aesara_nightly-2.9.1.post2/aesara/version.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/bin/aesara_cache.py` & `aesara_nightly-2.9.1.post2/aesara/bin/aesara_cache.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/builders.py` & `aesara_nightly-2.9.1.post2/aesara/compile/builders.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/compiledir.py` & `aesara_nightly-2.9.1.post2/aesara/compile/compiledir.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/compilelock.py` & `aesara_nightly-2.9.1.post2/aesara/compile/compilelock.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/debugmode.py` & `aesara_nightly-2.9.1.post2/aesara/compile/debugmode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/io.py` & `aesara_nightly-2.9.1.post2/aesara/compile/io.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/mode.py` & `aesara_nightly-2.9.1.post2/aesara/compile/mode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/monitormode.py` & `aesara_nightly-2.9.1.post2/aesara/compile/monitormode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/nanguardmode.py` & `aesara_nightly-2.9.1.post2/aesara/compile/nanguardmode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/ops.py` & `aesara_nightly-2.9.1.post2/aesara/compile/ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/profiling.py` & `aesara_nightly-2.9.1.post2/aesara/compile/profiling.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/sharedvalue.py` & `aesara_nightly-2.9.1.post2/aesara/compile/sharedvalue.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/function/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/compile/function/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/function/pfunc.py` & `aesara_nightly-2.9.1.post2/aesara/compile/function/pfunc.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/compile/function/types.py` & `aesara_nightly-2.9.1.post2/aesara/compile/function/types.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/d3viz.py` & `aesara_nightly-2.9.1.post2/aesara/d3viz/d3viz.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/formatting.py` & `aesara_nightly-2.9.1.post2/aesara/d3viz/formatting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/css/d3viz.css` & `aesara_nightly-2.9.1.post2/aesara/d3viz/css/d3viz.css`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/html/template.html` & `aesara_nightly-2.9.1.post2/aesara/d3viz/html/template.html`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/js/d3-context-menu.js` & `aesara_nightly-2.9.1.post2/aesara/d3viz/js/d3-context-menu.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/js/d3.v3.min.js` & `aesara_nightly-2.9.1.post2/aesara/d3viz/js/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/js/d3viz.js` & `aesara_nightly-2.9.1.post2/aesara/d3viz/js/d3viz.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/js/dagre-d3.min.js` & `aesara_nightly-2.9.1.post2/aesara/d3viz/js/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/d3viz/js/graphlib-dot.min.js` & `aesara_nightly-2.9.1.post2/aesara/d3viz/js/graphlib-dot.min.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/basic.py` & `aesara_nightly-2.9.1.post2/aesara/graph/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/destroyhandler.py` & `aesara_nightly-2.9.1.post2/aesara/graph/destroyhandler.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/features.py` & `aesara_nightly-2.9.1.post2/aesara/graph/features.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/fg.py` & `aesara_nightly-2.9.1.post2/aesara/graph/fg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/null_type.py` & `aesara_nightly-2.9.1.post2/aesara/graph/null_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/op.py` & `aesara_nightly-2.9.1.post2/aesara/graph/op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/opt.py` & `aesara_nightly-2.9.1.post2/aesara/graph/opt.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/opt_utils.py` & `aesara_nightly-2.9.1.post2/aesara/graph/opt_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/optdb.py` & `aesara_nightly-2.9.1.post2/aesara/graph/optdb.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/sched.py` & `aesara_nightly-2.9.1.post2/aesara/graph/sched.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/type.py` & `aesara_nightly-2.9.1.post2/aesara/graph/type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/utils.py` & `aesara_nightly-2.9.1.post2/aesara/graph/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/rewriting/basic.py` & `aesara_nightly-2.9.1.post2/aesara/graph/rewriting/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/rewriting/db.py` & `aesara_nightly-2.9.1.post2/aesara/graph/rewriting/db.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/rewriting/kanren.py` & `aesara_nightly-2.9.1.post2/aesara/graph/rewriting/kanren.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/rewriting/unify.py` & `aesara_nightly-2.9.1.post2/aesara/graph/rewriting/unify.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/graph/rewriting/utils.py` & `aesara_nightly-2.9.1.post2/aesara/graph/rewriting/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/basic.py` & `aesara_nightly-2.9.1.post2/aesara/link/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/utils.py` & `aesara_nightly-2.9.1.post2/aesara/link/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/vm.py` & `aesara_nightly-2.9.1.post2/aesara/link/vm.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/basic.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/cmodule.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/cmodule.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/cutils.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/cutils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/cvm.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/cvm.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/interface.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/interface.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/lazylinker_c.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/lazylinker_c.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/op.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/params_type.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/params_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/type.py` & `aesara_nightly-2.9.1.post2/aesara/link/c/type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/c_code/aesara_mod_helper.h` & `aesara_nightly-2.9.1.post2/aesara/link/c/c_code/aesara_mod_helper.h`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/c/c_code/lazylinker_c.c` & `aesara_nightly-2.9.1.post2/aesara/link/c/c_code/lazylinker_c.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/linker.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/linker.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/basic.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/elemwise.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/extra_ops.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/nlinalg.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/nlinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/random.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/random.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/scalar.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/scalar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/scan.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/scan.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/shape.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/slinalg.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/slinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/subtensor.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/subtensor.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/jax/dispatch/tensor_basic.py` & `aesara_nightly-2.9.1.post2/aesara/link/jax/dispatch/tensor_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/linker.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/linker.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/basic.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/elemwise.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/extra_ops.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/nlinalg.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/nlinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/random.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/random.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/scalar.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/scalar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/scan.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/scan.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/sparse.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/sparse.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/link/numba/dispatch/tensor_basic.py` & `aesara_nightly-2.9.1.post2/aesara/link/numba/dispatch/tensor_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/check_blas.py` & `aesara_nightly-2.9.1.post2/aesara/misc/check_blas.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/check_blas_many.sh` & `aesara_nightly-2.9.1.post2/aesara/misc/check_blas_many.sh`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/check_duplicate_key.py` & `aesara_nightly-2.9.1.post2/aesara/misc/check_duplicate_key.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/elemwise_openmp_speedup.py` & `aesara_nightly-2.9.1.post2/aesara/misc/elemwise_openmp_speedup.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/elemwise_time_test.py` & `aesara_nightly-2.9.1.post2/aesara/misc/elemwise_time_test.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/frozendict.py` & `aesara_nightly-2.9.1.post2/aesara/misc/frozendict.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/latence_gpu_transfert.py` & `aesara_nightly-2.9.1.post2/aesara/misc/latence_gpu_transfert.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/may_share_memory.py` & `aesara_nightly-2.9.1.post2/aesara/misc/may_share_memory.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/ordered_set.py` & `aesara_nightly-2.9.1.post2/aesara/misc/ordered_set.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/pkl_utils.py` & `aesara_nightly-2.9.1.post2/aesara/misc/pkl_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/misc/safe_asarray.py` & `aesara_nightly-2.9.1.post2/aesara/misc/safe_asarray.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sandbox/fourier.py` & `aesara_nightly-2.9.1.post2/aesara/sandbox/fourier.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sandbox/minimal.py` & `aesara_nightly-2.9.1.post2/aesara/sandbox/minimal.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sandbox/multinomial.py` & `aesara_nightly-2.9.1.post2/aesara/sandbox/multinomial.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sandbox/rng_mrg.py` & `aesara_nightly-2.9.1.post2/aesara/sandbox/rng_mrg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sandbox/samples_MRG31k3p_12_7_5.txt` & `aesara_nightly-2.9.1.post2/aesara/sandbox/samples_MRG31k3p_12_7_5.txt`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sandbox/linalg/ops.py` & `aesara_nightly-2.9.1.post2/aesara/sandbox/linalg/ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/basic.py` & `aesara_nightly-2.9.1.post2/aesara/scalar/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/basic_sympy.py` & `aesara_nightly-2.9.1.post2/aesara/scalar/basic_sympy.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/math.py` & `aesara_nightly-2.9.1.post2/aesara/scalar/math.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/sharedvar.py` & `aesara_nightly-2.9.1.post2/aesara/scalar/sharedvar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/c_code/Faddeeva.cc` & `aesara_nightly-2.9.1.post2/aesara/scalar/c_code/Faddeeva.cc`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/c_code/Faddeeva.hh` & `aesara_nightly-2.9.1.post2/aesara/scalar/c_code/Faddeeva.hh`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scalar/c_code/gamma.c` & `aesara_nightly-2.9.1.post2/aesara/scalar/c_code/gamma.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/scan/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/basic.py` & `aesara_nightly-2.9.1.post2/aesara/scan/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/checkpoints.py` & `aesara_nightly-2.9.1.post2/aesara/scan/checkpoints.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/op.py` & `aesara_nightly-2.9.1.post2/aesara/scan/op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/rewriting.py` & `aesara_nightly-2.9.1.post2/aesara/scan/rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/scan_perform.pyx` & `aesara_nightly-2.9.1.post2/aesara/scan/scan_perform.pyx`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/scan_perform_ext.py` & `aesara_nightly-2.9.1.post2/aesara/scan/scan_perform_ext.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/utils.py` & `aesara_nightly-2.9.1.post2/aesara/scan/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/views.py` & `aesara_nightly-2.9.1.post2/aesara/scan/views.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/scan/c_code/scan_perform.c` & `aesara_nightly-2.9.1.post2/aesara/scan/c_code/scan_perform.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/basic.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/rewriting.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/sharedvar.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/sharedvar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/type.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/utils.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/sandbox/sp.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/sandbox/sp.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/sparse/sandbox/sp2.py` & `aesara_nightly-2.9.1.post2/aesara/sparse/sandbox/sp2.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/basic.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/blas.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/blas.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/blas_c.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/blas_c.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/blas_headers.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/blas_headers.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/blas_scipy.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/blas_scipy.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/elemwise.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/elemwise_cgen.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/elemwise_cgen.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/extra_ops.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/fft.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/fft.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/fourier.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/fourier.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/inplace.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/inplace.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/io.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/io.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/math.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/math.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nlinalg.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nlinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/shape.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/shape.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/sharedvar.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/sharedvar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/slinalg.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/slinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/sort.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/sort.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/special.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/special.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/subtensor.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/subtensor.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/type.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/type_other.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/type_other.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/utils.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/var.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/var.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/xlogx.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/xlogx.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/c_code/alt_blas_common.h` & `aesara_nightly-2.9.1.post2/aesara/tensor/c_code/alt_blas_common.h`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/c_code/alt_blas_template.c` & `aesara_nightly-2.9.1.post2/aesara/tensor/c_code/alt_blas_template.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/c_code/dimshuffle.c` & `aesara_nightly-2.9.1.post2/aesara/tensor/c_code/dimshuffle.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/__init__.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/abstract_conv.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/abstract_conv.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/basic.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/batchnorm.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/batchnorm.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/blocksparse.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/blocksparse.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/conv.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/conv.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/conv3d2d.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/conv3d2d.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/corr.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/corr.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/corr3d.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/corr3d.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/ctc.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/ctc.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/neighbours.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/neighbours.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/rewriting.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/sigm.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/sigm.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/c_code/corr3d_gemm.c` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/c_code/corr3d_gemm.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/c_code/corr_gemm.c` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/c_code/corr_gemm.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/nnet/c_code/ctc_wrapper.c` & `aesara_nightly-2.9.1.post2/aesara/tensor/nnet/c_code/ctc_wrapper.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/random/basic.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/random/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/random/op.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/random/op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/random/type.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/random/type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/random/utils.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/random/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/random/var.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/random/var.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/random/rewriting/basic.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/random/rewriting/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/random/rewriting/jax.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/random/rewriting/jax.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/basic.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/elemwise.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/extra_ops.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/jax.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/jax.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/math.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/math.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/shape.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/shape.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/special.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/special.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/subtensor.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/subtensor.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/rewriting/uncanonicalize.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/rewriting/uncanonicalize.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/signal/conv.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/signal/conv.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/tensor/signal/pool.py` & `aesara_nightly-2.9.1.post2/aesara/tensor/signal/pool.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/typed_list/basic.py` & `aesara_nightly-2.9.1.post2/aesara/typed_list/basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/typed_list/rewriting.py` & `aesara_nightly-2.9.1.post2/aesara/typed_list/rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/aesara/typed_list/type.py` & `aesara_nightly-2.9.1.post2/aesara/typed_list/type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/acknowledgement.rst` & `aesara_nightly-2.9.1.post2/doc/acknowledgement.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/conf.py` & `aesara_nightly-2.9.1.post2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/config.rst` & `aesara_nightly-2.9.1.post2/doc/config.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/core_development_guide.rst` & `aesara_nightly-2.9.1.post2/doc/core_development_guide.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/dev_start_guide.rst` & `aesara_nightly-2.9.1.post2/doc/dev_start_guide.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/generate_dtype_tensor_table.py` & `aesara_nightly-2.9.1.post2/doc/generate_dtype_tensor_table.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/glossary.rst` & `aesara_nightly-2.9.1.post2/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/help.rst` & `aesara_nightly-2.9.1.post2/doc/help.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/how_to_think_in_aesara.rst` & `aesara_nightly-2.9.1.post2/doc/how_to_think_in_aesara.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/index.rst` & `aesara_nightly-2.9.1.post2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/install.rst` & `aesara_nightly-2.9.1.post2/doc/install.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/introduction.rst` & `aesara_nightly-2.9.1.post2/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/mission.rst` & `aesara_nightly-2.9.1.post2/doc/mission.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/pylintrc` & `aesara_nightly-2.9.1.post2/doc/pylintrc`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/.static/version_switch.js` & `aesara_nightly-2.9.1.post2/doc/.static/version_switch.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/.templates/layout.html` & `aesara_nightly-2.9.1.post2/doc/.templates/layout.html`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/debugmode.rst` & `aesara_nightly-2.9.1.post2/doc/compile/debugmode.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/function.rst` & `aesara_nightly-2.9.1.post2/doc/compile/function.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/io.rst` & `aesara_nightly-2.9.1.post2/doc/compile/io.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/mode.rst` & `aesara_nightly-2.9.1.post2/doc/compile/mode.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/modes.rst` & `aesara_nightly-2.9.1.post2/doc/compile/modes.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/modes_solution_1.py` & `aesara_nightly-2.9.1.post2/doc/compile/modes_solution_1.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/nanguardmode.rst` & `aesara_nightly-2.9.1.post2/doc/compile/nanguardmode.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/opfromgraph.rst` & `aesara_nightly-2.9.1.post2/doc/compile/opfromgraph.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/shared.rst` & `aesara_nightly-2.9.1.post2/doc/compile/shared.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/compile/rewrites/index.rst` & `aesara_nightly-2.9.1.post2/doc/compile/rewrites/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/backend/creating_a_c_op.rst` & `aesara_nightly-2.9.1.post2/doc/extend/backend/creating_a_c_op.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/backend/creating_a_numba_jax_op.rst` & `aesara_nightly-2.9.1.post2/doc/extend/backend/creating_a_numba_jax_op.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/backend/ctype.rst` & `aesara_nightly-2.9.1.post2/doc/extend/backend/ctype.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/op/apply.png` & `aesara_nightly-2.9.1.post2/doc/extend/op/apply.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/op/apply.svg` & `aesara_nightly-2.9.1.post2/doc/extend/op/apply.svg`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/op/apply2.svg` & `aesara_nightly-2.9.1.post2/doc/extend/op/apply2.svg`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/op/creating_an_op.rst` & `aesara_nightly-2.9.1.post2/doc/extend/op/creating_an_op.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/op/how_to_make_ops.rst` & `aesara_nightly-2.9.1.post2/doc/extend/op/how_to_make_ops.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/op/index.rst` & `aesara_nightly-2.9.1.post2/doc/extend/op/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/extend/op/inplace.rst` & `aesara_nightly-2.9.1.post2/doc/extend/op/inplace.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/compilation/pipeline.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/compilation/pipeline.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/apply.png` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/apply.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/apply.svg` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/apply.svg`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/apply2.svg` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/apply2.svg`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graphstructures.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graphstructures.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/op.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/op.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/other_ops.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/other_ops.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/symbolic_graph_opt.png` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/symbolic_graph_opt.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/symbolic_graph_unopt.png` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/symbolic_graph_unopt.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/type.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/type.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/using_params.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/using_params.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/features.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/features.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/graph/graph/fgraph.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/graph/graph/fgraph.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/rewrites/graph_rewriting.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/rewrites/graph_rewriting.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/fundamentals/rewrites/optimizations.rst` & `aesara_nightly-2.9.1.post2/doc/fundamentals/rewrites/optimizations.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/Elman_srnn.png` & `aesara_nightly-2.9.1.post2/doc/images/Elman_srnn.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/aesara_logo_200.png` & `aesara_nightly-2.9.1.post2/doc/images/aesara_logo_200.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/aesara_logo_2400.png` & `aesara_nightly-2.9.1.post2/doc/images/aesara_logo_2400.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/aesara_overview_diagram.png` & `aesara_nightly-2.9.1.post2/doc/images/aesara_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/blocksparse.png` & `aesara_nightly-2.9.1.post2/doc/images/blocksparse.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/lstm.png` & `aesara_nightly-2.9.1.post2/doc/images/lstm.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/lstm_memorycell.png` & `aesara_nightly-2.9.1.post2/doc/images/lstm_memorycell.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/talk2010.gif` & `aesara_nightly-2.9.1.post2/doc/images/talk2010.gif`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/images/talk2010.png` & `aesara_nightly-2.9.1.post2/doc/images/talk2010.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/conditionals.rst` & `aesara_nightly-2.9.1.post2/doc/reference/conditionals.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/gradient/dlogistic.png` & `aesara_nightly-2.9.1.post2/doc/reference/gradient/dlogistic.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/gradient/gradient_api.rst` & `aesara_nightly-2.9.1.post2/doc/reference/gradient/gradient_api.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/gradient/gradient_tutorial.rst` & `aesara_nightly-2.9.1.post2/doc/reference/gradient/gradient_tutorial.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/gradient/index.rst` & `aesara_nightly-2.9.1.post2/doc/reference/gradient/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/loops/index.rst` & `aesara_nightly-2.9.1.post2/doc/reference/loops/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/loops/loop_solution_1.py` & `aesara_nightly-2.9.1.post2/doc/reference/loops/loop_solution_1.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/loops/loops_api.rst` & `aesara_nightly-2.9.1.post2/doc/reference/loops/loops_api.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/loops/loops_tutorial.rst` & `aesara_nightly-2.9.1.post2/doc/reference/loops/loops_tutorial.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/loops/scan_extend.rst` & `aesara_nightly-2.9.1.post2/doc/reference/loops/scan_extend.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/random/index.rst` & `aesara_nightly-2.9.1.post2/doc/reference/random/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/bcast.png` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/bcast.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/bcast.svg` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/bcast.svg`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/create.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/create.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/index.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.binary_operations.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.binary_operations.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.discrete_fourier.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.discrete_fourier.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.indexing.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.indexing.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.linalg.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.linalg.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.logic.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.logic.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.mathematical_functions.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.mathematical_functions.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.tensor_creation.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.tensor_creation.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/operations.tensor_manipulation.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/operations.tensor_manipulation.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/shapes.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/shapes.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/tensor.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/tensor.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/shared/aliasing.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/shared/aliasing.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/sparse/index.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/sparse/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/sparse/sandbox.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/sparse/sandbox.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/reference/tensor/sparse/sparse_api.rst` & `aesara_nightly-2.9.1.post2/doc/reference/tensor/sparse/sparse_api.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/ccodegen.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/ccodegen.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/debugging_with_stepmode.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/debugging_with_stepmode.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/elemwise_compiler.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/elemwise_compiler.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/interactive_debugger.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/interactive_debugger.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/logistic_regression_example.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/logistic_regression_example.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/performance.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/performance.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/randomnumbers.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/randomnumbers.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/rethinkccodegen.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/rethinkccodegen.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/sandbox.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/sandbox.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/software.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/software.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/sandbox/sparse.rst` & `aesara_nightly-2.9.1.post2/doc/sandbox/sparse.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/scripts/docgen.py` & `aesara_nightly-2.9.1.post2/doc/scripts/docgen.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/serializing/loading_and_saving.rst` & `aesara_nightly-2.9.1.post2/doc/serializing/loading_and_saving.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/debug_faq.rst` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/debug_faq.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/logreg_pydotprint_predict.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/logreg_pydotprint_predict.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/logreg_pydotprint_prediction.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/logreg_pydotprint_prediction.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/logreg_pydotprint_train.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/logreg_pydotprint_train.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/nan_tutorial.rst` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/nan_tutorial.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/printing.rst` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/printing.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/printing_drawing.rst` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/printing_drawing.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/profiling.rst` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/profiling.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/profiling_example_out.prof` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/profiling_example_out.prof`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/troubleshooting.rst` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index.ipynb` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index.ipynb`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index.rst` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index.rst`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp.html` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp.html`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp2.html` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp2.html`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp2.pdf` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp2.pdf`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/mlp2.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/mlp2.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/ofg.html` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/ofg.html`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/ofg2.html` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/ofg2.html`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/css/d3viz.css` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/css/d3viz.css`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/d3-context-menu.js` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/d3-context-menu.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/d3.v3.min.js` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/d3viz.js` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/d3viz.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/dagre-d3.min.js` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/examples/d3viz/js/graphlib-dot.min.js` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/examples/d3viz/js/graphlib-dot.min.js`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_10_0.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_10_0.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_11_0.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_11_0.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_24_0.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_24_0.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/doc/troubleshoot/d3viz/index_files/index_25_0.png` & `aesara_nightly-2.9.1.post2/doc/troubleshoot/d3viz/index_files/index_25_0.png`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_breakpoint.py` & `aesara_nightly-2.9.1.post2/tests/test_breakpoint.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_config.py` & `aesara_nightly-2.9.1.post2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_gradient.py` & `aesara_nightly-2.9.1.post2/tests/test_gradient.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_ifelse.py` & `aesara_nightly-2.9.1.post2/tests/test_ifelse.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_printing.py` & `aesara_nightly-2.9.1.post2/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_raise_op.py` & `aesara_nightly-2.9.1.post2/tests/test_raise_op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_rop.py` & `aesara_nightly-2.9.1.post2/tests/test_rop.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/test_updates.py` & `aesara_nightly-2.9.1.post2/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/unittest_tools.py` & `aesara_nightly-2.9.1.post2/tests/unittest_tools.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_builders.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_builders.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_compilelock.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_compilelock.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_debugmode.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_debugmode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_misc.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_misc.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_mode.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_mode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_monitormode.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_monitormode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_nanguardmode.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_nanguardmode.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_ops.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_profiling.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_profiling.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/test_shared.py` & `aesara_nightly-2.9.1.post2/tests/compile/test_shared.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/function/test_function.py` & `aesara_nightly-2.9.1.post2/tests/compile/function/test_function.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/function/test_pfunc.py` & `aesara_nightly-2.9.1.post2/tests/compile/function/test_pfunc.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/compile/function/test_types.py` & `aesara_nightly-2.9.1.post2/tests/compile/function/test_types.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/d3viz/models.py` & `aesara_nightly-2.9.1.post2/tests/d3viz/models.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/d3viz/test_d3viz.py` & `aesara_nightly-2.9.1.post2/tests/d3viz/test_d3viz.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/d3viz/test_formatting.py` & `aesara_nightly-2.9.1.post2/tests/d3viz/test_formatting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_compute_test_value.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_compute_test_value.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_destroyhandler.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_destroyhandler.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_features.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_features.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_fg.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_fg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_op.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_sched.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_sched.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/test_types.py` & `aesara_nightly-2.9.1.post2/tests/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/utils.py` & `aesara_nightly-2.9.1.post2/tests/graph/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_db.py` & `aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_db.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_kanren.py` & `aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_kanren.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_unify.py` & `aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_unify.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/graph/rewriting/test_utils.py` & `aesara_nightly-2.9.1.post2/tests/graph/rewriting/test_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/test_link.py` & `aesara_nightly-2.9.1.post2/tests/link/test_link.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/test_utils.py` & `aesara_nightly-2.9.1.post2/tests/link/test_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/test_vm.py` & `aesara_nightly-2.9.1.post2/tests/link/test_vm.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/c/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/link/c/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/c/test_cmodule.py` & `aesara_nightly-2.9.1.post2/tests/link/c/test_cmodule.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/c/test_op.py` & `aesara_nightly-2.9.1.post2/tests/link/c/test_op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/c/test_params_type.py` & `aesara_nightly-2.9.1.post2/tests/link/c/test_params_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/c/test_type.py` & `aesara_nightly-2.9.1.post2/tests/link/c/test_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/c/c_code/test_quadratic_function.c` & `aesara_nightly-2.9.1.post2/tests/link/c/c_code/test_quadratic_function.c`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_elemwise.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_extra_ops.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_nlinalg.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_nlinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_random.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_random.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_scalar.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_scalar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_scan.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_scan.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_shape.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_shape.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_slinalg.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_slinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_subtensor.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/jax/test_tensor_basic.py` & `aesara_nightly-2.9.1.post2/tests/link/jax/test_tensor_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_elemwise.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_extra_ops.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_nlinalg.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_nlinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_performance.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_performance.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_random.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_random.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_scalar.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_scalar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_scan.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_scan.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_sparse.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_sparse.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/link/numba/test_tensor_basic.py` & `aesara_nightly-2.9.1.post2/tests/link/numba/test_tensor_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/misc/test_may_share_memory.py` & `aesara_nightly-2.9.1.post2/tests/misc/test_may_share_memory.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/misc/test_pkl_utils.py` & `aesara_nightly-2.9.1.post2/tests/misc/test_pkl_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sandbox/test_minimal.py` & `aesara_nightly-2.9.1.post2/tests/sandbox/test_minimal.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sandbox/test_multinomial.py` & `aesara_nightly-2.9.1.post2/tests/sandbox/test_multinomial.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sandbox/test_multinomial_wo_replacement.py` & `aesara_nightly-2.9.1.post2/tests/sandbox/test_multinomial_wo_replacement.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sandbox/test_rng_mrg.py` & `aesara_nightly-2.9.1.post2/tests/sandbox/test_rng_mrg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sandbox/linalg/test_linalg.py` & `aesara_nightly-2.9.1.post2/tests/sandbox/linalg/test_linalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scalar/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/scalar/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scalar/test_basic_sympy.py` & `aesara_nightly-2.9.1.post2/tests/scalar/test_basic_sympy.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scalar/test_math.py` & `aesara_nightly-2.9.1.post2/tests/scalar/test_math.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scalar/test_type.py` & `aesara_nightly-2.9.1.post2/tests/scalar/test_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scan/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/scan/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scan/test_checkpoints.py` & `aesara_nightly-2.9.1.post2/tests/scan/test_checkpoints.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scan/test_printing.py` & `aesara_nightly-2.9.1.post2/tests/scan/test_printing.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scan/test_rewriting.py` & `aesara_nightly-2.9.1.post2/tests/scan/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scan/test_utils.py` & `aesara_nightly-2.9.1.post2/tests/scan/test_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/scan/test_views.py` & `aesara_nightly-2.9.1.post2/tests/scan/test_views.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sparse/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/sparse/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sparse/test_rewriting.py` & `aesara_nightly-2.9.1.post2/tests/sparse/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sparse/test_sp2.py` & `aesara_nightly-2.9.1.post2/tests/sparse/test_sp2.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sparse/test_type.py` & `aesara_nightly-2.9.1.post2/tests/sparse/test_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sparse/test_utils.py` & `aesara_nightly-2.9.1.post2/tests/sparse/test_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sparse/test_var.py` & `aesara_nightly-2.9.1.post2/tests/sparse/test_var.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/sparse/sandbox/test_sp.py` & `aesara_nightly-2.9.1.post2/tests/sparse/sandbox/test_sp.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/_test_mpi_roundtrip.py` & `aesara_nightly-2.9.1.post2/tests/tensor/_test_mpi_roundtrip.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_blas.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_blas.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_blas_c.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_blas_c.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_blas_scipy.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_blas_scipy.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_casting.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_casting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_complex.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_complex.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_elemwise.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_extra_ops.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_fft.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_fft.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_fourier.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_fourier.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_gc.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_gc.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_inplace.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_inplace.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_io.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_io.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_keepdims.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_keepdims.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_math.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_math.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_math_scipy.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_math_scipy.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_merge.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_merge.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_misc.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_misc.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_mpi.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_mpi.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_nlinalg.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_nlinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_shape.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_shape.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_sharedvar.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_sharedvar.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_slinalg.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_slinalg.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_sort.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_sort.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_special.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_special.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_subtensor.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_type.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_type_other.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_type_other.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_utils.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_var.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_var.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/test_xlogx.py` & `aesara_nightly-2.9.1.post2/tests/tensor/test_xlogx.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/utils.py` & `aesara_nightly-2.9.1.post2/tests/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/speed_test_conv.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/speed_test_conv.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_abstract_conv.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_abstract_conv.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_batchnorm.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_batchnorm.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_blocksparse.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_blocksparse.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_conv.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_conv.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_conv3d2d.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_conv3d2d.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_corr.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_corr.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_corr3d.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_corr3d.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_ctc.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_ctc.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_neighbours.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_neighbours.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_rewriting.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/nnet/test_sigm.py` & `aesara_nightly-2.9.1.post2/tests/tensor/nnet/test_sigm.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/random/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/tensor/random/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/random/test_op.py` & `aesara_nightly-2.9.1.post2/tests/tensor/random/test_op.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/random/test_rewriting.py` & `aesara_nightly-2.9.1.post2/tests/tensor/random/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/random/test_type.py` & `aesara_nightly-2.9.1.post2/tests/tensor/random/test_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/random/test_utils.py` & `aesara_nightly-2.9.1.post2/tests/tensor/random/test_utils.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/random/test_var.py` & `aesara_nightly-2.9.1.post2/tests/tensor/random/test_var.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_elemwise.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_elemwise.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_extra_ops.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_extra_ops.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_math.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_math.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_shape.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_shape.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_special.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_special.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_subtensor.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/rewriting/test_uncanonicalize.py` & `aesara_nightly-2.9.1.post2/tests/tensor/rewriting/test_uncanonicalize.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/signal/test_conv.py` & `aesara_nightly-2.9.1.post2/tests/tensor/signal/test_conv.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/tensor/signal/test_pool.py` & `aesara_nightly-2.9.1.post2/tests/tensor/signal/test_pool.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/typed_list/test_basic.py` & `aesara_nightly-2.9.1.post2/tests/typed_list/test_basic.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/typed_list/test_rewriting.py` & `aesara_nightly-2.9.1.post2/tests/typed_list/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/tests/typed_list/test_type.py` & `aesara_nightly-2.9.1.post2/tests/typed_list/test_type.py`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/.gitignore` & `aesara_nightly-2.9.1.post2/.gitignore`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/DESCRIPTION.txt` & `aesara_nightly-2.9.1.post2/DESCRIPTION.txt`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/LICENSE.txt` & `aesara_nightly-2.9.1.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/pyproject.toml` & `aesara_nightly-2.9.1.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aesara_nightly-2.9.0.post4/PKG-INFO` & `aesara_nightly-2.9.1.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aesara-nightly
-Version: 2.9.0.post4
+Version: 2.9.1.post2
 Summary: A library for defining, optimizing, and efficiently evaluating mathematical expressions involving multi-dimensional arrays.
 Project-URL: Homepage, https://github.com/aesara-devs/aesara
 Author-email: aesara-devs <aesara.devs@gmail.com>
 License: BSD-3-Clause
 License-File: LICENSE.txt
 Keywords: aesara,autodiff,blas,differentiation,math,numerical,numpy,symbolic
 Classifier: Development Status :: 6 - Mature
```

