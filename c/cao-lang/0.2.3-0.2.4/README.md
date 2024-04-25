# Comparing `tmp/cao-lang-0.2.3.tar.gz` & `tmp/cao_lang-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cao-lang-0.2.3.tar", last modified: Thu Apr  4 21:06:25 2024, max compression
+gzip compressed data, was "cao_lang-0.2.4.tar", last modified: Thu Apr 25 18:37:12 2024, max compression
```

## Comparing `cao-lang-0.2.3.tar` & `cao_lang-0.2.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.705870 cao-lang-0.2.3/
--rw-r--r--   0 runner     (501) staff       (20)     1068 2024-04-04 21:06:14.000000 cao-lang-0.2.3/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      123 2024-04-04 21:06:14.000000 cao-lang-0.2.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 21:06:25.705318 cao-lang-0.2.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1098 2024-04-04 21:06:14.000000 cao-lang-0.2.3/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.677245 cao-lang-0.2.3/cao-lang/
--rw-r--r--   0 runner     (501) staff       (20)     1317 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/Cargo.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.678083 cao-lang-0.2.3/cao-lang/benches/
--rw-r--r--   0 runner     (501) staff       (20)     4146 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/benches/cao_lang_benches.rs
--rw-r--r--   0 runner     (501) staff       (20)     1246 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/build.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.683150 cao-lang-0.2.3/cao-lang/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.683556 cao-lang-0.2.3/cao-lang/src/alloc/
--rw-r--r--   0 runner     (501) staff       (20)     3168 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/alloc/caolang_alloc.rs
--rw-r--r--   0 runner     (501) staff       (20)      999 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/alloc.rs
--rw-r--r--   0 runner     (501) staff       (20)     1115 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/bytecode.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.685886 cao-lang-0.2.3/cao-lang/src/collections/
--rw-r--r--   0 runner     (501) staff       (20)     3084 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/bounded_stack.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.686679 cao-lang-0.2.3/cao-lang/src/collections/handle_table/
--rw-r--r--   0 runner     (501) staff       (20)     3731 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/handle_table/serde_impl.rs
--rw-r--r--   0 runner     (501) staff       (20)     2316 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/handle_table/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    16517 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/handle_table.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.687484 cao-lang-0.2.3/cao-lang/src/collections/hash_map/
--rw-r--r--   0 runner     (501) staff       (20)     3774 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/hash_map/serde_impl.rs
--rw-r--r--   0 runner     (501) staff       (20)     3547 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/hash_map/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    15603 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/hash_map.rs
--rw-r--r--   0 runner     (501) staff       (20)       84 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/mod.rs
--rw-r--r--   0 runner     (501) staff       (20)     5147 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/collections/value_stack.rs
--rw-r--r--   0 runner     (501) staff       (20)     6726 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiled_program.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.691843 cao-lang-0.2.3/cao-lang/src/compiler/
--rw-r--r--   0 runner     (501) staff       (20)    21508 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/card.rs
--rw-r--r--   0 runner     (501) staff       (20)     2273 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/compilation_error.rs
--rw-r--r--   0 runner     (501) staff       (20)      423 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/compile_options.rs
--rw-r--r--   0 runner     (501) staff       (20)      790 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/function.rs
--rw-r--r--   0 runner     (501) staff       (20)      793 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/function_ir.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.692237 cao-lang-0.2.3/cao-lang/src/compiler/module/
--rw-r--r--   0 runner     (501) staff       (20)     8441 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/module/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    17167 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/module.rs
--rw-r--r--   0 runner     (501) staff       (20)     3103 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    39021 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/compiler.rs
--rw-r--r--   0 runner     (501) staff       (20)     5505 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/instruction.rs
--rw-r--r--   0 runner     (501) staff       (20)     1606 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/lib.rs
--rw-r--r--   0 runner     (501) staff       (20)      403 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/prelude.rs
--rw-r--r--   0 runner     (501) staff       (20)     2992 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/procedures.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.692589 cao-lang-0.2.3/cao-lang/src/stdlib/
--rw-r--r--   0 runner     (501) staff       (20)    12839 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/stdlib/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    11742 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/stdlib.rs
--rw-r--r--   0 runner     (501) staff       (20)     5028 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/traits.rs
--rw-r--r--   0 runner     (501) staff       (20)    12013 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/value.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.694389 cao-lang-0.2.3/cao-lang/src/vm/
--rw-r--r--   0 runner     (501) staff       (20)    17984 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/instr_execution.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.696543 cao-lang-0.2.3/cao-lang/src/vm/runtime/
--rw-r--r--   0 runner     (501) staff       (20)     1006 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_function.rs
--rw-r--r--   0 runner     (501) staff       (20)     6511 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_object.rs
--rw-r--r--   0 runner     (501) staff       (20)     1105 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_string.rs
--rw-r--r--   0 runner     (501) staff       (20)     3729 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_table.rs
--rw-r--r--   0 runner     (501) staff       (20)    13858 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/runtime.rs
--rw-r--r--   0 runner     (501) staff       (20)     1882 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm/tests.rs
--rw-r--r--   0 runner     (501) staff       (20)    33219 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/src/vm.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.698609 cao-lang-0.2.3/cao-lang/tests/
--rw-r--r--   0 runner     (501) staff       (20)    46718 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/integration_tests.rs
--rw-r--r--   0 runner     (501) staff       (20)     1820 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/test_fibonacci.rs
--rw-r--r--   0 runner     (501) staff       (20)     1146 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/test_for_each.rs
--rw-r--r--   0 runner     (501) staff       (20)     3227 2024-04-04 21:06:14.000000 cao-lang-0.2.3/cao-lang/tests/test_tables.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.699120 cao-lang-0.2.3/py/
--rw-r--r--   0 runner     (501) staff       (20)      420 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/Cargo.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.701374 cao-lang-0.2.3/py/cao_lang/
--rw-r--r--   0 runner     (501) staff       (20)       27 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/cao_lang/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.704645 cao-lang-0.2.3/py/cao_lang.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1917 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-04 21:06:25.000000 cao-lang-0.2.3/py/cao_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.700141 cao-lang-0.2.3/py/src/
--rw-r--r--   0 runner     (501) staff       (20)     2664 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/src/lib.rs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 21:06:25.700600 cao-lang-0.2.3/py/tests/
--rw-r--r--   0 runner     (501) staff       (20)     2713 2024-04-04 21:06:14.000000 cao-lang-0.2.3/py/tests/test_cao_lang.py
--rw-r--r--   0 runner     (501) staff       (20)      117 2024-04-04 21:06:14.000000 cao-lang-0.2.3/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-04 21:06:25.705990 cao-lang-0.2.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1430 2024-04-04 21:06:14.000000 cao-lang-0.2.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.270860 cao_lang-0.2.4/
+-rw-r--r--   0 runner     (501) staff       (20)     1068 2024-04-25 18:36:55.000000 cao_lang-0.2.4/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      123 2024-04-25 18:36:55.000000 cao_lang-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-25 18:37:12.270246 cao_lang-0.2.4/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1098 2024-04-25 18:36:55.000000 cao_lang-0.2.4/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.240739 cao_lang-0.2.4/cao-lang/
+-rw-r--r--   0 runner     (501) staff       (20)     1317 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/Cargo.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.241304 cao_lang-0.2.4/cao-lang/benches/
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/benches/cao_lang_benches.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1246 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/build.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.247620 cao_lang-0.2.4/cao-lang/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.248273 cao_lang-0.2.4/cao-lang/src/alloc/
+-rw-r--r--   0 runner     (501) staff       (20)     3168 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/alloc/caolang_alloc.rs
+-rw-r--r--   0 runner     (501) staff       (20)      999 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/alloc.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1115 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/bytecode.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.250882 cao_lang-0.2.4/cao-lang/src/collections/
+-rw-r--r--   0 runner     (501) staff       (20)     3084 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/bounded_stack.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.251981 cao_lang-0.2.4/cao-lang/src/collections/handle_table/
+-rw-r--r--   0 runner     (501) staff       (20)     3731 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/handle_table/serde_impl.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2316 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/handle_table/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    16517 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/handle_table.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.253024 cao_lang-0.2.4/cao-lang/src/collections/hash_map/
+-rw-r--r--   0 runner     (501) staff       (20)     3774 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/hash_map/serde_impl.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3547 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/hash_map/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    15603 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/hash_map.rs
+-rw-r--r--   0 runner     (501) staff       (20)       84 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/mod.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5147 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/collections/value_stack.rs
+-rw-r--r--   0 runner     (501) staff       (20)     6726 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiled_program.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.256842 cao_lang-0.2.4/cao-lang/src/compiler/
+-rw-r--r--   0 runner     (501) staff       (20)    21508 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/card.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2273 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/compilation_error.rs
+-rw-r--r--   0 runner     (501) staff       (20)      423 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/compile_options.rs
+-rw-r--r--   0 runner     (501) staff       (20)      790 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/function.rs
+-rw-r--r--   0 runner     (501) staff       (20)      793 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/function_ir.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.257469 cao_lang-0.2.4/cao-lang/src/compiler/module/
+-rw-r--r--   0 runner     (501) staff       (20)     8441 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/module/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    17167 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/module.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3103 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    39222 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/compiler.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5505 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/instruction.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1606 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/lib.rs
+-rw-r--r--   0 runner     (501) staff       (20)      403 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/prelude.rs
+-rw-r--r--   0 runner     (501) staff       (20)     2992 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/procedures.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.257965 cao_lang-0.2.4/cao-lang/src/stdlib/
+-rw-r--r--   0 runner     (501) staff       (20)    12839 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/stdlib/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    11742 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/stdlib.rs
+-rw-r--r--   0 runner     (501) staff       (20)     5028 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/traits.rs
+-rw-r--r--   0 runner     (501) staff       (20)    12013 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/value.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.259734 cao_lang-0.2.4/cao-lang/src/vm/
+-rw-r--r--   0 runner     (501) staff       (20)    18548 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm/instr_execution.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.261702 cao_lang-0.2.4/cao-lang/src/vm/runtime/
+-rw-r--r--   0 runner     (501) staff       (20)     1006 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_function.rs
+-rw-r--r--   0 runner     (501) staff       (20)     6511 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_object.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_string.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3729 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_table.rs
+-rw-r--r--   0 runner     (501) staff       (20)    13858 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm/runtime.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1882 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm/tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)    33219 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/src/vm.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.263724 cao_lang-0.2.4/cao-lang/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    47668 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/tests/integration_tests.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1820 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/tests/test_fibonacci.rs
+-rw-r--r--   0 runner     (501) staff       (20)     1146 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/tests/test_for_each.rs
+-rw-r--r--   0 runner     (501) staff       (20)     3227 2024-04-25 18:36:55.000000 cao_lang-0.2.4/cao-lang/tests/test_tables.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.264276 cao_lang-0.2.4/py/
+-rw-r--r--   0 runner     (501) staff       (20)      420 2024-04-25 18:36:55.000000 cao_lang-0.2.4/py/Cargo.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.266377 cao_lang-0.2.4/py/cao_lang/
+-rw-r--r--   0 runner     (501) staff       (20)       27 2024-04-25 18:36:55.000000 cao_lang-0.2.4/py/cao_lang/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.269557 cao_lang-0.2.4/py/cao_lang.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-25 18:37:12.000000 cao_lang-0.2.4/py/cao_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1917 2024-04-25 18:37:12.000000 cao_lang-0.2.4/py/cao_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-25 18:37:12.000000 cao_lang-0.2.4/py/cao_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-25 18:37:11.000000 cao_lang-0.2.4/py/cao_lang.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-25 18:37:12.000000 cao_lang-0.2.4/py/cao_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.265241 cao_lang-0.2.4/py/src/
+-rw-r--r--   0 runner     (501) staff       (20)     2664 2024-04-25 18:36:55.000000 cao_lang-0.2.4/py/src/lib.rs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:37:12.265701 cao_lang-0.2.4/py/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     2713 2024-04-25 18:36:55.000000 cao_lang-0.2.4/py/tests/test_cao_lang.py
+-rw-r--r--   0 runner     (501) staff       (20)      117 2024-04-25 18:36:55.000000 cao_lang-0.2.4/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-25 18:37:12.270975 cao_lang-0.2.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1430 2024-04-25 18:36:55.000000 cao_lang-0.2.4/setup.py
```

### Comparing `cao-lang-0.2.3/LICENSE` & `cao_lang-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/PKG-INFO` & `cao_lang-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cao-lang
-Version: 0.2.3
+Version: 0.2.4
 Summary: The node based 'language' that governs the actors of the game Cao-Lo
 Home-page: https://github.com/caolo-game/cao-lang
 Author: Daniel Kiss
 Author-email: littlesnorrboy@gmail.com
 Project-URL: Bug Tracker, https://github.com/caolo-game/cao-lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cao-lang-0.2.3/README.md` & `cao_lang-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/Cargo.toml` & `cao_lang-0.2.4/cao-lang/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,8 @@
 build = "build.rs"
 description = "The back-end of cao-lang, a node based visual scripting language"
 edition = "2021"
 license = "MIT"
 name = "cao-lang"
 readme = "../README.md"
 repository = "https://github.com/caolo-game/cao-lang.git"
-version = "0.2.3"
+version = "0.2.4"
```

### Comparing `cao-lang-0.2.3/cao-lang/benches/cao_lang_benches.rs` & `cao_lang-0.2.4/cao-lang/benches/cao_lang_benches.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/build.rs` & `cao_lang-0.2.4/cao-lang/build.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/alloc/caolang_alloc.rs` & `cao_lang-0.2.4/cao-lang/src/alloc/caolang_alloc.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/alloc.rs` & `cao_lang-0.2.4/cao-lang/src/alloc.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/bytecode.rs` & `cao_lang-0.2.4/cao-lang/src/bytecode.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/bounded_stack.rs` & `cao_lang-0.2.4/cao-lang/src/collections/bounded_stack.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/handle_table/serde_impl.rs` & `cao_lang-0.2.4/cao-lang/src/collections/handle_table/serde_impl.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/handle_table/tests.rs` & `cao_lang-0.2.4/cao-lang/src/collections/handle_table/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/handle_table.rs` & `cao_lang-0.2.4/cao-lang/src/collections/handle_table.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/hash_map/serde_impl.rs` & `cao_lang-0.2.4/cao-lang/src/collections/hash_map/serde_impl.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/hash_map/tests.rs` & `cao_lang-0.2.4/cao-lang/src/collections/hash_map/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/hash_map.rs` & `cao_lang-0.2.4/cao-lang/src/collections/hash_map.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/collections/value_stack.rs` & `cao_lang-0.2.4/cao-lang/src/collections/value_stack.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiled_program.rs` & `cao_lang-0.2.4/cao-lang/src/compiled_program.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler/card.rs` & `cao_lang-0.2.4/cao-lang/src/compiler/card.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler/compilation_error.rs` & `cao_lang-0.2.4/cao-lang/src/compiler/compilation_error.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler/function.rs` & `cao_lang-0.2.4/cao-lang/src/compiler/function.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler/function_ir.rs` & `cao_lang-0.2.4/cao-lang/src/compiler/function_ir.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler/module/tests.rs` & `cao_lang-0.2.4/cao-lang/src/compiler/module/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler/module.rs` & `cao_lang-0.2.4/cao-lang/src/compiler/module.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler/tests.rs` & `cao_lang-0.2.4/cao-lang/src/compiler/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/compiler.rs` & `cao_lang-0.2.4/cao-lang/src/compiler.rs`

 * *Files 0% similar despite different names*

```diff
@@ -534,14 +534,17 @@
                 // ForEach instruction will push these values on the stack
                 let v_index = self.add_local_unchecked("")?;
                 let k_index = self.add_local_unchecked("")?;
                 let i_index = self.add_local_unchecked("")?;
                 self.push_instruction(Instruction::BeginForEach);
                 write_to_vec(loop_var, &mut self.program.bytecode);
                 write_to_vec(loop_item, &mut self.program.bytecode);
+                write_to_vec(i_index, &mut self.program.bytecode);
+                write_to_vec(k_index, &mut self.program.bytecode);
+                write_to_vec(v_index, &mut self.program.bytecode);
 
                 let block_begin = self.program.bytecode.len() as i32;
                 self.push_instruction(Instruction::ForEach);
                 write_to_vec(loop_var, &mut self.program.bytecode);
                 write_to_vec(loop_item, &mut self.program.bytecode);
                 write_to_vec(i_index, &mut self.program.bytecode);
                 write_to_vec(k_index, &mut self.program.bytecode);
```

### Comparing `cao-lang-0.2.3/cao-lang/src/instruction.rs` & `cao_lang-0.2.4/cao-lang/src/instruction.rs`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             Instruction::SetLocalVar
             | Instruction::SetUpvalue
             | Instruction::ReadUpvalue
             | Instruction::ReadLocalVar => size_of::<u32>(),
             Instruction::Goto | Instruction::GotoIfTrue | Instruction::GotoIfFalse => {
                 size_of::<i32>()
             }
-            Instruction::BeginForEach => size_of::<u32>() * 2,
+            Instruction::BeginForEach => size_of::<u32>() * 5,
             Instruction::ForEach => size_of::<u32>() * 5,
             Instruction::FunctionPointer => size_of::<Handle>() + size_of::<u32>(),
             Instruction::Closure => size_of::<Handle>() + size_of::<u32>(),
             Instruction::RegisterUpvalue => size_of::<u8>() * 2,
         };
         1 + data_span
     }
```

### Comparing `cao-lang-0.2.3/cao-lang/src/lib.rs` & `cao_lang-0.2.4/cao-lang/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/procedures.rs` & `cao_lang-0.2.4/cao-lang/src/procedures.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/stdlib/tests.rs` & `cao_lang-0.2.4/cao-lang/src/stdlib/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/stdlib.rs` & `cao_lang-0.2.4/cao-lang/src/stdlib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/traits.rs` & `cao_lang-0.2.4/cao-lang/src/traits.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/value.rs` & `cao_lang-0.2.4/cao-lang/src/value.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/vm/instr_execution.rs` & `cao_lang-0.2.4/cao-lang/src/vm/instr_execution.rs`

 * *Files 2% similar despite different names*

```diff
@@ -342,14 +342,25 @@
     // test if the input is a table
     let item = vm.get_table_mut(item_val)?;
     debug!("Starting for-each on table {:?}", item);
     let offset = stack_offset(vm);
     write_local_var(vm, i_handle, Value::Integer(0), offset)?;
     write_local_var(vm, t_handle, item_val, offset)?;
 
+    // initialize local variables
+    //
+    // must be initialized at this point, otherwise the scope end cleans up non-existent locals
+    // if for-each is called with an empty list
+    let i_handle: u32 = unsafe { decode_value(bytecode, instr_ptr) };
+    let k_handle: u32 = unsafe { decode_value(bytecode, instr_ptr) };
+    let v_handle: u32 = unsafe { decode_value(bytecode, instr_ptr) };
+    write_local_var(vm, v_handle, Value::Nil, offset)?;
+    write_local_var(vm, k_handle, Value::Nil, offset)?;
+    write_local_var(vm, i_handle, Value::Nil, offset)?;
+
     Ok(())
 }
 
 /// Assumes that [begin_for_each](begin_for_each) was called once to set up the loop
 ///
 /// Pushes the next key and the object onto the stack. Assumes that the function takes these as
 /// parameters.
```

### Comparing `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_function.rs` & `cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_function.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_object.rs` & `cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_object.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_string.rs` & `cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_string.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/vm/runtime/cao_lang_table.rs` & `cao_lang-0.2.4/cao-lang/src/vm/runtime/cao_lang_table.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/vm/runtime.rs` & `cao_lang-0.2.4/cao-lang/src/vm/runtime.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/vm/tests.rs` & `cao_lang-0.2.4/cao-lang/src/vm/tests.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/src/vm.rs` & `cao_lang-0.2.4/cao-lang/src/vm.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/tests/integration_tests.rs` & `cao_lang-0.2.4/cao-lang/tests/integration_tests.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1278,15 +1278,14 @@
     let mut vm = Vm::new(()).unwrap();
     vm.run(&program).expect("run");
 
     let result = vm
         .read_var_by_name("g_result", &program.variables)
         .expect("Failed to read g_result variable");
 
-
     unsafe {
         let result = result.as_str().unwrap();
 
         assert_eq!(result, "winnie the pooh");
     }
 }
 
@@ -1549,7 +1548,39 @@
 
         for ((_, a), b) in result.iter().zip(["a", "b", "c"].into_iter()) {
             let a = a.as_str().expect("results should be strings");
             assert_eq!(a, b);
         }
     }
 }
+
+#[test]
+fn test_empty_list_foreach() {
+    // regression test
+    // for-each with an empty array cleans up non-existent locals
+    //
+    let cu = Module {
+        submodules: Default::default(),
+        functions: vec![(
+            "main".to_string(),
+            Function {
+                arguments: Default::default(),
+                cards: vec![
+                    Card::ForEach(Box::new(ForEach {
+                        i: None,
+                        k: None,
+                        v: Some("v".to_string()),
+                        iterable: Box::new(Card::Array(vec![])),
+                        body: Default::default(),
+                    })),
+                    Card::set_var("asd", Card::Array(vec![])),
+                ],
+            },
+        )],
+        imports: Default::default(),
+    };
+
+    let program = compile(cu, None).expect("compile");
+
+    let mut vm = Vm::new(()).unwrap();
+    vm.run(&program).expect("run");
+}
```

### Comparing `cao-lang-0.2.3/cao-lang/tests/test_fibonacci.rs` & `cao_lang-0.2.4/cao-lang/tests/test_fibonacci.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/tests/test_for_each.rs` & `cao_lang-0.2.4/cao-lang/tests/test_for_each.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/cao-lang/tests/test_tables.rs` & `cao_lang-0.2.4/cao-lang/tests/test_tables.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/py/cao_lang.egg-info/PKG-INFO` & `cao_lang-0.2.4/py/cao_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cao-lang
-Version: 0.2.3
+Version: 0.2.4
 Summary: The node based 'language' that governs the actors of the game Cao-Lo
 Home-page: https://github.com/caolo-game/cao-lang
 Author: Daniel Kiss
 Author-email: littlesnorrboy@gmail.com
 Project-URL: Bug Tracker, https://github.com/caolo-game/cao-lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cao-lang-0.2.3/py/cao_lang.egg-info/SOURCES.txt` & `cao_lang-0.2.4/py/cao_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/py/src/lib.rs` & `cao_lang-0.2.4/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/py/tests/test_cao_lang.py` & `cao_lang-0.2.4/py/tests/test_cao_lang.py`

 * *Files identical despite different names*

### Comparing `cao-lang-0.2.3/setup.py` & `cao_lang-0.2.4/setup.py`

 * *Files identical despite different names*

