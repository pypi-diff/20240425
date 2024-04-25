# Comparing `tmp/rqalpha-5.3.8.tar.gz` & `tmp/rqalpha-5.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-7hwnafho/rqalpha-5.3.8.tar", last modified: Fri Mar 29 02:01:44 2024, max compression
+gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-rf3mmfs2/rqalpha-5.3.9.tar", last modified: Tue Apr 16 02:18:48 2024, max compression
```

## Comparing `rqalpha-5.3.8.tar` & `rqalpha-5.3.9.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    62409 2024-03-29 02:01:38.000000 rqalpha-5.3.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-29 02:01:38.000000 rqalpha-5.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-29 02:01:38.000000 rqalpha-5.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-29 02:01:44.000000 rqalpha-5.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-03-29 02:01:38.000000 rqalpha-5.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/apis/api_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    58869 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/apis/api_rqdatac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/apis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/cmds/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/cmds/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/cmds/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/cmds/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/global_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/strategy_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/strategy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/core/strategy_universe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/bar_dict_price_board.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/data/base_data_source/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/base_data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/base_data_source/adjust.py
--rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/base_data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/base_data_source/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/base_data_source/storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    34676 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/data_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/data/trading_dates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/IF1706_20161108.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/IF_macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/examples/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/data_source/get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/data_source/import_get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/data_source/read_csv_as_df.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/examples/extend_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/extend_api/test_extend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/golden_cross.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/pair_trading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/run_code_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/run_file_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/run_func_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/subscribe_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/examples/turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)    22394 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
--rw-r--r--   0 runner    (1001) docker     (127)    34463 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)    21406 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26335 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    22206 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_progress/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29447 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/mod_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/model/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25895 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/model/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/model/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/model/tick.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/model/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/portfolio/
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/portfolio/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/portfolio/position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/resource/
--rw-r--r--   0 runner    (1001) docker     (127)    32799 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/resource/ricequant-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/user_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/class_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/click_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/datetime_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/dict_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/package_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/persisit_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/risk_free_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/rq_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/strategy_loader_help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/testing/mocking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/utils/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19867 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    55970 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-29 02:01:38.000000 rqalpha-5.3.8/rqalpha/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 02:01:44.000000 rqalpha-5.3.8/rqalpha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-29 02:01:44.000000 rqalpha-5.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-29 02:01:38.000000 rqalpha-5.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/api_tests/mod/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_account_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_position_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_scheduler/test_physical_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_management_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/test_api_future.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/test_api_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/api_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_f_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_f_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_f_macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_f_macd_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_f_mean_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_f_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_s_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_s_dual_thrust.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_s_pit_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_s_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_s_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_s_turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_s_turtle_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/test_sf_buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/unittest/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/unittest/test_data/test_auto_update_bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_data/test_auto_update_bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_data/test_instrument_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_data/test_trading_dates_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/unittest/test_mod/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:01:44.000000 rqalpha-5.3.8/tests/unittest/test_mod/test_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_mod/test_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-29 02:01:38.000000 rqalpha-5.3.8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    86835 2024-03-29 02:01:38.000000 rqalpha-5.3.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    62409 2024-04-16 02:18:41.000000 rqalpha-5.3.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-16 02:18:41.000000 rqalpha-5.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 02:18:41.000000 rqalpha-5.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 02:18:48.000000 rqalpha-5.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-16 02:18:41.000000 rqalpha-5.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/api_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35275 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58869 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/api_rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy_universe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/bar_dict_price_board.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18961 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34676 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/data_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/trading_dates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/IF1706_20161108.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/IF_macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/examples/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/data_source/get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/data_source/import_get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/data_source/read_csv_as_df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/examples/extend_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/extend_api/test_extend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/golden_cross.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/pair_trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/run_code_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/run_file_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/run_func_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/subscribe_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22708 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34880 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21406 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28049 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29447 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25895 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/tick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21138 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/portfolio/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/portfolio/position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)    32799 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/resource/ricequant-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/user_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/class_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/click_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/datetime_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/dict_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/package_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/persisit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/risk_free_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/rq_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/strategy_loader_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/testing/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    56217 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 02:18:48.000000 rqalpha-5.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-16 02:18:41.000000 rqalpha-5.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_account_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_position_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_physical_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_management_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_api_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_macd_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_mean_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_dual_thrust.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_pit_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_turtle_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_sf_buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_instrument_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_trading_dates_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_mod/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86835 2024-04-16 02:18:41.000000 rqalpha-5.3.9/versioneer.py
```

### Comparing `rqalpha-5.3.8/CHANGELOG.rst` & `rqalpha-5.3.9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/LICENSE` & `rqalpha-5.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/PKG-INFO` & `rqalpha-5.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.3.8
+Version: 5.3.9
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.3.8/README.rst` & `rqalpha-5.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/__init__.py` & `rqalpha-5.3.9/rqalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/__main__.py` & `rqalpha-5.3.9/rqalpha/__main__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/api.py` & `rqalpha-5.3.9/rqalpha/api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/apis/__init__.py` & `rqalpha-5.3.9/rqalpha/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/apis/api_abstract.py` & `rqalpha-5.3.9/rqalpha/apis/api_abstract.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/apis/api_base.py` & `rqalpha-5.3.9/rqalpha/apis/api_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,19 +166,16 @@
         if "99" in order_book_id:
             raise RQInvalidArgument(
                 _(u"Index Future contracts[99] are not supported in paper trading.")
             )
     style = cal_style(price, None)
     market_price = env.get_last_price(order_book_id)
     if not is_valid_price(market_price):
-        user_system_log.warn(
-            _(u"Order Creation Failed: [{order_book_id}] No market data").format(
-                order_book_id=order_book_id
-            )
-        )
+        reason = _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=order_book_id)
+        env.order_creation_failed(order_book_id, reason)
         return
 
     amount = int(amount)
 
     order = Order.__from_create__(
         order_book_id=order_book_id,
         quantity=amount,
```

### Comparing `rqalpha-5.3.8/rqalpha/apis/api_rqdatac.py` & `rqalpha-5.3.9/rqalpha/apis/api_rqdatac.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/apis/names.py` & `rqalpha-5.3.9/rqalpha/apis/names.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/cmds/__init__.py` & `rqalpha-5.3.9/rqalpha/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/cmds/bundle.py` & `rqalpha-5.3.9/rqalpha/cmds/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/cmds/entry.py` & `rqalpha-5.3.9/rqalpha/cmds/entry.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/cmds/misc.py` & `rqalpha-5.3.9/rqalpha/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/cmds/mod.py` & `rqalpha-5.3.9/rqalpha/cmds/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/cmds/run.py` & `rqalpha-5.3.9/rqalpha/cmds/run.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/config.yml` & `rqalpha-5.3.9/rqalpha/config.yml`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/const.py` & `rqalpha-5.3.9/rqalpha/const.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/__init__.py` & `rqalpha-5.3.9/rqalpha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/events.py` & `rqalpha-5.3.9/rqalpha/core/events.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/execution_context.py` & `rqalpha-5.3.9/rqalpha/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/executor.py` & `rqalpha-5.3.9/rqalpha/core/executor.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/global_var.py` & `rqalpha-5.3.9/rqalpha/core/global_var.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/strategy.py` & `rqalpha-5.3.9/rqalpha/core/strategy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/strategy_context.py` & `rqalpha-5.3.9/rqalpha/core/strategy_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/strategy_loader.py` & `rqalpha-5.3.9/rqalpha/core/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/core/strategy_universe.py` & `rqalpha-5.3.9/rqalpha/core/strategy_universe.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/__init__.py` & `rqalpha-5.3.9/rqalpha/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/bar_dict_price_board.py` & `rqalpha-5.3.9/rqalpha/data/bar_dict_price_board.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/base_data_source/__init__.py` & `rqalpha-5.3.9/rqalpha/data/base_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/base_data_source/adjust.py` & `rqalpha-5.3.9/rqalpha/data/base_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/base_data_source/data_source.py` & `rqalpha-5.3.9/rqalpha/data/base_data_source/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from rqalpha.data.base_data_source.storage_interface import (AbstractCalendarStore, AbstractDateSet,
                                 AbstractDayBarStore, AbstractDividendStore,
                                 AbstractInstrumentStore)
 from rqalpha.data.base_data_source.storages import (DateSet, DayBarStore, DividendStore,
                        ExchangeTradingCalendarStore, FutureDayBarStore,
                        FutureInfoStore, FuturesTradingParametersStore,InstrumentStore,
                        ShareTransformationStore, SimpleFactorStore,
-                       YieldCurveStore)
+                       YieldCurveStore, FuturesTradingParameters)
 
 
 BAR_RESAMPLE_FIELD_METHODS = {
     "open": "first",
     "close": "last",
     "iopv": "last",
     "high": "max",
```

### Comparing `rqalpha-5.3.8/rqalpha/data/base_data_source/storage_interface.py` & `rqalpha-5.3.9/rqalpha/data/base_data_source/storage_interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/base_data_source/storages.py` & `rqalpha-5.3.9/rqalpha/data/base_data_source/storages.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/bundle.py` & `rqalpha-5.3.9/rqalpha/data/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/data/data_proxy.py` & `rqalpha-5.3.9/rqalpha/data/data_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,9 +322,7 @@
             return np.nan, 0
         # 存在一些有日线没分钟线的情况,如果不是缺了,通常都是因为volume为0,用日线先判断确认下
         day_bar = self.get_bar(order_book_id=id_or_ins.order_book_id, dt=dt, frequency="1d")
         if day_bar.volume == 0:
             return np.nan, 0
         bar = self._data_source.get_algo_bar(id_or_ins, order_style.start_min, order_style.end_min, dt)
         return (bar[order_style.TYPE], bar["volume"]) if bar else (np.nan, 0)
-
-
```

### Comparing `rqalpha-5.3.8/rqalpha/data/trading_dates_mixin.py` & `rqalpha-5.3.9/rqalpha/data/trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/environment.py` & `rqalpha-5.3.9/rqalpha/environment.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 from datetime import datetime
 from typing import Optional, Dict, List
 from itertools import chain
+from typing import TYPE_CHECKING
 
 import rqalpha
-from rqalpha.core.events import EventBus
+from rqalpha.core.events import EventBus, Event, EVENT
 from rqalpha.const import INSTRUMENT_TYPE
 from rqalpha.utils.logger import system_log, user_log, user_system_log
 from rqalpha.core.global_var import GlobalVars
 from rqalpha.utils.i18n import gettext as _
+if TYPE_CHECKING:
+    from rqalpha.model.order import Order
 
 
 class Environment(object):
     _env = None  # type: Environment
 
     def __init__(self, config, rqdatac_init):
         Environment._env = self
@@ -110,27 +113,40 @@
         else:
             self._default_frontend_validators.append(validator)
 
     def _get_frontend_validators(self, instrument_type):
         return chain(self._frontend_validators.get(instrument_type, []), self._default_frontend_validators)
 
     def submit_order(self, order):
-        instrument_type = self.data_proxy.instrument(order.order_book_id).type
-        account = self.portfolio.get_account(order.order_book_id)
-        if all(v.can_submit_order(order, account) for v in self._get_frontend_validators(instrument_type)):
+        if self.can_submit_order(order):
             self.broker.submit_order(order)
             return order
 
     def can_cancel_order(self, order):
         instrument_type = self.data_proxy.instrument(order.order_book_id).type
         account = self.portfolio.get_account(order.order_book_id)
         for v in chain(self._frontend_validators.get(instrument_type, []), self._default_frontend_validators):
-            if not v.can_cancel_order(order, account):
-                return False
+            try:
+                reason = v.validate_cancellation(order, account)
+                if reason:
+                    self.order_cancellation_failed(order_book_id=order.order_book_id, reason=reason)
+                    return False
+            except NotImplementedError:
+                # 避免由于某些 mod 版本未更新，Validator method 未修改
+                if not v.can_cancel_order(order, account):
+                    return False
         return True
+    
+    def order_creation_failed(self, order_book_id, reason):
+        user_system_log.warn(reason)
+        self.event_bus.publish_event(Event(EVENT.ORDER_CREATION_REJECT, order_book_id=order_book_id, reason=reason))
+
+    def order_cancellation_failed(self, order_book_id, reason):
+        user_system_log.warn(reason)
+        self.event_bus.publish_event(Event(EVENT.ORDER_CANCELLATION_REJECT, order_book_id=order_book_id, reason=reason))
 
     def get_universe(self):
         return self._universe.get()
 
     def update_universe(self, universe):
         self._universe.update(universe)
 
@@ -175,15 +191,22 @@
         return self._get_transaction_cost_decider(order.order_book_id).get_order_transaction_cost(order)
 
     def update_time(self, calendar_dt, trading_dt):
         # type: (datetime, datetime) -> None
         self.calendar_dt = calendar_dt
         self.trading_dt = trading_dt
 
-    def can_submit_order(self, order):
+    def can_submit_order(self, order: 'Order') -> bool:
         # forward compatible
         instrument_type = self.data_proxy.instrument(order.order_book_id).type
         account = self.portfolio.get_account(order.order_book_id)
         for v in self._get_frontend_validators(instrument_type):
-            if not v.can_submit_order(order, account):
-                return False
+            try:
+                reason = v.validate_submission(order, account)
+                if reason:
+                    self.order_creation_failed(order_book_id=order.order_book_id, reason=reason)
+                    return False
+            except NotImplementedError:
+                # 避免由于某些 mod 版本未更新，Validator method 未修改
+                if not v.can_submit_order(order, account):
+                    return False
         return True
```

### Comparing `rqalpha-5.3.8/rqalpha/examples/IF1706_20161108.csv` & `rqalpha-5.3.9/rqalpha/examples/IF1706_20161108.csv`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/IF_macd.py` & `rqalpha-5.3.9/rqalpha/examples/IF_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/buy_and_hold.py` & `rqalpha-5.3.9/rqalpha/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/data_source/get_csv_module.py` & `rqalpha-5.3.9/rqalpha/examples/data_source/get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/data_source/import_get_csv_module.py` & `rqalpha-5.3.9/rqalpha/examples/data_source/import_get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/data_source/read_csv_as_df.py` & `rqalpha-5.3.9/rqalpha/examples/data_source/read_csv_as_df.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py` & `rqalpha-5.3.9/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/extend_api/test_extend_api.py` & `rqalpha-5.3.9/rqalpha/examples/extend_api/test_extend_api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/golden_cross.py` & `rqalpha-5.3.9/rqalpha/examples/golden_cross.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/macd.py` & `rqalpha-5.3.9/rqalpha/examples/macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/pair_trading.py` & `rqalpha-5.3.9/rqalpha/examples/pair_trading.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/rsi.py` & `rqalpha-5.3.9/rqalpha/examples/rsi.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/run_code_demo.py` & `rqalpha-5.3.9/rqalpha/examples/run_code_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/run_func_demo.py` & `rqalpha-5.3.9/rqalpha/examples/run_func_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/subscribe_event.py` & `rqalpha-5.3.9/rqalpha/examples/subscribe_event.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/test_pt.py` & `rqalpha-5.3.9/rqalpha/examples/test_pt.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/examples/turtle.py` & `rqalpha-5.3.9/rqalpha/examples/turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/interface.py` & `rqalpha-5.3.9/rqalpha/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 import abc
 from datetime import datetime, date
-from typing import Any, Union, Optional, Iterable, Dict, List, Sequence
+from typing import Any, Union, Optional, Iterable, Dict, List, Sequence, TYPE_CHECKING
+if TYPE_CHECKING:
+    from rqalpha.portfolio.account import Account
 
 import numpy
 from six import with_metaclass
 import pandas
 
 from rqalpha.utils.typing import DateLike
 from rqalpha.model.tick import TickObject
@@ -645,26 +647,29 @@
 
 class AbstractFrontendValidator(with_metaclass(abc.ABCMeta)):
     """
     前端风控接口，下撤单请求在到达券商代理模块前会经过前端风控。
 
     扩展模块可以通过 env.add_frontend_validator 添加自定义的前端风控逻辑
     """
-
     @abc.abstractmethod
-    def can_submit_order(self, order, account=None):
+    def validate_submission(self, order: Order, account: Optional['Account'] = None) -> Optional[str]:
         """
-        判断是否可以下单
+        进行下单前的验证，若通过则返回 None
+
+        :return: `Optional[str]`
         """
         raise NotImplementedError
-
+    
     @abc.abstractmethod
-    def can_cancel_order(self, order, account=None):
+    def validate_cancellation(self, order: Order, account: Optional['Account'] = None) -> Optional[str]:
         """
-        判读是否可以撤单
+        进行撤销订单前的验证，若通过则返回 None
+
+        :return: `Optional[str]`
         """
         raise NotImplementedError
 
 
 class AbstractTransactionCostDecider((with_metaclass(abc.ABCMeta))):
     """
     订单税费计算接口，通过实现次接口可以定义不同市场、不同合约的个性化税费计算逻辑。
```

### Comparing `rqalpha-5.3.8/rqalpha/main.py` & `rqalpha-5.3.9/rqalpha/main.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,57 +43,55 @@
 def _submit_order(id_or_ins, amount, side, position_effect, style):
     instrument = assure_instrument(id_or_ins)
     order_book_id = instrument.order_book_id
     env = Environment.get_instance()
 
     amount = int(amount)
     if amount == 0:
-        user_system_log.warn(_(
-            u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
-        ).format(order_book_id=order_book_id))
+        reason = _(u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}").format(
+            order_book_id=order_book_id
+        )
+        env.order_creation_failed(order_book_id=order_book_id, reason=reason)
         return None
     if isinstance(style, LimitOrder) and np.isnan(style.get_limit_price()):
         raise RQInvalidArgument(_(u"Limit order price should not be nan."))
 
     if env.config.base.run_type != RUN_TYPE.BACKTEST and instrument.type == INSTRUMENT_TYPE.FUTURE:
         if "88" in order_book_id:
             raise RQInvalidArgument(_(u"Main Future contracts[88] are not supported in paper trading."))
         if "99" in order_book_id:
             raise RQInvalidArgument(_(u"Index Future contracts[99] are not supported in paper trading."))
 
     price = env.get_last_price(order_book_id)
     if not is_valid_price(price):
-        user_system_log.warn(
-            _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=order_book_id)
-        )
+        reason = _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=order_book_id)
+        env.order_creation_failed(order_book_id=order_book_id, reason=reason)
         return
 
-    env = Environment.get_instance()
-
     orders = []
     if position_effect in (POSITION_EFFECT.CLOSE_TODAY, POSITION_EFFECT.CLOSE):
         direction = POSITION_DIRECTION.LONG if side == SIDE.SELL else POSITION_DIRECTION.SHORT
         position = env.portfolio.get_position(order_book_id, direction)  # type: Position
         if position_effect == POSITION_EFFECT.CLOSE_TODAY:
             if amount > position.today_closable:
-                user_system_log.warning(_(
+                reason = _(
                     "Order Creation Failed: "
-                    "close today amount {amount} is larger than today closable quantity {quantity}"
-                ).format(amount=amount, quantity=position.today_closable))
+                    "close today amount {amount} is larger than today closable quantity {quantity}").format(
+                        amount=amount, quantity=position.today_closable)
+                env.order_creation_failed(order_book_id=order_book_id, reason=reason)
                 return []
             orders.append(Order.__from_create__(
                 order_book_id, amount, side, style, POSITION_EFFECT.CLOSE_TODAY
             ))
         else:
             quantity, old_quantity = position.quantity, position.old_quantity
             if amount > quantity:
-                user_system_log.warn(_(
-                    u"Order Creation Failed: close amount {amount} is larger than position quantity {quantity}").format(
-                    amount=amount, quantity=quantity
-                ))
+                reason = _(u"Order Creation Failed: close amount {amount} is larger than position quantity {quantity}").format(
+                    amount=amount, quantity=quantity)
+                env.order_creation_failed(order_book_id=order_book_id, reason=reason)
                 return []
             if amount > old_quantity:
                 if old_quantity != 0:
                     # 如果有昨仓，则创建一个 POSITION_EFFECT.CLOSE 的平仓单
                     orders.append(Order.__from_create__(
                         order_book_id, old_quantity, side, style, POSITION_EFFECT.CLOSE
                     ))
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,17 @@
                                        common_rules, TUPLE_PRICE_OR_STYLE_TYPE, PRICE_OR_STYLE_TYPE)
 from rqalpha.apis.api_base import (assure_instrument, assure_order_book_id,
                                    cal_style, calc_open_close_style)
 from rqalpha.const import (DEFAULT_ACCOUNT_TYPE, EXECUTION_PHASE,
                            INSTRUMENT_TYPE, ORDER_TYPE, POSITION_DIRECTION,
                            POSITION_EFFECT, SIDE)
 from rqalpha.core.execution_context import ExecutionContext
+from rqalpha.core.events import Event, EVENT
 from rqalpha.environment import Environment
-from rqalpha.mod.rqalpha_mod_sys_risk.validators.cash_validator import \
-    is_cash_enough
+from rqalpha.mod.rqalpha_mod_sys_risk.validators.cash_validator import validate_cash
 from rqalpha.model.instrument import IndustryCode as industry_code
 from rqalpha.model.instrument import IndustryCodeItem, Instrument
 from rqalpha.model.instrument import SectorCode as sector_code
 from rqalpha.model.instrument import SectorCodeItem
 from rqalpha.model.order import LimitOrder, MarketOrder, Order, OrderStyle, ALGO_ORDER_STYLES
 from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT, is_valid_price
 from rqalpha.utils.arg_checker import apply_rules, verify_that
@@ -96,72 +96,70 @@
 
 def _submit_order(ins, amount, side, position_effect, style, current_quantity, auto_switch_order_value):
     env = Environment.get_instance()
     if isinstance(style, LimitOrder) and np.isnan(style.get_limit_price()):
         raise RQInvalidArgument(_(u"Limit order price should not be nan."))
     price = env.data_proxy.get_last_price(ins.order_book_id)
     if not is_valid_price(price):
-        user_system_log.warn(
-            _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=ins.order_book_id))
+        reason = _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=ins.order_book_id)
+        env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
         return
 
     if (side == SIDE.BUY and current_quantity != -amount) or (side == SIDE.SELL and current_quantity != abs(amount)):
         # 在融券回测中，需要用买单作为平空，对于此种情况下出现的碎股，亦允许一次性申报卖出
         amount = _round_order_quantity(ins, amount)
 
     if amount == 0:
-        user_system_log.warn(_(
-            u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
-        ).format(order_book_id=ins.order_book_id))
+        reason = _(u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}").format(order_book_id=ins.order_book_id)
+        env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
         return
     order = Order.__from_create__(ins.order_book_id, abs(amount), side, style, position_effect)
     if side == SIDE.BUY and auto_switch_order_value:
         account, position, ins = _get_account_position_ins(ins)
-        if not is_cash_enough(env, order, account.cash):
+        if validate_cash(env, order, account.cash):
             user_system_log.warn(_(
                 "insufficient cash, use all remaining cash({}) to create order"
             ).format(account.cash))
             return _order_value(account, position, ins, account.cash, style)
     return env.submit_order(order)
 
 
 def _order_shares(ins, amount, style, quantity, auto_switch_order_value):
     side, position_effect = (SIDE.BUY, POSITION_EFFECT.OPEN) if amount > 0 else (SIDE.SELL, POSITION_EFFECT.CLOSE)
     return _submit_order(ins, amount, side, position_effect, style, quantity, auto_switch_order_value)
 
 
-def _order_value(account, position, ins, cash_amount, style):
+def _order_value(account, position, ins, cash_amount, style, zero_amount_as_exception=True):
     env = Environment.get_instance()
     if cash_amount > 0:
         cash_amount = min(cash_amount, account.cash)
     if isinstance(style, LimitOrder):
         price = style.get_limit_price()
     else:
         price = env.data_proxy.get_last_price(ins.order_book_id)
         if not is_valid_price(price):
-            user_system_log.warn(
-                _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=ins.order_book_id)
-            )
+            reason = _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=ins.order_book_id)
+            env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
             return
 
     amount = int(Decimal(cash_amount) / Decimal(price))
     round_lot = int(ins.round_lot)
     if cash_amount > 0:
         amount = _round_order_quantity(ins, amount)
         while amount > 0:
             expected_transaction_cost = env.get_order_transaction_cost(Order.__from_create__(
                 ins.order_book_id, amount, SIDE.BUY, LimitOrder(price), POSITION_EFFECT.OPEN
             ))
             if amount * price + expected_transaction_cost <= cash_amount:
                 break
             amount -= round_lot
         else:
-            user_system_log.warn(_(
-                u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
-            ).format(order_book_id=ins.order_book_id))
+            if zero_amount_as_exception:
+                reason = _(u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}").format(order_book_id=ins.order_book_id)
+                env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
             return
 
     if amount < 0:
         amount = max(amount, -position.closable)
 
     return _order_shares(ins, amount, style, position.quantity, auto_switch_order_value=False)
 
@@ -194,28 +192,28 @@
     open_style, close_style = calc_open_close_style(price, style, price_or_style)
     if cash_amount == 0:
         return _submit_order(
             ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, close_style, position.quantity, False
         )
     _delta = cash_amount - position.market_value
     _style = open_style if _delta > 0 else close_style
-    return _order_value(account, position, ins, _delta, _style)
+    return _order_value(account, position, ins, _delta, _style, zero_amount_as_exception=False)
 
 
 @order_target_percent.register(INST_TYPE_IN_STOCK_ACCOUNT)
 def stock_order_target_percent(id_or_ins, percent, price_or_style=None, price=None, style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
     open_style, close_style = calc_open_close_style(price, style, price_or_style)
     if percent == 0:
         return _submit_order(
             ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, close_style, position.quantity, False
         )
     _delta = account.total_value * percent - position.market_value
     _style = open_style if _delta > 0 else close_style
-    return _order_value(account, position, ins, _delta, _style)
+    return _order_value(account, position, ins, _delta, _style, zero_amount_as_exception=False)
 
 
 @order.register(INST_TYPE_IN_STOCK_ACCOUNT)
 def stock_order(order_book_id, quantity, price_or_style=None, price=None, style=None):
     result_order = stock_order_shares(order_book_id, quantity, price, style, price_or_style)
     if result_order:
         return [result_order]
@@ -338,17 +336,16 @@
         if ins.type not in ORDER_TARGET_PORTFOLIO_SUPPORTED_INS_TYPES:
             raise RQInvalidArgument(_(
                 "function order_target_portfolio: invalid instrument type, excepted CS/ETF/LOF/INDX, got {}"
             ).format(ins.order_book_id))
         order_book_id = ins.order_book_id
         last_price = env.data_proxy.get_last_price(order_book_id)
         if not is_valid_price(last_price):
-            user_system_log.warn(
-                _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=order_book_id)
-            )
+            reason = _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=order_book_id)
+            env.order_creation_failed(order_book_id=order_book_id, reason=reason)
             continue
 
         price_or_style = price_or_styles.get(ins.order_book_id)
         open_style, close_style = calc_open_close_style(price=None, style=None, price_or_style=price_or_style)
 
         if percent < 0:
             raise RQInvalidArgument(_(
@@ -376,20 +373,18 @@
 
     account_value = account.total_value
     close_orders, open_orders = [], []
     for order_book_id, (target_percent, open_style, close_style, last_price) in target.items():
         open_price = _get_order_style_price(order_book_id, open_style)
         close_price = _get_order_style_price(order_book_id, close_style)
         if not (is_valid_price(close_price) and is_valid_price(open_price)):
-            user_system_log.warn(_(
-                "Adjust position of {id_or_ins} Failed: "
-                "Invalid close/open price {close_price}/{open_price}").format(
-                    id_or_ins=order_book_id, close_price=close_price, open_price=open_price
-                )
+            reason = _("Adjust position of {id_or_ins} Failed: Invalid close/open price {close_price}/{open_price}").format(
+                id_or_ins=order_book_id, close_price=close_price, open_price=open_price
             )
+            env.order_creation_failed(order_book_id=order_book_id, reason=reason)
             continue
 
         delta_quantity = (account_value * target_percent / close_price) - current_quantities.get(order_book_id, 0)
         delta_quantity = _round_order_quantity(env.data_proxy.instrument(order_book_id), delta_quantity)
         if delta_quantity == 0:
             continue
         elif delta_quantity > 0:
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,22 @@
 class MarginComponentValidator(AbstractFrontendValidator):
     """ 融资融券股票池验证 """
 
     def __init__(self, margin_type="all"):
         self._margin_type = margin_type
         from rqalpha.apis.api_rqdatac import get_margin_stocks
         self._get_margin_stocks = get_margin_stocks
-
-    def can_cancel_order(self, order, account=None):
-        return True
-
-    def can_submit_order(self, order, account=None):
-        # type: (Order, Optional[Account]) -> bool
-
+        
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         # 没负债等于没融资，则不需要限制股票池
         if account.cash_liabilities == 0:
-            return True
-
+            return None
         symbols = self._get_margin_stocks(margin_type=self._margin_type)
-
         # 是否在股票池中
         if order.order_book_id in set(symbols):
-            return True
+            return None
         else:
-            user_system_log.warn("Order Creation Failed: margin stock pool not contains {}.".format(
-                order.order_book_id)
-            )
-            return False
+            reason = "Order Creation Failed: margin stock pool not contains {}.".format(order.order_book_id)
+            return reason
+    
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,36 +23,35 @@
 from rqalpha.model.order import Order
 from rqalpha.portfolio.account import Account
 
 from rqalpha.utils.i18n import gettext as _
 
 
 class PositionValidator(AbstractFrontendValidator):
-    def can_cancel_order(self, order, account=None):
-        return True
-
-    def can_submit_order(self, order, account=None):
-        # type: (Order, Optional[Account]) -> bool
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
+    
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         if account is None:
-            return True
+            return None
         if order.position_effect in (POSITION_EFFECT.OPEN, POSITION_EFFECT.EXERCISE):
-            return True
+            return None
         position = account.get_position(order.order_book_id, order.position_direction)  # type: AbstractPosition
         if order.position_effect == POSITION_EFFECT.CLOSE_TODAY and order.quantity > position.today_closable:
-            user_system_log.warn(_(
+            reason = _(
                 "Order Creation Failed: not enough today position {order_book_id} to close, target"
                 " quantity is {quantity}, closable today quantity is {closable}").format(
                 order_book_id=order.order_book_id,
                 quantity=order.quantity,
                 closable=position.today_closable,
-            ))
-            return False
+            )
+            return reason
         if order.position_effect == POSITION_EFFECT.CLOSE and order.quantity > position.closable:
-            user_system_log.warn(_(
+            reason = _(
                 "Order Creation Failed: not enough position {order_book_id} to close or exercise, target"
                 " sell quantity is {quantity}, closable quantity is {closable}").format(
                 order_book_id=order.order_book_id,
                 quantity=order.quantity,
                 closable=position.closable,
-            ))
-            return False
-        return True
+            )
+            return reason
+        return None
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,20 +5,16 @@
 from rqalpha.model.order import Order
 from rqalpha.portfolio.account import Account
 
 
 class MarginInstrumentValidator(AbstractFrontendValidator):
     """ 融资下单品种限制: 当开启股票池限制且有融资余额时只能交易股票和ETF """
 
-    def can_cancel_order(self, order, account=None):
-        return True
-
-    def can_submit_order(self, order, account=None):
-        # type: (Order, Optional[Account]) -> bool
-
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         if account.cash_liabilities > 0:
-            user_system_log.warn("Order Creation Failed: cash liabilities > 0, {} not support submit order".format(
-                order.order_book_id)
-            )
-            return False
+            reason = "Order Creation Failed: cash liabilities > 0, {} not support submit order".format(order.order_book_id)
+            return reason
         else:
-            return True
+            return None
+    
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from rqrisk import Risk, WEEKLY, MONTHLY
 
 from rqalpha.const import EXIT_CODE, DEFAULT_ACCOUNT_TYPE, INSTRUMENT_TYPE, POSITION_DIRECTION
 from rqalpha.core.events import EVENT
 from rqalpha.interface import AbstractMod, AbstractPosition
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils import INST_TYPE_IN_STOCK_ACCOUNT
+from rqalpha.utils.datetime_func import convert_int_to_date
 from rqalpha.utils.logger import user_system_log
 from rqalpha.const import DAYS_CNT
 from rqalpha.api import export_as_api
 from .plot.consts import DefaultPlot, PLOT_TEMPLATE
 from .plot.utils import max_ddd as _max_ddd
 from .plot_store import PlotStore
 
@@ -127,31 +128,68 @@
             bar = self._env.data_proxy.get_bar(benchmark[0], self._env.calendar_dt, '1d')
             if bar.close != bar.close:
                 daily_return_list.append((0.0, benchmark[1]))
             else:
                 daily_return_list.append((bar.close / bar.prev_close - 1.0, benchmark[1]))
             weights += benchmark[1]
         return sum([daily[0] * daily[1] / weights for daily in daily_return_list])
-
-    def _subscribe_events(self, event):
-        if self._benchmark:
-            _s = self._env.config.base.start_date
-            _e = self._env.config.base.end_date
-            for order_book_id, weight in self._benchmark:
-                ins = self._env.data_proxy.instrument(order_book_id)
-                if ins is None:
-                    raise RuntimeError(
-                        _("benchmark {} not exists, please entry correct order_book_id").format(order_book_id)
-                    )
-                if ins.listed_date.date() > _s or ins.de_listed_date.date() <= _e:
-                    raise RuntimeError(
-                        _("benchmark {} listed date {} > backtest start date {} or de_listed date {} <= backtest end "
-                          "date {}").format(order_book_id, ins.listed_date.date(), _s, ins.de_listed_date.date(), _e)
+    
+    def generate_benchmark_daily_returns_and_portfolio(self, event):
+        _s = self._env.config.base.start_date
+        _e = self._env.config.base.end_date
+        trading_dates = self._env.data_proxy.get_trading_dates(_s, _e)
+        if self._benchmark is None:
+            self._benchmark_daily_returns = list(np.full(len(trading_dates), np.nan))
+            return
+        
+        # generate benchmerk daily returns
+        self._benchmark_daily_returns = np.zeros(len(trading_dates))
+        weights = 0
+        for order_book_id, weight in self._benchmark:
+            ins = self._env.data_proxy.instrument(order_book_id)
+            if ins is None:
+                raise RuntimeError(
+                    _("benchmark {} not exists, please entry correct order_book_id").format(order_book_id)
+                )
+            bars = self._env.data_proxy.history_bars(
+                order_book_id = order_book_id,
+                bar_count = len(trading_dates) + 1,  # Get an extra day for calculation
+                frequency = "1d",
+                field = ["datetime", "close"],
+                dt = _e,
+                skip_suspended=False,
+            )
+            if len(bars) == len(trading_dates) + 1:
+                if convert_int_to_date(bars[1]['datetime']).date() != _s:
+                    raise RuntimeError(_(
+                        "benchmark {} missing data between backtest start date {} and end date {}").format(order_book_id, _s, _e)
                     )
+                daily_returns = (bars['close'] / np.roll(bars['close'], 1) - 1.0)[1: ]
+                self._benchmark_daily_returns = self._benchmark_daily_returns + daily_returns * weight
+                weights += weight
+            else:
+                if len(bars) == 0:
+                    (available_s, available_e) = (ins.listed_date, ins.de_listed_date)
+                else:
+                    (available_s, available_e) = (convert_int_to_date(bars[0]['datetime']).date(), convert_int_to_date(bars[-1]['datetime']).date())
+                raise RuntimeError(
+                    _("benchmark {} available data start date {} >= backtest start date {} or end date {} <= backtest end "
+                    "date {}").format(order_book_id, available_s, _s, available_e, _e)
+                )
+        self._benchmark_daily_returns = self._benchmark_daily_returns / weight
+        
+        # generate benchmark portfolio
+        unit_net_value = (self._benchmark_daily_returns + 1).cumprod()
+        self._total_benchmark_portfolios = {
+            "date": trading_dates,
+            "unit_net_value": unit_net_value
+        }
 
+    def _subscribe_events(self, event):
+        self._env.event_bus.add_listener(EVENT.BEFORE_STRATEGY_RUN, self.generate_benchmark_daily_returns_and_portfolio)
         self._env.event_bus.add_listener(EVENT.TRADE, self._collect_trade)
         self._env.event_bus.add_listener(EVENT.ORDER_CREATION_PASS, self._collect_order)
         self._env.event_bus.prepend_listener(EVENT.POST_SETTLEMENT, self._collect_daily)
 
     def _collect_trade(self, event):
         self._trades.append(self._to_trade_record(event.trade))
 
@@ -160,19 +198,14 @@
 
     def _collect_daily(self, _):
         date = self._env.calendar_dt.date()
         portfolio = self._env.portfolio
 
         self._portfolio_daily_returns.append(portfolio.daily_returns)
         self._total_portfolios.append(self._to_portfolio_record(date, portfolio))
-        self._benchmark_daily_returns.append(self.get_benchmark_daily_returns())
-        self._total_benchmark_portfolios.append({
-            "date": date,
-            "unit_net_value": (np.array(self._benchmark_daily_returns) + 1).prod()
-        })
         self._daily_pnl.append(portfolio.daily_pnl)
 
         for account_type, account in self._env.portfolio.accounts.items():
             self._sub_accounts[account_type].append(self._to_account_record(date, account))
             pos_dict = {}
             for pos in account.get_positions():
                 pos_dict.setdefault(pos.order_book_id, {})[pos.direction] = pos
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,27 +66,29 @@
 
 
 class VerticalSeriesSchema(SheetSchema):
     def fill_worksheet(self, ws: Worksheet, data: Dict[str, List]):
         if not data:
             for key, (row, column, style) in self._cell_map.items():
                 self._write_cell(ws, row, column, None, style)
-        for key, (row, column, style) in self._cell_map.items():
-            for i, item in enumerate(data.get(key, [])):
-                self._write_cell(ws, row + i, column, item, style)
+        else:
+            for key, (row, column, style) in self._cell_map.items():
+                for i, item in enumerate(data.get(key, [])):
+                    self._write_cell(ws, row + i, column, item, style)
 
 
 class SummaryTemplate(ExcelTemplate):
     TEMPLATE_NAME = "summary"
     SCHEMA_CLASSES = {
         "概览": SingleCellSchema,
         "年度指标": VerticalSeriesSchema,
         "月度收益": VerticalSeriesSchema,
         "月度超额收益（几何）": VerticalSeriesSchema,
         "个股权重": VerticalSeriesSchema,
+        "压力测试": VerticalSeriesSchema,
     }
 
 
 SUMMARY_TEMPLATE = SummaryTemplate()
 
 
 def generate_xlsx_reports(data, output_path):
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,41 +13,45 @@
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 import os
 from typing import Dict, Optional
+import datetime
 
 import numpy
 import pandas
-from collections import ChainMap
+from collections import ChainMap, defaultdict
 from pandas import Series, DataFrame
 
 from rqrisk import Risk
 from rqrisk import WEEKLY, MONTHLY
+from rqalpha.environment import Environment
 
 from rqalpha.mod.rqalpha_mod_sys_analyser.plot.utils import max_dd as _max_dd
 from rqalpha.mod.rqalpha_mod_sys_analyser.report.excel_template import generate_xlsx_reports
 
 
+PRESSURE_TEST_PERIOD = {
+    "打击壳价值": (datetime.date(2016, 11, 1), datetime.date(2018, 2, 1)),
+    "公募基金抱团": (datetime.date(2020, 10, 9), datetime.date(2021, 3, 1)),
+    "行业风格切换": (datetime.date(2021, 9, 1), datetime.date(2021, 12, 31)),
+    "小盘踩踏危机": (datetime.date(2024, 1, 5), datetime.date(2024, 2, 8)),
+}
+
+
 def _returns(unit_net_value: Series):
     return (unit_net_value / unit_net_value.shift(1).fillna(1)).fillna(0) - 1
 
 
 def _yearly_indicators(
         p_nav: Series, p_returns: Series, b_nav: Optional[Series], b_returns: Optional[Series], risk_free_rates: Dict
 ):
-    data = {field: [] for field in [
-        "year", "returns", "benchmark_returns", "geometric_excess_return", "geometric_excess_drawdown",
-        "geometric_excess_drawdown_days", "excess_annual_volatility", "annual_volatility", "sharpe_ratio",
-        "excess_sharpe",
-        "information_ratio", "annual_tracking_error", "weekly_excess_win_rate", "monthly_excess_win_rate",
-        "max_drawdown", "max_drawdown_days"
-    ]}
+    data = defaultdict(list)
 
     for year, p_year_returns in p_returns.groupby(p_returns.index.year):  # noqa
         year_slice = p_returns.index.year == year  # noqa
         if b_nav is not None:
             # 周胜率
             b_year_returns = b_returns[year_slice]
             weekly_p_returns = _returns(p_nav[year_slice].resample("W").last().dropna())
@@ -110,14 +114,52 @@
 
 
 def _gen_positions_weight(df):
     rename = {"{}%".format(i): "percent_{}".format(i) for i in [25, 50, 75]}
     return df.reset_index().rename(columns=rename).to_dict(orient="list")
 
 
+def _pressure_test(
+        p_nav: Series, p_returns: Series, b_nav: Optional[Series], b_returns: Optional[Series]
+    ):
+    env = Environment.get_instance()
+    # data = {field: [] for field in [
+    #     "title", "start_date", "end_date", "returns", "annual_return", "geometric_excess_return", "max_drawdown",
+    #     "geometric_excess_drawdown", "sharpe", "excess_sharpe"
+    # ]}
+    data = defaultdict(list)
+    
+    for title, (start, end) in PRESSURE_TEST_PERIOD.items():
+        p_period_returns = p_returns.loc[start: end]
+        if (p_period_returns is None or p_period_returns.empty):
+            continue
+        # 当且仅当回测周期完整包含压力测试的一个区间时才展示该区间的表现
+        if len(p_period_returns) != len(env.data_proxy.get_trading_dates(start, end)):
+            continue
+        if b_nav is not None:
+            b_period_returns = b_returns.loc[start: end]
+        else:
+            b_period_returns = Series(index=p_period_returns.index)
+        risk_free_rate = env.data_proxy.get_risk_free_rate(start, end)
+        risk = Risk(p_period_returns, b_period_returns, risk_free_rate)
+        data["title"].append(title)
+        data["start_date"].append(str(start))
+        data["end_date"].append(str(end))
+        data["returns"].append(risk.return_rate)
+        data["annual_return"].append(risk.annual_return)
+        data["geometric_excess_return"].append(risk.geometric_excess_return)
+        data["max_drawdown"].append(risk.max_drawdown)
+        data["geometric_excess_drawdown"].append(risk.geometric_excess_drawdown)
+        data["sharpe"].append(risk.sharpe)
+        data["excess_sharpe"].append(risk.excess_sharpe)
+    if not data["title"]:
+        return None
+    return data
+
+
 def generate_report(result_dict, output_path):
     from six import StringIO
 
     try:
         os.mkdir(output_path)
     except:
         pass
@@ -134,14 +176,15 @@
         b_nav = b_returns = None
     generate_xlsx_reports({
         "概览": summary,
         "年度指标": _yearly_indicators(p_nav, p_returns, b_nav, b_returns, result_dict["yearly_risk_free_rates"]),
         "月度收益": _monthly_returns(p_returns),
         "月度超额收益（几何）": _monthly_geometric_excess_returns(p_returns, b_returns),
         "个股权重": _gen_positions_weight(result_dict["positions_weight"]),
+        "压力测试": _pressure_test(p_nav, p_returns, b_nav, b_returns),
     }, output_path)
 
     for name in ["portfolio", "stock_account", "future_account",
                  "stock_positions", "future_positions", "trades", "positions_weight"]:
         try:
             df = result_dict[name]
         except KeyError:
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_progress/mod.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/mod.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,44 +10,43 @@
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
+from typing import Optional
 
 from rqalpha.interface import AbstractFrontendValidator
 from rqalpha.const import POSITION_EFFECT
-from rqalpha.utils.logger import user_system_log
+from rqalpha.model.order import Order
+from rqalpha.portfolio.account import Account
+from rqalpha.environment import Environment
 
 from rqalpha.utils.i18n import gettext as _
 
 
-def is_cash_enough(env, order, cash, warn=False):
+def validate_cash(env: Environment, order: Order, cash: float) -> Optional[str]:
     instrument = env.data_proxy.instrument(order.order_book_id)
     cost_money = instrument.calc_cash_occupation(order.frozen_price, order.quantity, order.position_direction, order.trading_datetime.date())
     cost_money += env.get_order_transaction_cost(order)
     if cost_money <= cash:
-        return True
-    if warn:
-        user_system_log.warn(
-            _("Order Creation Failed: not enough money to buy {order_book_id}, needs {cost_money:.2f},"
-              " cash {cash:.2f}").format(
-                order_book_id=order.order_book_id,
-                cost_money=cost_money,
-                cash=cash,
-            )
-        )
-    return False
+        return None
+    reason = _("Order Creation Failed: not enough money to buy {order_book_id}, needs {cost_money:.2f},"
+               " cash {cash:.2f}").format(
+                   order_book_id=order.order_book_id,
+                   cost_money=cost_money,
+                   cash=cash)
+    return reason
 
 
 class CashValidator(AbstractFrontendValidator):
     def __init__(self, env):
         self._env = env
 
-    def can_submit_order(self, order, account=None):
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
+    
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         if (account is None) or (order.position_effect != POSITION_EFFECT.OPEN):
-            return True
-        return is_cash_enough(self._env, order, account.cash, warn=True)
-
-    def can_cancel_order(self, order, account=None):
-        return True
+            return None
+        return validate_cash(self._env, order, account.cash)
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,38 +10,40 @@
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
+from typing import Optional
 
 from rqalpha.interface import AbstractFrontendValidator
 
+from rqalpha.model.order import Order
+from rqalpha.portfolio.account import Account
 from rqalpha.utils.logger import user_system_log
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.const import INSTRUMENT_TYPE
 
 
 class IsTradingValidator(AbstractFrontendValidator):
     def __init__(self, env):
         self._env = env
-
-    def can_submit_order(self, order, account=None):
+    
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         instrument = self._env.data_proxy.instrument(order.order_book_id)
         if instrument.type != INSTRUMENT_TYPE.INDX and not instrument.listing_at(self._env.trading_dt):
-            user_system_log.warn(_(u"Order Creation Failed: {order_book_id} is not listing!").format(
-                order_book_id=order.order_book_id,
-            ))
-            return False
+            reason = _(u"Order Creation Failed: {order_book_id} is not listing!").format(
+                order_book_id=order.order_book_id)
+            return reason
 
         if instrument.type == 'CS' and self._env.data_proxy.is_suspended(order.order_book_id, self._env.trading_dt):
-            user_system_log.warn(_(u"Order Creation Failed: security {order_book_id} is suspended on {date}").format(
+            reason = _(u"Order Creation Failed: security {order_book_id} is suspended on {date}").format(
                 order_book_id=order.order_book_id,
                 date=self._env.trading_dt.date()
-            ))
-            return False
-
-        return True
+            )
+            return reason
 
-    def can_cancel_order(self, order, account=None):
-        return True
+        return None
+    
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,55 +7,54 @@
 #         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
-
+from typing import Optional
 
 from rqalpha.interface import AbstractFrontendValidator
 from rqalpha.const import ORDER_TYPE, POSITION_EFFECT
+from rqalpha.model.order import Order
+from rqalpha.portfolio.account import Account
 from rqalpha.utils.logger import user_system_log
 
 from rqalpha.utils.i18n import gettext as _
 
 
 class PriceValidator(AbstractFrontendValidator):
     def __init__(self, env):
         self._env = env
-
-    def can_submit_order(self, order, account=None):
+    
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         if (order.type != ORDER_TYPE.LIMIT) or (order.position_effect == POSITION_EFFECT.EXERCISE):
-            return True
-
+            return None
+        
         # FIXME: it may be better to round price in data source
         limit_up = round(self._env.price_board.get_limit_up(order.order_book_id), 4)
         if order.price > limit_up:
             reason = _(
                 "Order Creation Failed: limit order price {limit_price} is higher "
                 "than limit up {limit_up}, order_book_id={order_book_id}"
             ).format(
                 order_book_id=order.order_book_id,
                 limit_price=order.price,
                 limit_up=limit_up
             )
-            user_system_log.warn(reason)
-            return False
+            return reason
 
         limit_down = round(self._env.price_board.get_limit_down(order.order_book_id), 4)
         if order.price < limit_down:
             reason = _(
                 "Order Creation Failed: limit order price {limit_price} is lower "
                 "than limit down {limit_down}, order_book_id={order_book_id}"
             ).format(
                 order_book_id=order.order_book_id,
                 limit_price=order.price,
                 limit_down=limit_down
             )
-            user_system_log.warn(reason)
-            return False
-
-        return True
+            return reason
+        return None
 
-    def can_cancel_order(self, order, account=None):
-        return True
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,42 +7,41 @@
 #         遵守 Apache License 2.0（下称“Apache 2.0 许可”），您可以在以下位置获得 Apache 2.0 许可的副本：http://www.apache.org/licenses/LICENSE-2.0。
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
-
+from typing import Optional
 
 from rqalpha.interface import AbstractFrontendValidator
 from rqalpha.const import ORDER_TYPE, SIDE, POSITION_EFFECT
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils.logger import user_system_log
+from rqalpha.model.order import Order
+from rqalpha.portfolio.account import Account
 
 
 class SelfTradeValidator(AbstractFrontendValidator):
     def __init__(self, env):
         self._env = env
 
-    def can_submit_order(self, order, account=None):
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         open_orders = [o for o in self._env.get_open_orders(order.order_book_id) if (
                 o.side != order.side and o.position_effect != POSITION_EFFECT.EXERCISE
         )]
         if len(open_orders) == 0:
-            return True
+            return None
         reason = _("Create order failed, there are active orders leading to the risk of self-trade: [{}...]")
         if order.type == ORDER_TYPE.MARKET:
-            user_system_log.warn(reason.format(open_orders[0]))
-            return False
+            return reason.format(open_orders[0])
         if order.side == SIDE.BUY:
             for open_order in open_orders:
                 if order.price >= open_order.price:
-                    user_system_log.warn(reason.format(open_order))
-                    return False
+                    return reason.format(open_order)
         else:
             for open_order in open_orders:
                 if order.price <= open_order.price:
-                    user_system_log.warn(reason.format(open_order))
-                    return False
-
-    def can_cancel_order(self, order, account=None):
-        return True
+                    return reason.format(open_order)
+    
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import Optional
 
-from rqalpha.model.order import ALGO_ORDER_STYLES
+from rqalpha.model.order import ALGO_ORDER_STYLES, Order
 from rqalpha.interface import AbstractFrontendValidator
+from rqalpha.portfolio.account import Account
 
 
 class OrderStyleValidator(AbstractFrontendValidator):
 
     def __init__(self, frequency):
         self._frequency = frequency
 
-    def can_submit_order(self, order, account=None):
+    def validate_submission(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
         if isinstance(order.style, ALGO_ORDER_STYLES) and self._frequency in ["1m", "tick"]:
-            raise RuntimeError("algo order no support 1m or tick frequency")
-        return True
-
-    def can_cancel_order(self, order, account=None):
-        return True
-
+            raise RuntimeError("algo order no support 1m and tick frequency")
+        return None
+    
+    def validate_cancellation(self, order: Order, account: Optional[Account] = None) -> Optional[str]:
+        return None
+
```

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py` & `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/mod/utils.py` & `rqalpha-5.3.9/rqalpha/mod/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/model/__init__.py` & `rqalpha-5.3.9/rqalpha/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/model/bar.py` & `rqalpha-5.3.9/rqalpha/model/bar.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/model/instrument.py` & `rqalpha-5.3.9/rqalpha/model/instrument.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/model/order.py` & `rqalpha-5.3.9/rqalpha/model/order.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/model/tick.py` & `rqalpha-5.3.9/rqalpha/model/tick.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/model/trade.py` & `rqalpha-5.3.9/rqalpha/model/trade.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/portfolio/__init__.py` & `rqalpha-5.3.9/rqalpha/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/portfolio/account.py` & `rqalpha-5.3.9/rqalpha/portfolio/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 
     def register_event(self):
         event_bus = self._env.event_bus
         event_bus.add_listener(
             EVENT.TRADE, lambda e: self.apply_trade(e.trade, e.order) if e.account == self else None
         )
         event_bus.add_listener(EVENT.ORDER_PENDING_NEW, self._on_order_pending_new)
-        event_bus.add_listener(EVENT.ORDER_CREATION_REJECT, self._on_order_unsolicited_update)
         event_bus.add_listener(EVENT.ORDER_UNSOLICITED_UPDATE, self._on_order_unsolicited_update)
         event_bus.add_listener(EVENT.ORDER_CANCELLATION_PASS, self._on_order_unsolicited_update)
 
         event_bus.add_listener(EVENT.PRE_BEFORE_TRADING, self._on_before_trading)
         event_bus.add_listener(EVENT.SETTLEMENT, self._on_settlement)
         event_bus.add_listener(EVENT.POST_SETTLEMENT, self._post_settlement)
```

### Comparing `rqalpha-5.3.8/rqalpha/portfolio/position.py` & `rqalpha-5.3.9/rqalpha/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/resource/ricequant-logo.png` & `rqalpha-5.3.9/rqalpha/resource/ricequant-logo.png`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/user_module.py` & `rqalpha-5.3.9/rqalpha/user_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/__init__.py` & `rqalpha-5.3.9/rqalpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/arg_checker.py` & `rqalpha-5.3.9/rqalpha/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/class_helper.py` & `rqalpha-5.3.9/rqalpha/utils/class_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/click_helper.py` & `rqalpha-5.3.9/rqalpha/utils/click_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/concurrent.py` & `rqalpha-5.3.9/rqalpha/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/config.py` & `rqalpha-5.3.9/rqalpha/utils/config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/datetime_func.py` & `rqalpha-5.3.9/rqalpha/utils/datetime_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/dict_func.py` & `rqalpha-5.3.9/rqalpha/utils/dict_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/exception.py` & `rqalpha-5.3.9/rqalpha/utils/exception.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/functools.py` & `rqalpha-5.3.9/rqalpha/utils/functools.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/i18n.py` & `rqalpha-5.3.9/rqalpha/utils/i18n.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/log_capture.py` & `rqalpha-5.3.9/rqalpha/utils/log_capture.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/logger.py` & `rqalpha-5.3.9/rqalpha/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/package_helper.py` & `rqalpha-5.3.9/rqalpha/utils/package_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/persisit_helper.py` & `rqalpha-5.3.9/rqalpha/utils/persisit_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/repr.py` & `rqalpha-5.3.9/rqalpha/utils/repr.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/risk_free_helper.py` & `rqalpha-5.3.9/rqalpha/utils/risk_free_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/rq_json.py` & `rqalpha-5.3.9/rqalpha/utils/rq_json.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/strategy_loader_help.py` & `rqalpha-5.3.9/rqalpha/utils/strategy_loader_help.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/testing/__init__.py` & `rqalpha-5.3.9/rqalpha/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/testing/fixtures.py` & `rqalpha-5.3.9/rqalpha/utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/testing/mocking.py` & `rqalpha-5.3.9/rqalpha/utils/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/translations/__init__.py` & `rqalpha-5.3.9/rqalpha/utils/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py` & `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo` & `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-01-19 17:56+0800\n"
+"POT-Creation-Date: 2024-04-12 15:23+0800\n"
 "PO-Revision-Date: 2016-10-24 21:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -283,14 +283,17 @@
 msgstr ""
 "订单创建失败：{order_book_id} 的今仓不足，目标平今仓量为 {quantity}，可平今仓"
 "量为 {closable}"
 
 msgid "Order Creation Failed: security {order_book_id} is suspended on {date}"
 msgstr "订单创建失败: {order_book_id} 在 {date} 时停牌"
 
+msgid "Order Creation Failed: {order_book_id} is not listing!"
+msgstr "订单创建失败: {order_book_id} 未上市或已退市"
+
 msgid "Order Rejected: {order_book_id} can not match. Market close."
 msgstr "订单被拒单: {order_book_id} 当天交易结束，订单无法成交。"
 
 msgid ""
 "Order was separated, original order: {original_order_repr}, new orders: "
 "[{new_orders_repr}]"
 msgstr "订单被拆分，原订单：{original_order_repr}，新订单：[{new_orders_repr}]"
@@ -412,22 +415,26 @@
 msgid "[sys_analyser] Generate report from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件生成报告"
 
 msgid "[sys_analyser] Plot from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件绘制收益图"
 
 msgid ""
-"benchmark {} listed date {} > backtest start date {} or de_listed date {} <= "
-"backtest end date {}"
+"benchmark {} available data start date {} >= backtest start date {} or end "
+"date {} <= backtest end date {}"
 msgstr ""
-"基准标的({})上市日期({})晚于回测起始日期({})或退市日期({})早于回测结束日期"
-"({})"
+"基准标的 {} 的可用行情数据开始日期 {} >= 回测起始日期 {} 或结束日期 {} <= 回"
+"测结束日期 {}"
+
+msgid ""
+"benchmark {} missing data between backtest start date {} and end date {}"
+msgstr "基准标的 {} 在回测起始日期 {} 结束日期 {} 间缺失数据"
 
 msgid "benchmark {} not exists, please entry correct order_book_id"
-msgstr "基准标的({})信息不存在，请输入正确的标的代码"
+msgstr "基准标的 {} 信息不存在，请输入正确的标的代码"
 
 msgid "bundle not exist, use \"rqalpha create-bundle\" command instead"
 msgstr "bundle 不存在，执行 \"rqalpha create-bundle\" 以创建 bundle"
 
 msgid "bundle's day bar is incomplete, please update bundle"
 msgstr "Bundle日线数据不完整，请及时更新bundle"
 
@@ -457,14 +464,21 @@
 msgid ""
 "function order_target_portfolio: invalid instrument type, excepted CS/ETF/"
 "LOF/INDX, got {}"
 msgstr ""
 "函数 order_target_portfolio：不合法的资产类型。应传入股票、ETF、LOF 或指数，"
 "实际传入了 {}。"
 
+msgid ""
+"function order_target_portfolio: invalid values of target_portfolio, "
+"excepted float between 0 and 1, got {} (key: {})"
+msgstr ""
+"函数 order_target_portfolio：不合法的目标权重，应传入 0 和 1 之间的浮点数，实"
+"际传入了 {}（类型：{}）。"
+
 msgid "function {} is not supported, please check your account or mod config"
 msgstr ""
 "不支持 API {}。请确保您设置了该 API 所需的账户并开启了包含该 API 实现的 Mod"
 
 msgid ""
 "function {}: invalid {} argument, expected an order_book_id or instrument "
 "with types {}, got {} (type: {})"
```

### Comparing `rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po` & `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-01-19 17:56+0800\n"
+"POT-Creation-Date: 2024-04-12 15:23+0800\n"
 "PO-Revision-Date: 2016-10-24 21:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.13.1\n"
 
-#: rqalpha/environment.py:70
+#: rqalpha/environment.py:74
 msgid ""
 "Environment has not been created. Please Use `Environment.get_instance()`"
 " after RQAlpha init"
 msgstr "Environment 并没有被创建，请再 RQAlpha 初始化之后使用 `Environment.get_instance() 函数`"
 
-#: rqalpha/environment.py:163
+#: rqalpha/environment.py:180
 msgid "No such transaction cost decider, order_book_id = {}"
 msgstr ""
 
 #: rqalpha/main.py:60
 msgid ""
 "There is no data between {start_date} and {end_date}. Please check your "
 "data bundle or select other backtest period."
@@ -36,52 +36,52 @@
 
 #: rqalpha/main.py:79
 msgid ""
 "Missing persist provider. You need to set persist_provider before use "
 "persist"
 msgstr "Persist provider 未加载，加载 Persist provider 方可使用 persist 功能。"
 
-#: rqalpha/main.py:126
+#: rqalpha/main.py:127
 msgid "rqdatac init failed, some apis will not function properly: {}"
 msgstr ""
 "rqdatac 初始化失败，部分扩展 API 可能无法使用，错误信息：{}。您可以访问 "
 "https://www.ricequant.com/welcome/rqdata 获取 rqdatac"
 
-#: rqalpha/main.py:219
+#: rqalpha/main.py:220
 msgid "system restored"
 msgstr ""
 
-#: rqalpha/main.py:249
+#: rqalpha/main.py:250
 msgid "strategy run successfully, normal exit"
 msgstr "策略运行成功，正常退出"
 
-#: rqalpha/main.py:254
+#: rqalpha/main.py:255
 msgid "strategy execute exception"
 msgstr "策略运行产生异常"
 
-#: rqalpha/apis/api_base.py:69 rqalpha/apis/api_base.py:286
-#: rqalpha/apis/api_base.py:322
+#: rqalpha/apis/api_base.py:69 rqalpha/apis/api_base.py:283
+#: rqalpha/apis/api_base.py:319
 msgid "unsupported order_book_id type"
 msgstr "不支持该 order_book_id 类型"
 
 #: rqalpha/apis/api_base.py:164
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:59
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:60
 msgid "Main Future contracts[88] are not supported in paper trading."
 msgstr "期货主力连续合约[88] 在实盘模拟中暂不支持。"
 
 #: rqalpha/apis/api_base.py:168
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:61
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:62
 msgid "Index Future contracts[99] are not supported in paper trading."
 msgstr "期货指数连续合约[99] 在实盘模拟中暂不支持。"
 
-#: rqalpha/apis/api_base.py:174
+#: rqalpha/apis/api_base.py:173
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:66
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:104
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:142
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:346
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:103
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:140
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:343
 msgid "Order Creation Failed: [{order_book_id}] No market data"
 msgstr "订单创建失败: 当前合约[{order_book_id}]没有市场数据。"
 
 #: rqalpha/apis/api_rqdatac.py:50
 msgid "rqdatac is not available, extension apis will not function properly"
 msgstr ""
 "rqdatac 不存在，扩展 API 无法使用，您可以访问 https://www.ricequant.com/welcome/rqdata 获取"
@@ -259,27 +259,27 @@
 msgid "not run {}({}, {}) because strategy is hold"
 msgstr "策略暂停中，取消执行 {}({}, {})"
 
 #: rqalpha/core/strategy.py:53
 msgid "deprecated parameter[bar_dict] in before_trading function."
 msgstr "[Deprecated]在before_trading函数中，第二个参数bar_dict已经不再使用了。"
 
-#: rqalpha/data/bundle.py:454
+#: rqalpha/data/bundle.py:460
 msgid ""
 "RQAlpha already supports backtesting using futures historical margins and"
 " rates, please upgrade RQDatac to version 2.11.12 and above to use it"
 msgstr "RQAlpha 已支持使用期货历史保证金和费率进行回测，请将 RQDatac 升级至 2.11.12 及以上版本进行使用"
 
-#: rqalpha/data/bundle.py:464 rqalpha/data/bundle.py:522
+#: rqalpha/data/bundle.py:470 rqalpha/data/bundle.py:531
 msgid ""
 "Futures historical trading parameters data is being updated, please "
 "wait......"
 msgstr "正在更新期货历史交易参数，请稍后......"
 
-#: rqalpha/data/bundle.py:516
+#: rqalpha/data/bundle.py:522 rqalpha/data/bundle.py:706
 msgid ""
 "File {} update failed, if it is using, please update later, or you can "
 "delete then update again"
 msgstr "{} 文件更新失败，如果其正在使用中，请稍后再进行更新，或者您可以将其删除后再重新更新"
 
 #: rqalpha/data/base_data_source/data_source.py:140
 msgid ""
@@ -301,20 +301,20 @@
 "Your bundle data is too old, please use 'rqalpha update-bundle' or "
 "'rqalpha download-bundle' to update it to lastest before using"
 msgstr ""
 "您的 Bundle 数据过旧，请使用 'rqalpha update-bundle' 或 'rqalpha download-bundle' "
 "将其更新至最新后再进行使用"
 
 #: rqalpha/data/base_data_source/storages.py:97
-#: rqalpha/data/base_data_source/storages.py:123
+#: rqalpha/data/base_data_source/storages.py:124
 msgid "unsupported future instrument {}"
 msgstr "不支持的期货标的{}"
 
-#: rqalpha/data/base_data_source/storages.py:194
-#: rqalpha/data/base_data_source/storages.py:204
+#: rqalpha/data/base_data_source/storages.py:195
+#: rqalpha/data/base_data_source/storages.py:205
 msgid ""
 "open data bundle failed, you can remove {} and try to regenerate bundle: "
 "{}"
 msgstr "读取 bundle 文件失败，请删除 {} 后尝试重新生成 bundle：{}"
 
 #: rqalpha/mod/__init__.py:53
 msgid "loading mod {}"
@@ -334,104 +334,103 @@
 msgid "mod tear_down [START] {}"
 msgstr ""
 
 #: rqalpha/mod/__init__.py:81
 msgid "mod tear_down [END]   {}"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py:314
+#: rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py:318
 msgid "{order_book_id} is expired, close all positions by system"
 msgstr "{order_book_id} 已退市/交割，系统自动平仓"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py:41
+#: rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py:40
 msgid ""
 "Order Creation Failed: not enough today position {order_book_id} to "
 "close, target quantity is {quantity}, closable today quantity is "
 "{closable}"
 msgstr "订单创建失败：{order_book_id} 的今仓不足，目标平今仓量为 {quantity}，可平今仓量为 {closable}"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py:50
+#: rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py:49
 msgid ""
 "Order Creation Failed: not enough position {order_book_id} to close or "
 "exercise, target sell quantity is {quantity}, closable quantity is "
 "{closable}"
 msgstr "订单创建失败：{order_book_id} 的仓位不足，目标平仓/行权量为 {quantity}，可平仓/行权量为 {closable}"
 
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:50
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:112
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:158
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:157
 msgid "Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
 msgstr "{order_book_id} 的订单创建失败：下单数量为 0"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:55
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:56
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:100
 msgid "Limit order price should not be nan."
 msgstr "限价单价格不能为 nan。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:78
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:76
 msgid ""
 "Order Creation Failed: close today amount {amount} is larger than today "
 "closable quantity {quantity}"
 msgstr "订单创建失败: 平今仓量 {amount} 大于当前可平今仓位 {quantity} "
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:89
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:88
 msgid ""
 "Order Creation Failed: close amount {amount} is larger than position "
 "quantity {quantity}"
 msgstr "订单创建失败: 平仓量 {amount} 大于当前持仓量 {quantity}"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:113
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:111
 msgid ""
 "Order was separated, original order: {original_order_repr}, new orders: "
 "[{new_orders_repr}]"
 msgstr "订单被拆分，原订单：{original_order_repr}，新订单：[{new_orders_repr}]"
 
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:66
 msgid ""
 "order_book_id: {order_book_id} needs stock account, please set and try "
 "again!"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:120
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:119
 msgid "insufficient cash, use all remaining cash({}) to create order"
 msgstr "现金不足，使用当前剩余资金({})创建订单"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:334
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:332
 #, fuzzy
 msgid ""
 "function order_target_portfolio: invalid keys of target_portfolio, "
 "expected order_book_ids or Instrument objects, got {} (type: {})"
 msgstr ""
 "函数 order_target_portfolio：不合法的参数。target_portfolio 的键应为合约代码或 Instrument "
 "对象，实际传入了 {}（类型：{}）。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:339
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:337
 msgid ""
 "function order_target_portfolio: invalid instrument type, excepted "
 "CS/ETF/LOF/INDX, got {}"
 msgstr "函数 order_target_portfolio：不合法的资产类型。应传入股票、ETF、LOF 或指数，实际传入了 {}。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:354
-#, fuzzy
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:351
 msgid ""
 "function order_target_portfolio: invalid values of target_portfolio, "
 "excepted float between 0 and 1, got {} (key: {})"
 msgstr "函数 order_target_portfolio：不合法的目标权重，应传入 0 和 1 之间的浮点数，实际传入了 {}（类型：{}）。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:363
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:360
 msgid "total percent should be lower than 1, current: {}"
 msgstr "目标持仓占比总和应小于 1，当前值：{}。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:383
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:380
 msgid ""
 "Adjust position of {id_or_ins} Failed: Invalid close/open price "
 "{close_price}/{open_price}"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:698
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:693
 msgid "in get_dividend, start_date {} is later than the previous test day {}"
 msgstr "在 get_dividend 函数中，start_date {} 晚于当前回测时间的上一个交易日 {}。"
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py:66
 msgid "[sys_analyser] save report"
 msgstr ""
 
@@ -475,35 +474,39 @@
 msgid "show weekly indicators and return curve on plot"
 msgstr ""
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py:115
 msgid "[sys_analyser] Generate report from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件生成报告"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:112
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:113
 msgid ""
 "config 'base.benchmark' is deprecated, use 'mod.sys_analyser.benchmark' "
 "instead"
 msgstr "配置'base.benchmark'已被弃用，使用'mod.sys_analyser.benchmark'代替"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:143
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:151
 msgid "benchmark {} not exists, please entry correct order_book_id"
-msgstr "基准标的({})信息不存在，请输入正确的标的代码"
+msgstr "基准标的 {} 信息不存在，请输入正确的标的代码"
+
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:163
+msgid "benchmark {} missing data between backtest start date {} and end date {}"
+msgstr "基准标的 {} 在回测起始日期 {} 结束日期 {} 间缺失数据"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:147
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:175
 msgid ""
-"benchmark {} listed date {} > backtest start date {} or de_listed date {}"
-" <= backtest end date {}"
-msgstr "基准标的({})上市日期({})晚于回测起始日期({})或退市日期({})早于回测结束日期({})"
+"benchmark {} available data start date {} >= backtest start date {} or end"
+" date {} <= backtest end date {}"
+msgstr "基准标的 {} 的可用行情数据开始日期 {} >= 回测起始日期 {} 或结束日期 {} <= 回测结束日期 {}"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:210
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:243
 msgid "invalid init benchmark {}, should be in format 'order_book_id:weight'"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:215
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:248
 msgid "invalid weight for instrument {order_book_id}: {weight}"
 msgstr ""
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:60
 msgid "Strategy"
 msgstr "策略收益"
 
@@ -705,42 +708,41 @@
 msgid "MonthlyVolatility"
 msgstr "月度波动率"
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:183
 msgid "ExcessWinRate"
 msgstr "超额胜率"
 
-#: rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py:33
+#: rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py:34
 msgid ""
 "Order Creation Failed: not enough money to buy {order_book_id}, needs "
 "{cost_money:.2f}, cash {cash:.2f}"
 msgstr "订单创建失败: 可用资金不足。当前资金: {cash:.2f}，{order_book_id} 下单所需资金: {cost_money:.2f}"
 
-#: rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py:32
-#, fuzzy
+#: rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py:35
 msgid "Order Creation Failed: {order_book_id} is not listing!"
 msgstr "订单创建失败: {order_book_id} 未上市或已退市"
 
-#: rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py:38
+#: rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py:40
 msgid "Order Creation Failed: security {order_book_id} is suspended on {date}"
 msgstr "订单创建失败: {order_book_id} 在 {date} 时停牌"
 
-#: rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py:34
+#: rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py:36
 msgid ""
 "Order Creation Failed: limit order price {limit_price} is higher than "
 "limit up {limit_up}, order_book_id={order_book_id}"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py:47
+#: rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py:48
 msgid ""
 "Order Creation Failed: limit order price {limit_price} is lower than "
 "limit down {limit_down}, order_book_id={order_book_id}"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py:32
+#: rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py:34
 msgid ""
 "Create order failed, there are active orders leading to the risk of self-"
 "trade: [{}...]"
 msgstr "订单创建失败，当前存在可能导致自成交的挂单：[{}...]"
 
 #: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:118
 #: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:335
```

### Comparing `rqalpha-5.3.8/rqalpha/utils/translations/zh_Hans_CN/__init__.py` & `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha/utils/typing.py` & `rqalpha-5.3.9/rqalpha/utils/typing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/rqalpha.egg-info/PKG-INFO` & `rqalpha-5.3.9/rqalpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.3.8
+Version: 5.3.9
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.3.8/rqalpha.egg-info/SOURCES.txt` & `rqalpha-5.3.9/rqalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/setup.py` & `rqalpha-5.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/__init__.py` & `rqalpha-5.3.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/__init__.py` & `rqalpha-5.3.9/tests/api_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/__init__.py` & `rqalpha-5.3.9/tests/api_tests/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/__init__.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_account_model.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_account_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_margin_stocks.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_margin_stocks.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_accounts/test_position_models.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_position_models.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_scheduler/test_physical_time.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_physical_time.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_scheduler/test_scheduler.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/__init__.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_management_fee.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_management_fee.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_match.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_match.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_signal_broker.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_simulation_broker.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py` & `rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/test_api_base.py` & `rqalpha-5.3.9/tests/api_tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/test_api_future.py` & `rqalpha-5.3.9/tests/api_tests/test_api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/test_api_stock.py` & `rqalpha-5.3.9/tests/api_tests/test_api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/api_tests/test_config.py` & `rqalpha-5.3.9/tests/api_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_f_buy_and_hold.py` & `rqalpha-5.3.9/tests/test_f_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_f_delivery.py` & `rqalpha-5.3.9/tests/test_f_delivery.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_f_macd.py` & `rqalpha-5.3.9/tests/test_f_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_f_macd_signal.py` & `rqalpha-5.3.9/tests/test_f_macd_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_f_mean_reverting.py` & `rqalpha-5.3.9/tests/test_f_mean_reverting.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_f_tick_size.py` & `rqalpha-5.3.9/tests/test_f_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_s_buy_and_hold.py` & `rqalpha-5.3.9/tests/test_s_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_s_dual_thrust.py` & `rqalpha-5.3.9/tests/test_s_dual_thrust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_s_pit_tax.py` & `rqalpha-5.3.9/tests/test_s_pit_tax.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_s_scheduler.py` & `rqalpha-5.3.9/tests/test_s_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_s_tick_size.py` & `rqalpha-5.3.9/tests/test_s_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_s_turtle.py` & `rqalpha-5.3.9/tests/test_s_turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_s_turtle_signal.py` & `rqalpha-5.3.9/tests/test_s_turtle_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/test_sf_buy_and_hold.py` & `rqalpha-5.3.9/tests/test_sf_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/unittest/__init__.py` & `rqalpha-5.3.9/tests/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py` & `rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/unittest/test_data/test_instrument_mixin.py` & `rqalpha-5.3.9/tests/unittest/test_data/test_instrument_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/unittest/test_data/test_trading_dates_mixin.py` & `rqalpha-5.3.9/tests/unittest/test_data/test_trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/unittest/test_mod/__init__.py` & `rqalpha-5.3.9/tests/unittest/test_mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/unittest/test_mod/test_sys_simulation/__init__.py` & `rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py` & `rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/tests/utils.py` & `rqalpha-5.3.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.8/versioneer.py` & `rqalpha-5.3.9/versioneer.py`

 * *Files identical despite different names*

