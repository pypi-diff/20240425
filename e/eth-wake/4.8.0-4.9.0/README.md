# Comparing `tmp/eth_wake-4.8.0.tar.gz` & `tmp/eth_wake-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth_wake-4.8.0.tar", max compression
+gzip compressed data, was "eth_wake-4.9.0.tar", max compression
```

## Comparing `eth_wake-4.8.0.tar` & `eth_wake-4.9.0.tar`

### file list

```diff
@@ -1,298 +1,298 @@
--rw-r--r--   0        0        0      751 2024-04-05 10:35:38.715089 eth_wake-4.8.0/LICENSE
--rw-r--r--   0        0        0     9113 2024-04-05 10:35:38.715089 eth_wake-4.8.0/README.md
--rw-r--r--   0        0        0       61 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/.gitignore
--rw-r--r--   0        0        0      431 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/README.md
--rw-r--r--   0        0        0     1198 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/contracts/Counter.sol
--rw-r--r--   0        0        0      622 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/contracts/Gateway.sol
--rw-r--r--   0        0        0      307 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/contracts/Imports.sol
--rw-r--r--   0        0        0      215 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/hardhat.config.js
--rw-r--r--   0        0        0      813 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/package-lock.json
--rw-r--r--   0        0        0       97 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/package.json
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/scripts/__init__.py
--rw-r--r--   0        0        0      350 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/scripts/deploy.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/__init__.py
--rw-r--r--   0        0        0     3559 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_counter.py
--rw-r--r--   0        0        0     1815 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz.py
--rw-r--r--   0        0        0     1170 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz_failing.py
--rw-r--r--   0        0        0     3404 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/tests/test_crosschain.py
--rw-r--r--   0        0        0       24 2024-04-05 10:35:38.739090 eth_wake-4.8.0/examples/counter/wake.toml
--rw-r--r--   0        0        0     3404 2024-04-05 10:35:38.743090 eth_wake-4.8.0/pyproject.toml
--rw-r--r--   0        0        0      355 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/__init__.py
--rw-r--r--   0        0        0       25 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/__init__.py
--rw-r--r--   0        0        0    37717 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/cfg.py
--rw-r--r--   0        0        0     7584 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/expressions.py
--rw-r--r--   0        0        0     2353 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/graph.py
--rw-r--r--   0        0        0     1543 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/interface.py
--rw-r--r--   0        0        0    16505 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/ownable.py
--rw-r--r--   0        0        0     1093 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/proxy.py
--rw-r--r--   0        0        0     7416 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/analysis/utils.py
--rw-r--r--   0        0        0       38 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/__init__.py
--rw-r--r--   0        0        0     7310 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/__main__.py
--rw-r--r--   0        0        0     8068 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/accounts.py
--rw-r--r--   0        0        0     8674 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/compile.py
--rw-r--r--   0        0        0       54 2024-04-05 10:35:38.743090 eth_wake-4.8.0/wake/cli/console.py
--rw-r--r--   0        0        0    30671 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/detect.py
--rw-r--r--   0        0        0    24955 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/init.py
--rw-r--r--   0        0        0     1298 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/lsp.py
--rw-r--r--   0        0        0     8269 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/open.py
--rw-r--r--   0        0        0     5495 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/param_types.py
--rw-r--r--   0        0        0    23532 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/print.py
--rw-r--r--   0        0        0     3583 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/run.py
--rw-r--r--   0        0        0     5877 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/svm.py
--rw-r--r--   0        0        0     9541 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/cli/test.py
--rw-r--r--   0        0        0      187 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/__init__.py
--rw-r--r--   0        0        0     4929 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/build_data_model.py
--rw-r--r--   0        0        0     3120 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/compilation_unit.py
--rw-r--r--   0        0        0    53031 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/compiler.py
--rw-r--r--   0        0        0       97 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/exceptions.py
--rw-r--r--   0        0        0      103 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/__init__.py
--rw-r--r--   0        0        0       48 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/exceptions.py
--rw-r--r--   0        0        0     8831 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/input_data_model.py
--rw-r--r--   0        0        0     9163 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/output_data_model.py
--rw-r--r--   0        0        0     3597 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/solc_frontend/solc_runner.py
--rw-r--r--   0        0        0     2455 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/source_path_resolver.py
--rw-r--r--   0        0        0     4912 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/compiler/source_unit_name_resolver.py
--rw-r--r--   0        0        0     1118 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/config/__init__.py
--rw-r--r--   0        0        0    11941 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/config/data_model.py
--rw-r--r--   0        0        0    15443 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/config/wake_config.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/contracts/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/contracts/wake/__init__.py
--rw-r--r--   0        0        0    64087 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/contracts/wake/console.sol
--rw-r--r--   0        0        0       32 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/__init__.py
--rw-r--r--   0        0        0      408 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/enums.py
--rw-r--r--   0        0        0      640 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/logging.py
--rw-r--r--   0        0        0    11342 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/lsp_provider.py
--rw-r--r--   0        0        0    29888 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/solidity_version.py
--rw-r--r--   0        0        0    27317 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/visitor.py
--rw-r--r--   0        0        0     1793 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/core/wake_comments.py
--rw-r--r--   0        0        0      734 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/deployment/__init__.py
--rw-r--r--   0        0        0    14991 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/deployment/core.py
--rw-r--r--   0        0        0      141 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/__init__.py
--rw-r--r--   0        0        0    29661 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/api.py
--rw-r--r--   0        0        0      649 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/template.py
--rw-r--r--   0        0        0     7760 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/detectors/utils.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/__init__.py
--rw-r--r--   0        0        0     4552 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/blocks.py
--rw-r--r--   0        0        0    50133 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/call_trace.py
--rw-r--r--   0        0        0    29599 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/chain_interfaces.py
--rw-r--r--   0        0        0     1320 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/constants.py
--rw-r--r--   0        0        0   111039 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/core.py
--rw-r--r--   0        0        0     8429 2024-04-05 10:35:38.747090 eth_wake-4.8.0/wake/development/globals.py
--rw-r--r--   0        0        0   161115 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/hardhat_console.py
--rw-r--r--   0        0        0     1267 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/internal.py
--rw-r--r--   0        0        0       39 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/abc.py
--rw-r--r--   0        0        0     2092 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/communicator.py
--rw-r--r--   0        0        0      825 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/http.py
--rw-r--r--   0        0        0     2912 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/ipc.py
--rw-r--r--   0        0        0      668 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/json_rpc/websocket.py
--rw-r--r--   0        0        0    17584 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/primitive_types.py
--rw-r--r--   0        0        0    96402 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/pytypes_generator.py
--rw-r--r--   0        0        0    29435 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/transactions.py
--rw-r--r--   0        0        0    45923 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/development/utils.py
--rw-r--r--   0        0        0     4197 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/__init__.py
--rw-r--r--   0        0        0     4947 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/abc.py
--rw-r--r--   0        0        0    39042 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/ast.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/__init__.py
--rw-r--r--   0        0        0     5827 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/abc.py
--rw-r--r--   0        0        0    19160 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/contract_definition.py
--rw-r--r--   0        0        0     4102 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/enum_definition.py
--rw-r--r--   0        0        0     2047 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/enum_value.py
--rw-r--r--   0        0        0     5380 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/error_definition.py
--rw-r--r--   0        0        0     6611 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/event_definition.py
--rw-r--r--   0        0        0    20351 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/function_definition.py
--rw-r--r--   0        0        0    14120 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/modifier_definition.py
--rw-r--r--   0        0        0     4401 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/struct_definition.py
--rw-r--r--   0        0        0     3662 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/user_defined_value_type_definition.py
--rw-r--r--   0        0        0    20534 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/declarations/variable_declaration.py
--rw-r--r--   0        0        0    11238 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/enums.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/__init__.py
--rw-r--r--   0        0        0     8026 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/abc.py
--rw-r--r--   0        0        0     5988 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/assignment.py
--rw-r--r--   0        0        0     4316 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/binary_operation.py
--rw-r--r--   0        0        0     2627 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/conditional.py
--rw-r--r--   0        0        0     2001 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/elementary_type_name_expression.py
--rw-r--r--   0        0        0    11941 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/function_call.py
--rw-r--r--   0        0        0     3383 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/function_call_options.py
--rw-r--r--   0        0        0     9399 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/identifier.py
--rw-r--r--   0        0        0     2612 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/index_access.py
--rw-r--r--   0        0        0     3662 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/index_range_access.py
--rw-r--r--   0        0        0     2850 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/literal.py
--rw-r--r--   0        0        0    20305 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/member_access.py
--rw-r--r--   0        0        0     2372 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/new_expression.py
--rw-r--r--   0        0        0     3325 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/tuple_expression.py
--rw-r--r--   0        0        0     4515 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/expressions/unary_operation.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/__init__.py
--rw-r--r--   0        0        0    10622 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/identifier_path.py
--rw-r--r--   0        0        0     9570 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/import_directive.py
--rw-r--r--   0        0        0     3751 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/inheritance_specifier.py
--rw-r--r--   0        0        0     6082 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/modifier_invocation.py
--rw-r--r--   0        0        0     3449 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/override_specifier.py
--rw-r--r--   0        0        0     4305 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/parameter_list.py
--rw-r--r--   0        0        0     1553 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/pragma_directive.py
--rw-r--r--   0        0        0    12331 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/source_unit.py
--rw-r--r--   0        0        0     2539 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/structured_documentation.py
--rw-r--r--   0        0        0     4686 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/try_catch_clause.py
--rw-r--r--   0        0        0     5668 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/meta/using_for_directive.py
--rw-r--r--   0        0        0     9999 2024-04-05 10:35:38.751090 eth_wake-4.8.0/wake/ir/reference_resolver.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/__init__.py
--rw-r--r--   0        0        0     6652 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/abc.py
--rw-r--r--   0        0        0     3254 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/block.py
--rw-r--r--   0        0        0     1722 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/break_statement.py
--rw-r--r--   0        0        0     1746 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/continue_statement.py
--rw-r--r--   0        0        0     2628 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/do_while_statement.py
--rw-r--r--   0        0        0     2545 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/emit_statement.py
--rw-r--r--   0        0        0     4836 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/expression_statement.py
--rw-r--r--   0        0        0     5797 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/for_statement.py
--rw-r--r--   0        0        0     3488 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/if_statement.py
--rw-r--r--   0        0        0    11028 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/inline_assembly.py
--rw-r--r--   0        0        0     1694 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/placeholder_statement.py
--rw-r--r--   0        0        0     3423 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/return_statement.py
--rw-r--r--   0        0        0     2717 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/revert_statement.py
--rw-r--r--   0        0        0     3243 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/try_statement.py
--rw-r--r--   0        0        0     2571 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/unchecked_block.py
--rw-r--r--   0        0        0     4389 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/variable_declaration_statement.py
--rw-r--r--   0        0        0     2661 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/statements/while_statement.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/__init__.py
--rw-r--r--   0        0        0     5137 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/abc.py
--rw-r--r--   0        0        0     4062 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/array_type_name.py
--rw-r--r--   0        0        0     5924 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/elementary_type_name.py
--rw-r--r--   0        0        0     3961 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/function_type_name.py
--rw-r--r--   0        0        0     6502 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/mapping.py
--rw-r--r--   0        0        0    11357 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/type_names/user_defined_type_name.py
--rw-r--r--   0        0        0    61318 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/types.py
--rw-r--r--   0        0        0      822 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/utils.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/__init__.py
--rw-r--r--   0        0        0     1718 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/abc.py
--rw-r--r--   0        0        0     3025 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/assignment.py
--rw-r--r--   0        0        0     4701 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/block.py
--rw-r--r--   0        0        0     1007 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/break_statement.py
--rw-r--r--   0        0        0     2453 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/case_.py
--rw-r--r--   0        0        0     1064 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/continue_statement.py
--rw-r--r--   0        0        0     1860 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/expression_statement.py
--rw-r--r--   0        0        0     3256 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/for_loop.py
--rw-r--r--   0        0        0     6392 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/function_call.py
--rw-r--r--   0        0        0     3516 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/function_definition.py
--rw-r--r--   0        0        0     2828 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/identifier.py
--rw-r--r--   0        0        0     2731 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/if_statement.py
--rw-r--r--   0        0        0     1266 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/leave.py
--rw-r--r--   0        0        0     3619 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/literal.py
--rw-r--r--   0        0        0     3147 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/switch.py
--rw-r--r--   0        0        0     2198 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/typed_name.py
--rw-r--r--   0        0        0     3235 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/ir/yul/variable_declaration.py
--rw-r--r--   0        0        0       47 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/__init__.py
--rw-r--r--   0        0        0      310 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/__init__.py
--rw-r--r--   0        0        0     3842 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_control_flow_graph.py
--rw-r--r--   0        0        0     1123 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_imports_graph.py
--rw-r--r--   0        0        0     4303 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_inheritance_graph.py
--rw-r--r--   0        0        0     2291 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/generate_linearized_inheritance_graph.py
--rw-r--r--   0        0        0     4128 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/commands/init.py
--rw-r--r--   0        0        0    31620 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/common_structures.py
--rw-r--r--   0        0        0     2552 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/context.py
--rw-r--r--   0        0        0     2574 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/document_sync.py
--rw-r--r--   0        0        0      130 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/enums.py
--rw-r--r--   0        0        0      471 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/__init__.py
--rw-r--r--   0        0        0     6969 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/code_action.py
--rw-r--r--   0        0        0    11750 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/code_lens.py
--rw-r--r--   0        0        0    20068 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/completion.py
--rw-r--r--   0        0        0    10194 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/definition.py
--rw-r--r--   0        0        0     1472 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/diagnostic.py
--rw-r--r--   0        0        0     4331 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/document_link.py
--rw-r--r--   0        0        0     8062 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/document_symbol.py
--rw-r--r--   0        0        0    18513 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/hover.py
--rw-r--r--   0        0        0     3927 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/implementation.py
--rw-r--r--   0        0        0     3525 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/inlay_hint.py
--rw-r--r--   0        0        0     5115 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/references.py
--rw-r--r--   0        0        0     8941 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/rename.py
--rw-r--r--   0        0        0     9389 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/type_definition.py
--rw-r--r--   0        0        0    11131 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/features/type_hierarchy.py
--rw-r--r--   0        0        0      750 2024-04-05 10:35:38.755090 eth_wake-4.8.0/wake/lsp/logging_handler.py
--rw-r--r--   0        0        0    66467 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/lsp_compiler.py
--rw-r--r--   0        0        0      328 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/lsp_data_model.py
--rw-r--r--   0        0        0     8941 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/lsp_parser.py
--rw-r--r--   0        0        0     5551 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/methods.py
--rw-r--r--   0        0        0     1897 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/protocol_structures.py
--rw-r--r--   0        0        0     2229 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/rpc_protocol.py
--rw-r--r--   0        0        0    55986 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/server.py
--rw-r--r--   0        0        0     6793 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/server_capabilities.py
--rw-r--r--   0        0        0       86 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/utils/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/utils/position.py
--rw-r--r--   0        0        0      459 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/lsp/utils/uri.py
--rw-r--r--   0        0        0      102 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/migrations/__init__.py
--rw-r--r--   0        0        0     9091 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/migrations/woke_wake_migration.py
--rw-r--r--   0        0        0     3307 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/migrations/xdg_migration.py
--rw-r--r--   0        0        0       74 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/printers/__init__.py
--rw-r--r--   0        0        0    14954 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/printers/api.py
--rw-r--r--   0        0        0      412 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/printers/template.py
--rw-r--r--   0        0        0       50 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/regex_parser/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/regex_parser/solidity_import.py
--rw-r--r--   0        0        0    10611 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/regex_parser/solidity_parser.py
--rw-r--r--   0        0        0       36 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/__init__.py
--rw-r--r--   0        0        0     1815 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/abc.py
--rw-r--r--   0        0        0      270 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/exceptions.py
--rw-r--r--   0        0        0    12254 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/svm/svm.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/scripts/__init__.py
--rw-r--r--   0        0        0      184 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/scripts/deploy.py
--rw-r--r--   0        0        0        0 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/tests/__init__.py
--rw-r--r--   0        0        0      253 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/templates/tests/test_default.py
--rw-r--r--   0        0        0      838 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/__init__.py
--rw-r--r--   0        0        0    11116 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/core.py
--rw-r--r--   0        0        0    23995 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/coverage.py
--rw-r--r--   0        0        0      187 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/__init__.py
--rw-r--r--   0        0        0     5028 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/fuzz_test.py
--rw-r--r--   0        0        0    10577 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/fuzzer.py
--rw-r--r--   0        0        0     5407 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/fuzzing/generators.py
--rw-r--r--   0        0        0     8240 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess.py
--rw-r--r--   0        0        0    12854 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess_server.py
--rw-r--r--   0        0        0     3057 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/testing/pytest_plugin_single.py
--rw-r--r--   0        0        0      288 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/__init__.py
--rw-r--r--   0        0        0      654 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/context_managers.py
--rw-r--r--   0        0        0      975 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/decorators.py
--rw-r--r--   0        0        0      158 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/enums.py
--rw-r--r--   0        0        0     1699 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/file_utils.py
--rw-r--r--   0        0        0      518 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/formatters.py
--rw-r--r--   0        0        0      875 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/general.py
--rw-r--r--   0        0        0      384 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/keyed_default_dict.py
--rw-r--r--   0        0        0      194 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/networking.py
--rw-r--r--   0        0        0     1569 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/null_file.py
--rw-r--r--   0        0        0     1017 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/openzeppelin.py
--rw-r--r--   0        0        0      630 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/string.py
--rw-r--r--   0        0        0     1747 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/tee.py
--rw-r--r--   0        0        0     3792 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/threaded_child_watcher.py
--rw-r--r--   0        0        0      424 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake/utils/version.py
--rw-r--r--   0        0        0     1296 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/__init__.py
--rw-r--r--   0        0        0     3726 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/abi_encode_with_signature.py
--rw-r--r--   0        0        0    15179 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/axelar_proxy_contract_id.py
--rw-r--r--   0        0        0     5656 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/balance_relied_on.py
--rw-r--r--   0        0        0     3197 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/call_options_not_called.py
--rw-r--r--   0        0        0     9968 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py
--rw-r--r--   0        0        0     2525 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/complex_struct_getter.py
--rw-r--r--   0        0        0     3434 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/empty_byte_array_copy_bug.py
--rw-r--r--   0        0        0    18811 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/incorrect_interface.py
--rw-r--r--   0        0        0     4318 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/missing_return.py
--rw-r--r--   0        0        0     4082 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/msg_value_nonpayable_function.py
--rw-r--r--   0        0        0    11049 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/reentrancy.py
--rw-r--r--   0        0        0     2364 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/struct_mapping_deletion.py
--rw-r--r--   0        0        0     3590 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/tx_origin.py
--rw-r--r--   0        0        0     4019 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/unchecked_return_value.py
--rw-r--r--   0        0        0     1681 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/unprotected_selfdestruct.py
--rw-r--r--   0        0        0     6655 2024-04-05 10:35:38.759090 eth_wake-4.8.0/wake_detectors/unsafe_delegatecall.py
--rw-r--r--   0        0        0     2198 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unsafe_erc20_call.py
--rw-r--r--   0        0        0     2225 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_contract.py
--rw-r--r--   0        0        0     1790 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_function.py
--rw-r--r--   0        0        0     2781 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_import.py
--rw-r--r--   0        0        0     1520 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/unused_modifier.py
--rw-r--r--   0        0        0      229 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_detectors/utils.py
--rw-r--r--   0        0        0      462 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/__init__.py
--rw-r--r--   0        0        0     3487 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/abi.py
--rw-r--r--   0        0        0     3223 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/c3_linearization.py
--rw-r--r--   0        0        0     4260 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/control_flow_graph.py
--rw-r--r--   0        0        0     5435 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/imports_graph.py
--rw-r--r--   0        0        0     6127 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/inheritance_graph.py
--rw-r--r--   0        0        0     1574 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/inheritance_tree.py
--rw-r--r--   0        0        0     5805 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/modifiers.py
--rw-r--r--   0        0        0     5748 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/state_changes.py
--rw-r--r--   0        0        0     3600 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/storage_layout.py
--rw-r--r--   0        0        0     8131 2024-04-05 10:35:38.763090 eth_wake-4.8.0/wake_printers/tokens.py
--rw-r--r--   0        0        0    12327 1970-01-01 00:00:00.000000 eth_wake-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0      751 2024-04-25 15:45:13.739084 eth_wake-4.9.0/LICENSE
+-rw-r--r--   0        0        0     9043 2024-04-25 15:45:13.739084 eth_wake-4.9.0/README.md
+-rw-r--r--   0        0        0       61 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/.gitignore
+-rw-r--r--   0        0        0      431 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/README.md
+-rw-r--r--   0        0        0     1198 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/contracts/Counter.sol
+-rw-r--r--   0        0        0      622 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/contracts/Gateway.sol
+-rw-r--r--   0        0        0      307 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/contracts/Imports.sol
+-rw-r--r--   0        0        0      215 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/hardhat.config.js
+-rw-r--r--   0        0        0      813 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/package-lock.json
+-rw-r--r--   0        0        0       97 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/package.json
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/scripts/__init__.py
+-rw-r--r--   0        0        0      350 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/tests/__init__.py
+-rw-r--r--   0        0        0     3559 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/tests/test_counter.py
+-rw-r--r--   0        0        0     1815 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/tests/test_counter_fuzz.py
+-rw-r--r--   0        0        0     1170 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/tests/test_counter_fuzz_failing.py
+-rw-r--r--   0        0        0     3404 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/tests/test_crosschain.py
+-rw-r--r--   0        0        0       24 2024-04-25 15:45:13.763084 eth_wake-4.9.0/examples/counter/wake.toml
+-rw-r--r--   0        0        0     3394 2024-04-25 15:45:13.767084 eth_wake-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0      355 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/__init__.py
+-rw-r--r--   0        0        0    37645 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/cfg.py
+-rw-r--r--   0        0        0     7584 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/expressions.py
+-rw-r--r--   0        0        0     2353 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/graph.py
+-rw-r--r--   0        0        0     1543 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/interface.py
+-rw-r--r--   0        0        0    16573 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/ownable.py
+-rw-r--r--   0        0        0     1093 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/proxy.py
+-rw-r--r--   0        0        0     7416 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/analysis/utils.py
+-rw-r--r--   0        0        0       38 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/__init__.py
+-rw-r--r--   0        0        0     7310 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/__main__.py
+-rw-r--r--   0        0        0     8068 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/accounts.py
+-rw-r--r--   0        0        0     8674 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/compile.py
+-rw-r--r--   0        0        0       54 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/console.py
+-rw-r--r--   0        0        0    30671 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/detect.py
+-rw-r--r--   0        0        0    24955 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/init.py
+-rw-r--r--   0        0        0     1298 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/lsp.py
+-rw-r--r--   0        0        0     8269 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/open.py
+-rw-r--r--   0        0        0     5495 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/param_types.py
+-rw-r--r--   0        0        0    23532 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/print.py
+-rw-r--r--   0        0        0     3583 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/run.py
+-rw-r--r--   0        0        0     5877 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/svm.py
+-rw-r--r--   0        0        0     9541 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/cli/test.py
+-rw-r--r--   0        0        0      187 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/__init__.py
+-rw-r--r--   0        0        0     4929 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/build_data_model.py
+-rw-r--r--   0        0        0     3120 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/compilation_unit.py
+-rw-r--r--   0        0        0    53031 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/compiler.py
+-rw-r--r--   0        0        0       97 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/exceptions.py
+-rw-r--r--   0        0        0      103 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/solc_frontend/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/solc_frontend/exceptions.py
+-rw-r--r--   0        0        0     8831 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/solc_frontend/input_data_model.py
+-rw-r--r--   0        0        0     9163 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/solc_frontend/output_data_model.py
+-rw-r--r--   0        0        0     3597 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/solc_frontend/solc_runner.py
+-rw-r--r--   0        0        0     2455 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/source_path_resolver.py
+-rw-r--r--   0        0        0     4912 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/compiler/source_unit_name_resolver.py
+-rw-r--r--   0        0        0     1118 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/config/__init__.py
+-rw-r--r--   0        0        0    11941 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/config/data_model.py
+-rw-r--r--   0        0        0    15443 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/config/wake_config.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/contracts/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/contracts/wake/__init__.py
+-rw-r--r--   0        0        0    64087 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/contracts/wake/console.sol
+-rw-r--r--   0        0        0       32 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/core/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/core/enums.py
+-rw-r--r--   0        0        0      640 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/core/logging.py
+-rw-r--r--   0        0        0    11312 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/core/lsp_provider.py
+-rw-r--r--   0        0        0    29888 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/core/solidity_version.py
+-rw-r--r--   0        0        0    27317 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/core/visitor.py
+-rw-r--r--   0        0        0     1793 2024-04-25 15:45:13.771084 eth_wake-4.9.0/wake/core/wake_comments.py
+-rw-r--r--   0        0        0      757 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/deployment/__init__.py
+-rw-r--r--   0        0        0    15097 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/deployment/core.py
+-rw-r--r--   0        0        0      141 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/detectors/__init__.py
+-rw-r--r--   0        0        0    29661 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/detectors/api.py
+-rw-r--r--   0        0        0      649 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/detectors/template.py
+-rw-r--r--   0        0        0     7760 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/detectors/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/__init__.py
+-rw-r--r--   0        0        0     4552 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/blocks.py
+-rw-r--r--   0        0        0    50133 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/call_trace.py
+-rw-r--r--   0        0        0    29599 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/chain_interfaces.py
+-rw-r--r--   0        0        0     1320 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/constants.py
+-rw-r--r--   0        0        0   117142 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/core.py
+-rw-r--r--   0        0        0     8429 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/globals.py
+-rw-r--r--   0        0        0   161115 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/hardhat_console.py
+-rw-r--r--   0        0        0     1267 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/internal.py
+-rw-r--r--   0        0        0       39 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/json_rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/json_rpc/abc.py
+-rw-r--r--   0        0        0     2092 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/json_rpc/communicator.py
+-rw-r--r--   0        0        0      825 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/json_rpc/http.py
+-rw-r--r--   0        0        0     2912 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/json_rpc/ipc.py
+-rw-r--r--   0        0        0      668 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/json_rpc/websocket.py
+-rw-r--r--   0        0        0    17584 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/primitive_types.py
+-rw-r--r--   0        0        0    97373 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/pytypes_generator.py
+-rw-r--r--   0        0        0    29657 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/transactions.py
+-rw-r--r--   0        0        0    45923 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/development/utils.py
+-rw-r--r--   0        0        0     4197 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/__init__.py
+-rw-r--r--   0        0        0     4947 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/abc.py
+-rw-r--r--   0        0        0    39042 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/ast.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/__init__.py
+-rw-r--r--   0        0        0     5827 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/abc.py
+-rw-r--r--   0        0        0    19651 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/contract_definition.py
+-rw-r--r--   0        0        0     4628 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/enum_definition.py
+-rw-r--r--   0        0        0     2047 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/enum_value.py
+-rw-r--r--   0        0        0     5380 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/error_definition.py
+-rw-r--r--   0        0        0     7137 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/event_definition.py
+-rw-r--r--   0        0        0    20877 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/function_definition.py
+-rw-r--r--   0        0        0    14646 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/modifier_definition.py
+-rw-r--r--   0        0        0     4927 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/struct_definition.py
+-rw-r--r--   0        0        0     4188 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/user_defined_value_type_definition.py
+-rw-r--r--   0        0        0    21101 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/declarations/variable_declaration.py
+-rw-r--r--   0        0        0    11238 2024-04-25 15:45:13.775084 eth_wake-4.9.0/wake/ir/enums.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/__init__.py
+-rw-r--r--   0        0        0     8026 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/abc.py
+-rw-r--r--   0        0        0     5988 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/assignment.py
+-rw-r--r--   0        0        0     4316 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/binary_operation.py
+-rw-r--r--   0        0        0     2627 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/conditional.py
+-rw-r--r--   0        0        0     2001 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/elementary_type_name_expression.py
+-rw-r--r--   0        0        0    11941 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/function_call.py
+-rw-r--r--   0        0        0     3383 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/function_call_options.py
+-rw-r--r--   0        0        0     9399 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/identifier.py
+-rw-r--r--   0        0        0     2612 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/index_access.py
+-rw-r--r--   0        0        0     3662 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/index_range_access.py
+-rw-r--r--   0        0        0     2850 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/literal.py
+-rw-r--r--   0        0        0    20812 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/member_access.py
+-rw-r--r--   0        0        0     2372 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/new_expression.py
+-rw-r--r--   0        0        0     3325 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/tuple_expression.py
+-rw-r--r--   0        0        0     4515 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/expressions/unary_operation.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/__init__.py
+-rw-r--r--   0        0        0    11137 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/identifier_path.py
+-rw-r--r--   0        0        0    10079 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/import_directive.py
+-rw-r--r--   0        0        0     3751 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/inheritance_specifier.py
+-rw-r--r--   0        0        0     6082 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/modifier_invocation.py
+-rw-r--r--   0        0        0     3449 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/override_specifier.py
+-rw-r--r--   0        0        0     4305 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/parameter_list.py
+-rw-r--r--   0        0        0     1553 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/pragma_directive.py
+-rw-r--r--   0        0        0    12331 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/source_unit.py
+-rw-r--r--   0        0        0     2539 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/structured_documentation.py
+-rw-r--r--   0        0        0     4686 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/try_catch_clause.py
+-rw-r--r--   0        0        0     5668 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/meta/using_for_directive.py
+-rw-r--r--   0        0        0     9999 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/reference_resolver.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/__init__.py
+-rw-r--r--   0        0        0     6652 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/abc.py
+-rw-r--r--   0        0        0     3254 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/block.py
+-rw-r--r--   0        0        0     1722 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/break_statement.py
+-rw-r--r--   0        0        0     1746 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/continue_statement.py
+-rw-r--r--   0        0        0     2628 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/do_while_statement.py
+-rw-r--r--   0        0        0     2545 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/emit_statement.py
+-rw-r--r--   0        0        0     4836 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/expression_statement.py
+-rw-r--r--   0        0        0     5797 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/for_statement.py
+-rw-r--r--   0        0        0     3488 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/if_statement.py
+-rw-r--r--   0        0        0    11511 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/inline_assembly.py
+-rw-r--r--   0        0        0     1694 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/placeholder_statement.py
+-rw-r--r--   0        0        0     3423 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/return_statement.py
+-rw-r--r--   0        0        0     2717 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/revert_statement.py
+-rw-r--r--   0        0        0     3243 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/try_statement.py
+-rw-r--r--   0        0        0     2571 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/unchecked_block.py
+-rw-r--r--   0        0        0     4389 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/variable_declaration_statement.py
+-rw-r--r--   0        0        0     2661 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/statements/while_statement.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/type_names/__init__.py
+-rw-r--r--   0        0        0     5137 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/type_names/abc.py
+-rw-r--r--   0        0        0     4062 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/type_names/array_type_name.py
+-rw-r--r--   0        0        0     5924 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/type_names/elementary_type_name.py
+-rw-r--r--   0        0        0     3961 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/type_names/function_type_name.py
+-rw-r--r--   0        0        0     6502 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/type_names/mapping.py
+-rw-r--r--   0        0        0    11871 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/type_names/user_defined_type_name.py
+-rw-r--r--   0        0        0    61318 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/types.py
+-rw-r--r--   0        0        0      822 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/__init__.py
+-rw-r--r--   0        0        0     1718 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/abc.py
+-rw-r--r--   0        0        0     3025 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/assignment.py
+-rw-r--r--   0        0        0     4701 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/block.py
+-rw-r--r--   0        0        0     1007 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/break_statement.py
+-rw-r--r--   0        0        0     2453 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/case_.py
+-rw-r--r--   0        0        0     1064 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/continue_statement.py
+-rw-r--r--   0        0        0     1860 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/expression_statement.py
+-rw-r--r--   0        0        0     3256 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/for_loop.py
+-rw-r--r--   0        0        0     6392 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/function_call.py
+-rw-r--r--   0        0        0     3516 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/function_definition.py
+-rw-r--r--   0        0        0     2828 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/identifier.py
+-rw-r--r--   0        0        0     2731 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/if_statement.py
+-rw-r--r--   0        0        0     1266 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/leave.py
+-rw-r--r--   0        0        0     3619 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/literal.py
+-rw-r--r--   0        0        0     3147 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/switch.py
+-rw-r--r--   0        0        0     2198 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/typed_name.py
+-rw-r--r--   0        0        0     3235 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/ir/yul/variable_declaration.py
+-rw-r--r--   0        0        0       47 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/lsp/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-25 15:45:13.779084 eth_wake-4.9.0/wake/lsp/commands/__init__.py
+-rw-r--r--   0        0        0     3842 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/commands/generate_control_flow_graph.py
+-rw-r--r--   0        0        0     1123 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/commands/generate_imports_graph.py
+-rw-r--r--   0        0        0     4303 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/commands/generate_inheritance_graph.py
+-rw-r--r--   0        0        0     2291 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/commands/generate_linearized_inheritance_graph.py
+-rw-r--r--   0        0        0     4128 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/commands/init.py
+-rw-r--r--   0        0        0    31620 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/common_structures.py
+-rw-r--r--   0        0        0     2552 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/context.py
+-rw-r--r--   0        0        0     2574 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/document_sync.py
+-rw-r--r--   0        0        0      130 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/enums.py
+-rw-r--r--   0        0        0      471 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/__init__.py
+-rw-r--r--   0        0        0     6969 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/code_action.py
+-rw-r--r--   0        0        0    11750 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/code_lens.py
+-rw-r--r--   0        0        0    20068 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/completion.py
+-rw-r--r--   0        0        0    10182 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/definition.py
+-rw-r--r--   0        0        0     1472 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/diagnostic.py
+-rw-r--r--   0        0        0     4331 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/document_link.py
+-rw-r--r--   0        0        0     8062 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/document_symbol.py
+-rw-r--r--   0        0        0    18501 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/hover.py
+-rw-r--r--   0        0        0     3927 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/implementation.py
+-rw-r--r--   0        0        0     3525 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/inlay_hint.py
+-rw-r--r--   0        0        0     5115 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/references.py
+-rw-r--r--   0        0        0     8941 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/rename.py
+-rw-r--r--   0        0        0     9377 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/type_definition.py
+-rw-r--r--   0        0        0    11131 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/features/type_hierarchy.py
+-rw-r--r--   0        0        0      750 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/logging_handler.py
+-rw-r--r--   0        0        0    66919 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/lsp_compiler.py
+-rw-r--r--   0        0        0      328 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/lsp_data_model.py
+-rw-r--r--   0        0        0     8941 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/lsp_parser.py
+-rw-r--r--   0        0        0     5551 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/methods.py
+-rw-r--r--   0        0        0     1897 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/protocol_structures.py
+-rw-r--r--   0        0        0     2229 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/rpc_protocol.py
+-rw-r--r--   0        0        0    55986 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/server.py
+-rw-r--r--   0        0        0     6793 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/server_capabilities.py
+-rw-r--r--   0        0        0       86 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/utils/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/utils/position.py
+-rw-r--r--   0        0        0      459 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/lsp/utils/uri.py
+-rw-r--r--   0        0        0      102 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/migrations/__init__.py
+-rw-r--r--   0        0        0     9091 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/migrations/woke_wake_migration.py
+-rw-r--r--   0        0        0     3307 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/migrations/xdg_migration.py
+-rw-r--r--   0        0        0       74 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/printers/__init__.py
+-rw-r--r--   0        0        0    14954 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/printers/api.py
+-rw-r--r--   0        0        0      412 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/printers/template.py
+-rw-r--r--   0        0        0       50 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/regex_parser/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/regex_parser/solidity_import.py
+-rw-r--r--   0        0        0    10964 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/regex_parser/solidity_parser.py
+-rw-r--r--   0        0        0       36 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/svm/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/svm/abc.py
+-rw-r--r--   0        0        0      270 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/svm/exceptions.py
+-rw-r--r--   0        0        0    12254 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/svm/svm.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/templates/scripts/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/templates/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/templates/tests/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/templates/tests/test_default.py
+-rw-r--r--   0        0        0      861 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/testing/__init__.py
+-rw-r--r--   0        0        0    11222 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/testing/core.py
+-rw-r--r--   0        0        0    23995 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/testing/coverage.py
+-rw-r--r--   0        0        0      187 2024-04-25 15:45:13.783084 eth_wake-4.9.0/wake/testing/fuzzing/__init__.py
+-rw-r--r--   0        0        0     5028 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/testing/fuzzing/fuzz_test.py
+-rw-r--r--   0        0        0    10577 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/testing/fuzzing/fuzzer.py
+-rw-r--r--   0        0        0     5407 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/testing/fuzzing/generators.py
+-rw-r--r--   0        0        0     8240 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/testing/pytest_plugin_multiprocess.py
+-rw-r--r--   0        0        0    12967 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/testing/pytest_plugin_multiprocess_server.py
+-rw-r--r--   0        0        0     3057 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/testing/pytest_plugin_single.py
+-rw-r--r--   0        0        0      288 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/context_managers.py
+-rw-r--r--   0        0        0      975 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/decorators.py
+-rw-r--r--   0        0        0      158 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/enums.py
+-rw-r--r--   0        0        0     1699 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/file_utils.py
+-rw-r--r--   0        0        0      518 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/formatters.py
+-rw-r--r--   0        0        0      875 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/general.py
+-rw-r--r--   0        0        0      384 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/keyed_default_dict.py
+-rw-r--r--   0        0        0      194 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/networking.py
+-rw-r--r--   0        0        0     1569 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/null_file.py
+-rw-r--r--   0        0        0     1017 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/openzeppelin.py
+-rw-r--r--   0        0        0      630 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/string.py
+-rw-r--r--   0        0        0     1747 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/tee.py
+-rw-r--r--   0        0        0     3792 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/threaded_child_watcher.py
+-rw-r--r--   0        0        0      424 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake/utils/version.py
+-rw-r--r--   0        0        0     1296 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/__init__.py
+-rw-r--r--   0        0        0     3726 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/abi_encode_with_signature.py
+-rw-r--r--   0        0        0    15179 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/axelar_proxy_contract_id.py
+-rw-r--r--   0        0        0     5747 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/balance_relied_on.py
+-rw-r--r--   0        0        0     3197 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/call_options_not_called.py
+-rw-r--r--   0        0        0     9968 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py
+-rw-r--r--   0        0        0     2525 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/complex_struct_getter.py
+-rw-r--r--   0        0        0     3517 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/empty_byte_array_copy_bug.py
+-rw-r--r--   0        0        0    18811 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/incorrect_interface.py
+-rw-r--r--   0        0        0     4318 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/missing_return.py
+-rw-r--r--   0        0        0     4082 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/msg_value_nonpayable_function.py
+-rw-r--r--   0        0        0    11049 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/reentrancy.py
+-rw-r--r--   0        0        0     2364 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/struct_mapping_deletion.py
+-rw-r--r--   0        0        0     3590 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/tx_origin.py
+-rw-r--r--   0        0        0     4019 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unchecked_return_value.py
+-rw-r--r--   0        0        0     1681 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unprotected_selfdestruct.py
+-rw-r--r--   0        0        0     6655 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unsafe_delegatecall.py
+-rw-r--r--   0        0        0     2198 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unsafe_erc20_call.py
+-rw-r--r--   0        0        0     2225 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unused_contract.py
+-rw-r--r--   0        0        0     1790 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unused_function.py
+-rw-r--r--   0        0        0     2781 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unused_import.py
+-rw-r--r--   0        0        0     1520 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/unused_modifier.py
+-rw-r--r--   0        0        0      219 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_detectors/utils.py
+-rw-r--r--   0        0        0      462 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/__init__.py
+-rw-r--r--   0        0        0     3487 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/abi.py
+-rw-r--r--   0        0        0     3223 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/c3_linearization.py
+-rw-r--r--   0        0        0     4260 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/control_flow_graph.py
+-rw-r--r--   0        0        0     5435 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/imports_graph.py
+-rw-r--r--   0        0        0     6127 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/inheritance_graph.py
+-rw-r--r--   0        0        0     1574 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/inheritance_tree.py
+-rw-r--r--   0        0        0     5805 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/modifiers.py
+-rw-r--r--   0        0        0     5748 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/state_changes.py
+-rw-r--r--   0        0        0     3600 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/storage_layout.py
+-rw-r--r--   0        0        0     8131 2024-04-25 15:45:13.787084 eth_wake-4.9.0/wake_printers/tokens.py
+-rw-r--r--   0        0        0    12247 1970-01-01 00:00:00.000000 eth_wake-4.9.0/PKG-INFO
```

### Comparing `eth_wake-4.8.0/LICENSE` & `eth_wake-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/README.md` & `eth_wake-4.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
 ```shell
 pip3 install eth-wake
 ```
 
 ## Documentation & Contribution
 
-Wake documentation can be found [here](https://ackeeblockchain.com/wake/docs/latest).
+Wake documentation can be found [here](https://ackee.xyz/wake/docs/latest).
 
-There you can also find a section on [contributing](https://ackeeblockchain.com/wake/docs/latest/contributing/).
+There you can also find a section on [contributing](https://ackee.xyz/wake/docs/latest/contributing/).
 
 ## Discovered vulnerabilities
 
 | Vulnerability                                   | Severity | Project | Method           | Discovered by    | Resources                                                                                                                                                                                                                       |
 |-------------------------------------------------|----------|---------|------------------|------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Profit & loss accounted twice                   | Critical | IPOR    | Fuzz test        | Ackee Blockchain | [Report](https://github.com/Ackee-Blockchain/public-audit-reports/blob/master/2023/ackee-blockchain-ipor-protocol-report.pdf), [Wake tests](https://github.com/Ackee-Blockchain/tests-ipor/blob/main/tests/test_fuzz.py)        |
 | Console permanent denial of service             | High     | Brahma  | Fuzz test        | Ackee Blockchain | [Report](https://github.com/Ackee-Blockchain/public-audit-reports/blob/master/2023/ackee-blockchain-brahma-console-v2-report.pdf)                                                                                               |
@@ -52,15 +52,15 @@
 | Missing receive function                        | Medium   | Axelar  | Fuzz test        | Ackee Blockchain | [Wake tests](https://github.com/Ackee-Blockchain/tests-axelar-interchain-governance-executor/blob/main/tests/test_fuzz.py)                                                                                                      |
 | `SafeERC20` not used for `approve`              | Medium   | Lido    | Fuzz test        | Ackee Blockchain | [Wake tests](https://github.com/Ackee-Blockchain/tests-lido-stonks/blob/main/tests/test_fuzz.py)                                                                                                                                |
 
 ## Features
 
 ### Testing framework
 
-See [examples](https://github.com/Ackee-Blockchain/wake/tree/main/examples) and [documentation](https://ackeeblockchain.com/wake/docs/latest/testing-framework/overview) for more information.
+See [examples](https://github.com/Ackee-Blockchain/wake/tree/main/examples) and [documentation](https://ackee.xyz/wake/docs/latest/testing-framework/overview) for more information.
 
 Writing tests is as simple as:
 
 ```python
 from wake.testing import *
 from pytypes.contracts.Counter import Counter
 
@@ -119,28 +119,28 @@
 ```
 
 A specific detector can be run using:
 ```shell
 wake detect <detector-name>
 ```
 
-See the [documentation](https://ackeeblockchain.com/wake/docs/latest/static-analysis/using-detectors/) for a list of all detectors.
+See the [documentation](https://ackee.xyz/wake/docs/latest/static-analysis/using-detectors/) for a list of all detectors.
 
 ### Printers
 
 A specific printer can be run using:
 ```shell
 wake print <printer-name>
 ```
 
-See the [documentation](https://ackeeblockchain.com/wake/docs/latest/static-analysis/using-printers/) for a list of all printers.
+See the [documentation](https://ackee.xyz/wake/docs/latest/static-analysis/using-printers/) for a list of all printers.
 
 ### Custom detectors & printers
 
-Refer to the [getting started](https://ackeeblockchain.com/wake/docs/latest/static-analysis/getting-started/) guide for more information.
+Refer to the [getting started](https://ackee.xyz/wake/docs/latest/static-analysis/getting-started/) guide for more information.
 Also check out [wake_detectors](https://github.com/Ackee-Blockchain/wake/tree/main/wake_detectors) and [wake_printers](https://github.com/Ackee-Blockchain/wake/tree/main/wake_printers) for the implementation of built-in detectors and printers.
 
 ### LSP server
 
 Wake implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.
 
 Wake LSP server can be run using:
@@ -151,15 +151,15 @@
 
 Or with an optional --port argument (default 65432):
 
 ```shell
 wake lsp --port 1234
 ```
 
-All LSP server features can be found in the [documentation](https://ackeeblockchain.com/wake/docs/latest/language-server/).
+All LSP server features can be found in the [documentation](https://ackee.xyz/wake/docs/latest/language-server/).
 
 ## License
 
 This project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/wake/blob/main/LICENSE).
 
 ## Partners
```

### Comparing `eth_wake-4.8.0/examples/counter/contracts/Counter.sol` & `eth_wake-4.9.0/examples/counter/contracts/Counter.sol`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/examples/counter/contracts/Gateway.sol` & `eth_wake-4.9.0/examples/counter/contracts/Gateway.sol`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/examples/counter/package-lock.json` & `eth_wake-4.9.0/examples/counter/package-lock.json`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/examples/counter/tests/test_counter.py` & `eth_wake-4.9.0/examples/counter/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz.py` & `eth_wake-4.9.0/examples/counter/tests/test_counter_fuzz.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/examples/counter/tests/test_counter_fuzz_failing.py` & `eth_wake-4.9.0/examples/counter/tests/test_counter_fuzz_failing.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/examples/counter/tests/test_crosschain.py` & `eth_wake-4.9.0/examples/counter/tests/test_crosschain.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/pyproject.toml` & `eth_wake-4.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "eth-wake"
-version = "4.8.0"
+version = "4.9.0"
 description = "Wake is a Python-based Solidity development and testing framework with built-in vulnerability detectors."
 license = "ISC"
 authors = ["Ackee Blockchain"]
 readme = "README.md"
 homepage = "https://getwake.io"
 repository = "https://github.com/Ackee-Blockchain/wake"
-documentation = "https://ackeeblockchain.com/wake/docs/latest"
+documentation = "https://ackee.xyz/wake/docs/latest"
 keywords = ["ethereum", "solidity", "security", "testing", "development", "static analysis", "framework", "audit"]
 packages = [
     { include = "wake" },
     { include = "wake_detectors" },
     { include = "wake_printers" }
 ]
 include = [
```

### Comparing `eth_wake-4.8.0/wake/analysis/cfg.py` & `eth_wake-4.9.0/wake/analysis/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,44 +240,44 @@
 
     def is_reachable(
         self,
         start: Union[StatementAbc, YulStatementAbc],
         end: Union[StatementAbc, YulStatementAbc],
     ) -> bool:
         """
+        Returns False for `start == end` unless there is a loop in the CFG containing `start`.
+
         Args:
             start: Statement that is expected to be executed before `end`.
             end: Statement that is expected to be executed after `start`.
 
         Returns:
             True if there is an execution path from `start` to `end` in this CFG, False otherwise.
         """
         start_node = self._statements_lookup[start]
         end_node = self._statements_lookup[end]
         if start_node == end_node:
-            if start == start_node.control_statement:
-                if end == start_node.control_statement:
-                    return True
-                try:
-                    nx.find_cycle(self._graph, start_node)
-                    return True
-                except nx.NetworkXNoCycle:
-                    return False
-            if end == end_node.control_statement:
+            start_index = (
+                start_node.statements.index(start)
+                if start != start_node.control_statement
+                else len(start_node.statements)
+            )
+            end_index = (
+                end_node.statements.index(end)
+                if end != end_node.control_statement
+                else len(end_node.statements)
+            )
+            if start_index < end_index:
                 return True
 
-            start_index = start_node.statements.index(start)
-            end_index = end_node.statements.index(end)
-            if start_index <= end_index:  # also EQUAL?
-                return True
-            try:
-                nx.find_cycle(self._graph, start_node)
-                return True
-            except nx.NetworkXNoCycle:
-                return False
+            for _, to in nx.edge_dfs(self._graph, start_node):
+                if to == end_node:
+                    return True
+
+            return False
         else:
             return nx.has_path(self._graph, start_node, end_node)
 
 
 def _normalize(
     graph: nx.DiGraph, start: CfgNode, success_end: CfgNode, revert_end: CfgNode
 ) -> bool:
```

### Comparing `eth_wake-4.8.0/wake/analysis/expressions.py` & `eth_wake-4.9.0/wake/analysis/expressions.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/analysis/graph.py` & `eth_wake-4.9.0/wake/analysis/graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/analysis/interface.py` & `eth_wake-4.9.0/wake/analysis/interface.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/analysis/ownable.py` & `eth_wake-4.9.0/wake/analysis/ownable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from collections import deque
-from typing import Optional, Set, Tuple, Union
+from typing import FrozenSet, Optional, Set, Tuple, Union
 
 import wake.ir.types as types
 from wake.analysis.cfg import CfgNode, ControlFlowGraph, TransitionConditionKind
 from wake.analysis.utils import pair_function_call_arguments
 from wake.core import get_logger
 from wake.ir import (
     Assignment,
@@ -40,17 +40,18 @@
     expression_is_global_symbol,
     get_variable_declarations_from_expression,
 )
 
 logger = get_logger(__name__)
 
 
+@return_on_recursion(False)
 def expression_is_only_owner(
     expression: ExpressionAbc,
-    msg_sender_variables: Set[VariableDeclaration],
+    msg_sender_variables: FrozenSet[VariableDeclaration],
     check_only_eoa: bool = False,
     inverted: bool = False,
 ) -> bool:
     if isinstance(expression, BinaryOperation):
         if expression.operator in {BinaryOpOperator.EQ, BinaryOpOperator.NEQ}:
             left = get_variable_declarations_from_expression(expression.left_expression)
             right = get_variable_declarations_from_expression(
@@ -151,15 +152,15 @@
             returns = []
             for statement in func.body.statements_iter():
                 if isinstance(statement, Return):
                     returns.append(statement)
             if len(returns) > 0 and all(
                 expression_is_only_owner(
                     return_.expression,
-                    sender_variables,
+                    frozenset(sender_variables),
                     check_only_eoa=check_only_eoa,
                     inverted=inverted,
                 )
                 for return_ in returns
                 if return_.expression is not None
             ):
                 logger.debug(f"Expression is only owner: {expression.source}")
@@ -303,24 +304,24 @@
                 if (
                     (condition[0] == TransitionConditionKind.NEVER)
                     or (
                         condition[0] == TransitionConditionKind.IS_TRUE
                         and condition[1] is not None
                         and expression_is_only_owner(
                             condition[1],  # pyright: ignore reportGeneralTypeIssues
-                            set(),
+                            frozenset(),
                             check_only_eoa=check_only_eoa,
                         )
                     )
                     or (
                         condition[0] == TransitionConditionKind.IS_FALSE
                         and condition[1] is not None
                         and expression_is_only_owner(
                             condition[1],  # pyright: ignore reportGeneralTypeIssues
-                            set(),
+                            frozenset(),
                             check_only_eoa=check_only_eoa,
                             inverted=True,
                         )
                     )
                 ):
                     continue
```

### Comparing `eth_wake-4.8.0/wake/analysis/proxy.py` & `eth_wake-4.9.0/wake/analysis/proxy.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/analysis/utils.py` & `eth_wake-4.9.0/wake/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/__main__.py` & `eth_wake-4.9.0/wake/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/accounts.py` & `eth_wake-4.9.0/wake/cli/accounts.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/compile.py` & `eth_wake-4.9.0/wake/cli/compile.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/detect.py` & `eth_wake-4.9.0/wake/cli/detect.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/init.py` & `eth_wake-4.9.0/wake/cli/init.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/lsp.py` & `eth_wake-4.9.0/wake/cli/lsp.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/open.py` & `eth_wake-4.9.0/wake/cli/open.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/param_types.py` & `eth_wake-4.9.0/wake/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/print.py` & `eth_wake-4.9.0/wake/cli/print.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/run.py` & `eth_wake-4.9.0/wake/cli/run.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/svm.py` & `eth_wake-4.9.0/wake/cli/svm.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/cli/test.py` & `eth_wake-4.9.0/wake/cli/test.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/build_data_model.py` & `eth_wake-4.9.0/wake/compiler/build_data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/compilation_unit.py` & `eth_wake-4.9.0/wake/compiler/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/compiler.py` & `eth_wake-4.9.0/wake/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/solc_frontend/input_data_model.py` & `eth_wake-4.9.0/wake/compiler/solc_frontend/input_data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/solc_frontend/output_data_model.py` & `eth_wake-4.9.0/wake/compiler/solc_frontend/output_data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/solc_frontend/solc_runner.py` & `eth_wake-4.9.0/wake/compiler/solc_frontend/solc_runner.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/source_path_resolver.py` & `eth_wake-4.9.0/wake/compiler/source_path_resolver.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/compiler/source_unit_name_resolver.py` & `eth_wake-4.9.0/wake/compiler/source_unit_name_resolver.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/config/__init__.py` & `eth_wake-4.9.0/wake/config/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/config/data_model.py` & `eth_wake-4.9.0/wake/config/data_model.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/config/wake_config.py` & `eth_wake-4.9.0/wake/config/wake_config.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/contracts/wake/console.sol` & `eth_wake-4.9.0/wake/contracts/wake/console.sol`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/core/logging.py` & `eth_wake-4.9.0/wake/core/logging.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/core/lsp_provider.py` & `eth_wake-4.9.0/wake/core/lsp_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,17 +237,17 @@
 
     def add_hover(self, node: ir.IrAbc, text: str, *, on_child: bool = False) -> None:
         self._hovers[node.source_unit.file][node.byte_location].add(
             HoverOptions(text, on_child)
         )
 
     def add_hover_from_offsets(
-        self, path: Path, start: int, end: int, text: str, *, on_child: bool = False
+        self, path: Path, start: int, end: int, text: str,
     ) -> None:
-        self._hovers[path][(start, end)].add(HoverOptions(text, on_child))
+        self._hovers[path][(start, end)].add(HoverOptions(text, True))
 
     def add_code_lens(
         self,
         node: ir.IrAbc,
         title: str,
         *,
         on_click: Optional[Callable[[], None]] = None,
```

### Comparing `eth_wake-4.8.0/wake/core/solidity_version.py` & `eth_wake-4.9.0/wake/core/solidity_version.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/core/visitor.py` & `eth_wake-4.9.0/wake/core/visitor.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/core/wake_comments.py` & `eth_wake-4.9.0/wake/core/wake_comments.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/deployment/__init__.py` & `eth_wake-4.9.0/wake/deployment/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,7 +23,9 @@
     get_create_address,
     get_logic_contract,
     keccak256,
     read_storage_variable,
 )
 
 from .core import Chain, default_chain
+
+chain = default_chain
```

### Comparing `eth_wake-4.8.0/wake/deployment/core.py` & `eth_wake-4.9.0/wake/deployment/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
         self._snapshots[snapshot_id] = {
             "nonces": self._nonces.copy(),
             "accounts": self._accounts.copy(),
             "default_call_account": self._default_call_account,
             "default_tx_account": self._default_tx_account,
             "txs": dict(self._txs._transactions),
+            "tx_hashes": list(self._txs._tx_hashes),
             "blocks": dict(self._blocks._blocks),
         }
         return snapshot_id
 
     @check_connected
     def revert(self, snapshot_id: str) -> None:
         reverted = self._chain_interface.revert(snapshot_id)
@@ -101,14 +102,15 @@
 
         snapshot = self._snapshots[snapshot_id]
         self._nonces = snapshot["nonces"]
         self._accounts = snapshot["accounts"]
         self._default_call_account = snapshot["default_call_account"]
         self._default_tx_account = snapshot["default_tx_account"]
         self._txs._transactions = snapshot["txs"]
+        self._txs._tx_hashes = snapshot["tx_hashes"]
         self._blocks._blocks = snapshot["blocks"]
         del self._snapshots[snapshot_id]
 
     @property
     @check_connected
     def block_gas_limit(self) -> int:
         return self._blocks["pending"].gas_limit
```

### Comparing `eth_wake-4.8.0/wake/detectors/api.py` & `eth_wake-4.9.0/wake/detectors/api.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/detectors/template.py` & `eth_wake-4.9.0/wake/detectors/template.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/detectors/utils.py` & `eth_wake-4.9.0/wake/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/blocks.py` & `eth_wake-4.9.0/wake/development/blocks.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/call_trace.py` & `eth_wake-4.9.0/wake/development/call_trace.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/chain_interfaces.py` & `eth_wake-4.9.0/wake/development/chain_interfaces.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/constants.py` & `eth_wake-4.9.0/wake/development/constants.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/core.py` & `eth_wake-4.9.0/wake/development/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     Union,
     cast,
+    overload,
 )
 from urllib.error import HTTPError
 
 import eth_abi
 import eth_abi.abi
 import eth_abi.grammar
 import eth_abi.packed
@@ -75,14 +76,15 @@
     FixedSizeBytes,
     FixedSizeList,
     Integer,
     fixed_bytes_map,
     fixed_list_map,
     int_map,
     uint_map,
+    uint256,
 )
 
 if TYPE_CHECKING:
     from .transactions import (
         ChainTransactions,
         TransactionAbc,
         TransactionRevertedError,
@@ -1676,16 +1678,16 @@
     @property
     @check_connected
     def chain_interface(self) -> ChainInterfaceAbc:
         return self._chain_interface
 
     @property
     @check_connected
-    def chain_id(self) -> int:
-        return self._chain_id
+    def chain_id(self) -> uint256:
+        return uint256(self._chain_id)
 
     @property
     @check_connected
     def accounts(self) -> Tuple[Account, ...]:
         return tuple(self._accounts)
 
     @property
@@ -1905,14 +1907,181 @@
                 exception_handler = get_exception_handler()
                 if exception_handler is not None:
                     exception_handler(*sys.exc_info())
                 raise
         finally:
             self.revert(snapshot_id)
 
+    @overload
+    def deploy(
+        self,
+        creation_code: bytes,
+        *,
+        request_type: Literal["call"],
+        return_tx: Literal[False] = False,
+        from_: Optional[Union[Account, Address, str]] = None,
+        value: Union[int, str] = 0,
+        gas_limit: Optional[Union[int, Literal["max", "auto"]]] = None,
+        gas_price: Optional[Union[int, str]] = None,
+        max_fee_per_gas: Optional[Union[int, str]] = None,
+        max_priority_fee_per_gas: Optional[Union[int, str]] = None,
+        access_list: Optional[
+            Union[Dict[Union[Account, Address, str], List[int]], Literal["auto"]]
+        ] = None,
+        type: Optional[int] = None,
+        block: Optional[
+            Union[int, Literal["latest", "pending", "earliest", "safe", "finalized"]]
+        ] = None,
+        confirmations: Optional[int] = None,
+    ) -> bytearray:
+        ...
+
+    @overload
+    def deploy(
+        self,
+        creation_code: bytes,
+        *,
+        request_type: Literal["tx"] = "tx",
+        return_tx: Literal[False] = False,
+        from_: Optional[Union[Account, Address, str]] = None,
+        value: Union[int, str] = 0,
+        gas_limit: Optional[Union[int, Literal["max", "auto"]]] = None,
+        gas_price: Optional[Union[int, str]] = None,
+        max_fee_per_gas: Optional[Union[int, str]] = None,
+        max_priority_fee_per_gas: Optional[Union[int, str]] = None,
+        access_list: Optional[
+            Union[Dict[Union[Account, Address, str], List[int]], Literal["auto"]]
+        ] = None,
+        type: Optional[int] = None,
+        block: Optional[
+            Union[int, Literal["latest", "pending", "earliest", "safe", "finalized"]]
+        ] = None,
+        confirmations: Optional[int] = None,
+    ) -> Contract:
+        ...
+
+    @overload
+    def deploy(
+        self,
+        creation_code: bytes,
+        *,
+        request_type: Literal["estimate"],
+        return_tx: Literal[False] = False,
+        from_: Optional[Union[Account, Address, str]] = None,
+        value: Union[int, str] = 0,
+        gas_limit: Optional[Union[int, Literal["max", "auto"]]] = None,
+        gas_price: Optional[Union[int, str]] = None,
+        max_fee_per_gas: Optional[Union[int, str]] = None,
+        max_priority_fee_per_gas: Optional[Union[int, str]] = None,
+        access_list: Optional[
+            Union[Dict[Union[Account, Address, str], List[int]], Literal["auto"]]
+        ] = None,
+        type: Optional[int] = None,
+        block: Optional[
+            Union[int, Literal["latest", "pending", "earliest", "safe", "finalized"]]
+        ] = None,
+        confirmations: Optional[int] = None,
+    ) -> int:
+        ...
+
+    @overload
+    def deploy(
+        self,
+        creation_code: bytes,
+        *,
+        request_type: Literal["access_list"],
+        return_tx: Literal[False] = False,
+        from_: Optional[Union[Account, Address, str]] = None,
+        value: Union[int, str] = 0,
+        gas_limit: Optional[Union[int, Literal["max", "auto"]]] = None,
+        gas_price: Optional[Union[int, str]] = None,
+        max_fee_per_gas: Optional[Union[int, str]] = None,
+        max_priority_fee_per_gas: Optional[Union[int, str]] = None,
+        access_list: Optional[
+            Union[Dict[Union[Account, Address, str], List[int]], Literal["auto"]]
+        ] = None,
+        type: Optional[int] = None,
+        block: Optional[
+            Union[int, Literal["latest", "pending", "earliest", "safe", "finalized"]]
+        ] = None,
+        confirmations: Optional[int] = None,
+    ) -> Tuple[Dict[Address, List[int]], int]:
+        ...
+
+    @overload
+    def deploy(
+        self,
+        creation_code: bytes,
+        *,
+        request_type: Literal["tx"] = "tx",
+        return_tx: Literal[True],
+        from_: Optional[Union[Account, Address, str]] = None,
+        value: Union[int, str] = 0,
+        gas_limit: Optional[Union[int, Literal["max", "auto"]]] = None,
+        gas_price: Optional[Union[int, str]] = None,
+        max_fee_per_gas: Optional[Union[int, str]] = None,
+        max_priority_fee_per_gas: Optional[Union[int, str]] = None,
+        access_list: Optional[
+            Union[Dict[Union[Account, Address, str], List[int]], Literal["auto"]]
+        ] = None,
+        type: Optional[int] = None,
+        block: Optional[
+            Union[int, Literal["latest", "pending", "earliest", "safe", "finalized"]]
+        ] = None,
+        confirmations: Optional[int] = None,
+    ) -> TransactionAbc[Contract]:
+        ...
+
+    def deploy(
+        self,
+        creation_code: bytes,
+        *,
+        request_type: RequestType = "tx",
+        return_tx: bool = False,
+        from_: Optional[Union[Account, Address, str]] = None,
+        value: Union[int, str] = 0,
+        gas_limit: Optional[Union[int, Literal["max", "auto"]]] = None,
+        gas_price: Optional[Union[int, str]] = None,
+        max_fee_per_gas: Optional[Union[int, str]] = None,
+        max_priority_fee_per_gas: Optional[Union[int, str]] = None,
+        access_list: Optional[
+            Union[Dict[Union[Account, Address, str], List[int]], Literal["auto"]]
+        ] = None,
+        type: Optional[int] = None,
+        block: Optional[
+            Union[int, Literal["latest", "pending", "earliest", "safe", "finalized"]]
+        ] = None,
+        confirmations: Optional[int] = None,
+    ) -> Union[
+        bytearray,
+        Contract,
+        int,
+        Tuple[Dict[Address, List[int]], int],
+        TransactionAbc[Contract],
+    ]:
+        return Contract._execute(
+            self,
+            request_type,
+            creation_code.hex(),
+            [],
+            return_tx,
+            Contract,
+            from_,
+            None,
+            value,
+            gas_limit,
+            gas_price,
+            max_fee_per_gas,
+            max_priority_fee_per_gas,
+            access_list,
+            type,
+            block,
+            confirmations,
+        )
+
     def _update_nonce(self, address: Address, nonce: int) -> None:
         self._nonces[address] = nonce
 
     def _convert_to_web3_type(self, value: Any) -> Any:
         if dataclasses.is_dataclass(value):
             return tuple(
                 self._convert_to_web3_type(getattr(value, f.name))
@@ -2386,14 +2555,17 @@
                         tx_hash = self._chain_interface.send_transaction(tx_params)
                     except (ValueError, JsonRpcError) as e:
                         try:
                             tx_hash = e.args[0]["data"]["txHash"]
                         except Exception:
                             raise e
                     self._update_nonce(sender.address, tx_params["nonce"] + 1)
+
+        self._txs.register_tx(tx_hash)
+
         return tx_hash
 
     @check_connected
     def _call(
         self,
         abi: Optional[Dict],
         arguments: Iterable,
@@ -3063,15 +3235,19 @@
 
         if type is not None:
             params["type"] = type
 
         params["data"] = bytes.fromhex(data)
 
         if to is None:
-            abi = cls._abi["constructor"] if "constructor" in cls._abi else None
+            abi = (
+                cls._abi["constructor"]
+                if hasattr(cls, "_abi") and "constructor" in cls._abi
+                else None
+            )
         else:
             abi = cls._abi[params["data"]]
 
         if request_type == RequestType.TX:
             return chain._transact(
                 abi,
                 arguments,
```

### Comparing `eth_wake-4.8.0/wake/development/globals.py` & `eth_wake-4.9.0/wake/development/globals.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/hardhat_console.py` & `eth_wake-4.9.0/wake/development/hardhat_console.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/internal.py` & `eth_wake-4.9.0/wake/development/internal.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/json_rpc/communicator.py` & `eth_wake-4.9.0/wake/development/json_rpc/communicator.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/json_rpc/http.py` & `eth_wake-4.9.0/wake/development/json_rpc/http.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/json_rpc/ipc.py` & `eth_wake-4.9.0/wake/development/json_rpc/ipc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/json_rpc/websocket.py` & `eth_wake-4.9.0/wake/development/json_rpc/websocket.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/primitive_types.py` & `eth_wake-4.9.0/wake/development/primitive_types.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/development/pytypes_generator.py` & `eth_wake-4.9.0/wake/development/pytypes_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2125,20 +2125,44 @@
     def _check_global(self, name: str) -> bool:
         return (
             name in self.__global_reserved
             or name in set(self.__global_renames.values())
             or keyword.iskeyword(name)
         )
 
-    def _check_contract(self, name: str, contract: ContractDefinition) -> bool:
+    def _check_contract(
+        self, name: str, selector: Optional[bytes], contract: ContractDefinition
+    ) -> bool:
+        occupied = False
+        for c in contract.linearized_base_contracts:
+            same_name = [k for k, v in self.__contract_renames[c].items() if v == name]
+            if selector is None and len(same_name) > 0:
+                occupied = True
+            else:
+                for declaration in same_name:
+                    if isinstance(declaration, FunctionDefinition):
+                        if declaration.function_selector != selector:
+                            occupied = True
+                            break
+                    elif isinstance(declaration, VariableDeclaration):
+                        if declaration.function_selector != selector:
+                            occupied = True
+                            break
+                    else:
+                        occupied = True
+                        break
+
+            if occupied:
+                break
+
         return (
             name in self.__global_reserved
             or name in set(self.__global_renames)
             or name in self.__contract_reserved
-            or name in set(self.__contract_renames[contract].values())
+            or occupied
             or keyword.iskeyword(name)
             or (
                 name.startswith("__")
                 and name.endswith("__")
                 and not name.endswith("___")
             )
         )
@@ -2213,15 +2237,17 @@
 
     def sanitize_name(self, declaration: DeclarationAbc) -> str:
         parent = declaration.parent
         if isinstance(parent, SourceUnit):
             check = self._check_global
             renames = self.__global_renames
         elif isinstance(parent, ContractDefinition):
-            check = lambda name: self._check_contract(name, parent)
+            check = lambda name: self._check_contract(
+                name, getattr(declaration, "function_selector", None), parent
+            )
             renames = self.__contract_renames[parent]
         elif isinstance(parent, StructDefinition):
             check = lambda name: self._check_struct(name, parent)
             renames = self.__struct_renames[parent]
         elif isinstance(parent, EnumDefinition):
             check = lambda name: self._check_enum(name, parent)
             renames = self.__enum_renames[parent]
```

### Comparing `eth_wake-4.8.0/wake/development/transactions.py` & `eth_wake-4.9.0/wake/development/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,20 +83,25 @@
 
     return wrapper
 
 
 class ChainTransactions:
     _chain: Chain
     _transactions: Dict[str, TransactionAbc]
+    _tx_hashes: List[str]
 
     def __init__(self, chain: Chain):
         self._chain = chain
         self._transactions = {}
+        self._tx_hashes = []
+
+    def __getitem__(self, key: Union[str, int]) -> TransactionAbc:
+        if isinstance(key, int):
+            key = self._tx_hashes[key]
 
-    def __getitem__(self, key: str) -> TransactionAbc:
         if not key.startswith("0x"):
             key = "0x" + key
         key = key.lower()
         if key in self._transactions:
             return self._transactions[key]
 
         tx_data = self._chain.chain_interface.get_transaction(key)
@@ -175,14 +180,17 @@
             tx = Eip1559Transaction(key, tx_params, abi, return_type, self._chain)
         else:
             raise ValueError(f"Unknown transaction type {type}")
 
         self._transactions[key] = tx
         return tx
 
+    def register_tx(self, tx_hash: str):
+        self._tx_hashes.append(tx_hash)
+
 
 class TransactionAbc(ABC, Generic[T]):
     _tx_hash: str
     _tx_params: TxParams
     _chain: Chain
     _abi: Optional[Dict]
     _return_type: Type
```

### Comparing `eth_wake-4.8.0/wake/development/utils.py` & `eth_wake-4.9.0/wake/development/utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/__init__.py` & `eth_wake-4.9.0/wake/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/abc.py` & `eth_wake-4.9.0/wake/ir/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/ast.py` & `eth_wake-4.9.0/wake/ir/ast.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/declarations/abc.py` & `eth_wake-4.9.0/wake/ir/declarations/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/declarations/contract_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/contract_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from functools import lru_cache, partial
 from typing import TYPE_CHECKING, FrozenSet, Iterator, List, Optional, Set, Tuple, Union
 
+from ...regex_parser import SoliditySourceParser
 from ..abc import IrAbc
 from ..meta.inheritance_specifier import InheritanceSpecifier
 from ..meta.using_for_directive import UsingForDirective
 from ..reference_resolver import CallbackParams
 from .abc import DeclarationAbc
 
 if TYPE_CHECKING:
@@ -264,27 +266,40 @@
         )
         LIBRARY_RE = re.compile(
             r"^\s*library\s+(?P<name>{identifier})".format(
                 identifier=IDENTIFIER
             ).encode("utf-8")
         )
 
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
         if self.kind == ContractKind.CONTRACT:
-            match = CONTRACT_RE.match(self._source)
+            match = CONTRACT_RE.match(source)
         elif self.kind == ContractKind.INTERFACE:
-            match = INTERFACE_RE.match(self._source)
+            match = INTERFACE_RE.match(source)
         elif self.kind == ContractKind.LIBRARY:
-            match = LIBRARY_RE.match(self._source)
+            match = LIBRARY_RE.match(source)
         else:
             raise ValueError(f"Unknown contract kind: {self.kind}")
         assert match
 
-        return self.byte_location[0] + match.start("name"), self.byte_location[
-            0
-        ] + match.end("name")
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            self.byte_location[0] + match.start("name") + stripped,
+            self.byte_location[0] + match.end("name") + stripped,
+        )
 
     @property
     def parent(self) -> SourceUnit:
         """
         Returns:
             Parent IR node.
         """
```

### Comparing `eth_wake-4.8.0/wake/ir/declarations/enum_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/enum_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import logging
 import re
+from bisect import bisect
 from functools import lru_cache
 from typing import TYPE_CHECKING, FrozenSet, Iterator, List, Optional, Tuple, Union
 
 from wake.core import get_logger
 from wake.ir.ast import SolcEnumDefinition
 
+from ...regex_parser import SoliditySourceParser
 from ..abc import IrAbc, SolidityAbc
 from ..meta.structured_documentation import StructuredDocumentation
 from ..utils import IrInitTuple
 from .abc import DeclarationAbc
 from .enum_value import EnumValue
 
 if TYPE_CHECKING:
@@ -66,18 +68,34 @@
         IDENTIFIER = r"[a-zA-Z$_][a-zA-Z0-9$_]*"
         ENUM_RE = re.compile(
             r"^\s*enum\s+(?P<name>{identifier})".format(identifier=IDENTIFIER).encode(
                 "utf-8"
             )
         )
 
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
         byte_start = self._ast_node.src.byte_offset
-        match = ENUM_RE.match(self._source)
+        match = ENUM_RE.match(source)
         assert match
-        return byte_start + match.start("name"), byte_start + match.end("name")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            byte_start + match.start("name") + stripped,
+            byte_start + match.end("name") + stripped,
+        )
 
     @property
     def parent(self) -> Union[SourceUnit, ContractDefinition]:
         """
         Returns:
             Parent IR node.
         """
```

### Comparing `eth_wake-4.8.0/wake/ir/declarations/enum_value.py` & `eth_wake-4.9.0/wake/ir/declarations/enum_value.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/declarations/error_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/error_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/declarations/event_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/event_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from functools import lru_cache
 from typing import TYPE_CHECKING, FrozenSet, Iterator, Optional, Set, Tuple, Union
 
 from Crypto.Hash import keccak
 
+from ...regex_parser import SoliditySourceParser
 from .abc import DeclarationAbc
 
 if TYPE_CHECKING:
     from .contract_definition import ContractDefinition
     from ..expressions.identifier import Identifier
     from ..expressions.member_access import MemberAccess
     from ..meta.source_unit import SourceUnit
@@ -75,18 +77,34 @@
         IDENTIFIER = r"[a-zA-Z$_][a-zA-Z0-9$_]*"
         EVENT_RE = re.compile(
             r"^\s*event\s+(?P<name>{identifier})".format(identifier=IDENTIFIER).encode(
                 "utf-8"
             )
         )
 
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
         byte_start = self._ast_node.src.byte_offset
-        match = EVENT_RE.match(self._source)
+        match = EVENT_RE.match(source)
         assert match
-        return byte_start + match.start("name"), byte_start + match.end("name")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            byte_start + match.start("name") + stripped,
+            byte_start + match.end("name") + stripped,
+        )
 
     @property
     def parent(self) -> Union[ContractDefinition, SourceUnit]:
         """
         Returns:
             Parent IR node.
         """
```

### Comparing `eth_wake-4.8.0/wake/ir/declarations/function_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/function_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from collections import deque
 from functools import lru_cache, partial
 from typing import (
     TYPE_CHECKING,
     Deque,
     FrozenSet,
     Iterator,
     List,
     Optional,
     Set,
     Tuple,
     Union,
 )
 
+from ...regex_parser import SoliditySourceParser
 from ..meta.modifier_invocation import ModifierInvocation
 from ..meta.override_specifier import OverrideSpecifier
 from ..reference_resolver import CallbackParams
 from ..statements.block import Block
 from .abc import DeclarationAbc
 
 if TYPE_CHECKING:
@@ -201,21 +203,37 @@
                 identifier=IDENTIFIER
             ).encode("utf-8")
         )
         CONSTRUCTOR_RE = re.compile(r"^\s*(?P<name>constructor)".encode("utf-8"))
         FALLBACK_RE = re.compile(r"^\s*(?P<name>fallback)".encode("utf-8"))
         RECEIVE_RE = re.compile(r"^\s*(?P<name>receive)".encode("utf-8"))
 
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
         regexps = [FUNCTION_RE, CONSTRUCTOR_RE, FALLBACK_RE, RECEIVE_RE]
-        matches = [regexp.match(self._source) for regexp in regexps]
+        matches = [regexp.match(source) for regexp in regexps]
         assert any(matches)
 
         byte_start = self._ast_node.src.byte_offset
         match = next(match for match in matches if match)
-        return byte_start + match.start("name"), byte_start + match.end("name")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            byte_start + match.start("name") + stripped,
+            byte_start + match.end("name") + stripped,
+        )
 
     def get_all_references(
         self, include_declarations: bool
     ) -> Iterator[
         Union[
             DeclarationAbc,
             Identifier,
```

### Comparing `eth_wake-4.8.0/wake/ir/declarations/modifier_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/modifier_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from collections import deque
 from functools import lru_cache, partial
 from typing import (
     TYPE_CHECKING,
     Deque,
     FrozenSet,
     Iterator,
     List,
     Optional,
     Set,
     Tuple,
     Union,
 )
 
+from ...regex_parser import SoliditySourceParser
 from ..meta.override_specifier import OverrideSpecifier
 from ..reference_resolver import CallbackParams
 from ..statements.block import Block
 from .abc import DeclarationAbc
 
 if TYPE_CHECKING:
     from wake.analysis.cfg import ControlFlowGraph
@@ -123,18 +125,34 @@
         IDENTIFIER = r"[a-zA-Z$_][a-zA-Z0-9$_]*"
         MODIFIER_RE = re.compile(
             r"^\s*modifier\s+(?P<name>{identifier})".format(
                 identifier=IDENTIFIER
             ).encode("utf-8")
         )
 
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
         byte_start = self._ast_node.src.byte_offset
-        match = MODIFIER_RE.match(self._source)
+        match = MODIFIER_RE.match(source)
         assert match
-        return byte_start + match.start("name"), byte_start + match.end("name")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            byte_start + match.start("name") + stripped,
+            byte_start + match.end("name") + stripped,
+        )
 
     def get_all_references(
         self, include_declarations: bool
     ) -> Iterator[
         Union[
             DeclarationAbc,
             Identifier,
```

### Comparing `eth_wake-4.8.0/wake/ir/declarations/struct_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/struct_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from functools import lru_cache
 from typing import TYPE_CHECKING, FrozenSet, Iterator, List, Optional, Tuple, Union
 
+from ...regex_parser import SoliditySourceParser
 from ..meta.structured_documentation import StructuredDocumentation
 from .abc import DeclarationAbc
 
 if TYPE_CHECKING:
     from .contract_definition import ContractDefinition
     from ..expressions.identifier import Identifier
     from ..expressions.member_access import MemberAccess
@@ -71,18 +73,34 @@
         IDENTIFIER = r"[a-zA-Z$_][a-zA-Z0-9$_]*"
         STRUCT_RE = re.compile(
             r"^\s*struct\s+(?P<name>{identifier})".format(identifier=IDENTIFIER).encode(
                 "utf-8"
             )
         )
 
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
         byte_start = self._ast_node.src.byte_offset
-        match = STRUCT_RE.match(self._source)
+        match = STRUCT_RE.match(source)
         assert match
-        return byte_start + match.start("name"), byte_start + match.end("name")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            byte_start + match.start("name") + stripped,
+            byte_start + match.end("name") + stripped,
+        )
 
     @property
     def parent(self) -> Union[ContractDefinition, SourceUnit]:
         """
         Returns:
             Parent IR node.
         """
```

### Comparing `eth_wake-4.8.0/wake/ir/declarations/user_defined_value_type_definition.py` & `eth_wake-4.9.0/wake/ir/declarations/user_defined_value_type_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from functools import lru_cache
 from typing import TYPE_CHECKING, FrozenSet, Iterator, Tuple, Union
 
+from ...regex_parser import SoliditySourceParser
 from ..type_names.elementary_type_name import ElementaryTypeName
 from .abc import DeclarationAbc
 
 if TYPE_CHECKING:
     from .contract_definition import ContractDefinition
     from ..expressions.identifier import Identifier
     from ..expressions.member_access import MemberAccess
@@ -53,18 +55,34 @@
         IDENTIFIER = r"[a-zA-Z$_][a-zA-Z0-9$_]*"
         USER_DEF_VAL_TYPE_RE = re.compile(
             r"^\s*type\s+(?P<name>{identifier})".format(identifier=IDENTIFIER).encode(
                 "utf-8"
             )
         )
 
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
         byte_start = self._ast_node.src.byte_offset
-        match = USER_DEF_VAL_TYPE_RE.match(self._source)
+        match = USER_DEF_VAL_TYPE_RE.match(source)
         assert match
-        return byte_start + match.start("name"), byte_start + match.end("name")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            byte_start + match.start("name") + stripped,
+            byte_start + match.end("name") + stripped,
+        )
 
     @property
     def parent(self) -> Union[ContractDefinition, SourceUnit]:
         """
         Returns:
             Parent IR node.
         """
```

### Comparing `eth_wake-4.8.0/wake/ir/declarations/variable_declaration.py` & `eth_wake-4.9.0/wake/ir/declarations/variable_declaration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 import re
+from bisect import bisect
 from collections import deque
 from functools import lru_cache, partial
 from typing import (
     TYPE_CHECKING,
     Deque,
     FrozenSet,
     Iterator,
@@ -24,14 +25,15 @@
 from wake.ir.expressions.abc import ExpressionAbc
 from wake.ir.meta.structured_documentation import StructuredDocumentation
 from wake.ir.type_names.abc import TypeNameAbc
 from wake.ir.types import TypeAbc
 from wake.ir.utils import IrInitTuple
 from wake.utils.string import StringReader
 
+from ...regex_parser import SoliditySourceParser
 from ..meta.override_specifier import OverrideSpecifier
 from ..reference_resolver import CallbackParams
 
 if TYPE_CHECKING:
     from ..declarations.contract_definition import ContractDefinition
     from ..declarations.function_definition import FunctionDefinition
     from ..declarations.struct_definition import StructDefinition
@@ -222,25 +224,40 @@
         # this one is a bit tricky
         # it is easier to parse the variable declaration from the end (while omitting an optional assigned expression)
         if self._value is None:
             source_without_value = self._source
         else:
             length_without_value = self._value.byte_location[0] - self.byte_location[0]
             source_without_value = self._source[:length_without_value]
+        source_without_value = bytearray(source_without_value)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source_without_value)
 
         IDENTIFIER = r"[a-zA-Z$_][a-zA-Z0-9$_]*"
         VARIABLE_RE = re.compile(
             r"(?P<name>{identifier})(\s*=)?\s*$".format(identifier=IDENTIFIER).encode(
                 "utf-8"
             )
         )
         match = VARIABLE_RE.search(source_without_value)
         assert match
         byte_start = self._ast_node.src.byte_offset
-        return byte_start + match.start("name"), byte_start + match.end("name")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("name"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            byte_start + match.start("name") + stripped,
+            byte_start + match.end("name") + stripped,
+        )
 
     def get_all_references(
         self, include_declarations: bool
     ) -> Iterator[
         Union[
             DeclarationAbc,
             Identifier,
```

### Comparing `eth_wake-4.8.0/wake/ir/enums.py` & `eth_wake-4.9.0/wake/ir/enums.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/abc.py` & `eth_wake-4.9.0/wake/ir/expressions/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/assignment.py` & `eth_wake-4.9.0/wake/ir/expressions/assignment.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/binary_operation.py` & `eth_wake-4.9.0/wake/ir/expressions/binary_operation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/conditional.py` & `eth_wake-4.9.0/wake/ir/expressions/conditional.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/elementary_type_name_expression.py` & `eth_wake-4.9.0/wake/ir/expressions/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/function_call.py` & `eth_wake-4.9.0/wake/ir/expressions/function_call.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/function_call_options.py` & `eth_wake-4.9.0/wake/ir/expressions/function_call_options.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/identifier.py` & `eth_wake-4.9.0/wake/ir/expressions/identifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/index_access.py` & `eth_wake-4.9.0/wake/ir/expressions/index_access.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/index_range_access.py` & `eth_wake-4.9.0/wake/ir/expressions/index_range_access.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/literal.py` & `eth_wake-4.9.0/wake/ir/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/member_access.py` & `eth_wake-4.9.0/wake/ir/expressions/member_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from functools import lru_cache, partial
 from typing import TYPE_CHECKING, Iterator, Optional, Set, Tuple, Union
 
 from wake.core import get_logger
 from wake.ir.abc import IrAbc, SolidityAbc
 from wake.ir.ast import AstNodeId, SolcMemberAccess
 from wake.ir.declarations.abc import DeclarationAbc
@@ -26,14 +27,16 @@
     MagicTypeKind,
     String,
     Type,
     UserDefinedValueType,
 )
 from wake.ir.utils import IrInitTuple
 
+from ...regex_parser import SoliditySourceParser
+
 if TYPE_CHECKING:
     from ..statements.abc import StatementAbc
     from ..yul.abc import YulAbc
 
 MEMBER_RE = re.compile(r"\s*.\s*(?P<member>.+)".encode("utf-8"))
 
 
@@ -409,19 +412,33 @@
 
         Returns:
             Byte location of the member name.
         """
         relative_expression_end = (
             self._expression.byte_location[1] - self.byte_location[0]
         )
-        match = MEMBER_RE.match(self._source[relative_expression_end:])
+        source = bytearray(self._source[relative_expression_end:])
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
+        match = MEMBER_RE.match(source)
         assert match
-        return self._expression.byte_location[1] + match.start(
-            "member"
-        ), self._expression.byte_location[1] + match.end("member")
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("member"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            self._expression.byte_location[1] + match.start("member") + stripped,
+            self._expression.byte_location[1] + match.end("member") + stripped,
+        )
 
     @property
     def referenced_declaration(
         self,
     ) -> Union[DeclarationAbc, GlobalSymbol, SourceUnit]:
         """
         Returns:
```

### Comparing `eth_wake-4.8.0/wake/ir/expressions/new_expression.py` & `eth_wake-4.9.0/wake/ir/expressions/new_expression.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/tuple_expression.py` & `eth_wake-4.9.0/wake/ir/expressions/tuple_expression.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/expressions/unary_operation.py` & `eth_wake-4.9.0/wake/ir/expressions/unary_operation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/identifier_path.py` & `eth_wake-4.9.0/wake/ir/meta/identifier_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from collections import deque
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Deque, Optional, Set, Tuple, Union
 
+from ...regex_parser import SoliditySourceParser
+
 if TYPE_CHECKING:
     from .inheritance_specifier import InheritanceSpecifier
     from .modifier_invocation import ModifierInvocation
     from .override_specifier import OverrideSpecifier
     from .source_unit import SourceUnit
     from .using_for_directive import UsingForDirective
     from ..type_names.user_defined_type_name import UserDefinedTypeName
@@ -191,15 +194,18 @@
                         processed_source_units.add(import_.imported_file)
 
             assert referenced_declaration is not None
             return referenced_declaration
 
         from ..meta.source_unit import SourceUnit
 
-        matches = list(IDENTIFIER_RE.finditer(self._source))
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
+        matches = list(IDENTIFIER_RE.finditer(source))
         groups_count = len(matches)
         assert groups_count > 0
 
         self._parts = IntervalTree()
         start_source_unit = callback_params.source_units[self.source_unit.file]
 
         ref = self.referenced_declaration
@@ -228,16 +234,25 @@
             )
             referenced_node_id = (
                 self._reference_resolver.get_ast_id_from_cu_node_path_order(
                     node_path_order, self.source_unit.cu_hash
                 )
             )
 
-            start = self.byte_location[0] + match.start()
-            end = self.byte_location[0] + match.end()
+            if len(stripped_sums) == 0:
+                stripped = 0
+            else:
+                index = bisect([s[0] for s in stripped_sums], match.start())
+                if index == 0:
+                    stripped = 0
+                else:
+                    stripped = stripped_sums[index - 1][1]
+
+            start = self.byte_location[0] + match.start() + stripped
+            end = self.byte_location[0] + match.end() + stripped
             self._parts[start:end] = IdentifierPathPart(
                 self,
                 (start, end),
                 name,
                 referenced_node_id,
                 self._reference_resolver,
                 self.source_unit,
```

### Comparing `eth_wake-4.8.0/wake/ir/meta/import_directive.py` & `eth_wake-4.9.0/wake/ir/meta/import_directive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import logging
 import re
+from bisect import bisect
 from collections import deque
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
 from typing import TYPE_CHECKING, Deque, Iterator, List, Optional, Set, Tuple
 
+from ...regex_parser import SoliditySourceParser
 from ..expressions.identifier import Identifier
 from ..reference_resolver import CallbackParams
 
 if TYPE_CHECKING:
     from .source_unit import SourceUnit
 
 from wake.core import get_logger
@@ -279,13 +281,28 @@
 
         res = (
             IMPORT_FILENAME_RE,
             IMPORT_AS_FROM_RE,
             IMPORT_AS_RE,
             IMPORT_ALIAS_LIST,
         )
-        matches = list(re.match(self._source) for re in res)
+
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
+        matches = list(re.match(source) for re in res)
         assert any(matches)
         match = next(m for m in matches if m)
-        return source_start + match.start("filename"), source_start + match.end(
-            "filename"
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start("filename"))
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        return (
+            source_start + match.start("filename") + stripped,
+            source_start + match.end("filename") + stripped,
         )
```

### Comparing `eth_wake-4.8.0/wake/ir/meta/inheritance_specifier.py` & `eth_wake-4.9.0/wake/ir/meta/inheritance_specifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/modifier_invocation.py` & `eth_wake-4.9.0/wake/ir/meta/modifier_invocation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/override_specifier.py` & `eth_wake-4.9.0/wake/ir/meta/override_specifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/parameter_list.py` & `eth_wake-4.9.0/wake/ir/meta/parameter_list.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/pragma_directive.py` & `eth_wake-4.9.0/wake/ir/meta/pragma_directive.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/source_unit.py` & `eth_wake-4.9.0/wake/ir/meta/source_unit.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/structured_documentation.py` & `eth_wake-4.9.0/wake/ir/meta/structured_documentation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/try_catch_clause.py` & `eth_wake-4.9.0/wake/ir/meta/try_catch_clause.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/meta/using_for_directive.py` & `eth_wake-4.9.0/wake/ir/meta/using_for_directive.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/reference_resolver.py` & `eth_wake-4.9.0/wake/ir/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/abc.py` & `eth_wake-4.9.0/wake/ir/statements/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/block.py` & `eth_wake-4.9.0/wake/ir/statements/block.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/break_statement.py` & `eth_wake-4.9.0/wake/ir/statements/break_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/continue_statement.py` & `eth_wake-4.9.0/wake/ir/statements/continue_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/do_while_statement.py` & `eth_wake-4.9.0/wake/ir/statements/do_while_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/emit_statement.py` & `eth_wake-4.9.0/wake/ir/statements/emit_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/expression_statement.py` & `eth_wake-4.9.0/wake/ir/statements/expression_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/for_statement.py` & `eth_wake-4.9.0/wake/ir/statements/for_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/if_statement.py` & `eth_wake-4.9.0/wake/ir/statements/if_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/inline_assembly.py` & `eth_wake-4.9.0/wake/ir/statements/inline_assembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import re
+from bisect import bisect
 from functools import lru_cache, partial
 from typing import TYPE_CHECKING, FrozenSet, Iterator, Optional, Set, Tuple, Union
 
 from intervaltree import IntervalTree
 
 from wake.ir.abc import IrAbc, SolidityAbc
 from wake.ir.ast import AstNodeId, ExternalReferenceModel, SolcInlineAssembly
@@ -16,14 +17,15 @@
     ModifiesStateFlag,
 )
 from wake.ir.reference_resolver import CallbackParams, ReferenceResolver
 from wake.ir.statements.abc import StatementAbc
 from wake.ir.utils import IrInitTuple
 from wake.ir.yul.block import YulBlock
 
+from ...regex_parser import SoliditySourceParser
 from ..yul.identifier import YulIdentifier
 
 if TYPE_CHECKING:
     from ..expressions.abc import ExpressionAbc
     from ..meta.source_unit import SourceUnit
     from ..yul.abc import YulAbc
     from .block import Block
@@ -138,18 +140,31 @@
                 }
             }
             ```
 
         Returns:
             Byte offsets (start and end) of the identifier representing the external reference in the source file.
         """
-        match = IDENTIFIER_RE.match(self._source)
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
+        match = IDENTIFIER_RE.match(source)
         assert match
-        start = self.byte_location[0] + match.start()
-        end = self.byte_location[0] + match.end()
+
+        if len(stripped_sums) == 0:
+            stripped = 0
+        else:
+            index = bisect([s[0] for s in stripped_sums], match.start())
+            if index == 0:
+                stripped = 0
+            else:
+                stripped = stripped_sums[index - 1][1]
+
+        start = self.byte_location[0] + match.start() + stripped
+        end = self.byte_location[0] + match.end() + stripped
         return start, end
 
     @property
     def referenced_declaration(self) -> VariableDeclaration:
         """
         Returns:
             Solidity variable declaration referenced by this external reference.
```

### Comparing `eth_wake-4.8.0/wake/ir/statements/placeholder_statement.py` & `eth_wake-4.9.0/wake/ir/statements/placeholder_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/return_statement.py` & `eth_wake-4.9.0/wake/ir/statements/return_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/revert_statement.py` & `eth_wake-4.9.0/wake/ir/statements/revert_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/try_statement.py` & `eth_wake-4.9.0/wake/ir/statements/try_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/unchecked_block.py` & `eth_wake-4.9.0/wake/ir/statements/unchecked_block.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/variable_declaration_statement.py` & `eth_wake-4.9.0/wake/ir/statements/variable_declaration_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/statements/while_statement.py` & `eth_wake-4.9.0/wake/ir/statements/while_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/type_names/abc.py` & `eth_wake-4.9.0/wake/ir/type_names/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/type_names/array_type_name.py` & `eth_wake-4.9.0/wake/ir/type_names/array_type_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/type_names/elementary_type_name.py` & `eth_wake-4.9.0/wake/ir/type_names/elementary_type_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/type_names/function_type_name.py` & `eth_wake-4.9.0/wake/ir/type_names/function_type_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/type_names/mapping.py` & `eth_wake-4.9.0/wake/ir/type_names/mapping.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/type_names/user_defined_type_name.py` & `eth_wake-4.9.0/wake/ir/type_names/user_defined_type_name.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
+from bisect import bisect
 from collections import deque
 from pathlib import Path
 from typing import TYPE_CHECKING, Deque, Iterator, Optional, Set, Tuple, Union
 
 from intervaltree import IntervalTree
 
 from wake.ir.types import Contract, Enum, Struct, UserDefinedValueType
 
+from ...regex_parser import SoliditySourceParser
 from ..reference_resolver import CallbackParams
 
 if TYPE_CHECKING:
     from ..declarations.variable_declaration import VariableDeclaration
     from ..expressions.new_expression import NewExpression
     from ..meta.inheritance_specifier import InheritanceSpecifier
     from ..meta.override_specifier import OverrideSpecifier
@@ -164,15 +166,18 @@
                         processed_source_units.add(import_.imported_file)
 
             assert referenced_declaration is not None
             return referenced_declaration
 
         from ..meta.source_unit import SourceUnit
 
-        matches = list(IDENTIFIER_RE.finditer(self._source))
+        source = bytearray(self._source)
+        _, stripped_sums = SoliditySourceParser.strip_comments(source)
+
+        matches = list(IDENTIFIER_RE.finditer(source))
         groups_count = len(matches)
         assert groups_count > 0
 
         self._parts = IntervalTree()
         start_source_unit = callback_params.source_units[self.source_unit.file]
 
         ref = self.referenced_declaration
@@ -201,16 +206,25 @@
             )
             referenced_node_id = (
                 self._reference_resolver.get_ast_id_from_cu_node_path_order(
                     node_path_order, self.source_unit.cu_hash
                 )
             )
 
-            start = self.byte_location[0] + match.start()
-            end = self.byte_location[0] + match.end()
+            if len(stripped_sums) == 0:
+                stripped = 0
+            else:
+                index = bisect([s[0] for s in stripped_sums], match.start())
+                if index == 0:
+                    stripped = 0
+                else:
+                    stripped = stripped_sums[index - 1][1]
+
+            start = self.byte_location[0] + match.start() + stripped
+            end = self.byte_location[0] + match.end() + stripped
             self._parts[start:end] = IdentifierPathPart(
                 self,
                 (start, end),
                 name,
                 referenced_node_id,
                 self._reference_resolver,
                 self.source_unit,
```

### Comparing `eth_wake-4.8.0/wake/ir/types.py` & `eth_wake-4.9.0/wake/ir/types.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/utils.py` & `eth_wake-4.9.0/wake/ir/utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/abc.py` & `eth_wake-4.9.0/wake/ir/yul/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/assignment.py` & `eth_wake-4.9.0/wake/ir/yul/assignment.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/block.py` & `eth_wake-4.9.0/wake/ir/yul/block.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/break_statement.py` & `eth_wake-4.9.0/wake/ir/yul/break_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/case_.py` & `eth_wake-4.9.0/wake/ir/yul/case_.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/continue_statement.py` & `eth_wake-4.9.0/wake/ir/yul/continue_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/expression_statement.py` & `eth_wake-4.9.0/wake/ir/yul/expression_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/for_loop.py` & `eth_wake-4.9.0/wake/ir/yul/for_loop.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/function_call.py` & `eth_wake-4.9.0/wake/ir/yul/function_call.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/function_definition.py` & `eth_wake-4.9.0/wake/ir/yul/function_definition.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/identifier.py` & `eth_wake-4.9.0/wake/ir/yul/identifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/if_statement.py` & `eth_wake-4.9.0/wake/ir/yul/if_statement.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/leave.py` & `eth_wake-4.9.0/wake/ir/yul/leave.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/literal.py` & `eth_wake-4.9.0/wake/ir/yul/literal.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/switch.py` & `eth_wake-4.9.0/wake/ir/yul/switch.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/typed_name.py` & `eth_wake-4.9.0/wake/ir/yul/typed_name.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/ir/yul/variable_declaration.py` & `eth_wake-4.9.0/wake/ir/yul/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/commands/generate_control_flow_graph.py` & `eth_wake-4.9.0/wake/lsp/commands/generate_control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/commands/generate_imports_graph.py` & `eth_wake-4.9.0/wake/lsp/commands/generate_imports_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/commands/generate_inheritance_graph.py` & `eth_wake-4.9.0/wake/lsp/commands/generate_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/commands/generate_linearized_inheritance_graph.py` & `eth_wake-4.9.0/wake/lsp/commands/generate_linearized_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/commands/init.py` & `eth_wake-4.9.0/wake/lsp/commands/init.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/common_structures.py` & `eth_wake-4.9.0/wake/lsp/common_structures.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/context.py` & `eth_wake-4.9.0/wake/lsp/context.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/document_sync.py` & `eth_wake-4.9.0/wake/lsp/document_sync.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/code_action.py` & `eth_wake-4.9.0/wake/lsp/features/code_action.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/code_lens.py` & `eth_wake-4.9.0/wake/lsp/features/code_lens.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/completion.py` & `eth_wake-4.9.0/wake/lsp/features/completion.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/definition.py` & `eth_wake-4.9.0/wake/lsp/features/definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             definitions |= resolve(n)
     else:
         definitions = resolve(node)
 
     return list(definitions)
 
 
-async def _get_definition_from_cache(
+def _get_definition_from_cache(
     path: Path,
     position: Position,
     context: LspContext,
 ):
     new_byte_offset = context.compiler.get_byte_offset_from_line_pos(
         path, position.line, position.character
     )
@@ -246,15 +246,15 @@
     path = uri_to_path(params.text_document.uri).resolve()
     if (
         path not in context.compiler.interval_trees
         or not context.compiler.output_ready.is_set()
     ):
         # try to use old build artifacts
         try:
-            return await _get_definition_from_cache(path, params.position, context)
+            return _get_definition_from_cache(path, params.position, context)
         except Exception:
             pass
 
     await context.compiler.output_ready.wait()
     if path not in context.compiler.interval_trees:
         return None
```

### Comparing `eth_wake-4.8.0/wake/lsp/features/diagnostic.py` & `eth_wake-4.9.0/wake/lsp/features/diagnostic.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/document_link.py` & `eth_wake-4.9.0/wake/lsp/features/document_link.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/document_symbol.py` & `eth_wake-4.9.0/wake/lsp/features/document_symbol.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/hover.py` & `eth_wake-4.9.0/wake/lsp/features/hover.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
             return (
                 f"```solidity\n{yul_definitions[node.name]}\n```",
                 original_node_location,
             )
     return None
 
 
-async def _get_hover_from_cache(path: Path, position: Position, context: LspContext):
+def _get_hover_from_cache(path: Path, position: Position, context: LspContext):
     new_byte_offset = context.compiler.get_byte_offset_from_line_pos(
         path, position.line, position.character
     )
     backward_changes = context.compiler.get_last_compilation_backward_changes(path)
     if backward_changes is None:
         raise Exception("No backward changes found")
     changes_before = backward_changes[0:new_byte_offset]
@@ -370,15 +370,15 @@
 
     path = uri_to_path(params.text_document.uri).resolve()
     if (
         path not in context.compiler.interval_trees
         or not context.compiler.output_ready.is_set()
     ):
         try:
-            return await _get_hover_from_cache(path, params.position, context)
+            return _get_hover_from_cache(path, params.position, context)
         except Exception:
             pass
 
     await context.compiler.output_ready.wait()
     if path not in context.compiler.interval_trees:
         return None
```

### Comparing `eth_wake-4.8.0/wake/lsp/features/implementation.py` & `eth_wake-4.9.0/wake/lsp/features/implementation.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/inlay_hint.py` & `eth_wake-4.9.0/wake/lsp/features/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/references.py` & `eth_wake-4.9.0/wake/lsp/features/references.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/rename.py` & `eth_wake-4.9.0/wake/lsp/features/rename.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/features/type_definition.py` & `eth_wake-4.9.0/wake/lsp/features/type_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 type_name.referenced_declaration.name_location,
             )
         ]
     else:
         return None
 
 
-async def _get_type_definition_from_cache(
+def _get_type_definition_from_cache(
     path: Path,
     position: Position,
     context: LspContext,
 ):
     new_byte_offset = context.compiler.get_byte_offset_from_line_pos(
         path, position.line, position.character
     )
@@ -186,15 +186,15 @@
     path = uri_to_path(params.text_document.uri).resolve()
     if (
         path not in context.compiler.interval_trees
         or not context.compiler.output_ready.is_set()
     ):
         # try to use old build artifacts
         try:
-            return await _get_type_definition_from_cache(path, params.position, context)
+            return _get_type_definition_from_cache(path, params.position, context)
         except Exception:
             pass
 
     await context.compiler.output_ready.wait()
     if path not in context.compiler.interval_trees:
         return None
```

### Comparing `eth_wake-4.8.0/wake/lsp/features/type_hierarchy.py` & `eth_wake-4.9.0/wake/lsp/features/type_hierarchy.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/logging_handler.py` & `eth_wake-4.9.0/wake/lsp/logging_handler.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/lsp_compiler.py` & `eth_wake-4.9.0/wake/lsp/lsp_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -558,16 +558,14 @@
                 and not self.__file_excluded(path)
                 and path.suffix == ".sol"
             ):
                 self.__discovered_files.add(path)
                 self.__force_compile_files.add(path)
             elif change.text_document.text != self.get_compiled_file(path).text:
                 self.__force_compile_files.add(path)
-            else:
-                self.__output_contents[path] = self.__opened_files[path]
 
         elif isinstance(change, DidCloseTextDocumentParams):
             pass
         elif isinstance(change, DidChangeTextDocumentParams):
             path = uri_to_path(change.text_document.uri).resolve()
             self.__modified_files.add(path)
 
@@ -647,40 +645,54 @@
                 await self.__diagnostic_queue.put((file, set()))
             self.__interval_trees.clear()
             self.__source_units.clear()
             self.__ir_reference_resolver.clear_all_indexed_nodes()
             return
 
         try:
+            modified_files = {
+                path: info.text.encode("utf-8")
+                for path, info in self.__opened_files.items()
+            }
+            for p in self.__output_contents:
+                if p not in modified_files:
+                    modified_files[p] = self.__output_contents[p].text.encode("utf-8")
+
             if full_compile:
                 graph, source_units_to_paths = self.__compiler.build_graph(
                     self.__discovered_files,
-                    {
-                        path: info.text.encode("utf-8")
-                        for path, info in self.__opened_files.items()
-                    },
+                    modified_files,
                     True,
                 )
 
                 # add to deleted files previously compiled files that are now excluded from build
                 # will trigger post-destroy callbacks and remove them from source units
                 for p in self.__source_units:
                     # use graph.nodes - i.e. discovered files + their dependencies from exclude paths
                     if p not in source_units_to_paths.values():
                         self.__deleted_files.add(p)
                 self.__last_graph = graph
             else:
                 graph, _ = self.__compiler.build_graph(
                     files_to_compile,
-                    {
-                        path: info.text.encode("utf-8")
-                        for path, info in self.__opened_files.items()
-                    },
+                    modified_files,
                     True,
                 )
+
+            for source_unit_name in graph.nodes:
+                path = graph.nodes[source_unit_name]["path"]
+                content = graph.nodes[source_unit_name]["content"]
+                if (
+                    path not in self.__opened_files
+                    and path not in self.__output_contents
+                ):
+                    self.__output_contents[path] = VersionedFile(
+                        content.decode(encoding="utf-8"), None
+                    )
+
         except CompilationError as e:
             await self.__server.log_message(str(e), MessageType.ERROR)
             for file in self.__discovered_files:
                 # clear diagnostics
                 await self.__diagnostic_queue.put((file, set()))
             self.__interval_trees.clear()
             self.__source_units.clear()
```

### Comparing `eth_wake-4.8.0/wake/lsp/lsp_parser.py` & `eth_wake-4.9.0/wake/lsp/lsp_parser.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/methods.py` & `eth_wake-4.9.0/wake/lsp/methods.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/protocol_structures.py` & `eth_wake-4.9.0/wake/lsp/protocol_structures.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/rpc_protocol.py` & `eth_wake-4.9.0/wake/lsp/rpc_protocol.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/server.py` & `eth_wake-4.9.0/wake/lsp/server.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/server_capabilities.py` & `eth_wake-4.9.0/wake/lsp/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/lsp/utils/position.py` & `eth_wake-4.9.0/wake/lsp/utils/position.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/migrations/woke_wake_migration.py` & `eth_wake-4.9.0/wake/migrations/woke_wake_migration.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/migrations/xdg_migration.py` & `eth_wake-4.9.0/wake/migrations/xdg_migration.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/printers/api.py` & `eth_wake-4.9.0/wake/printers/api.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/regex_parser/solidity_import.py` & `eth_wake-4.9.0/wake/regex_parser/solidity_import.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/regex_parser/solidity_parser.py` & `eth_wake-4.9.0/wake/regex_parser/solidity_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,25 @@
                 raise
             imports.add(import_expr.filename)
         return list(imports)
 
     @classmethod
     def strip_comments(
         cls, source_code: bytearray
-    ) -> Dict[str, List[Tuple[List[str], Tuple[int, int]]]]:
+    ) -> Tuple[
+        Dict[str, List[Tuple[List[str], Tuple[int, int]]]], List[Tuple[int, int]]
+    ]:
         if len(source_code) == 0:
-            return {}
+            return {}, []
 
         wake_comments: DefaultDict[
             str, List[Tuple[List[str], Tuple[int, int]]]
         ] = defaultdict(list)
         stripped_sum = 0
+        stripped_sums: List[Tuple[int, int]] = []
         search_start = 0
 
         while len(source_code) > search_start:
             match = cls.ONELINE_COMMENT_OR_MULTILINE_COMMENT_START_RE.search(
                 source_code, search_start
             )
             if match is None:
@@ -230,15 +233,20 @@
 
                 source_code[match.start() : match.end()] = b""
                 stripped = match.end() - match.start()
 
             search_start = match.end() - stripped
             stripped_sum += stripped
 
-        return wake_comments
+            if len(stripped_sums) > 0 and stripped_sums[-1][0] == match.start():
+                stripped_sums[-1] = (match.start(), stripped_sum)
+            else:
+                stripped_sums.append((match.start(), stripped_sum))
+
+        return wake_comments, stripped_sums
 
     @classmethod
     def parse(
         cls, path: Path, ignore_errors: bool = False
     ) -> Tuple[
         SolidityVersionRanges,
         List[str],
@@ -251,15 +259,15 @@
         the given file. The second list contains filenames / URLs that are imported from the given file.
         """
         raw_content = path.read_bytes()
         h = BLAKE2b.new(data=raw_content, digest_bits=256)
 
         # strip all comments, parse wake comments
         stripped_content = bytearray(raw_content)
-        wake_comments = cls.strip_comments(stripped_content)
+        wake_comments, _ = cls.strip_comments(stripped_content)
 
         return (
             cls._parse_version_pragma(stripped_content, ignore_errors),
             cls._parse_import(stripped_content, ignore_errors),
             h.digest(),
             raw_content,
             wake_comments,
@@ -280,15 +288,15 @@
         Return a tuple of two lists. The first list contains Solidity version ranges that can be used to compile
         the given file. The second list contains filenames / URLs that are imported from the given file.
         """
         h = BLAKE2b.new(data=source_code, digest_bits=256)
 
         # strip all comments, parse wake comments
         stripped_source_code = bytearray(source_code)
-        wake_comments = cls.strip_comments(stripped_source_code)
+        wake_comments, _ = cls.strip_comments(stripped_source_code)
 
         return (
             cls._parse_version_pragma(stripped_source_code, ignore_errors),
             cls._parse_import(stripped_source_code, ignore_errors),
             h.digest(),
             wake_comments,
         )
```

### Comparing `eth_wake-4.8.0/wake/svm/abc.py` & `eth_wake-4.9.0/wake/svm/abc.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/svm/svm.py` & `eth_wake-4.9.0/wake/svm/svm.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/testing/__init__.py` & `eth_wake-4.9.0/wake/testing/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,7 +27,9 @@
     keccak256,
     mint_erc20,
     read_storage_variable,
     write_storage_variable,
 )
 
 from .core import Chain, default_chain
+
+chain = default_chain
```

### Comparing `eth_wake-4.8.0/wake/testing/core.py` & `eth_wake-4.9.0/wake/testing/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         self._snapshots[snapshot_id] = {
             "nonces": self._nonces.copy(),
             "accounts": self._accounts.copy(),
             "default_call_account": self._default_call_account,
             "default_tx_account": self._default_tx_account,
             "block_gas_limit": self._block_gas_limit,
             "txs": dict(self._txs._transactions),
+            "tx_hashes": list(self._txs._tx_hashes),
             "blocks": dict(self._blocks._blocks),
         }
         return snapshot_id
 
     @check_connected
     def revert(self, snapshot_id: str) -> None:
         reverted = self._chain_interface.revert(snapshot_id)
@@ -111,14 +112,15 @@
         snapshot = self._snapshots[snapshot_id]
         self._nonces = snapshot["nonces"]
         self._accounts = snapshot["accounts"]
         self._default_call_account = snapshot["default_call_account"]
         self._default_tx_account = snapshot["default_tx_account"]
         self._block_gas_limit = snapshot["block_gas_limit"]
         self._txs._transactions = snapshot["txs"]
+        self._txs._tx_hashes = snapshot["tx_hashes"]
         self._blocks._blocks = snapshot["blocks"]
         del self._snapshots[snapshot_id]
 
     @property
     @check_connected
     def block_gas_limit(self) -> int:
         return self._block_gas_limit
```

### Comparing `eth_wake-4.8.0/wake/testing/coverage.py` & `eth_wake-4.9.0/wake/testing/coverage.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/testing/fuzzing/fuzz_test.py` & `eth_wake-4.9.0/wake/testing/fuzzing/fuzz_test.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/testing/fuzzing/fuzzer.py` & `eth_wake-4.9.0/wake/testing/fuzzing/fuzzer.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/testing/fuzzing/generators.py` & `eth_wake-4.9.0/wake/testing/fuzzing/generators.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess.py` & `eth_wake-4.9.0/wake/testing/pytest_plugin_multiprocess.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/testing/pytest_plugin_multiprocess_server.py` & `eth_wake-4.9.0/wake/testing/pytest_plugin_multiprocess_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 args=(self._pytest_args,),
                 kwargs={
                     "plugins": [
                         PytestWakePluginMultiprocess(
                             i,
                             child_conn,  # pyright: ignore reportGeneralTypeIssues
                             self._queue,
-                            empty_coverage,
+                            empty_coverage if i < self._coverage else None,
                             logs_dir,
                             self._random_seeds[i],
                             self._attach_first and i == 0,
                             self._debug,
                         ),
                     ]
                 },
@@ -254,15 +254,15 @@
                                 progress,
                                 index,
                                 tasks[index],
                                 current_tests[index],
                                 test_reports[index],
                             )
                     elif msg[0] == "pytest_warning_recorded":
-                        session.config.hook.pytest_warning_recorded.call_historic(
+                        session.config.hook.pytest_warning_recorded.call_historic(  # pyright: ignore reportFunctionMemberAccess
                             kwargs={
                                 "warning_message": msg[2],
                                 "when": msg[3],
                                 "nodeid": msg[4],
                                 "location": msg[5],
                             },
                         )
@@ -284,15 +284,18 @@
             for report in reports:
                 session.config.hook.pytest_runtest_logreport(report=report)
 
         return True
 
     def pytest_terminal_summary(self, terminalreporter, exitstatus, config):
         terminalreporter.section("Wake")
-        terminalreporter.write_line("Random seeds: " + ", ".join(s.hex() for s in self._random_seeds[:self._proc_count]))
+        terminalreporter.write_line(
+            "Random seeds: "
+            + ", ".join(s.hex() for s in self._random_seeds[: self._proc_count])
+        )
 
     def _update_progress(
         self,
         progress: rich.progress.Progress,
         index: int,
         task_id: rich.progress.TaskID,
         current_test: Optional[str],
```

### Comparing `eth_wake-4.8.0/wake/testing/pytest_plugin_single.py` & `eth_wake-4.9.0/wake/testing/pytest_plugin_single.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/context_managers.py` & `eth_wake-4.9.0/wake/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/decorators.py` & `eth_wake-4.9.0/wake/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/file_utils.py` & `eth_wake-4.9.0/wake/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/formatters.py` & `eth_wake-4.9.0/wake/utils/formatters.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/general.py` & `eth_wake-4.9.0/wake/utils/general.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/null_file.py` & `eth_wake-4.9.0/wake/utils/null_file.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/openzeppelin.py` & `eth_wake-4.9.0/wake/utils/openzeppelin.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/string.py` & `eth_wake-4.9.0/wake/utils/string.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/tee.py` & `eth_wake-4.9.0/wake/utils/tee.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake/utils/threaded_child_watcher.py` & `eth_wake-4.9.0/wake/utils/threaded_child_watcher.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/__init__.py` & `eth_wake-4.9.0/wake_detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/abi_encode_with_signature.py` & `eth_wake-4.9.0/wake_detectors/abi_encode_with_signature.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/axelar_proxy_contract_id.py` & `eth_wake-4.9.0/wake_detectors/axelar_proxy_contract_id.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/balance_relied_on.py` & `eth_wake-4.9.0/wake_detectors/balance_relied_on.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,18 @@
             while ref_statement is not None:
                 if isinstance(ref_statement, ir.StatementAbc):
                     break
                 ref_statement = ref_statement.parent
             if ref_statement is None or ref_statement == assigned_var_statement:
                 continue
 
-            if cfg.is_reachable(assigned_var_statement, ref_statement):
+            if (
+                cfg.is_reachable(assigned_var_statement, ref_statement)
+                or assigned_var_statement == ref_statement
+            ):
                 ret.extend(_process_assigned_vars(ref))
     return ret
 
 
 class BalanceReliedOnDetector(Detector):
     _detections: List[DetectorResult]
```

### Comparing `eth_wake-4.8.0/wake_detectors/call_options_not_called.py` & `eth_wake-4.9.0/wake_detectors/call_options_not_called.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py` & `eth_wake-4.9.0/wake_detectors/calldata_tuple_reencoding_head_overflow_bug.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/complex_struct_getter.py` & `eth_wake-4.9.0/wake_detectors/complex_struct_getter.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/empty_byte_array_copy_bug.py` & `eth_wake-4.9.0/wake_detectors/empty_byte_array_copy_bug.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,15 +80,18 @@
             if (
                 not isinstance(t, types.Bytes)
                 or t.data_location == ir.enums.DataLocation.STORAGE
             ):
                 continue
 
             # .push() may happen after the assignment
-            if cfg.is_reachable(ref.statement, node.statement):
+            if (
+                cfg.is_reachable(ref.statement, node.statement)
+                or ref.statement == node.statement
+            ):
                 self._detections.append(
                     DetectorResult(
                         Detection(
                             node.parent,
                             ".push() may append non-zero byte because of compiler bug",
                         ),
                         DetectorImpact.MEDIUM,
```

### Comparing `eth_wake-4.8.0/wake_detectors/incorrect_interface.py` & `eth_wake-4.9.0/wake_detectors/incorrect_interface.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/missing_return.py` & `eth_wake-4.9.0/wake_detectors/missing_return.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/msg_value_nonpayable_function.py` & `eth_wake-4.9.0/wake_detectors/msg_value_nonpayable_function.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/reentrancy.py` & `eth_wake-4.9.0/wake_detectors/reentrancy.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/struct_mapping_deletion.py` & `eth_wake-4.9.0/wake_detectors/struct_mapping_deletion.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/tx_origin.py` & `eth_wake-4.9.0/wake_detectors/tx_origin.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unchecked_return_value.py` & `eth_wake-4.9.0/wake_detectors/unchecked_return_value.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unprotected_selfdestruct.py` & `eth_wake-4.9.0/wake_detectors/unprotected_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unsafe_delegatecall.py` & `eth_wake-4.9.0/wake_detectors/unsafe_delegatecall.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unsafe_erc20_call.py` & `eth_wake-4.9.0/wake_detectors/unsafe_erc20_call.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unused_contract.py` & `eth_wake-4.9.0/wake_detectors/unused_contract.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unused_function.py` & `eth_wake-4.9.0/wake_detectors/unused_function.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unused_import.py` & `eth_wake-4.9.0/wake_detectors/unused_import.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_detectors/unused_modifier.py` & `eth_wake-4.9.0/wake_detectors/unused_modifier.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/abi.py` & `eth_wake-4.9.0/wake_printers/abi.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/c3_linearization.py` & `eth_wake-4.9.0/wake_printers/c3_linearization.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/control_flow_graph.py` & `eth_wake-4.9.0/wake_printers/control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/imports_graph.py` & `eth_wake-4.9.0/wake_printers/imports_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/inheritance_graph.py` & `eth_wake-4.9.0/wake_printers/inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/inheritance_tree.py` & `eth_wake-4.9.0/wake_printers/inheritance_tree.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/modifiers.py` & `eth_wake-4.9.0/wake_printers/modifiers.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/state_changes.py` & `eth_wake-4.9.0/wake_printers/state_changes.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/storage_layout.py` & `eth_wake-4.9.0/wake_printers/storage_layout.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/wake_printers/tokens.py` & `eth_wake-4.9.0/wake_printers/tokens.py`

 * *Files identical despite different names*

### Comparing `eth_wake-4.8.0/PKG-INFO` & `eth_wake-4.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-wake
-Version: 4.8.0
+Version: 4.9.0
 Summary: Wake is a Python-based Solidity development and testing framework with built-in vulnerability detectors.
 Home-page: https://getwake.io
 License: ISC
 Keywords: ethereum,solidity,security,testing,development,static analysis,framework,audit
 Author: Ackee Blockchain
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved
@@ -57,15 +57,15 @@
 Requires-Dist: sarif-om (>=1.0.4,<2.0.0)
 Requires-Dist: tblib (>=1.7,<2.0)
 Requires-Dist: tomli (>=2,<3)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4,<5)
 Requires-Dist: watchdog (>=2.2.0,<2.3.0)
 Requires-Dist: websocket-client (>=1.4,<2.0)
-Project-URL: Documentation, https://ackeeblockchain.com/wake/docs/latest
+Project-URL: Documentation, https://ackee.xyz/wake/docs/latest
 Project-URL: Repository, https://github.com/Ackee-Blockchain/wake
 Project-URL: VS Code Extension, https://marketplace.visualstudio.com/items?itemName=AckeeBlockchain.tools-for-solidity
 Description-Content-Type: text/markdown
 
 # Wake, a Python-based Solidity development and testing framework with built-in vulnerability detectors
 
 ![Wake cover](https://github.com/Ackee-Blockchain/wake/blob/main/images/wake_cover.png?raw=true)
@@ -96,17 +96,17 @@
 
 ```shell
 pip3 install eth-wake
 ```
 
 ## Documentation & Contribution
 
-Wake documentation can be found [here](https://ackeeblockchain.com/wake/docs/latest).
+Wake documentation can be found [here](https://ackee.xyz/wake/docs/latest).
 
-There you can also find a section on [contributing](https://ackeeblockchain.com/wake/docs/latest/contributing/).
+There you can also find a section on [contributing](https://ackee.xyz/wake/docs/latest/contributing/).
 
 ## Discovered vulnerabilities
 
 | Vulnerability                                   | Severity | Project | Method           | Discovered by    | Resources                                                                                                                                                                                                                       |
 |-------------------------------------------------|----------|---------|------------------|------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Profit & loss accounted twice                   | Critical | IPOR    | Fuzz test        | Ackee Blockchain | [Report](https://github.com/Ackee-Blockchain/public-audit-reports/blob/master/2023/ackee-blockchain-ipor-protocol-report.pdf), [Wake tests](https://github.com/Ackee-Blockchain/tests-ipor/blob/main/tests/test_fuzz.py)        |
 | Console permanent denial of service             | High     | Brahma  | Fuzz test        | Ackee Blockchain | [Report](https://github.com/Ackee-Blockchain/public-audit-reports/blob/master/2023/ackee-blockchain-brahma-console-v2-report.pdf)                                                                                               |
@@ -120,15 +120,15 @@
 | Missing receive function                        | Medium   | Axelar  | Fuzz test        | Ackee Blockchain | [Wake tests](https://github.com/Ackee-Blockchain/tests-axelar-interchain-governance-executor/blob/main/tests/test_fuzz.py)                                                                                                      |
 | `SafeERC20` not used for `approve`              | Medium   | Lido    | Fuzz test        | Ackee Blockchain | [Wake tests](https://github.com/Ackee-Blockchain/tests-lido-stonks/blob/main/tests/test_fuzz.py)                                                                                                                                |
 
 ## Features
 
 ### Testing framework
 
-See [examples](https://github.com/Ackee-Blockchain/wake/tree/main/examples) and [documentation](https://ackeeblockchain.com/wake/docs/latest/testing-framework/overview) for more information.
+See [examples](https://github.com/Ackee-Blockchain/wake/tree/main/examples) and [documentation](https://ackee.xyz/wake/docs/latest/testing-framework/overview) for more information.
 
 Writing tests is as simple as:
 
 ```python
 from wake.testing import *
 from pytypes.contracts.Counter import Counter
 
@@ -187,28 +187,28 @@
 ```
 
 A specific detector can be run using:
 ```shell
 wake detect <detector-name>
 ```
 
-See the [documentation](https://ackeeblockchain.com/wake/docs/latest/static-analysis/using-detectors/) for a list of all detectors.
+See the [documentation](https://ackee.xyz/wake/docs/latest/static-analysis/using-detectors/) for a list of all detectors.
 
 ### Printers
 
 A specific printer can be run using:
 ```shell
 wake print <printer-name>
 ```
 
-See the [documentation](https://ackeeblockchain.com/wake/docs/latest/static-analysis/using-printers/) for a list of all printers.
+See the [documentation](https://ackee.xyz/wake/docs/latest/static-analysis/using-printers/) for a list of all printers.
 
 ### Custom detectors & printers
 
-Refer to the [getting started](https://ackeeblockchain.com/wake/docs/latest/static-analysis/getting-started/) guide for more information.
+Refer to the [getting started](https://ackee.xyz/wake/docs/latest/static-analysis/getting-started/) guide for more information.
 Also check out [wake_detectors](https://github.com/Ackee-Blockchain/wake/tree/main/wake_detectors) and [wake_printers](https://github.com/Ackee-Blockchain/wake/tree/main/wake_printers) for the implementation of built-in detectors and printers.
 
 ### LSP server
 
 Wake implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.
 
 Wake LSP server can be run using:
@@ -219,15 +219,15 @@
 
 Or with an optional --port argument (default 65432):
 
 ```shell
 wake lsp --port 1234
 ```
 
-All LSP server features can be found in the [documentation](https://ackeeblockchain.com/wake/docs/latest/language-server/).
+All LSP server features can be found in the [documentation](https://ackee.xyz/wake/docs/latest/language-server/).
 
 ## License
 
 This project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/wake/blob/main/LICENSE).
 
 ## Partners
```

