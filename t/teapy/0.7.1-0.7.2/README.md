# Comparing `tmp/teapy-0.7.1.tar.gz` & `tmp/teapy-0.7.2.tar.gz`

## Comparing `teapy-0.7.1.tar` & `teapy-0.7.2.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0     1001      127     1303 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/Cargo.toml
--rw-r--r--   0     1001      127      483 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/benches/inplace.rs
--rw-r--r--   0     1001      127     3128 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/benches/rolling.rs
--rw-r--r--   0     1001      127     7438 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/agg/corr.rs
--rw-r--r--   0     1001      127     4196 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/agg/impl_lazy.rs
--rw-r--r--   0     1001      127    15258 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/agg/mod.rs
--rw-r--r--   0     1001      127     2200 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/create.rs
--rw-r--r--   0     1001      127     3794 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/from_py.rs
--rw-r--r--   0     1001      127      507 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/lib.rs
--rw-r--r--   0     1001      127     8740 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/linalg.rs
--rw-r--r--   0     1001      127     1993 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/macros.rs
--rw-r--r--   0     1001      127     9585 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_1d.rs
--rw-r--r--   0     1001      127     8689 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_arrok.rs
--rw-r--r--   0     1001      127     9095 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_inplace.rs
--rw-r--r--   0     1001      127    10333 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/impl_view.rs
--rw-r--r--   0     1001      127    15659 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/mod.rs
--rw-r--r--   0     1001      127     2000 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/stat.rs
--rw-r--r--   0     1001      127     1220 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/time.rs
--rw-r--r--   0     1001      127      834 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_string.rs
--rw-r--r--   0     1001      127      787 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_time.rs
--rw-r--r--   0     1001      127    21550 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/mod.rs
--rw-r--r--   0     1001      127    15701 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/cmp.rs
--rw-r--r--   0     1001      127     8069 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/corr.rs
--rw-r--r--   0     1001      127    26072 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/feature.rs
--rw-r--r--   0     1001      127    22724 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/impl_lazy/common.rs
--rw-r--r--   0     1001      127      311 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/impl_lazy/mod.rs
--rw-r--r--   0     1001      127      225 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/mod.rs
--rw-r--r--   0     1001      127     9721 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/norm.rs
--rw-r--r--   0     1001      127    32087 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/reg.rs
--rw-r--r--   0     1001      127      488 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/Cargo.toml
--rw-r--r--   0     1001      127    14011 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/lazy_impls.rs
--rw-r--r--   0     1001      127     1606 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/lib.rs
--rw-r--r--   0     1001      127     6291 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/methods_impls.rs
--rw-r--r--   0     1001      127    21958 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/tools.rs
--rw-r--r--   0     1001      127      811 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/Cargo.toml
--rw-r--r--   0     1001      127      236 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/context.rs
--rw-r--r--   0     1001      127    23144 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/dict.rs
--rw-r--r--   0     1001      127     3254 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/get_set.rs
--rw-r--r--   0     1001      127      189 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/mod.rs
--rw-r--r--   0     1001      127     3114 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/selector.rs
--rw-r--r--   0     1001      127    11891 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/data.rs
--rw-r--r--   0     1001      127    11943 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/expr.rs
--rw-r--r--   0     1001      127     1172 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/expr_element.rs
--rw-r--r--   0     1001      127    11553 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/expr_inner.rs
--rw-r--r--   0     1001      127     6642 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/auto_impl.rs
--rw-r--r--   0     1001      127     3184 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_cast.rs
--rw-r--r--   0     1001      127     1394 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
--rw-r--r--   0     1001      127    15326 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_ops.rs
--rw-r--r--   0     1001      127      889 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/mod.rs
--rw-r--r--   0     1001      127     2393 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/utils.rs
--rw-r--r--   0     1001      127      404 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/mod.rs
--rw-r--r--   0     1001      127    14135 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/groupby.rs
--rw-r--r--   0     1001      127    11113 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/join.rs
--rw-r--r--   0     1001      127      355 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/lib.rs
--rw-r--r--   0     1001      127     8791 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/linalg.rs
--rw-r--r--   0     1001      127      708 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/Cargo.toml
--rw-r--r--   0     1001      127     2062 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/impl_lazy.rs
--rw-r--r--   0     1001      127     5281 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/ipc.rs
--rw-r--r--   0     1001      127      203 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/mod.rs
--rw-r--r--   0     1001      127      966 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/utils.rs
--rw-r--r--   0     1001      127     2394 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/colselect.rs
--rw-r--r--   0     1001      127      251 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/lib.rs
--rw-r--r--   0     1001      127      271 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/Cargo.toml
--rw-r--r--   0     1001      127     3666 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/algos.rs
--rw-r--r--   0     1001      127     1798 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/alloc.rs
--rw-r--r--   0     1001      127      231 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/lib.rs
--rw-r--r--   0     1001      127      324 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/macros.rs
--rw-r--r--   0     1001      127     2274 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/traits.rs
--rw-r--r--   0     1001      127     1583 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/Cargo.toml
--rw-r--r--   0     1001      127    15544 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/arbarray.rs
--rw-r--r--   0     1001      127    25348 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/arrok.rs
--rw-r--r--   0     1001      127    16304 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_1d_method.rs
--rw-r--r--   0     1001      127     4115 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_basic.rs
--rw-r--r--   0     1001      127     8421 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_method.rs
--rw-r--r--   0     1001      127     8160 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_numeric.rs
--rw-r--r--   0     1001      127      648 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_time.rs
--rw-r--r--   0     1001      127     6070 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_traits.rs
--rw-r--r--   0     1001      127      451 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/generate.rs
--rw-r--r--   0     1001      127     7390 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/layout.rs
--rw-r--r--   0     1001      127     9188 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/least_squares.rs
--rw-r--r--   0     1001      127      242 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/mod.rs
--rw-r--r--   0     1001      127     5004 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/svd.rs
--rw-r--r--   0     1001      127      436 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/utils.rs
--rw-r--r--   0     1001      127      312 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/mod.rs
--rw-r--r--   0     1001      127    10460 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/iterators.rs
--rw-r--r--   0     1001      127    14095 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/lib.rs
--rw-r--r--   0     1001      127    10802 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/macros.rs
--rw-r--r--   0     1001      127     3011 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/own.rs
--rw-r--r--   0     1001      127      721 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/prelude.rs
--rw-r--r--   0     1001      127      694 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/traits.rs
--rw-r--r--   0     1001      127     3042 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/view.rs
--rw-r--r--   0     1001      127     2031 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/viewmut.rs
--rw-r--r--   0     1001      127     1030 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/Cargo.toml
--rw-r--r--   0     1001      127     1044 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/benches/groupby.rs
--rw-r--r--   0     1001      127      613 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/from_py.rs
--rw-r--r--   0     1001      127     9610 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/groupby_agg.rs
--rw-r--r--   0     1001      127     5202 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/impl_lazy.rs
--rw-r--r--   0     1001      127    15347 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/join.rs
--rw-r--r--   0     1001      127    15380 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/lib.rs
--rw-r--r--   0     1001      127     7106 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/unique.rs
--rw-r--r--   0     1001      127      463 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-hash/Cargo.toml
--rw-r--r--   0     1001      127     3243 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-hash/src/lib.rs
--rw-r--r--   0     1001      127      619 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/Cargo.toml
--rw-r--r--   0     1001      127    13696 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/cast.rs
--rw-r--r--   0     1001      127    14632 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/lib.rs
--rw-r--r--   0     1001      127    12152 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/option_datatype.rs
--rw-r--r--   0     1001      127     2752 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/pyvalue.rs
--rw-r--r--   0     1001      127      289 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/Cargo.toml
--rw-r--r--   0     1001      127      755 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/convert.rs
--rw-r--r--   0     1001      127     9144 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/datetime.rs
--rw-r--r--   0     1001      127     2036 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/impl_datetime.rs
--rw-r--r--   0     1001      127     2135 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/impl_ops.rs
--rw-r--r--   0     1001      127      869 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/impl_timedelta.rs
--rw-r--r--   0     1001      127       53 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/mod.rs
--rw-r--r--   0     1001      127      198 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/lib.rs
--rw-r--r--   0     1001      127     2980 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/timedelta.rs
--rw-r--r--   0     1001      127      842 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/timeunit.rs
--rw-r--r--   0     1001      127      286 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-error/Cargo.toml
--rw-r--r--   0     1001      127     1398 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-error/src/lib.rs
--rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 teapy-0.7.1/tea-py/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/.python-version
--rw-r--r--   0     1001      127     1053 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/LICENSE
--rw-r--r--   0     1001      127     1417 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/Makefile
--rw-r--r--   0     1001      127     2202 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/README.md
--rw-r--r--   0     1001      127      232 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/build.requirements.txt
--rw-r--r--   0     1001      127     2765 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/__init__.py
--rw-r--r--   0     1001      127     4525 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/array_func.py
--rw-r--r--   0     1001      127    11351 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/expr.py
--rw-r--r--   0     1001      127     3253 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/mod_func.py
--rw-r--r--   0     1001      127    18730 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/py_datadict.py
--rw-r--r--   0     1001      127     9635 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/regression.py
--rw-r--r--   0     1001      127     7368 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/selector.py
--rw-r--r--   0     1001      127     3455 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/testing.py
--rw-r--r--   0     1001      127    12448 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      127     2094 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_common.py
--rw-r--r--   0     1001      127      967 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_context.py
--rw-r--r--   0     1001      127     8565 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      127     2303 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_equity.py
--rw-r--r--   0     1001      127     4772 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_expr.py
--rw-r--r--   0     1001      127      465 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_memory.py
--rw-r--r--   0     1001      127      339 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_time.py
--rw-r--r--   0     1001      127     3210 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      127     1417 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      127     5771 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      127     1994 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      127     3194 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      127     3458 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/window_func.py
--rw-r--r--   0     1001      127     1232 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/wrapper.py
--rw-r--r--   0     1001      127     1291 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/requirements-dev.lock
--rw-r--r--   0     1001      127      197 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/requirements.lock
--rw-r--r--   0     1001      127    23237 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/equity.rs
--rw-r--r--   0     1001      127     7135 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/from_py.rs
--rw-r--r--   0     1001      127     1127 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/lib.rs
--rw-r--r--   0     1001      127    13232 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/datadict.rs
--rw-r--r--   0     1001      127      322 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/export.rs
--rw-r--r--   0     1001      127     2929 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/groupby.rs
--rw-r--r--   0     1001      127    97651 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      127     1898 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/mod.rs
--rw-r--r--   0     1001      127     5443 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      127    18957 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      127     2202 2024-04-25 05:39:11.000000 teapy-0.7.1/README.md
--rw-r--r--   0     1001      127    57288 2024-04-25 05:40:04.000000 teapy-0.7.1/Cargo.lock
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 teapy-0.7.1/Cargo.toml
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 teapy-0.7.1/pyproject.toml
--rw-r--r--   0     1001      127     3253 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/mod_func.py
--rw-r--r--   0     1001      127     1232 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/wrapper.py
--rw-r--r--   0     1001      127    18730 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/py_datadict.py
--rw-r--r--   0     1001      127     7368 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/selector.py
--rw-r--r--   0     1001      127     2765 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/__init__.py
--rw-r--r--   0     1001      127     4525 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/array_func.py
--rw-r--r--   0     1001      127      967 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_context.py
--rw-r--r--   0     1001      127    12448 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      127     4772 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_expr.py
--rw-r--r--   0     1001      127     2303 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_equity.py
--rw-r--r--   0     1001      127     1994 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      127     3194 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      127     1417 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      127     5771 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      127     3210 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      127     8565 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      127      339 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_time.py
--rw-r--r--   0     1001      127      465 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_memory.py
--rw-r--r--   0     1001      127     2094 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_common.py
--rw-r--r--   0     1001      127     3458 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/window_func.py
--rw-r--r--   0     1001      127     9635 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/regression.py
--rw-r--r--   0     1001      127     3455 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/testing.py
--rw-r--r--   0     1001      127    11351 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/expr.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 teapy-0.7.1/PKG-INFO
+-rw-r--r--   0     1001      127     1583 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/Cargo.toml
+-rw-r--r--   0     1001      127    15544 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/arbarray.rs
+-rw-r--r--   0     1001      127    25348 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/arrok.rs
+-rw-r--r--   0     1001      127    16304 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      127     4115 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_basic.rs
+-rw-r--r--   0     1001      127     8421 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_method.rs
+-rw-r--r--   0     1001      127     8160 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_numeric.rs
+-rw-r--r--   0     1001      127      648 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_time.rs
+-rw-r--r--   0     1001      127     6070 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/impl_traits.rs
+-rw-r--r--   0     1001      127      451 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/generate.rs
+-rw-r--r--   0     1001      127     7390 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/layout.rs
+-rw-r--r--   0     1001      127     9188 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/least_squares.rs
+-rw-r--r--   0     1001      127      242 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/mod.rs
+-rw-r--r--   0     1001      127     5004 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/svd.rs
+-rw-r--r--   0     1001      127      436 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/linalg/utils.rs
+-rw-r--r--   0     1001      127      312 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/impls/mod.rs
+-rw-r--r--   0     1001      127    10460 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/iterators.rs
+-rw-r--r--   0     1001      127    14095 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/lib.rs
+-rw-r--r--   0     1001      127    10802 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/macros.rs
+-rw-r--r--   0     1001      127     3011 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/own.rs
+-rw-r--r--   0     1001      127      721 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/prelude.rs
+-rw-r--r--   0     1001      127      694 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/traits.rs
+-rw-r--r--   0     1001      127     3042 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/view.rs
+-rw-r--r--   0     1001      127     2031 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-core/src/viewmut.rs
+-rw-r--r--   0     1001      127     1030 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/Cargo.toml
+-rw-r--r--   0     1001      127     1044 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/benches/groupby.rs
+-rw-r--r--   0     1001      127      613 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/from_py.rs
+-rw-r--r--   0     1001      127     9610 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/groupby_agg.rs
+-rw-r--r--   0     1001      127     5202 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/impl_lazy.rs
+-rw-r--r--   0     1001      127    15347 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/join.rs
+-rw-r--r--   0     1001      127    15380 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/lib.rs
+-rw-r--r--   0     1001      127     7106 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-groupby/src/unique.rs
+-rw-r--r--   0     1001      127      488 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/Cargo.toml
+-rw-r--r--   0     1001      127    14011 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/lazy_impls.rs
+-rw-r--r--   0     1001      127     1606 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/lib.rs
+-rw-r--r--   0     1001      127     6291 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/methods_impls.rs
+-rw-r--r--   0     1001      127    21958 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-macros/src/tools.rs
+-rw-r--r--   0     1001      127     1303 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/Cargo.toml
+-rw-r--r--   0     1001      127      483 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/benches/inplace.rs
+-rw-r--r--   0     1001      127     3128 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/benches/rolling.rs
+-rw-r--r--   0     1001      127     7438 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/agg/corr.rs
+-rw-r--r--   0     1001      127     4196 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/agg/impl_lazy.rs
+-rw-r--r--   0     1001      127    15258 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/agg/mod.rs
+-rw-r--r--   0     1001      127     2200 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/create.rs
+-rw-r--r--   0     1001      127     3794 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/from_py.rs
+-rw-r--r--   0     1001      127      507 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/lib.rs
+-rw-r--r--   0     1001      127     8740 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/linalg.rs
+-rw-r--r--   0     1001      127     1993 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/macros.rs
+-rw-r--r--   0     1001      127     9585 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_1d.rs
+-rw-r--r--   0     1001      127     8689 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_arrok.rs
+-rw-r--r--   0     1001      127     9095 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_inplace.rs
+-rw-r--r--   0     1001      127    10333 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/impl_view.rs
+-rw-r--r--   0     1001      127    15659 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127     2000 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/stat.rs
+-rw-r--r--   0     1001      127     1220 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_lazy/time.rs
+-rw-r--r--   0     1001      127      834 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_string.rs
+-rw-r--r--   0     1001      127      787 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/impl_time.rs
+-rw-r--r--   0     1001      127    21550 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/map/mod.rs
+-rw-r--r--   0     1001      127    15701 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/cmp.rs
+-rw-r--r--   0     1001      127     8069 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/corr.rs
+-rw-r--r--   0     1001      127    26072 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/feature.rs
+-rw-r--r--   0     1001      127    22724 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/impl_lazy/common.rs
+-rw-r--r--   0     1001      127      311 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127      225 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/mod.rs
+-rw-r--r--   0     1001      127     9721 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/norm.rs
+-rw-r--r--   0     1001      127    32087 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-ext/src/rolling/reg.rs
+-rw-r--r--   0     1001      127      289 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/Cargo.toml
+-rw-r--r--   0     1001      127      755 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/convert.rs
+-rw-r--r--   0     1001      127     9202 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/datetime.rs
+-rw-r--r--   0     1001      127     2062 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/impl_datetime.rs
+-rw-r--r--   0     1001      127     2135 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      869 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/impl_timedelta.rs
+-rw-r--r--   0     1001      127       53 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/impls/mod.rs
+-rw-r--r--   0     1001      127      198 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/lib.rs
+-rw-r--r--   0     1001      127     2980 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/timedelta.rs
+-rw-r--r--   0     1001      127      842 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-time/src/timeunit.rs
+-rw-r--r--   0     1001      127      286 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-error/Cargo.toml
+-rw-r--r--   0     1001      127     1398 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-error/src/lib.rs
+-rw-r--r--   0     1001      127      271 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/Cargo.toml
+-rw-r--r--   0     1001      127     3666 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/algos.rs
+-rw-r--r--   0     1001      127     1798 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/alloc.rs
+-rw-r--r--   0     1001      127      231 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/lib.rs
+-rw-r--r--   0     1001      127      324 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/macros.rs
+-rw-r--r--   0     1001      127     2274 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-utils/src/traits.rs
+-rw-r--r--   0     1001      127      619 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/Cargo.toml
+-rw-r--r--   0     1001      127    13696 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/cast.rs
+-rw-r--r--   0     1001      127    14632 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/lib.rs
+-rw-r--r--   0     1001      127    12152 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/option_datatype.rs
+-rw-r--r--   0     1001      127     2752 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-dtype/src/pyvalue.rs
+-rw-r--r--   0     1001      127      463 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-hash/Cargo.toml
+-rw-r--r--   0     1001      127     3243 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-hash/src/lib.rs
+-rw-r--r--   0     1001      127      811 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/Cargo.toml
+-rw-r--r--   0     1001      127      236 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/context.rs
+-rw-r--r--   0     1001      127    23144 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/dict.rs
+-rw-r--r--   0     1001      127     3254 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/get_set.rs
+-rw-r--r--   0     1001      127      189 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/mod.rs
+-rw-r--r--   0     1001      127     3114 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/datadict/selector.rs
+-rw-r--r--   0     1001      127    11891 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/data.rs
+-rw-r--r--   0     1001      127    11943 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/expr.rs
+-rw-r--r--   0     1001      127     1172 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/expr_element.rs
+-rw-r--r--   0     1001      127    11553 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/expr_inner.rs
+-rw-r--r--   0     1001      127     6642 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/auto_impl.rs
+-rw-r--r--   0     1001      127     3184 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_cast.rs
+-rw-r--r--   0     1001      127     1394 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
+-rw-r--r--   0     1001      127    15326 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      889 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/mod.rs
+-rw-r--r--   0     1001      127     2393 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/impls/utils.rs
+-rw-r--r--   0     1001      127      404 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/expr_core/mod.rs
+-rw-r--r--   0     1001      127    14135 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/groupby.rs
+-rw-r--r--   0     1001      127    11113 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/join.rs
+-rw-r--r--   0     1001      127      355 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/lib.rs
+-rw-r--r--   0     1001      127     8791 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-lazy/src/linalg.rs
+-rw-r--r--   0     1001      127      708 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/Cargo.toml
+-rw-r--r--   0     1001      127     2062 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/impl_lazy.rs
+-rw-r--r--   0     1001      127     5281 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/ipc.rs
+-rw-r--r--   0     1001      127      203 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/mod.rs
+-rw-r--r--   0     1001      127      966 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/arrow_io/utils.rs
+-rw-r--r--   0     1001      127     2394 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/colselect.rs
+-rw-r--r--   0     1001      127      251 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-io/src/lib.rs
+-rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 teapy-0.7.2/tea-py/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/.python-version
+-rw-r--r--   0     1001      127     1053 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/LICENSE
+-rw-r--r--   0     1001      127     1417 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/Makefile
+-rw-r--r--   0     1001      127     2202 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/README.md
+-rw-r--r--   0     1001      127      232 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/build.requirements.txt
+-rw-r--r--   0     1001      127     2765 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     4525 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/array_func.py
+-rw-r--r--   0     1001      127    11351 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/expr.py
+-rw-r--r--   0     1001      127     3253 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127    18730 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     9635 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/regression.py
+-rw-r--r--   0     1001      127     7368 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/selector.py
+-rw-r--r--   0     1001      127     3455 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/testing.py
+-rw-r--r--   0     1001      127    12448 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     2094 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127      967 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127     8565 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127     2303 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     4772 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127      465 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127      339 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127     3210 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     1417 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     1994 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     3194 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     3458 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127     1291 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/requirements-dev.lock
+-rw-r--r--   0     1001      127      197 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/requirements.lock
+-rw-r--r--   0     1001      127    23237 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/equity.rs
+-rw-r--r--   0     1001      127     7135 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/from_py.rs
+-rw-r--r--   0     1001      127     1127 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/lib.rs
+-rw-r--r--   0     1001      127    13232 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      127      322 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/export.rs
+-rw-r--r--   0     1001      127     2929 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      127    97651 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      127     1898 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/mod.rs
+-rw-r--r--   0     1001      127     5443 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      127    18957 2024-04-25 09:24:05.000000 teapy-0.7.2/tea-py/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      127     2202 2024-04-25 09:24:05.000000 teapy-0.7.2/README.md
+-rw-r--r--   0     1001      127    57288 2024-04-25 09:24:21.000000 teapy-0.7.2/Cargo.lock
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 teapy-0.7.2/Cargo.toml
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 teapy-0.7.2/pyproject.toml
+-rw-r--r--   0     1001      127     3253 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127    18730 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     7368 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/selector.py
+-rw-r--r--   0     1001      127     2765 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     4525 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/array_func.py
+-rw-r--r--   0     1001      127      967 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127    12448 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     4772 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127     2303 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     1994 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     3194 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     1417 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     3210 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     8565 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127      339 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127      465 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127     2094 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127     3458 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     9635 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/regression.py
+-rw-r--r--   0     1001      127     3455 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/testing.py
+-rw-r--r--   0     1001      127    11351 2024-04-25 09:24:05.000000 teapy-0.7.2/python/teapy/expr.py
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 teapy-0.7.2/PKG-INFO
```

### Comparing `teapy-0.7.1/tea-ext/Cargo.toml` & `teapy-0.7.2/tea-ext/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/benches/rolling.rs` & `teapy-0.7.2/tea-ext/benches/rolling.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/agg/corr.rs` & `teapy-0.7.2/tea-ext/src/agg/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/agg/impl_lazy.rs` & `teapy-0.7.2/tea-ext/src/agg/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/agg/mod.rs` & `teapy-0.7.2/tea-ext/src/agg/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/create.rs` & `teapy-0.7.2/tea-ext/src/create.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/from_py.rs` & `teapy-0.7.2/tea-ext/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/linalg.rs` & `teapy-0.7.2/tea-ext/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/macros.rs` & `teapy-0.7.2/tea-ext/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_1d.rs` & `teapy-0.7.2/tea-ext/src/map/impl_1d.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_arrok.rs` & `teapy-0.7.2/tea-ext/src/map/impl_arrok.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_inplace.rs` & `teapy-0.7.2/tea-ext/src/map/impl_inplace.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_lazy/impl_view.rs` & `teapy-0.7.2/tea-ext/src/map/impl_lazy/impl_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_lazy/mod.rs` & `teapy-0.7.2/tea-ext/src/map/impl_lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_lazy/stat.rs` & `teapy-0.7.2/tea-ext/src/map/impl_lazy/stat.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_lazy/time.rs` & `teapy-0.7.2/tea-ext/src/map/impl_lazy/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_string.rs` & `teapy-0.7.2/tea-ext/src/map/impl_string.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/impl_time.rs` & `teapy-0.7.2/tea-ext/src/map/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/map/mod.rs` & `teapy-0.7.2/tea-ext/src/map/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/rolling/cmp.rs` & `teapy-0.7.2/tea-ext/src/rolling/cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/rolling/corr.rs` & `teapy-0.7.2/tea-ext/src/rolling/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/rolling/feature.rs` & `teapy-0.7.2/tea-ext/src/rolling/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/rolling/impl_lazy/common.rs` & `teapy-0.7.2/tea-ext/src/rolling/impl_lazy/common.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/rolling/norm.rs` & `teapy-0.7.2/tea-ext/src/rolling/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-ext/src/rolling/reg.rs` & `teapy-0.7.2/tea-ext/src/rolling/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-macros/src/lazy_impls.rs` & `teapy-0.7.2/tea-macros/src/lazy_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-macros/src/lib.rs` & `teapy-0.7.2/tea-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-macros/src/methods_impls.rs` & `teapy-0.7.2/tea-macros/src/methods_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-macros/src/tools.rs` & `teapy-0.7.2/tea-macros/src/tools.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/Cargo.toml` & `teapy-0.7.2/tea-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/datadict/dict.rs` & `teapy-0.7.2/tea-lazy/src/datadict/dict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/datadict/get_set.rs` & `teapy-0.7.2/tea-lazy/src/datadict/get_set.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/datadict/selector.rs` & `teapy-0.7.2/tea-lazy/src/datadict/selector.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/data.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/data.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/expr.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/expr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/expr_element.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/expr_element.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/expr_inner.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/expr_inner.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/impls/auto_impl.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/impls/auto_impl.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_cast.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_ops.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/impls/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/impls/mod.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/impls/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/expr_core/impls/utils.rs` & `teapy-0.7.2/tea-lazy/src/expr_core/impls/utils.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/groupby.rs` & `teapy-0.7.2/tea-lazy/src/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/join.rs` & `teapy-0.7.2/tea-lazy/src/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-lazy/src/linalg.rs` & `teapy-0.7.2/tea-lazy/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-io/Cargo.toml` & `teapy-0.7.2/tea-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-io/src/arrow_io/impl_lazy.rs` & `teapy-0.7.2/tea-io/src/arrow_io/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-io/src/arrow_io/ipc.rs` & `teapy-0.7.2/tea-io/src/arrow_io/ipc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-io/src/arrow_io/utils.rs` & `teapy-0.7.2/tea-io/src/arrow_io/utils.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-io/src/colselect.rs` & `teapy-0.7.2/tea-io/src/colselect.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-utils/src/algos.rs` & `teapy-0.7.2/tea-utils/src/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-utils/src/alloc.rs` & `teapy-0.7.2/tea-utils/src/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-utils/src/traits.rs` & `teapy-0.7.2/tea-utils/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/Cargo.toml` & `teapy-0.7.2/tea-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/arbarray.rs` & `teapy-0.7.2/tea-core/src/arbarray.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/arrok.rs` & `teapy-0.7.2/tea-core/src/arrok.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/impl_1d_method.rs` & `teapy-0.7.2/tea-core/src/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/impl_basic.rs` & `teapy-0.7.2/tea-core/src/impls/impl_basic.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/impl_method.rs` & `teapy-0.7.2/tea-core/src/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/impl_numeric.rs` & `teapy-0.7.2/tea-core/src/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/impl_time.rs` & `teapy-0.7.2/tea-core/src/impls/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/impl_traits.rs` & `teapy-0.7.2/tea-core/src/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/linalg/layout.rs` & `teapy-0.7.2/tea-core/src/impls/linalg/layout.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/linalg/least_squares.rs` & `teapy-0.7.2/tea-core/src/impls/linalg/least_squares.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/impls/linalg/svd.rs` & `teapy-0.7.2/tea-core/src/impls/linalg/svd.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/iterators.rs` & `teapy-0.7.2/tea-core/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/lib.rs` & `teapy-0.7.2/tea-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/macros.rs` & `teapy-0.7.2/tea-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/own.rs` & `teapy-0.7.2/tea-core/src/own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/prelude.rs` & `teapy-0.7.2/tea-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/traits.rs` & `teapy-0.7.2/tea-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/view.rs` & `teapy-0.7.2/tea-core/src/view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-core/src/viewmut.rs` & `teapy-0.7.2/tea-core/src/viewmut.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/Cargo.toml` & `teapy-0.7.2/tea-groupby/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/benches/groupby.rs` & `teapy-0.7.2/tea-groupby/benches/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/src/from_py.rs` & `teapy-0.7.2/tea-groupby/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/src/groupby_agg.rs` & `teapy-0.7.2/tea-groupby/src/groupby_agg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/src/impl_lazy.rs` & `teapy-0.7.2/tea-groupby/src/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/src/join.rs` & `teapy-0.7.2/tea-groupby/src/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/src/lib.rs` & `teapy-0.7.2/tea-groupby/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-groupby/src/unique.rs` & `teapy-0.7.2/tea-groupby/src/unique.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-hash/src/lib.rs` & `teapy-0.7.2/tea-hash/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-dtype/Cargo.toml` & `teapy-0.7.2/tea-dtype/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-dtype/src/cast.rs` & `teapy-0.7.2/tea-dtype/src/cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-dtype/src/lib.rs` & `teapy-0.7.2/tea-dtype/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-dtype/src/option_datatype.rs` & `teapy-0.7.2/tea-dtype/src/option_datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-dtype/src/pyvalue.rs` & `teapy-0.7.2/tea-dtype/src/pyvalue.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-time/src/convert.rs` & `teapy-0.7.2/tea-time/src/convert.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-time/src/datetime.rs` & `teapy-0.7.2/tea-time/src/datetime.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 // use serde::{Deserialize, Serialize};
 use std::{
     cmp::Ordering,
     hash::Hash,
     ops::{Add, Div, Mul, Neg, Sub},
 };
 
-use chrono::{Datelike, DurationRound, Months, NaiveDateTime, NaiveTime, Timelike};
+use chrono::{DateTime as CrDateTime, Datelike, DurationRound, Months, NaiveTime, Timelike, Utc};
 
 use crate::{convert::*, TimeDelta};
 
 #[derive(Clone, Copy, Default, Hash, Eq, PartialEq, PartialOrd)]
-pub struct DateTime(pub Option<NaiveDateTime>);
+pub struct DateTime(pub Option<CrDateTime<Utc>>);
 
 impl DateTime {
     #[inline]
     pub fn into_i64(self) -> i64 {
         // self.map_or(i64::MIN, |dt| dt.timestamp_micros())
         self.0
             .map_or(i64::MIN, |dt| dt.timestamp_nanos_opt().unwrap_or(i64::MIN))
     }
 
     #[inline]
     pub fn from_timestamp_opt(secs: i64, nsecs: u32) -> Self {
-        Self(NaiveDateTime::from_timestamp_opt(secs, nsecs))
+        Self(CrDateTime::from_timestamp(secs, nsecs))
     }
 
     #[inline]
     pub fn from_timestamp_ms(ms: i64) -> Option<Self> {
         let mut secs = ms / MILLIS_PER_SEC;
         if ms < 0 {
             secs = secs.checked_sub(1)?;
@@ -94,15 +94,17 @@
         };
         Some(Self::from_timestamp_opt(secs, nsecs))
     }
 
     #[inline(always)]
     pub fn parse(s: &str, fmt: &str) -> Result<Self, String> {
         Ok(Self(Some(
-            NaiveDateTime::parse_from_str(s, fmt).map_err(|e| format!("{e}"))?,
+            CrDateTime::parse_from_str(s, fmt)
+                .map(|v| v.into())
+                .map_err(|e| format!("{e}"))?,
         )))
     }
 
     #[inline]
     pub fn strftime(&self, fmt: Option<&str>) -> String {
         if let Some(fmt) = fmt {
             self.0
```

### Comparing `teapy-0.7.1/tea-time/src/impls/impl_datetime.rs` & `teapy-0.7.2/tea-time/src/impls/impl_datetime.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use chrono::NaiveDateTime;
+use chrono::{DateTime as CrDateTime, Utc};
 use numpy::{
     datetime::{Datetime as NPDatetime, Unit as NPUnit},
     npyffi::NPY_DATETIMEUNIT,
 };
 // use serde::{Deserialize, Serialize};
 use crate::DateTime;
 use std::ops::Deref;
@@ -14,37 +14,37 @@
         } else {
             write!(f, "None")
         }
     }
 }
 
 impl Deref for DateTime {
-    type Target = Option<NaiveDateTime>;
+    type Target = Option<CrDateTime<Utc>>;
     #[inline(always)]
     fn deref(&self) -> &Self::Target {
         &self.0
     }
 }
 
 // impl Cast<i64> for DateTime {
 //     fn cast(self) -> i64 {
 //         self.into_i64()
 //     }
 // }
 
-impl From<Option<NaiveDateTime>> for DateTime {
+impl From<Option<CrDateTime<Utc>>> for DateTime {
     #[inline(always)]
-    fn from(dt: Option<NaiveDateTime>) -> Self {
+    fn from(dt: Option<CrDateTime<Utc>>) -> Self {
         Self(dt)
     }
 }
 
-impl From<NaiveDateTime> for DateTime {
+impl From<CrDateTime<Utc>> for DateTime {
     #[inline(always)]
-    fn from(dt: NaiveDateTime) -> Self {
+    fn from(dt: CrDateTime<Utc>) -> Self {
         Self(Some(dt))
     }
 }
 
 impl From<i64> for DateTime {
     #[inline]
     fn from(dt: i64) -> Self {
```

### Comparing `teapy-0.7.1/tea-time/src/impls/impl_ops.rs` & `teapy-0.7.2/tea-time/src/impls/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-time/src/impls/impl_timedelta.rs` & `teapy-0.7.2/tea-time/src/impls/impl_timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-time/src/timedelta.rs` & `teapy-0.7.2/tea-time/src/timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-time/src/timeunit.rs` & `teapy-0.7.2/tea-time/src/timeunit.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-error/src/lib.rs` & `teapy-0.7.2/tea-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/Cargo.toml` & `teapy-0.7.2/tea-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/LICENSE` & `teapy-0.7.2/tea-py/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/Makefile` & `teapy-0.7.2/tea-py/Makefile`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/README.md` & `teapy-0.7.2/tea-py/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/__init__.py` & `teapy-0.7.2/tea-py/python/teapy/__init__.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/array_func.py` & `teapy-0.7.2/tea-py/python/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/expr.py` & `teapy-0.7.2/tea-py/python/teapy/expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/mod_func.py` & `teapy-0.7.2/tea-py/python/teapy/mod_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/py_datadict.py` & `teapy-0.7.2/tea-py/python/teapy/py_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/regression.py` & `teapy-0.7.2/tea-py/python/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/selector.py` & `teapy-0.7.2/tea-py/python/teapy/selector.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/testing.py` & `teapy-0.7.2/tea-py/python/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/test_array_func.py` & `teapy-0.7.2/tea-py/python/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/test_common.py` & `teapy-0.7.2/tea-py/python/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/test_context.py` & `teapy-0.7.2/tea-py/python/teapy/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/test_datadict.py` & `teapy-0.7.2/tea-py/python/teapy/tests/test_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/test_equity.py` & `teapy-0.7.2/tea-py/python/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/test_expr.py` & `teapy-0.7.2/tea-py/python/teapy/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/window/test_compare.py` & `teapy-0.7.2/tea-py/python/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/window/test_corr.py` & `teapy-0.7.2/tea-py/python/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/window/test_feature.py` & `teapy-0.7.2/tea-py/python/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/window/test_norm.py` & `teapy-0.7.2/tea-py/python/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/tests/window/test_reg.py` & `teapy-0.7.2/tea-py/python/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/window_func.py` & `teapy-0.7.2/tea-py/python/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/python/teapy/wrapper.py` & `teapy-0.7.2/tea-py/python/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/requirements-dev.lock` & `teapy-0.7.2/tea-py/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/equity.rs` & `teapy-0.7.2/tea-py/src/equity.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/from_py.rs` & `teapy-0.7.2/tea-py/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/lib.rs` & `teapy-0.7.2/tea-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/pylazy/datadict.rs` & `teapy-0.7.2/tea-py/src/pylazy/datadict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/pylazy/groupby.rs` & `teapy-0.7.2/tea-py/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/pylazy/impl_pyexpr.rs` & `teapy-0.7.2/tea-py/src/pylazy/impl_pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/pylazy/mod.rs` & `teapy-0.7.2/tea-py/src/pylazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/pylazy/pyexpr.rs` & `teapy-0.7.2/tea-py/src/pylazy/pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/tea-py/src/pylazy/pyfunc.rs` & `teapy-0.7.2/tea-py/src/pylazy/pyfunc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/README.md` & `teapy-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/Cargo.lock` & `teapy-0.7.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1653,15 +1653,15 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tea-core"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "arrow2",
  "intel-mkl-src",
  "lapack-sys",
  "libc",
  "ndarray",
  "num",
@@ -1671,36 +1671,36 @@
  "tea-dtype",
  "tea-error",
  "tea-utils",
 ]
 
 [[package]]
 name = "tea-dtype"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ndarray",
  "num",
  "numpy",
  "pyo3",
  "serde",
  "tea-time",
  "tea-utils",
 ]
 
 [[package]]
 name = "tea-error"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "arrow2",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-ext"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ndarray",
  "num",
  "paste",
  "pyo3",
  "rayon",
  "statrs",
@@ -1708,74 +1708,74 @@
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-groupby"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ndarray",
  "pyo3",
  "rayon",
  "tea-core",
  "tea-ext",
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-hash"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ahash",
  "gxhash",
  "tea-dtype",
 ]
 
 [[package]]
 name = "tea-io"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "arrow2",
  "memmap2",
  "rayon",
  "tea-core",
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-lazy"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ndarray",
  "parking_lot",
  "pyo3",
  "rayon",
  "regex",
  "tea-core",
  "tea-hash",
 ]
 
 [[package]]
 name = "tea-macros"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ndarray",
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "tea-py"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "ahash",
  "chrono",
  "ndarray",
  "numpy",
  "once_cell",
  "parking_lot",
@@ -1788,25 +1788,25 @@
  "tea-hash",
  "tea-io",
  "tea-lazy",
 ]
 
 [[package]]
 name = "tea-time"
-version = "0.7.1"
+version = "0.7.2"
 dependencies = [
  "chrono",
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-utils"
-version = "0.7.1"
+version = "0.7.2"
 
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
```

### Comparing `teapy-0.7.1/Cargo.toml` & `teapy-0.7.2/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 resolver = "2"
 members = ["tea-core", "tea-dtype", "tea-error", "tea-ext", "tea-groupby", "tea-hash", "tea-io", "tea-lazy", "tea-macros", "tea-py", "tea-time", "tea-utils"]
 
 [workspace.package]
-version = "0.7.1"
+version = "0.7.2"
 authors = ["Teamon"]
 edition = "2021"
 repository = "https://github.com/Teamon9161/teapy"
 license = "MIT"
 
 [profile.release]
 lto = true
@@ -22,12 +22,12 @@
 regex = "1"
 serde = { version = "1.0", features = ["derive", "rc"] }
 # serde_with = {version = "3.0", features = ["chrono"]}
 ndarray = {features=['rayon', 'serde'], version="0.15"}
 numpy = "0.21.0"
 pyo3 = {version = "0.21.2", features = ["extension-module", "abi3-py38", "macros", "serde", "gil-refs"]}
 parking_lot = "0.12"
-chrono = {version = "0.4.31", features = ["serde"]}
+chrono = {version = "0.4.37", features = ["serde"]}
 arrow = {package = "arrow2", version = "0.18.0", default-features = false, features = ["io_ipc", "io_ipc_compression"]}
 
 [profile.dev]
 incremental = true
```

### Comparing `teapy-0.7.1/pyproject.toml` & `teapy-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/mod_func.py` & `teapy-0.7.2/python/teapy/mod_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/wrapper.py` & `teapy-0.7.2/python/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/py_datadict.py` & `teapy-0.7.2/python/teapy/py_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/selector.py` & `teapy-0.7.2/python/teapy/selector.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/__init__.py` & `teapy-0.7.2/python/teapy/__init__.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/array_func.py` & `teapy-0.7.2/python/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/test_context.py` & `teapy-0.7.2/python/teapy/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/test_array_func.py` & `teapy-0.7.2/python/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/test_expr.py` & `teapy-0.7.2/python/teapy/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/test_equity.py` & `teapy-0.7.2/python/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/window/test_norm.py` & `teapy-0.7.2/python/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/window/test_reg.py` & `teapy-0.7.2/python/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/window/test_corr.py` & `teapy-0.7.2/python/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/window/test_feature.py` & `teapy-0.7.2/python/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/window/test_compare.py` & `teapy-0.7.2/python/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/test_datadict.py` & `teapy-0.7.2/python/teapy/tests/test_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/tests/test_common.py` & `teapy-0.7.2/python/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/window_func.py` & `teapy-0.7.2/python/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/regression.py` & `teapy-0.7.2/python/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/testing.py` & `teapy-0.7.2/python/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/python/teapy/expr.py` & `teapy-0.7.2/python/teapy/expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.1/PKG-INFO` & `teapy-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: teapy
-Version: 0.7.1
+Version: 0.7.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
```

