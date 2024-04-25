# Comparing `tmp/teapy-0.7.0.tar.gz` & `tmp/teapy-0.7.1.tar.gz`

## Comparing `teapy-0.7.0.tar` & `teapy-0.7.1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0     1001      127      811 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/Cargo.toml
--rw-r--r--   0     1001      127      236 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/context.rs
--rw-r--r--   0     1001      127    23111 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/dict.rs
--rw-r--r--   0     1001      127     3254 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/get_set.rs
--rw-r--r--   0     1001      127      189 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/mod.rs
--rw-r--r--   0     1001      127     3114 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/selector.rs
--rw-r--r--   0     1001      127    11891 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/data.rs
--rw-r--r--   0     1001      127    11857 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/expr.rs
--rw-r--r--   0     1001      127     1172 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/expr_element.rs
--rw-r--r--   0     1001      127    11553 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/expr_inner.rs
--rw-r--r--   0     1001      127     6642 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/auto_impl.rs
--rw-r--r--   0     1001      127     3184 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_cast.rs
--rw-r--r--   0     1001      127     1394 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
--rw-r--r--   0     1001      127    15326 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_ops.rs
--rw-r--r--   0     1001      127      889 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/mod.rs
--rw-r--r--   0     1001      127     2393 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/utils.rs
--rw-r--r--   0     1001      127      404 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/mod.rs
--rw-r--r--   0     1001      127    14135 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/groupby.rs
--rw-r--r--   0     1001      127    11113 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/join.rs
--rw-r--r--   0     1001      127      415 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/lib.rs
--rw-r--r--   0     1001      127     8791 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/linalg.rs
--rw-r--r--   0     1001      127     1303 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/Cargo.toml
--rw-r--r--   0     1001      127      483 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/benches/inplace.rs
--rw-r--r--   0     1001      127     3128 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/benches/rolling.rs
--rw-r--r--   0     1001      127     7438 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/agg/corr.rs
--rw-r--r--   0     1001      127     4196 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/agg/impl_lazy.rs
--rw-r--r--   0     1001      127    15258 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/agg/mod.rs
--rw-r--r--   0     1001      127     2200 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/create.rs
--rw-r--r--   0     1001      127     3794 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/from_py.rs
--rw-r--r--   0     1001      127      507 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/lib.rs
--rw-r--r--   0     1001      127     8740 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/linalg.rs
--rw-r--r--   0     1001      127     1993 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/macros.rs
--rw-r--r--   0     1001      127     9597 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_1d.rs
--rw-r--r--   0     1001      127     8689 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_arrok.rs
--rw-r--r--   0     1001      127     9095 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_inplace.rs
--rw-r--r--   0     1001      127    10244 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/impl_view.rs
--rw-r--r--   0     1001      127    15659 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/mod.rs
--rw-r--r--   0     1001      127     2000 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/stat.rs
--rw-r--r--   0     1001      127     1220 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/time.rs
--rw-r--r--   0     1001      127      834 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_string.rs
--rw-r--r--   0     1001      127      787 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_time.rs
--rw-r--r--   0     1001      127    21550 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/mod.rs
--rw-r--r--   0     1001      127    15701 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/cmp.rs
--rw-r--r--   0     1001      127     8069 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/corr.rs
--rw-r--r--   0     1001      127    26072 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/feature.rs
--rw-r--r--   0     1001      127    22608 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/impl_lazy/common.rs
--rw-r--r--   0     1001      127      311 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/impl_lazy/mod.rs
--rw-r--r--   0     1001      127      225 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/mod.rs
--rw-r--r--   0     1001      127     9721 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/norm.rs
--rw-r--r--   0     1001      127    32087 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/reg.rs
--rw-r--r--   0     1001      127      463 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-hash/Cargo.toml
--rw-r--r--   0     1001      127     3243 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-hash/src/lib.rs
--rw-r--r--   0     1001      127      289 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/Cargo.toml
--rw-r--r--   0     1001      127      755 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/convert.rs
--rw-r--r--   0     1001      127     9104 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/datetime.rs
--rw-r--r--   0     1001      127     1995 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/impl_datetime.rs
--rw-r--r--   0     1001      127     2094 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/impl_ops.rs
--rw-r--r--   0     1001      127      869 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/impl_timedelta.rs
--rw-r--r--   0     1001      127       53 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/mod.rs
--rw-r--r--   0     1001      127      198 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/lib.rs
--rw-r--r--   0     1001      127     2980 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/timedelta.rs
--rw-r--r--   0     1001      127      842 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/timeunit.rs
--rw-r--r--   0     1001      127     1583 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/Cargo.toml
--rw-r--r--   0     1001      127    15449 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/arbarray.rs
--rw-r--r--   0     1001      127    25285 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/arrok.rs
--rw-r--r--   0     1001      127    16304 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_1d_method.rs
--rw-r--r--   0     1001      127     4115 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_basic.rs
--rw-r--r--   0     1001      127     8421 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_method.rs
--rw-r--r--   0     1001      127     8160 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_numeric.rs
--rw-r--r--   0     1001      127      648 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_time.rs
--rw-r--r--   0     1001      127     6070 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_traits.rs
--rw-r--r--   0     1001      127      451 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/generate.rs
--rw-r--r--   0     1001      127     7390 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/layout.rs
--rw-r--r--   0     1001      127     9212 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/least_squares.rs
--rw-r--r--   0     1001      127      242 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/mod.rs
--rw-r--r--   0     1001      127     5016 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/svd.rs
--rw-r--r--   0     1001      127      436 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/utils.rs
--rw-r--r--   0     1001      127      312 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/mod.rs
--rw-r--r--   0     1001      127    10460 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/iterators.rs
--rw-r--r--   0     1001      127    14095 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/lib.rs
--rw-r--r--   0     1001      127    10802 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/macros.rs
--rw-r--r--   0     1001      127     3011 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/own.rs
--rw-r--r--   0     1001      127      721 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/prelude.rs
--rw-r--r--   0     1001      127      694 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/traits.rs
--rw-r--r--   0     1001      127     3045 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/view.rs
--rw-r--r--   0     1001      127     2031 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/viewmut.rs
--rw-r--r--   0     1001      127     1030 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/Cargo.toml
--rw-r--r--   0     1001      127     1044 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/benches/groupby.rs
--rw-r--r--   0     1001      127      613 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/from_py.rs
--rw-r--r--   0     1001      127     9556 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/groupby_agg.rs
--rw-r--r--   0     1001      127     5194 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/impl_lazy.rs
--rw-r--r--   0     1001      127    15329 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/join.rs
--rw-r--r--   0     1001      127    15486 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/lib.rs
--rw-r--r--   0     1001      127     7104 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/unique.rs
--rw-r--r--   0     1001      127      708 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/Cargo.toml
--rw-r--r--   0     1001      127     2062 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/impl_lazy.rs
--rw-r--r--   0     1001      127     5490 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/ipc.rs
--rw-r--r--   0     1001      127      203 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/mod.rs
--rw-r--r--   0     1001      127     1004 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/utils.rs
--rw-r--r--   0     1001      127     2394 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/colselect.rs
--rw-r--r--   0     1001      127      251 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/lib.rs
--rw-r--r--   0     1001      127      488 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/Cargo.toml
--rw-r--r--   0     1001      127    14011 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/lazy_impls.rs
--rw-r--r--   0     1001      127     1606 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/lib.rs
--rw-r--r--   0     1001      127     6291 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/methods_impls.rs
--rw-r--r--   0     1001      127    21958 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/tools.rs
--rw-r--r--   0     1001      127      619 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/Cargo.toml
--rw-r--r--   0     1001      127    13696 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/cast.rs
--rw-r--r--   0     1001      127    14610 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/lib.rs
--rw-r--r--   0     1001      127    12152 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/option_datatype.rs
--rw-r--r--   0     1001      127     2524 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/pyvalue.rs
--rw-r--r--   0     1001      127      271 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/Cargo.toml
--rw-r--r--   0     1001      127     3666 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/algos.rs
--rw-r--r--   0     1001      127     1798 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/alloc.rs
--rw-r--r--   0     1001      127      231 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/lib.rs
--rw-r--r--   0     1001      127      324 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/macros.rs
--rw-r--r--   0     1001      127     2274 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/traits.rs
--rw-r--r--   0     1001      127      286 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-error/Cargo.toml
--rw-r--r--   0     1001      127     1398 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-error/src/lib.rs
--rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 teapy-0.7.0/tea-py/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/.python-version
--rw-r--r--   0     1001      127     1053 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/LICENSE
--rw-r--r--   0     1001      127     1417 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/Makefile
--rw-r--r--   0     1001      127     2202 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/README.md
--rw-r--r--   0     1001      127      232 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/build.requirements.txt
--rw-r--r--   0     1001      127     2765 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/__init__.py
--rw-r--r--   0     1001      127     4525 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/array_func.py
--rw-r--r--   0     1001      127    11351 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/expr.py
--rw-r--r--   0     1001      127     3271 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/mod_func.py
--rw-r--r--   0     1001      127    18730 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/py_datadict.py
--rw-r--r--   0     1001      127     9635 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/regression.py
--rw-r--r--   0     1001      127     7368 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/selector.py
--rw-r--r--   0     1001      127     3455 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/testing.py
--rw-r--r--   0     1001      127    12448 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      127     2094 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_common.py
--rw-r--r--   0     1001      127      967 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_context.py
--rw-r--r--   0     1001      127     8565 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      127     2303 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_equity.py
--rw-r--r--   0     1001      127     4772 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_expr.py
--rw-r--r--   0     1001      127      465 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_memory.py
--rw-r--r--   0     1001      127      339 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_time.py
--rw-r--r--   0     1001      127     3210 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      127     1417 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      127     5771 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      127     1994 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      127     3194 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      127     3458 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/window_func.py
--rw-r--r--   0     1001      127     1232 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/wrapper.py
--rw-r--r--   0     1001      127     1291 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/requirements-dev.lock
--rw-r--r--   0     1001      127      197 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/requirements.lock
--rw-r--r--   0     1001      127    23237 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/equity.rs
--rw-r--r--   0     1001      127     7135 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/from_py.rs
--rw-r--r--   0     1001      127     1127 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/lib.rs
--rw-r--r--   0     1001      127    13232 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/datadict.rs
--rw-r--r--   0     1001      127      322 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/export.rs
--rw-r--r--   0     1001      127     2929 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/groupby.rs
--rw-r--r--   0     1001      127    97443 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      127     1898 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/mod.rs
--rw-r--r--   0     1001      127     5339 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      127    18850 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      127     2202 2024-04-08 02:51:41.000000 teapy-0.7.0/README.md
--rw-r--r--   0     1001      127    55023 2024-04-08 02:52:23.000000 teapy-0.7.0/Cargo.lock
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 teapy-0.7.0/Cargo.toml
--rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 teapy-0.7.0/pyproject.toml
--rw-r--r--   0     1001      127    11351 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/expr.py
--rw-r--r--   0     1001      127     2765 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/__init__.py
--rw-r--r--   0     1001      127     3271 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/mod_func.py
--rw-r--r--   0     1001      127      339 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_time.py
--rw-r--r--   0     1001      127      967 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_context.py
--rw-r--r--   0     1001      127     2303 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_equity.py
--rw-r--r--   0     1001      127     2094 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_common.py
--rw-r--r--   0     1001      127     4772 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_expr.py
--rw-r--r--   0     1001      127      465 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_memory.py
--rw-r--r--   0     1001      127    12448 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      127     8565 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      127     3210 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      127     1417 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      127     5771 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      127     3194 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      127     1994 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      127     9635 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/regression.py
--rw-r--r--   0     1001      127    18730 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/py_datadict.py
--rw-r--r--   0     1001      127     3458 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/window_func.py
--rw-r--r--   0     1001      127     4525 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/array_func.py
--rw-r--r--   0     1001      127     1232 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/wrapper.py
--rw-r--r--   0     1001      127     7368 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/selector.py
--rw-r--r--   0     1001      127     3455 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/testing.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 teapy-0.7.0/PKG-INFO
+-rw-r--r--   0     1001      127     1303 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/Cargo.toml
+-rw-r--r--   0     1001      127      483 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/benches/inplace.rs
+-rw-r--r--   0     1001      127     3128 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/benches/rolling.rs
+-rw-r--r--   0     1001      127     7438 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/agg/corr.rs
+-rw-r--r--   0     1001      127     4196 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/agg/impl_lazy.rs
+-rw-r--r--   0     1001      127    15258 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/agg/mod.rs
+-rw-r--r--   0     1001      127     2200 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/create.rs
+-rw-r--r--   0     1001      127     3794 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/from_py.rs
+-rw-r--r--   0     1001      127      507 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/lib.rs
+-rw-r--r--   0     1001      127     8740 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/linalg.rs
+-rw-r--r--   0     1001      127     1993 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/macros.rs
+-rw-r--r--   0     1001      127     9585 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_1d.rs
+-rw-r--r--   0     1001      127     8689 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_arrok.rs
+-rw-r--r--   0     1001      127     9095 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_inplace.rs
+-rw-r--r--   0     1001      127    10333 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/impl_view.rs
+-rw-r--r--   0     1001      127    15659 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127     2000 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/stat.rs
+-rw-r--r--   0     1001      127     1220 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_lazy/time.rs
+-rw-r--r--   0     1001      127      834 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_string.rs
+-rw-r--r--   0     1001      127      787 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/impl_time.rs
+-rw-r--r--   0     1001      127    21550 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/map/mod.rs
+-rw-r--r--   0     1001      127    15701 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/cmp.rs
+-rw-r--r--   0     1001      127     8069 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/corr.rs
+-rw-r--r--   0     1001      127    26072 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/feature.rs
+-rw-r--r--   0     1001      127    22724 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/impl_lazy/common.rs
+-rw-r--r--   0     1001      127      311 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127      225 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/mod.rs
+-rw-r--r--   0     1001      127     9721 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/norm.rs
+-rw-r--r--   0     1001      127    32087 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-ext/src/rolling/reg.rs
+-rw-r--r--   0     1001      127      488 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/Cargo.toml
+-rw-r--r--   0     1001      127    14011 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/lazy_impls.rs
+-rw-r--r--   0     1001      127     1606 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/lib.rs
+-rw-r--r--   0     1001      127     6291 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/methods_impls.rs
+-rw-r--r--   0     1001      127    21958 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-macros/src/tools.rs
+-rw-r--r--   0     1001      127      811 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/Cargo.toml
+-rw-r--r--   0     1001      127      236 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/context.rs
+-rw-r--r--   0     1001      127    23144 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/dict.rs
+-rw-r--r--   0     1001      127     3254 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/get_set.rs
+-rw-r--r--   0     1001      127      189 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/mod.rs
+-rw-r--r--   0     1001      127     3114 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/datadict/selector.rs
+-rw-r--r--   0     1001      127    11891 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/data.rs
+-rw-r--r--   0     1001      127    11943 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/expr.rs
+-rw-r--r--   0     1001      127     1172 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/expr_element.rs
+-rw-r--r--   0     1001      127    11553 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/expr_inner.rs
+-rw-r--r--   0     1001      127     6642 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/auto_impl.rs
+-rw-r--r--   0     1001      127     3184 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_cast.rs
+-rw-r--r--   0     1001      127     1394 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
+-rw-r--r--   0     1001      127    15326 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      889 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/mod.rs
+-rw-r--r--   0     1001      127     2393 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/impls/utils.rs
+-rw-r--r--   0     1001      127      404 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/expr_core/mod.rs
+-rw-r--r--   0     1001      127    14135 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/groupby.rs
+-rw-r--r--   0     1001      127    11113 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/join.rs
+-rw-r--r--   0     1001      127      355 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/lib.rs
+-rw-r--r--   0     1001      127     8791 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-lazy/src/linalg.rs
+-rw-r--r--   0     1001      127      708 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/Cargo.toml
+-rw-r--r--   0     1001      127     2062 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/impl_lazy.rs
+-rw-r--r--   0     1001      127     5281 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/ipc.rs
+-rw-r--r--   0     1001      127      203 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/mod.rs
+-rw-r--r--   0     1001      127      966 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/arrow_io/utils.rs
+-rw-r--r--   0     1001      127     2394 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/colselect.rs
+-rw-r--r--   0     1001      127      251 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-io/src/lib.rs
+-rw-r--r--   0     1001      127      271 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/Cargo.toml
+-rw-r--r--   0     1001      127     3666 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/algos.rs
+-rw-r--r--   0     1001      127     1798 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/alloc.rs
+-rw-r--r--   0     1001      127      231 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/lib.rs
+-rw-r--r--   0     1001      127      324 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/macros.rs
+-rw-r--r--   0     1001      127     2274 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-utils/src/traits.rs
+-rw-r--r--   0     1001      127     1583 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/Cargo.toml
+-rw-r--r--   0     1001      127    15544 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/arbarray.rs
+-rw-r--r--   0     1001      127    25348 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/arrok.rs
+-rw-r--r--   0     1001      127    16304 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      127     4115 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_basic.rs
+-rw-r--r--   0     1001      127     8421 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_method.rs
+-rw-r--r--   0     1001      127     8160 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_numeric.rs
+-rw-r--r--   0     1001      127      648 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_time.rs
+-rw-r--r--   0     1001      127     6070 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/impl_traits.rs
+-rw-r--r--   0     1001      127      451 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/generate.rs
+-rw-r--r--   0     1001      127     7390 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/layout.rs
+-rw-r--r--   0     1001      127     9188 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/least_squares.rs
+-rw-r--r--   0     1001      127      242 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/mod.rs
+-rw-r--r--   0     1001      127     5004 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/svd.rs
+-rw-r--r--   0     1001      127      436 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/linalg/utils.rs
+-rw-r--r--   0     1001      127      312 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/impls/mod.rs
+-rw-r--r--   0     1001      127    10460 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/iterators.rs
+-rw-r--r--   0     1001      127    14095 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/lib.rs
+-rw-r--r--   0     1001      127    10802 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/macros.rs
+-rw-r--r--   0     1001      127     3011 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/own.rs
+-rw-r--r--   0     1001      127      721 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/prelude.rs
+-rw-r--r--   0     1001      127      694 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/traits.rs
+-rw-r--r--   0     1001      127     3042 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/view.rs
+-rw-r--r--   0     1001      127     2031 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-core/src/viewmut.rs
+-rw-r--r--   0     1001      127     1030 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/Cargo.toml
+-rw-r--r--   0     1001      127     1044 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/benches/groupby.rs
+-rw-r--r--   0     1001      127      613 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/from_py.rs
+-rw-r--r--   0     1001      127     9610 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/groupby_agg.rs
+-rw-r--r--   0     1001      127     5202 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/impl_lazy.rs
+-rw-r--r--   0     1001      127    15347 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/join.rs
+-rw-r--r--   0     1001      127    15380 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/lib.rs
+-rw-r--r--   0     1001      127     7106 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-groupby/src/unique.rs
+-rw-r--r--   0     1001      127      463 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-hash/Cargo.toml
+-rw-r--r--   0     1001      127     3243 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-hash/src/lib.rs
+-rw-r--r--   0     1001      127      619 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/Cargo.toml
+-rw-r--r--   0     1001      127    13696 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/cast.rs
+-rw-r--r--   0     1001      127    14632 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/lib.rs
+-rw-r--r--   0     1001      127    12152 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/option_datatype.rs
+-rw-r--r--   0     1001      127     2752 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-dtype/src/pyvalue.rs
+-rw-r--r--   0     1001      127      289 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/Cargo.toml
+-rw-r--r--   0     1001      127      755 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/convert.rs
+-rw-r--r--   0     1001      127     9144 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/datetime.rs
+-rw-r--r--   0     1001      127     2036 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/impl_datetime.rs
+-rw-r--r--   0     1001      127     2135 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      869 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/impl_timedelta.rs
+-rw-r--r--   0     1001      127       53 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/impls/mod.rs
+-rw-r--r--   0     1001      127      198 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/lib.rs
+-rw-r--r--   0     1001      127     2980 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/timedelta.rs
+-rw-r--r--   0     1001      127      842 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-time/src/timeunit.rs
+-rw-r--r--   0     1001      127      286 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-error/Cargo.toml
+-rw-r--r--   0     1001      127     1398 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-error/src/lib.rs
+-rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 teapy-0.7.1/tea-py/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/.python-version
+-rw-r--r--   0     1001      127     1053 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/LICENSE
+-rw-r--r--   0     1001      127     1417 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/Makefile
+-rw-r--r--   0     1001      127     2202 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/README.md
+-rw-r--r--   0     1001      127      232 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/build.requirements.txt
+-rw-r--r--   0     1001      127     2765 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     4525 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/array_func.py
+-rw-r--r--   0     1001      127    11351 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/expr.py
+-rw-r--r--   0     1001      127     3253 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127    18730 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     9635 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/regression.py
+-rw-r--r--   0     1001      127     7368 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/selector.py
+-rw-r--r--   0     1001      127     3455 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/testing.py
+-rw-r--r--   0     1001      127    12448 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     2094 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127      967 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127     8565 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127     2303 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     4772 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127      465 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127      339 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127     3210 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     1417 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     1994 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     3194 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     3458 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127     1291 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/requirements-dev.lock
+-rw-r--r--   0     1001      127      197 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/requirements.lock
+-rw-r--r--   0     1001      127    23237 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/equity.rs
+-rw-r--r--   0     1001      127     7135 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/from_py.rs
+-rw-r--r--   0     1001      127     1127 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/lib.rs
+-rw-r--r--   0     1001      127    13232 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      127      322 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/export.rs
+-rw-r--r--   0     1001      127     2929 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      127    97651 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      127     1898 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/mod.rs
+-rw-r--r--   0     1001      127     5443 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      127    18957 2024-04-25 05:39:11.000000 teapy-0.7.1/tea-py/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      127     2202 2024-04-25 05:39:11.000000 teapy-0.7.1/README.md
+-rw-r--r--   0     1001      127    57288 2024-04-25 05:40:04.000000 teapy-0.7.1/Cargo.lock
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 teapy-0.7.1/Cargo.toml
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 teapy-0.7.1/pyproject.toml
+-rw-r--r--   0     1001      127     3253 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127    18730 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     7368 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/selector.py
+-rw-r--r--   0     1001      127     2765 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     4525 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/array_func.py
+-rw-r--r--   0     1001      127      967 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127    12448 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     4772 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127     2303 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     1994 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     3194 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     1417 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     3210 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     8565 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127      339 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127      465 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127     2094 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127     3458 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     9635 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/regression.py
+-rw-r--r--   0     1001      127     3455 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/testing.py
+-rw-r--r--   0     1001      127    11351 2024-04-25 05:39:11.000000 teapy-0.7.1/python/teapy/expr.py
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 teapy-0.7.1/PKG-INFO
```

### Comparing `teapy-0.7.0/tea-lazy/Cargo.toml` & `teapy-0.7.1/tea-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/datadict/dict.rs` & `teapy-0.7.1/tea-lazy/src/datadict/dict.rs`

 * *Files 2% similar despite different names*

```diff
@@ -207,25 +207,25 @@
                 .collect::<Vec<_>>(),
             ColumnSelector::VecNameOwned(name_vec) => self.get_selector_out_name(
                 name_vec.iter().map(|s| s.as_str()).collect_trusted().into(),
             ),
         }
     }
 
-    /// drop some columns inplace, return the name of the dropped columns
-    #[inline]
-    pub fn drop_inplace(&mut self, col: ColumnSelector) -> TpResult<Vec<String>> {
-        let drop_cols = self.get_selector_out_name(col);
-        self.data = self
-            .data
-            .drain_filter(|e| !drop_cols.contains(&e.name().unwrap()))
-            .collect::<Vec<_>>();
-        self.reproduce_map();
-        Ok(drop_cols)
-    }
+    // /// drop some columns inplace, return the name of the dropped columns
+    // #[inline]
+    // pub fn drop_inplace(&mut self, col: ColumnSelector) -> TpResult<Vec<String>> {
+    //     let drop_cols = self.get_selector_out_name(col);
+    //     self.data = self
+    //         .data
+    //         .drain_filter(|e| !drop_cols.contains(&e.name().unwrap()))
+    //         .collect::<Vec<_>>();
+    //     self.reproduce_map();
+    //     Ok(drop_cols)
+    // }
 
     /// Adjust when idx < 0
     #[inline]
     fn valid_idx(&self, col_idx: i32) -> TpResult<usize> {
         let mut col_idx = col_idx;
         if col_idx < 0 {
             col_idx += self.len() as i32;
```

### Comparing `teapy-0.7.0/tea-lazy/src/datadict/get_set.rs` & `teapy-0.7.1/tea-lazy/src/datadict/get_set.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/datadict/selector.rs` & `teapy-0.7.1/tea-lazy/src/datadict/selector.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/data.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/data.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/expr.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/expr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -342,15 +342,15 @@
 
     #[inline]
     pub fn view_data(&self, context: Option<&Context<'a>>) -> TpResult<&Data<'a>> {
         let e = self.lock();
         let data = e.view_data(context)?;
         // safety: the array can only be read when the expression is already evaluated
         // so the data of the array should not be changed
-        unsafe { Ok(std::mem::transmute(data)) }
+        unsafe { Ok(std::mem::transmute::<&Data<'_>, &Data<'a>>(data)) }
     }
 
     #[inline]
     #[cfg(feature = "blas")]
     pub fn view_ols_res(&self, ctx: Option<&Context<'a>>) -> TpResult<Arc<OlsResult<'a>>> {
         let mut e = self.lock();
         e.eval_inplace(ctx.cloned(), false)?;
@@ -364,25 +364,25 @@
     #[inline]
     pub fn view_arr(&self, ctx: Option<&Context<'a>>) -> TpResult<&ArrOk<'a>> {
         let mut e = self.lock();
         e.eval_inplace(ctx.cloned(), false)?;
         let arr = e.view_arr(ctx)?;
         // safety: the array can only be read when the expression is already evaluated
         // so the data of the array should not be changed
-        unsafe { Ok(std::mem::transmute(arr)) }
+        unsafe { Ok(std::mem::transmute::<&ArrOk<'_>, &ArrOk<'a>>(arr)) }
     }
 
     #[inline]
     pub fn view_arr_vec(&self, ctx: Option<&Context<'a>>) -> TpResult<Vec<&ArrOk<'a>>> {
         let mut e = self.lock();
         e.eval_inplace(ctx.cloned(), false)?;
         let arr = e.view_arr_vec(ctx)?;
         // safety: the array can only be read when the expression is already evaluated
         // so the data of the array should not be changed
-        unsafe { Ok(std::mem::transmute(arr)) }
+        unsafe { Ok(std::mem::transmute::<Vec<&ArrOk<'_>>, Vec<&ArrOk<'a>>>(arr)) }
     }
 
     #[inline(always)]
     pub fn prepare(&self) {
         self.lock().prepare();
     }
```

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/expr_element.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/expr_element.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/expr_inner.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/expr_inner.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/impls/auto_impl.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/impls/auto_impl.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_cast.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_ops.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/impls/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/impls/mod.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/impls/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/expr_core/impls/utils.rs` & `teapy-0.7.1/tea-lazy/src/expr_core/impls/utils.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/groupby.rs` & `teapy-0.7.1/tea-lazy/src/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/join.rs` & `teapy-0.7.1/tea-lazy/src/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-lazy/src/linalg.rs` & `teapy-0.7.1/tea-lazy/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/Cargo.toml` & `teapy-0.7.1/tea-ext/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/benches/rolling.rs` & `teapy-0.7.1/tea-ext/benches/rolling.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/agg/corr.rs` & `teapy-0.7.1/tea-ext/src/agg/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/agg/impl_lazy.rs` & `teapy-0.7.1/tea-ext/src/agg/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/agg/mod.rs` & `teapy-0.7.1/tea-ext/src/agg/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/create.rs` & `teapy-0.7.1/tea-ext/src/create.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/from_py.rs` & `teapy-0.7.1/tea-ext/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/linalg.rs` & `teapy-0.7.1/tea-ext/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/macros.rs` & `teapy-0.7.1/tea-ext/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_1d.rs` & `teapy-0.7.1/tea-ext/src/map/impl_1d.rs`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     #[inline]
     fn filter_1d<SO, S3>(&self, mut out: ArrBase<SO, Ix1>, mask: ArrBase<S3, Ix1>)
     where
         T: Clone,
         SO: DataMut<Elem = T>,
         S3: Data<Elem = bool> + Send + Sync,
     {
-        zip(self, mask.into_iter())
+        zip(self, mask)
             .filter(|(_v, m)| *m)
             .zip(out.iter_mut())
             .for_each(|((v, _m), o)| *o = v.clone())
     }
 
     #[inline]
     fn put_mask_1d<SO, S3>(&mut self, mask: &ArrBase<SO, Ix1>, value: &ArrBase<S3, Ix1>)
```

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_arrok.rs` & `teapy-0.7.1/tea-ext/src/map/impl_arrok.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_inplace.rs` & `teapy-0.7.1/tea-ext/src/map/impl_inplace.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_lazy/impl_view.rs` & `teapy-0.7.1/tea-ext/src/map/impl_lazy/impl_view.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+#![allow(clippy::missing_transmute_annotations)]
+
 use lazy::{adjust_slice, Expr};
 use ndarray::SliceInfoElem;
 use std::mem::transmute;
 use tea_core::prelude::*;
 
 #[ext_trait]
 impl<'a> ExprViewExt for Expr<'a> {
-    #[allow(unreachable_patterns)]
+    #[allow(unreachable_patterns, clippy::missing_transmute_annotations)]
     fn index_axis(&mut self, index: Expr<'a>, axis: i32) -> &mut Self {
         self.chain_f_ctx(move |(data, ctx)| {
             let arr = data.into_arr(ctx.clone())?;
             let axis = arr.norm_axis(axis);
             let index = index
                 .view_arr(ctx.as_ref())?
                 .deref()
```

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_lazy/mod.rs` & `teapy-0.7.1/tea-ext/src/map/impl_lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_lazy/stat.rs` & `teapy-0.7.1/tea-ext/src/map/impl_lazy/stat.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_lazy/time.rs` & `teapy-0.7.1/tea-ext/src/map/impl_lazy/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_string.rs` & `teapy-0.7.1/tea-ext/src/map/impl_string.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/impl_time.rs` & `teapy-0.7.1/tea-ext/src/map/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/map/mod.rs` & `teapy-0.7.1/tea-ext/src/map/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/rolling/cmp.rs` & `teapy-0.7.1/tea-ext/src/rolling/cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/rolling/corr.rs` & `teapy-0.7.1/tea-ext/src/rolling/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/rolling/feature.rs` & `teapy-0.7.1/tea-ext/src/rolling/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/rolling/impl_lazy/common.rs` & `teapy-0.7.1/tea-ext/src/rolling/impl_lazy/common.rs`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,17 @@
                             } else {
                                 let dd = DataDict::new(exprs, Some(columns.clone()));
                                 map = Some(dd.map.clone());
                                 dd
                             };
                             // this is safe as we don't return a view on the current context
                             // into_owned is important here to guarantee the above
-                            let current_ctx: Arc<DataDict> =
-                                Arc::new(unsafe { std::mem::transmute(current_ctx) });
+                            let current_ctx: Arc<DataDict> = Arc::new(unsafe {
+                                std::mem::transmute::<DataDict<'_>, DataDict<'a>>(current_ctx)
+                            });
                             let mut data = init_data.clone();
                             let mut ctx = Some(current_ctx);
                             for f in &nodes {
                                 (data, ctx) = f((data, ctx)).unwrap();
                             }
                             data.into_arr(ctx).unwrap()
                             // arr0(1).to_dimd().into()
@@ -190,16 +191,17 @@
                             } else {
                                 let dd = DataDict::new(exprs, Some(columns.clone()));
                                 map = Some(dd.map.clone());
                                 dd
                             };
                             // this is safe as we don't return a view on the current context
                             // into_owned is important here to guarantee the above
-                            let current_ctx: Arc<DataDict> =
-                                Arc::new(unsafe { std::mem::transmute(current_ctx) });
+                            let current_ctx: Arc<DataDict> = Arc::new(unsafe {
+                                std::mem::transmute::<DataDict<'_>, DataDict<'a>>(current_ctx)
+                            });
                             let mut data = init_data.clone();
                             let mut ctx = Some(current_ctx);
                             for f in &nodes {
                                 (data, ctx) = f((data, ctx)).unwrap();
                             }
                             data.into_arr(ctx).unwrap()
                         })
```

### Comparing `teapy-0.7.0/tea-ext/src/rolling/norm.rs` & `teapy-0.7.1/tea-ext/src/rolling/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-ext/src/rolling/reg.rs` & `teapy-0.7.1/tea-ext/src/rolling/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-hash/src/lib.rs` & `teapy-0.7.1/tea-hash/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-time/src/convert.rs` & `teapy-0.7.1/tea-time/src/convert.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-time/src/datetime.rs` & `teapy-0.7.1/tea-time/src/datetime.rs`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
         }
         dt.duration_trunc(duration.inner)
             .expect("Rounding Error")
             .into()
     }
 }
 
+#[allow(dead_code)]
 #[pyclass]
 pub struct PyDateTime(DateTime);
 
 impl ToPyObject for DateTime {
     #[inline(always)]
     fn to_object(&self, py: Python<'_>) -> PyObject {
         PyDateTime(*self).into_py(py)
@@ -318,14 +319,15 @@
 impl From<&str> for TimeDelta {
     #[inline(always)]
     fn from(s: &str) -> Self {
         TimeDelta::parse(s)
     }
 }
 
+#[allow(dead_code)]
 #[pyclass]
 pub struct PyTimeDelta(TimeDelta);
 
 #[pymethods]
 impl PyTimeDelta {
     #[staticmethod]
     #[inline(always)]
```

### Comparing `teapy-0.7.0/tea-time/src/impls/impl_datetime.rs` & `teapy-0.7.1/tea-time/src/impls/impl_datetime.rs`

 * *Files 4% similar despite different names*

```diff
@@ -68,13 +68,12 @@
             NPY_FR_us => DateTime::from_timestamp_us(dt.into()).unwrap_or_default(),
             NPY_FR_ns => DateTime::from_timestamp_ns(dt.into()).unwrap_or_default(),
             _ => unimplemented!("not support other timeunit yet"),
         }
     }
 }
 
-impl ToString for DateTime {
-    #[inline(always)]
-    fn to_string(&self) -> String {
-        self.strftime(None)
+impl std::fmt::Display for DateTime {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        write!(f, "{}", self.strftime(None))
     }
 }
```

### Comparing `teapy-0.7.0/tea-time/src/impls/impl_ops.rs` & `teapy-0.7.1/tea-time/src/impls/impl_ops.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use crate::{DateTime, TimeDelta};
 use chrono::Months;
 use std::ops::{Add, Sub};
 
 impl Add<TimeDelta> for DateTime {
     type Output = DateTime;
     fn add(self, rhs: TimeDelta) -> Self::Output {
-        if let Some(dt) = self.0 && rhs.is_not_nat() {
+        if let Some(dt) = self.0
+            && rhs.is_not_nat()
+        {
             let out = if rhs.months != 0 {
                 if rhs.months > 0 {
                     dt + Months::new(rhs.months as u32)
                 } else {
                     dt - Months::new((-rhs.months) as u32)
                 }
             } else {
@@ -21,15 +23,17 @@
         }
     }
 }
 
 impl Sub<TimeDelta> for DateTime {
     type Output = DateTime;
     fn sub(self, rhs: TimeDelta) -> Self::Output {
-        if let Some(dt) = self.0 && rhs.is_not_nat(){
+        if let Some(dt) = self.0
+            && rhs.is_not_nat()
+        {
             let out = if rhs.months != 0 {
                 if rhs.months > 0 {
                     dt - Months::new(rhs.months as u32)
                 } else {
                     dt + Months::new((-rhs.months) as u32)
                 }
             } else {
```

### Comparing `teapy-0.7.0/tea-time/src/impls/impl_timedelta.rs` & `teapy-0.7.1/tea-time/src/impls/impl_timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-time/src/timedelta.rs` & `teapy-0.7.1/tea-time/src/timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-time/src/timeunit.rs` & `teapy-0.7.1/tea-time/src/timeunit.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/Cargo.toml` & `teapy-0.7.1/tea-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/arbarray.rs` & `teapy-0.7.1/tea-core/src/arbarray.rs`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         ArrOk<'a>: Cast<Self>,
     {
         if let ArbArray::ArrowChunk(_) = &self {
             let arrow_chunk = std::mem::take(self);
             if let ArbArray::ArrowChunk(arrow_chunk) = arrow_chunk {
                 let arr_vec = arrow_chunk
                     .into_par_iter()
-                    .map(|arr| ArrOk::from_arrow(arr))
+                    .map(ArrOk::from_arrow)
                     .collect::<Vec<_>>();
                 let arr = ArrOk::same_dtype_concat_1d(arr_vec);
                 *self = arr.cast()
             }
         }
     }
 
@@ -317,43 +317,43 @@
     pub fn cast<T2>(self) -> ArbArray<'a, T2>
     where
         T: GetDataType + Cast<T2> + Clone,
         T2: GetDataType + Clone + 'a,
     {
         if T::dtype() == T2::dtype() {
             // safety: T and T2 are the same type
-            unsafe { std::mem::transmute(self) }
+            unsafe { std::mem::transmute::<ArbArray<'a, T>, ArbArray<'a, T2>>(self) }
         } else {
             self.view().cast::<T2>().into()
         }
     }
 
     #[inline]
-    pub fn cast_with<'b, T2>(self, _other: &'b ArbArray<'a, T2>) -> ArbArray<'b, T2>
+    pub fn cast_with<T2>(self, _other: &ArbArray<'a, T2>) -> ArbArray<'a, T2>
     where
         T2: GetDataType,
         T: GetDataType,
     {
         if T::dtype() == T2::dtype() {
             // safety: T and T2 are the same type
-            unsafe { std::mem::transmute(self) }
+            unsafe { std::mem::transmute::<ArbArray<'a, T>, ArbArray<'a, T2>>(self) }
         } else {
             unreachable!()
         }
     }
 
     #[inline]
     pub fn cast_ref_with<T2>(&self, _other: &ArbArray<'a, T2>) -> &ArbArray<'a, T2>
     where
         T2: GetDataType,
         T: GetDataType,
     {
         if T::dtype() == T2::dtype() {
             // safety: T and T2 are the same type
-            unsafe { std::mem::transmute(self) }
+            unsafe { std::mem::transmute::<&ArbArray<'a, T>, &ArbArray<'a, T2>>(self) }
         } else {
             unreachable!()
         }
     }
 
     #[allow(unreachable_patterns)]
     #[inline]
```

### Comparing `teapy-0.7.0/tea-core/src/arrok.rs` & `teapy-0.7.1/tea-core/src/arrok.rs`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         match_arrok!(self, a, {
             let a: ArrOk<'a> = a.into_owned().into();
             // this is safe because we only need it for &str type
             // and the lifetime of str should be longer than both
             // 'a and 'b
             // remove this transmute once we add a different lifetime
             // for &str datatype
-            unsafe { std::mem::transmute(a) }
+            unsafe { std::mem::transmute::<ArrOk<'a>, ArrOk<'b>>(a) }
         })
     }
 
     #[inline]
     pub fn is_float(&self) -> bool {
         self.dtype().is_float()
     }
@@ -322,15 +322,15 @@
         if self.dtype().is_int() {
             self.deref()
         } else {
             self.deref().cast_int()
         }
     }
 
-    #[allow(unreachable_patterns)]
+    #[allow(unreachable_patterns, clippy::missing_transmute_annotations)]
     #[inline]
     pub fn view(&self) -> ArrOk<'_> {
         match self {
             ArrOk::Bool(arr) => arr.view().into(),
             ArrOk::F32(arr) => arr.view().into(),
             ArrOk::F64(arr) => arr.view().into(),
             ArrOk::I32(arr) => arr.view().into(),
```

### Comparing `teapy-0.7.0/tea-core/src/impls/impl_1d_method.rs` & `teapy-0.7.1/tea-core/src/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/impls/impl_basic.rs` & `teapy-0.7.1/tea-core/src/impls/impl_basic.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/impls/impl_method.rs` & `teapy-0.7.1/tea-core/src/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/impls/impl_numeric.rs` & `teapy-0.7.1/tea-core/src/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/impls/impl_time.rs` & `teapy-0.7.1/tea-core/src/impls/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/impls/impl_traits.rs` & `teapy-0.7.1/tea-core/src/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/impls/linalg/layout.rs` & `teapy-0.7.1/tea-core/src/impls/linalg/layout.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/impls/linalg/least_squares.rs` & `teapy-0.7.1/tea-core/src/impls/linalg/least_squares.rs`

 * *Files 2% similar despite different names*

```diff
@@ -219,19 +219,19 @@
     unsafe {
         dgelsd_(
             &m,
             &n,
             &nrhs,
             a_t.as_mut()
                 .map(|x| x.as_mut_ptr())
-                .unwrap_or(mut_a.as_mut_ptr()) as *mut f64,
+                .unwrap_or(mut_a.as_mut_ptr()),
             &m,
             b_t.as_mut()
                 .map(|x| x.as_mut_ptr())
-                .unwrap_or(mut_b.as_mut_ptr()) as *mut f64,
+                .unwrap_or(mut_b.as_mut_ptr()),
             &m_,
             singular_values.as_mut_ptr() as *mut f64,
             &rcond,
             &mut rank,
             work.as_mut_ptr() as *mut f64,
             &lwork,
             iwork.as_mut_ptr() as *mut i32,
```

### Comparing `teapy-0.7.0/tea-core/src/impls/linalg/svd.rs` & `teapy-0.7.1/tea-core/src/impls/linalg/svd.rs`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                     .map(|x| x.as_mut_ptr())
                     .unwrap_or([].as_mut_ptr()) as *mut f64, // u
                 &m,                         // ldu
                 vt.as_mut()
                     .map(|x| x.as_mut_ptr())
                     .unwrap_or([].as_mut_ptr()) as *mut f64, // vt
                 &vt_row,                    // ldvt
-                work_size.as_mut_ptr() as *mut f64,
+                work_size.as_mut_ptr(),
                 &(-1), // lwork
                 &mut info,
             );
         }
         if info != 0 {
             panic!("SVD error: info = {info}");
         }
```

### Comparing `teapy-0.7.0/tea-core/src/iterators.rs` & `teapy-0.7.1/tea-core/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/lib.rs` & `teapy-0.7.1/tea-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/macros.rs` & `teapy-0.7.1/tea-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/own.rs` & `teapy-0.7.1/tea-core/src/own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/prelude.rs` & `teapy-0.7.1/tea-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/traits.rs` & `teapy-0.7.1/tea-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-core/src/view.rs` & `teapy-0.7.1/tea-core/src/view.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 .deref_into_view()
                 .wrap()
         }
     }
 
     /// Create an array view from vec directly.
     #[inline]
-    pub fn from_ref_vec<Sh>(shape: Sh, vec: &Vec<T>) -> Self
+    pub fn from_ref_vec<Sh>(shape: Sh, vec: &[T]) -> Self
     where
         Sh: Into<StrideShape<D>>,
     {
         unsafe {
             RawArrayView::from_shape_ptr(shape, vec.as_ptr())
                 .deref_into_view()
                 .wrap()
```

### Comparing `teapy-0.7.0/tea-core/src/viewmut.rs` & `teapy-0.7.1/tea-core/src/viewmut.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-groupby/Cargo.toml` & `teapy-0.7.1/tea-groupby/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-groupby/benches/groupby.rs` & `teapy-0.7.1/tea-groupby/benches/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-groupby/src/from_py.rs` & `teapy-0.7.1/tea-groupby/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-groupby/src/groupby_agg.rs` & `teapy-0.7.1/tea-groupby/src/groupby_agg.rs`

 * *Files 2% similar despite different names*

```diff
@@ -132,16 +132,17 @@
                             let dd = DataDict::new(exprs, Some(columns.clone()));
                             map = Some(dd.map.clone());
                             dd
                         };
                         // let out_e = agg_expr.context_clone();
                         // this is safe as we don't return a view on the current context
                         // into_owned is important here to guarantee the above
-                        let current_ctx: Arc<DataDict> =
-                            Arc::new(unsafe { std::mem::transmute(current_ctx) });
+                        let current_ctx: Arc<DataDict> = Arc::new(unsafe {
+                            std::mem::transmute::<DataDict<'_>, DataDict<'a>>(current_ctx)
+                        });
                         let mut data = init_data.clone();
                         let mut ctx = Some(current_ctx);
                         for f in &nodes {
                             (data, ctx) = f((data, ctx)).unwrap();
                         }
                         data.into_arr(ctx).unwrap()
                         // let o = out_e
```

### Comparing `teapy-0.7.0/tea-groupby/src/impl_lazy.rs` & `teapy-0.7.1/tea-groupby/src/impl_lazy.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     pub fn get_group_by_idx(&mut self, others: Vec<Expr<'a>>, sort: bool, par: bool) -> &mut Self {
         self.chain_f_ctx(move |(data, ctx)| {
             let arr = data.view_arr(ctx.as_ref())?;
             let others_ref = others
                 .par_iter()
                 .map(|e| e.view_arr(ctx.as_ref()).unwrap())
                 .collect::<Vec<_>>();
-            let keys = std::iter::once(arr)
-                .chain(others_ref.into_iter())
-                .collect::<Vec<_>>();
+            let keys = std::iter::once(arr).chain(others_ref).collect::<Vec<_>>();
             let group_idx = if par {
                 // groupby_par(&keys, sort)
                 unimplemented!()
             } else {
                 groupby(&keys, sort)
             };
             let output = group_idx.into_iter().map(|v| v.1).collect_trusted();
@@ -89,16 +87,17 @@
                             let dd = DataDict::new(exprs, Some(columns.clone()));
                             map = Some(dd.map.clone());
                             dd
                         };
                         // let out_e = agg_expr.context_clone();
                         // this is safe as we don't return a view on the current context
                         // into_owned is important here to guarantee the above
-                        let current_ctx: Arc<DataDict> =
-                            Arc::new(unsafe { std::mem::transmute(current_ctx) });
+                        let current_ctx: Arc<DataDict> = Arc::new(unsafe {
+                            std::mem::transmute::<DataDict<'_>, DataDict<'a>>(current_ctx)
+                        });
                         let mut data = init_data.clone();
                         let mut ctx = Some(current_ctx);
                         for f in &nodes {
                             (data, ctx) = f((data, ctx)).unwrap();
                         }
                         data.into_arr(ctx).unwrap()
                         // let o = out_e
```

### Comparing `teapy-0.7.0/tea-groupby/src/join.rs` & `teapy-0.7.1/tea-groupby/src/join.rs`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             }
         }
     }
     output
 }
 
 // #[allow(clippy::useless_conversion, clippy::type_complexity)]
-#[allow(suspicious_double_ref_op, clippy::clone_on_copy)]
+#[allow(suspicious_double_ref_op, noop_method_call, clippy::clone_on_copy)]
 /// return outer_keys, left_idx and right_idx to select from left and right table
 pub fn join_outer<'a>(
     left_keys: &[&ArrOk<'a>],
     right_keys: &[&ArrOk<'a>],
 ) -> (Vec<ArrOk<'a>>, Vec<OptUsize>, Vec<OptUsize>) {
     assert_eq!(
         left_keys.len(),
```

### Comparing `teapy-0.7.0/tea-groupby/src/lib.rs` & `teapy-0.7.1/tea-groupby/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,15 @@
 impl<T, S: Data<Elem = T>> HashExt1d for ArrBase<S, Ix1> {
     /// Hash each element of the array.
     #[inline]
     fn hash_1d(self) -> Arr1<u64>
     where
         T: Hash,
     {
-        self.map(|v| {
-            let mut hasher = BUILD_HASHER.build_hasher();
-            v.hash(&mut hasher);
-            hasher.finish()
-        })
+        self.map(|v| BUILD_HASHER.hash_one(v))
     }
 
     /// Hash each element of the array.
     #[inline]
     fn tphash_1d(self) -> Arr1<u64>
     where
         T: TpHash,
```

### Comparing `teapy-0.7.0/tea-groupby/src/unique.rs` & `teapy-0.7.1/tea-groupby/src/unique.rs`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             let others = others
                 .as_ref()
                 .map(|vecs| {
                     vecs.into_par_iter()
                         .map(|e| e.view_arr(ctx.as_ref()).unwrap().deref())
                         .collect::<Vec<_>>()
                 })
-                .unwrap_or(vec![]);
+                .unwrap_or_default();
             let others_ref = others.iter().collect::<Vec<_>>();
             let arr = data.view_arr(ctx.as_ref()).unwrap();
             let len = arr.len();
             let out_idx = if others_ref.is_empty() {
                 if &keep == "first" {
                     let mut out_idx = Vec::with_capacity(len);
                     let arr: ArrOk = if arr.is_float() {
```

### Comparing `teapy-0.7.0/tea-io/Cargo.toml` & `teapy-0.7.1/tea-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-io/src/arrow_io/impl_lazy.rs` & `teapy-0.7.1/tea-io/src/arrow_io/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-io/src/arrow_io/ipc.rs` & `teapy-0.7.1/tea-io/src/arrow_io/ipc.rs`

 * *Files 3% similar despite different names*

```diff
@@ -45,38 +45,35 @@
                     // unimplemented!("mmap can only be done on uncompressed IPC files")
                     let mut reader = read::FileReader::new(file, metadata, proj, None);
                     let schema = reader.schema().clone();
                     let out: Vec<ArrOk<'a>> = if blocks_num > 1 {
                         let mut arrs = reader
                             .map(|batch| batch.unwrap().into_arrays())
                             .collect::<Vec<_>>();
-                        let arrs = (0..arrs.get(0).unwrap().len())
+                        let arrs = (0..arrs.first().unwrap().len())
                             .map(|_| {
                                 let mut out = Vec::with_capacity(arrs.len());
                                 // out.push(arrs.pop().unwrap());
                                 arrs.iter_mut().for_each(|a| out.push(a.pop().unwrap()));
                                 out
                             })
                             .collect::<Vec<_>>();
                         arrs.into_par_iter()
                             .rev()
                             .map(|a| {
-                                let a = a
-                                    .into_par_iter()
-                                    .map(|arr| ArrOk::from_arrow(arr))
-                                    .collect();
+                                let a = a.into_par_iter().map(ArrOk::from_arrow).collect();
                                 ArrOk::same_dtype_concat_1d(a)
                             })
                             .collect()
                     } else {
                         let chunk = reader.next().unwrap().unwrap();
                         chunk
                             .into_arrays()
                             .into_par_iter()
-                            .map(|a| ArrOk::from_arrow(a))
+                            .map(ArrOk::from_arrow)
                             .collect()
                     };
                     return Ok((schema, out));
                 } else {
                     return Err(e.to_owned().into());
                 }
             } else {
@@ -123,19 +120,16 @@
                     .for_each(|a| out.push(a.pop().unwrap()));
                 out
             })
             .collect::<Vec<_>>();
         arrs.into_par_iter()
             .rev()
             .map(|a| {
-                let a = a
-                    .into_par_iter()
-                    .map(|arr| ArrOk::from_arrow(arr))
-                    .collect();
+                let a = a.into_par_iter().map(ArrOk::from_arrow).collect();
                 ArrOk::same_dtype_concat_1d(a)
             })
             .collect()
     } else {
-        arrs.into_par_iter().map(|a| ArrOk::from_arrow(a)).collect()
+        arrs.into_par_iter().map(ArrOk::from_arrow).collect()
     };
     Ok((schema, out))
 }
```

### Comparing `teapy-0.7.0/tea-io/src/arrow_io/utils.rs` & `teapy-0.7.1/tea-io/src/arrow_io/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,15 @@
         let mut column_names = TpHashMap::with_capacity(schema.fields.len());
         schema.fields.iter().enumerate().for_each(|(i, c)| {
             column_names.insert(c.name.as_str(), i);
         });
 
         for column in columns {
             let Some(&i) = column_names.get(column) else {
-                return Err(
-                    format!("unable to find column {:?}", column).into(),
-                )
+                return Err(format!("unable to find column {:?}", column).into());
             };
             prj.push(i);
         }
     } else {
         for column in columns {
             for (i, f) in schema.fields.iter().enumerate() {
                 if f.name == *column {
```

### Comparing `teapy-0.7.0/tea-io/src/colselect.rs` & `teapy-0.7.1/tea-io/src/colselect.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-macros/src/lazy_impls.rs` & `teapy-0.7.1/tea-macros/src/lazy_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-macros/src/lib.rs` & `teapy-0.7.1/tea-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-macros/src/methods_impls.rs` & `teapy-0.7.1/tea-macros/src/methods_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-macros/src/tools.rs` & `teapy-0.7.1/tea-macros/src/tools.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-dtype/Cargo.toml` & `teapy-0.7.1/tea-dtype/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-dtype/src/cast.rs` & `teapy-0.7.1/tea-dtype/src/cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-dtype/src/lib.rs` & `teapy-0.7.1/tea-dtype/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -614,14 +614,15 @@
 );
 
 pub trait BoolType {
     fn bool_(self) -> bool;
 }
 
 impl BoolType for bool {
+    #[inline(always)]
     fn bool_(self) -> bool {
         self
     }
 }
 
 #[cfg(feature = "option_dtype")]
 impl BoolType for OptBool {
```

### Comparing `teapy-0.7.0/tea-dtype/src/option_datatype.rs` & `teapy-0.7.1/tea-dtype/src/option_datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-dtype/src/pyvalue.rs` & `teapy-0.7.1/tea-dtype/src/pyvalue.rs`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,25 @@
 use serde::{Serialize, Serializer};
 use std::string::ToString;
 
 #[derive(Clone)]
 #[repr(transparent)]
 pub struct PyValue(pub PyObject);
 
-impl ToString for PyValue {
-    #[inline(always)]
-    fn to_string(&self) -> String {
-        self.0.to_string()
+// impl ToString for PyValue {
+//     #[inline(always)]
+//     fn to_string(&self) -> String {
+//         self.0.to_string()
+//     }
+// }
+
+impl std::fmt::Display for PyValue {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        // write!(f, "{}", self.strftime(None))
+        std::fmt::Display::fmt(&self.0, f)
     }
 }
 
 impl Debug for PyValue {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f, "{:?}", &self.0)
     }
```

### Comparing `teapy-0.7.0/tea-utils/src/algos.rs` & `teapy-0.7.1/tea-utils/src/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-utils/src/alloc.rs` & `teapy-0.7.1/tea-utils/src/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-utils/src/traits.rs` & `teapy-0.7.1/tea-utils/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-error/src/lib.rs` & `teapy-0.7.1/tea-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/Cargo.toml` & `teapy-0.7.1/tea-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/LICENSE` & `teapy-0.7.1/tea-py/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/Makefile` & `teapy-0.7.1/tea-py/Makefile`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/README.md` & `teapy-0.7.1/tea-py/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/__init__.py` & `teapy-0.7.1/tea-py/python/teapy/__init__.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/array_func.py` & `teapy-0.7.1/tea-py/python/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/expr.py` & `teapy-0.7.1/tea-py/python/teapy/expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/mod_func.py` & `teapy-0.7.1/tea-py/python/teapy/mod_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 from .selector import Selector
 from .tears import arange, stack
 from .tears import corr as _corr
 
 
 def select_wrapper(func):
     name = func.__qualname__
-    print(name)
-
     @wraps(func)
     def _wrap_func(exprs, *args, **kwargs):
         if len(exprs) and isinstance(exprs[0], Selector):
             return Selector().mod_func(name)(exprs, *args, **kwargs)
         else:
             return func(exprs, *args, **kwargs)
-
     return _wrap_func
 
 
 @select_wrapper
 def hcorr(exprs, method="pearson", stable=False):
     return _corr(exprs, method=method, stable=stable)
     # return PyDataDict(exprs).corr(method=method, stable=stable)
```

### Comparing `teapy-0.7.0/tea-py/python/teapy/py_datadict.py` & `teapy-0.7.1/tea-py/python/teapy/py_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/regression.py` & `teapy-0.7.1/tea-py/python/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/selector.py` & `teapy-0.7.1/tea-py/python/teapy/selector.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/testing.py` & `teapy-0.7.1/tea-py/python/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/test_array_func.py` & `teapy-0.7.1/tea-py/python/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/test_common.py` & `teapy-0.7.1/tea-py/python/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/test_context.py` & `teapy-0.7.1/tea-py/python/teapy/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/test_datadict.py` & `teapy-0.7.1/tea-py/python/teapy/tests/test_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/test_equity.py` & `teapy-0.7.1/tea-py/python/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/test_expr.py` & `teapy-0.7.1/tea-py/python/teapy/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/window/test_compare.py` & `teapy-0.7.1/tea-py/python/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/window/test_corr.py` & `teapy-0.7.1/tea-py/python/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/window/test_feature.py` & `teapy-0.7.1/tea-py/python/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/window/test_norm.py` & `teapy-0.7.1/tea-py/python/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/tests/window/test_reg.py` & `teapy-0.7.1/tea-py/python/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/window_func.py` & `teapy-0.7.1/tea-py/python/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/python/teapy/wrapper.py` & `teapy-0.7.1/tea-py/python/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/requirements-dev.lock` & `teapy-0.7.1/tea-py/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/src/equity.rs` & `teapy-0.7.1/tea-py/src/equity.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/src/from_py.rs` & `teapy-0.7.1/tea-py/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/src/lib.rs` & `teapy-0.7.1/tea-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/src/pylazy/datadict.rs` & `teapy-0.7.1/tea-py/src/pylazy/datadict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/src/pylazy/groupby.rs` & `teapy-0.7.1/tea-py/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/src/pylazy/impl_pyexpr.rs` & `teapy-0.7.1/tea-py/src/pylazy/impl_pyexpr.rs`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,19 @@
     pub fn view_in(
         // slf: PyRefMut<'_, Self>,
         slf: Bound<'_, PyExpr>,
         context: Option<&Bound<'_, PyAny>>,
         py: Python,
     ) -> PyResult<PyObject> {
         let ct: PyContext<'static> = if let Some(context) = context {
-            unsafe { std::mem::transmute(context.extract::<PyContext>()?) }
+            unsafe {
+                std::mem::transmute::<PyContext<'_>, PyContext<'static>>(
+                    context.extract::<PyContext>()?,
+                )
+            }
         } else {
             Default::default()
         };
         let (ct_rs, _obj_map) = (ct.ct, ct.obj_map);
         let slf_ref = slf.borrow();
         let data = slf_ref
             .e
@@ -325,15 +329,19 @@
     pub fn value<'py>(
         &'py mut self,
         unit: Option<&'py str>,
         context: Option<&Bound<'py, PyAny>>,
         py: Python<'py>,
     ) -> PyResult<PyObject> {
         let ct: PyContext<'static> = if let Some(context) = context {
-            unsafe { std::mem::transmute(context.extract::<PyContext>()?) }
+            unsafe {
+                std::mem::transmute::<PyContext<'_>, PyContext<'static>>(
+                    context.extract::<PyContext>()?,
+                )
+            }
         } else {
             Default::default()
         };
         let (ct_rs, _obj_map) = (ct.ct, ct.obj_map);
         self.e.eval_inplace(ct_rs.clone())?;
         let data = self.e.view_data(ct_rs.as_ref()).map_err(StrError::to_py)?;
         if matches!(&data, Data::ArrVec(_)) {
```

### Comparing `teapy-0.7.0/tea-py/src/pylazy/mod.rs` & `teapy-0.7.1/tea-py/src/pylazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/tea-py/src/pylazy/pyexpr.rs` & `teapy-0.7.1/tea-py/src/pylazy/pyexpr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,19 @@
     //     self.eval_inplace(context, freeze)?;
     //     Ok(self)
     // }
 
     #[allow(unreachable_patterns)]
     pub fn eval_inplace(&mut self, context: Option<&PyAny>, freeze: bool) -> PyResult<()> {
         let ct: PyContext<'static> = if let Some(context) = context {
-            unsafe { std::mem::transmute(context.extract::<PyContext>()?) }
+            unsafe {
+                std::mem::transmute::<PyContext<'_>, PyContext<'static>>(
+                    context.extract::<PyContext>()?,
+                )
+            }
         } else {
             Default::default()
         };
         let (ct_rs, obj_map) = (ct.ct, ct.obj_map);
         for obj in obj_map.into_values() {
             self.add_obj(obj);
         }
```

### Comparing `teapy-0.7.0/tea-py/src/pylazy/pyfunc.rs` & `teapy-0.7.1/tea-py/src/pylazy/pyfunc.rs`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 }
 
 #[pyfunction]
 #[pyo3(signature=(obj, copy=false))]
 /// A util function to convert python object to PyExpr
 ///
 /// copy: whether to copy numpy.ndarray when creating the PyExpr
+///
+/// # Safety
+///
+/// we need python object to be alive when we are using the PyExpr if copy is false
 pub unsafe fn parse_expr(obj: &PyAny, copy: bool) -> PyResult<PyExpr> {
     if let Ok(expr) = obj.extract::<PyExpr>() {
         Ok(expr)
     } else if obj.get_type().qualname()? == "Expr" {
         // For any crate that extends this crate
         let module_name = obj.getattr("__module__")?.extract::<&str>()?;
         if module_name == "teapy" {
@@ -275,15 +279,15 @@
 }
 
 #[cfg(all(feature = "concat", feature = "map"))]
 #[pyfunction]
 #[pyo3(signature=(exprs, axis=0))]
 #[allow(unreachable_patterns)]
 pub fn concat_expr(exprs: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
-    let mut e1 = exprs.get(0).unwrap().clone();
+    let mut e1 = exprs.first().unwrap().clone();
     let obj_vec = exprs.iter().skip(1).map(|e| e.obj()).collect_trusted();
     e1.e.concat(
         exprs.into_iter().skip(1).map(|e| e.e).collect_trusted(),
         axis,
     );
     Ok(e1.add_obj_vec_into(obj_vec))
 }
@@ -301,15 +305,15 @@
 }
 
 #[cfg(all(feature = "concat", feature = "map"))]
 #[pyfunction]
 #[pyo3(signature=(exprs, axis=0))]
 #[allow(unreachable_patterns)]
 pub fn stack_expr(exprs: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
-    let mut e1 = exprs.get(0).unwrap().clone();
+    let mut e1 = exprs.first().unwrap().clone();
     let obj_vec = exprs.iter().skip(1).map(|e| e.obj()).collect_trusted();
     e1.e.stack(
         exprs.into_iter().skip(1).map(|e| e.e).collect_trusted(),
         axis,
     );
     Ok(e1.add_obj_vec_into(obj_vec))
 }
```

### Comparing `teapy-0.7.0/README.md` & `teapy-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/Cargo.lock` & `teapy-0.7.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
@@ -104,23 +104,17 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base16ct"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "349a06037c7bf932dd7e7d1f653678b2038b9ad46a74102f1fc7bd7872678cce"
-
-[[package]]
-name = "base64"
-version = "0.13.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
@@ -149,17 +143,17 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
@@ -170,55 +164,56 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "cblas-sys"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6feecd82cce51b0204cf063f0041d69f24ce83f680d87514b004248e7b0fa65"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.91"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fd97381a8cc6493395a5afc4c691c1084b3768db713b73aa215217aa245d153"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "core-foundation"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
@@ -284,137 +279,155 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "darling"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "derive_builder"
-version = "0.11.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d07adf7be193b71cc36b193d0f5fe60b918a3a9db4dad0449f57bcfd519704a3"
+checksum = "0350b5cb0331628a5916d6c5c0b72e97393b8b6b03b47a9284f4e7f5a405ffd7"
 dependencies = [
  "derive_builder_macro",
 ]
 
 [[package]]
 name = "derive_builder_core"
-version = "0.11.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f91d4cfa921f1c05904dc3c57b4a32c38aed3340cce209f3a6fd1478babafc4"
+checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "derive_builder_macro"
-version = "0.11.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f0314b72bed045f3a68671b3c86328386762c93f82d98c65c3cb5e5f573dd68"
+checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "directories"
-version = "4.0.1"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f51c5d4ddabd36886dd3e1438cb358cdcb0d7c499cb99cb4ac2e38e18b5cb210"
+checksum = "9a49173b84e034382284f27f1af4dcbbd231ffa358c0fe316541a7337f376a35"
 dependencies = [
- "dirs-sys",
+ "dirs-sys 0.4.1",
 ]
 
 [[package]]
 name = "dirs"
 version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30baa043103c9d0c2a57cf537cc2f35623889dc0d405e6c3cccfadbc81c71309"
 dependencies = [
- "dirs-sys",
+ "dirs-sys 0.3.7",
 ]
 
 [[package]]
 name = "dirs-sys"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
 dependencies = [
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
+name = "dirs-sys"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
+dependencies = [
+ "libc",
+ "option-ext",
+ "redox_users",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "dyn-clone"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+
+[[package]]
+name = "equivalent"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ethnum"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b90ca2580b73ab6a1f724b76ca11ab632df820fd6040c336200d2c1df7b3c82c"
@@ -430,15 +443,15 @@
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
@@ -491,17 +504,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -584,14 +597,24 @@
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
+dependencies = [
+ "equivalent",
+ "hashbrown",
+]
+
+[[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "intel-mkl-src"
@@ -619,17 +642,17 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -823,17 +846,17 @@
  "rawpointer",
  "rayon",
  "serde",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -914,33 +937,33 @@
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "oci-spec"
-version = "0.5.8"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98135224dd4faeb24c05a2fac911ed53ea6b09ecb09d7cada1cb79963ab2ee34"
+checksum = "e423c4f827362c0d8d8da4b1f571270f389ebde73bcd3240a3d23c6d6f61d0f0"
 dependencies = [
  "derive_builder",
  "getset",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "ocipkg"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60cf01280832705a4e4c4d046d9e67a54b900297c69191457a8fc6d198ddefa2"
+checksum = "9bb3293021f06540803301af45e7ab81693d50e89a7398a3420bdab139e7ba5e"
 dependencies = [
  "base16ct",
- "base64 0.13.1",
+ "base64 0.22.0",
  "chrono",
  "directories",
  "flate2",
  "lazy_static",
  "log",
  "oci-spec",
  "regex",
@@ -1007,15 +1030,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1029,14 +1052,20 @@
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1116,26 +1145,26 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -1144,62 +1173,62 @@
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1323,15 +1352,15 @@
 dependencies = [
  "cc",
  "cfg-if",
  "getrandom",
  "libc",
  "spin",
  "untrusted",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
@@ -1343,30 +1372,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.3"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
  "rustls-webpki",
  "subtle",
  "zeroize",
@@ -1393,23 +1422,23 @@
 dependencies = [
  "base64 0.22.0",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
@@ -1438,15 +1467,15 @@
 
 [[package]]
 name = "schannel"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
@@ -1478,44 +1507,53 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_spanned"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "sha2"
 version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "793db75ad2bcafc3ffa7c68b215fee268f537982cd901d132f89c6343f3a3dc8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
@@ -1587,17 +1625,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1615,15 +1653,15 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tea-core"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "arrow2",
  "intel-mkl-src",
  "lapack-sys",
  "libc",
  "ndarray",
  "num",
@@ -1633,36 +1671,36 @@
  "tea-dtype",
  "tea-error",
  "tea-utils",
 ]
 
 [[package]]
 name = "tea-dtype"
-version = "0.7.0"
+version = "0.7.1"
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
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "arrow2",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-ext"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ndarray",
  "num",
  "paste",
  "pyo3",
  "rayon",
  "statrs",
@@ -1670,74 +1708,74 @@
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-groupby"
-version = "0.7.0"
+version = "0.7.1"
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
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ahash",
  "gxhash",
  "tea-dtype",
 ]
 
 [[package]]
 name = "tea-io"
-version = "0.7.0"
+version = "0.7.1"
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
-version = "0.7.0"
+version = "0.7.1"
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
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ndarray",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tea-py"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ahash",
  "chrono",
  "ndarray",
  "numpy",
  "once_cell",
  "parking_lot",
@@ -1750,56 +1788,56 @@
  "tea-hash",
  "tea-io",
  "tea-lazy",
 ]
 
 [[package]]
 name = "tea-time"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "chrono",
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-utils"
-version = "0.7.0"
+version = "0.7.1"
 
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
  "rustix",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1811,22 +1849,47 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml"
-version = "0.5.11"
+version = "0.8.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
+dependencies = [
+ "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "toml_edit",
+]
+
+[[package]]
+name = "toml_datetime"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "toml_edit"
+version = "0.22.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
+dependencies = [
+ "indexmap",
+ "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-bidi"
@@ -1947,15 +2010,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1969,15 +2032,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1991,17 +2054,17 @@
 checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
 dependencies = [
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.15"
+version = "0.7.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
+checksum = "81a1851a719f11d1d2fea40e15c72f6c00de8c142d7ac47c1441cc7e4d0d5bc6"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -2017,43 +2080,52 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2065,110 +2137,126 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+
+[[package]]
+name = "winnow"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
+dependencies = [
+ "memchr",
+]
 
 [[package]]
 name = "xattr"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
 dependencies = [
@@ -2190,22 +2278,22 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+checksum = "63381fa6624bf92130a6b87c0d07380116f80b565c42cf0d754136f0238359ef"
 
 [[package]]
 name = "zstd"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
```

### Comparing `teapy-0.7.0/Cargo.toml` & `teapy-0.7.1/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [workspace]
 resolver = "2"
 members = ["tea-core", "tea-dtype", "tea-error", "tea-ext", "tea-groupby", "tea-hash", "tea-io", "tea-lazy", "tea-macros", "tea-py", "tea-time", "tea-utils"]
 
 [workspace.package]
-version = "0.7.0"
+version = "0.7.1"
 authors = ["Teamon"]
 edition = "2021"
 repository = "https://github.com/Teamon9161/teapy"
 license = "MIT"
 
 [profile.release]
 lto = true
 
 [workspace.dependencies]
 num = "0.4"
 libc = "0.2"
 rayon = "1.5"
 paste = "1.0"
-ahash = { version = "0.8", features = ["std", "runtime-rng"]}
+ahash = { version = "0.8.11", features = ["std", "runtime-rng"]}
 once_cell = "1.18"
 regex = "1"
 serde = { version = "1.0", features = ["derive", "rc"] }
 # serde_with = {version = "3.0", features = ["chrono"]}
 ndarray = {features=['rayon', 'serde'], version="0.15"}
 numpy = "0.21.0"
-pyo3 = {version = "0.21.0", features = ["extension-module", "abi3-py38", "macros", "serde", "gil-refs"]}
+pyo3 = {version = "0.21.2", features = ["extension-module", "abi3-py38", "macros", "serde", "gil-refs"]}
 parking_lot = "0.12"
 chrono = {version = "0.4.31", features = ["serde"]}
 arrow = {package = "arrow2", version = "0.18.0", default-features = false, features = ["io_ipc", "io_ipc_compression"]}
 
 [profile.dev]
 incremental = true
```

### Comparing `teapy-0.7.0/pyproject.toml` & `teapy-0.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 [build-system]
 requires = ["maturin>=1.2,<2.0"]
 build-backend = "maturin"
 
 [tool.rye]
 managed = true
+virtual = true
 dev-dependencies = [
     "pip>=23.3.1",
     "ruff>=0.3.5",
     "pytest>=7.4.3",
     "pytest-cov>=4.1.0",
     "pytest-xdist>=3.4.0",
     "hypothesis>=6.89.0",
@@ -71,17 +72,14 @@
   "FA", # flake8-future-annotations
   "PIE", # flake8-pie
   "TD", # flake8-todos
   "TRY", # tryceratops
   "EM", # flake8-errmsg
   "FBT001", # flake8-boolean-trap
 ]
-# extend-select = [
-#     "E501" # line too long
-# ]
 
 ignore = [
     "F401", # imported but unused
     "F403", # unable to detect undefined names
     "EM101", # Exception must not use a string literal, assign to variable first
     "TRY003", # Avoid specifying long messages outside the exception class
     "E501", # line too long
```

### Comparing `teapy-0.7.0/python/teapy/expr.py` & `teapy-0.7.1/python/teapy/expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/__init__.py` & `teapy-0.7.1/python/teapy/__init__.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/mod_func.py` & `teapy-0.7.1/python/teapy/mod_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 from .selector import Selector
 from .tears import arange, stack
 from .tears import corr as _corr
 
 
 def select_wrapper(func):
     name = func.__qualname__
-    print(name)
-
     @wraps(func)
     def _wrap_func(exprs, *args, **kwargs):
         if len(exprs) and isinstance(exprs[0], Selector):
             return Selector().mod_func(name)(exprs, *args, **kwargs)
         else:
             return func(exprs, *args, **kwargs)
-
     return _wrap_func
 
 
 @select_wrapper
 def hcorr(exprs, method="pearson", stable=False):
     return _corr(exprs, method=method, stable=stable)
     # return PyDataDict(exprs).corr(method=method, stable=stable)
```

### Comparing `teapy-0.7.0/python/teapy/tests/test_context.py` & `teapy-0.7.1/python/teapy/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/test_equity.py` & `teapy-0.7.1/python/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/test_common.py` & `teapy-0.7.1/python/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/test_expr.py` & `teapy-0.7.1/python/teapy/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/test_array_func.py` & `teapy-0.7.1/python/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/test_datadict.py` & `teapy-0.7.1/python/teapy/tests/test_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/window/test_compare.py` & `teapy-0.7.1/python/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/window/test_corr.py` & `teapy-0.7.1/python/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/window/test_feature.py` & `teapy-0.7.1/python/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/window/test_reg.py` & `teapy-0.7.1/python/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/tests/window/test_norm.py` & `teapy-0.7.1/python/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/regression.py` & `teapy-0.7.1/python/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/py_datadict.py` & `teapy-0.7.1/python/teapy/py_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/window_func.py` & `teapy-0.7.1/python/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/array_func.py` & `teapy-0.7.1/python/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/wrapper.py` & `teapy-0.7.1/python/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/selector.py` & `teapy-0.7.1/python/teapy/selector.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/python/teapy/testing.py` & `teapy-0.7.1/python/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.7.0/PKG-INFO` & `teapy-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: teapy
-Version: 0.7.0
+Version: 0.7.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
```

