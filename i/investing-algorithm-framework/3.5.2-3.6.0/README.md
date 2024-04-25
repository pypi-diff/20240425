# Comparing `tmp/investing_algorithm_framework-3.5.2.tar.gz` & `tmp/investing_algorithm_framework-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-3.5.2.tar", max compression
+gzip compressed data, was "investing_algorithm_framework-3.6.0.tar", max compression
```

## Comparing `investing_algorithm_framework-3.5.2.tar` & `investing_algorithm_framework-3.6.0.tar`

### file list

```diff
@@ -1,142 +1,141 @@
--rw-r--r--   0        0        0    11343 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/LICENSE
--rw-r--r--   0        0        0    21956 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/README.md
--rw-r--r--   0        0        0     2084 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/__init__.py
--rw-r--r--   0        0        0      501 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0        0        0    34948 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0        0        0    32200 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/app.py
--rw-r--r--   0        0        0     1092 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/__init__.py
--rw-r--r--   0        0        0     2362 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0        0        0      154 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0        0        0      452 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0        0        0     1062 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0        0        0     1085 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0        0        0     3887 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0        0        0      963 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/task.py
--rw-r--r--   0        0        0      134 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/__init__.py
--rw-r--r--   0        0        0      587 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0        0        0      694 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0        0        0      727 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0        0        0      617 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0        0        0      506 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0        0        0     2020 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0        0        0      585 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0        0        0      158 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/run_strategies.py
--rw-r--r--   0        0        0      361 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0        0        0      442 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0        0        0      743 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0        0        0      438 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0        0        0       80 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0        0        0      603 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/create_app.py
--rw-r--r--   0        0        0     6312 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/dependency_container.py
--rw-r--r--   0        0        0     3912 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/config.py
--rw-r--r--   0        0        0     2293 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0        0        0      962 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/data_structures.py
--rw-r--r--   0        0        0      823 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/decimal_parsing.py
--rw-r--r--   0        0        0     1628 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/exceptions.py
--rw-r--r--   0        0        0     1121 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0        0        0      812 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/app_mode.py
--rw-r--r--   0        0        0      253 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/backtesting/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
--rw-r--r--   0        0        0    13619 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
--rw-r--r--   0        0        0     2309 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
--rw-r--r--   0        0        0      659 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/base_model.py
--rw-r--r--   0        0        0       87 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/market/__init__.py
--rw-r--r--   0        0        0      779 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/market/market_credential.py
--rw-r--r--   0        0        0      237 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0        0        0    10363 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0        0        0     1110 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0        0        0      814 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0        0        0      937 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0        0        0      751 2024-04-13 07:54:16.352982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order_type.py
--rw-r--r--   0        0        0      230 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0        0        0     2495 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1752 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
--rw-r--r--   0        0        0     3141 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      123 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0        0        0     1131 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/position/position_snapshot.py
--rw-r--r--   0        0        0     4598 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/strategy_profile.py
--rw-r--r--   0        0        0     2659 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0        0        0     2798 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0        0        0     2011 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0        0        0       99 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trade/__init__.py
--rw-r--r--   0        0        0     7114 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trade/trade.py
--rw-r--r--   0        0        0      807 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trade/trade_status.py
--rw-r--r--   0        0        0     1119 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0        0        0     6791 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0        0        0      634 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/market_credential_service.py
--rw-r--r--   0        0        0     9941 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/market_data_sources.py
--rw-r--r--   0        0        0     3522 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/market_service.py
--rw-r--r--   0        0        0      115 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/portfolios/__init__.py
--rw-r--r--   0        0        0      320 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0      699 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/rounding_service.py
--rw-r--r--   0        0        0      258 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0        0        0      156 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0        0        0     1805 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/strategy.py
--rw-r--r--   0        0        0      700 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0        0        0    25794 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/backtesting.py
--rw-r--r--   0        0        0     2746 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0        0        0      275 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0        0        0      417 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0        0        0      608 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0        0        0      253 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/synchronized.py
--rw-r--r--   0        0        0     1361 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/__init__.py
--rw-r--r--   0        0        0      176 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
--rw-r--r--   0        0        0      732 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      327 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/decimal_parser.py
--rw-r--r--   0        0        0      437 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
--rw-r--r--   0        0        0    17538 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
--rw-r--r--   0        0        0     5472 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
--rw-r--r--   0        0        0      142 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/model_extension.py
--rw-r--r--   0        0        0      102 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0        0        0     4877 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0        0        0      847 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/order/order_fee.py
--rw-r--r--   0        0        0      141 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0        0        0     3226 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1238 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      135 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0        0        0     1898 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0        0        0      842 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
--rw-r--r--   0        0        0      567 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      487 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0        0        0     3351 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0        0        0     1073 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0        0        0     1967 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
--rw-r--r--   0        0        0     1994 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0        0        0      680 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
--rw-r--r--   0        0        0     7661 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/repository.py
--rw-r--r--   0        0        0      163 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0        0        0       91 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
--rw-r--r--   0        0        0    15303 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
--rw-r--r--   0        0        0      195 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
--rw-r--r--   0        0        0       43 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
--rw-r--r--   0        0        0    11933 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
--rw-r--r--   0        0        0     1318 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0        0        0      191 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/backtesting/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
--rw-r--r--   0        0        0    15033 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/backtesting/backtest_service.py
--rw-r--r--   0        0        0      624 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/configuration_service.py
--rw-r--r--   0        0        0      821 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/market_credential_service.py
--rw-r--r--   0        0        0      235 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/market_data_source_service/__init__.py
--rw-r--r--   0        0        0     5264 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
--rw-r--r--   0        0        0     6832 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
--rw-r--r--   0        0        0      159 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/order_service/__init__.py
--rw-r--r--   0        0        0     7834 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/order_service/order_backtest_service.py
--rw-r--r--   0        0        0    27824 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/order_service/order_service.py
--rw-r--r--   0        0        0      509 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/__init__.py
--rw-r--r--   0        0        0      825 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
--rw-r--r--   0        0        0     2055 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
--rw-r--r--   0        0        0     4493 2024-04-13 07:54:16.356982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_service.py
--rw-r--r--   0        0        0     1984 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
--rw-r--r--   0        0        0    16127 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0     1052 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0        0        0      525 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/position_snapshot_service.py
--rw-r--r--   0        0        0      995 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0        0        0     8077 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0        0        0       68 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/trade_service/__init__.py
--rw-r--r--   0        0        0    14761 2024-04-13 07:54:16.360982 investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/trade_service/trade_service.py
--rw-r--r--   0        0        0      742 2024-04-13 07:54:24.141043 investing_algorithm_framework-3.5.2/pyproject.toml
--rw-r--r--   0        0        0    23028 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/LICENSE
+-rw-r--r--   0        0        0    21956 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/README.md
+-rw-r--r--   0        0        0     2184 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0        0        0    36188 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0        0        0    32504 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/app.py
+-rw-r--r--   0        0        0     1092 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/__init__.py
+-rw-r--r--   0        0        0     2362 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0        0        0      452 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0        0        0     1062 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0        0        0     1085 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0        0        0     3887 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0        0        0      963 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/task.py
+-rw-r--r--   0        0        0      134 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0        0        0      727 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0        0        0      617 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0        0        0      506 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0        0        0     2020 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0        0        0      585 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0        0        0      158 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/run_strategies.py
+-rw-r--r--   0        0        0      361 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0        0        0      743 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0        0        0      438 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0        0        0       80 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0        0        0      603 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/create_app.py
+-rw-r--r--   0        0        0     6170 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/dependency_container.py
+-rw-r--r--   0        0        0     3986 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0        0        0     2293 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0        0        0      962 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/data_structures.py
+-rw-r--r--   0        0        0      823 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/decimal_parsing.py
+-rw-r--r--   0        0        0     1628 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/exceptions.py
+-rw-r--r--   0        0        0     1139 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/app_mode.py
+-rw-r--r--   0        0        0      328 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/__init__.py
+-rw-r--r--   0        0        0      553 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/backtest_date_range.py
+-rw-r--r--   0        0        0     2860 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
+-rw-r--r--   0        0        0    14101 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
+-rw-r--r--   0        0        0     2309 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
+-rw-r--r--   0        0        0      659 2024-04-25 20:56:00.791692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/base_model.py
+-rw-r--r--   0        0        0       87 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/market/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/market/market_credential.py
+-rw-r--r--   0        0        0      193 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0        0        0    11833 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0        0        0      814 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0        0        0      937 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0        0        0      751 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order_type.py
+-rw-r--r--   0        0        0      230 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     2495 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1752 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+-rw-r--r--   0        0        0     3141 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      123 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0        0        0     1131 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/position/position_snapshot.py
+-rw-r--r--   0        0        0     4598 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/strategy_profile.py
+-rw-r--r--   0        0        0     2659 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0        0        0     2798 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0        0        0     2011 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0        0        0       99 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trade/__init__.py
+-rw-r--r--   0        0        0     7787 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trade/trade.py
+-rw-r--r--   0        0        0      807 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trade/trade_status.py
+-rw-r--r--   0        0        0     1119 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0        0        0     6791 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0        0        0      634 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/market_credential_service.py
+-rw-r--r--   0        0        0     9941 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/market_data_sources.py
+-rw-r--r--   0        0        0     3522 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/market_service.py
+-rw-r--r--   0        0        0      115 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0      699 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/rounding_service.py
+-rw-r--r--   0        0        0      258 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0        0        0      156 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0        0        0     1805 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/strategy.py
+-rw-r--r--   0        0        0      750 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0        0        0    26274 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/backtesting.py
+-rw-r--r--   0        0        0     2746 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0        0        0      275 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0        0        0      417 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0        0        0      608 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0        0        0      253 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/synchronized.py
+-rw-r--r--   0        0        0     1277 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0        0        0     1386 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+-rw-r--r--   0        0        0      700 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/decimal_parser.py
+-rw-r--r--   0        0        0      437 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
+-rw-r--r--   0        0        0    17538 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
+-rw-r--r--   0        0        0     5472 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
+-rw-r--r--   0        0        0     1641 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/market_data_sources/us_treasury_yield.py
+-rw-r--r--   0        0        0      142 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/model_extension.py
+-rw-r--r--   0        0        0       52 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0        0        0     5387 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0        0        0      141 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     3226 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1238 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      135 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0        0        0      842 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
+-rw-r--r--   0        0        0      482 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0     3351 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0        0        0     1073 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0        0        0     1967 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
+-rw-r--r--   0        0        0     1994 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0        0        0      680 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
+-rw-r--r--   0        0        0     7661 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/repository.py
+-rw-r--r--   0        0        0      163 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
+-rw-r--r--   0        0        0    15303 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
+-rw-r--r--   0        0        0      195 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
+-rw-r--r--   0        0        0    11933 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
+-rw-r--r--   0        0        0     1318 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/backtesting/__init__.py
+-rw-r--r--   0        0        0     2651 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
+-rw-r--r--   0        0        0    15138 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/backtesting/backtest_service.py
+-rw-r--r--   0        0        0      624 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/configuration_service.py
+-rw-r--r--   0        0        0      821 2024-04-25 20:56:00.795692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/market_credential_service.py
+-rw-r--r--   0        0        0      235 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/market_data_source_service/__init__.py
+-rw-r--r--   0        0        0     5264 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
+-rw-r--r--   0        0        0     6832 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
+-rw-r--r--   0        0        0      159 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/order_service/__init__.py
+-rw-r--r--   0        0        0     7747 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/order_service/order_backtest_service.py
+-rw-r--r--   0        0        0    26845 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/order_service/order_service.py
+-rw-r--r--   0        0        0      509 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
+-rw-r--r--   0        0        0     2055 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
+-rw-r--r--   0        0        0     4493 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_service.py
+-rw-r--r--   0        0        0     1984 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
+-rw-r--r--   0        0        0    16127 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0     1052 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0        0        0      525 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/position_snapshot_service.py
+-rw-r--r--   0        0        0      995 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0        0        0     8077 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0        0        0       68 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/trade_service/__init__.py
+-rw-r--r--   0        0        0    14761 2024-04-25 20:56:00.799692 investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/trade_service/trade_service.py
+-rw-r--r--   0        0        0      742 2024-04-25 20:56:11.235681 investing_algorithm_framework-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23028 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.6.0/PKG-INFO
```

### Comparing `investing_algorithm_framework-3.5.2/LICENSE` & `investing_algorithm_framework-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/README.md` & `investing_algorithm_framework-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     TradingDataType, TradingTimeFrame, OrderType, OperationalException, \
     OrderStatus, OrderSide, Config, TimeUnit, TimeInterval, Order, Portfolio, \
     Position, TimeFrame, BACKTESTING_INDEX_DATETIME, MarketCredential, \
     PortfolioConfiguration, RESOURCE_DIRECTORY, pretty_print_backtest, \
     Trade, OHLCVMarketDataSource, OrderBookMarketDataSource, SYMBOLS, \
     TickerMarketDataSource, MarketService, BacktestReportsEvaluation, \
     pretty_print_backtest_reports_evaluation, load_backtest_reports, \
-    RESERVED_BALANCES, APP_MODE, AppMode, DATETIME_FORMAT
+    RESERVED_BALANCES, APP_MODE, AppMode, DATETIME_FORMAT, \
+    load_backtest_report, BacktestDateRange
 from investing_algorithm_framework.infrastructure import \
     CCXTOrderBookMarketDataSource, CCXTOHLCVMarketDataSource, \
     CCXTTickerMarketDataSource, CSVOHLCVMarketDataSource, \
     CSVTickerMarketDataSource
 from .create_app import create_app
 
 __all__ = [
@@ -57,8 +58,10 @@
     "BacktestReportsEvaluation",
     "load_backtest_reports",
     "SYMBOLS",
     "RESERVED_BALANCES",
     "APP_MODE",
     "AppMode",
     "DATETIME_FORMAT",
+    "load_backtest_report",
+    "BacktestDateRange",
 ]
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,66 @@
 import inspect
 import logging
-from typing import List
+from typing import List, Dict
 
-from investing_algorithm_framework.domain import OrderStatus, OrderFee, \
+from investing_algorithm_framework.domain import OrderStatus, \
     Position, Order, Portfolio, OrderType, OrderSide, \
     BACKTESTING_FLAG, BACKTESTING_INDEX_DATETIME, MarketService, TimeUnit, \
     OperationalException, random_string, RoundingService
 from investing_algorithm_framework.services import MarketCredentialService, \
     MarketDataSourceService, PortfolioService, PositionService, TradeService, \
     OrderService, ConfigurationService, StrategyOrchestratorService, \
     PortfolioConfigurationService
 from .task import Task
 
 logger = logging.getLogger("investing_algorithm_framework")
 
 
 class Algorithm:
-
-    def __init__(self, name=None, description=None):
+    """
+    Class to represent an algorithm. An algorithm is a collection of
+    strategies that are executed in a specific order. The algorithm
+    class is responsible for managing the strategies and executing
+    them in the correct order.
+
+    :param name: The name of the algorithm
+    :param description: The description of the algorithm
+    :param context: The context of the algorithm, for backtest references
+    """
+    def __init__(
+        self,
+        name: str = None,
+        description: str = None,
+        context: Dict[str, str] = None
+    ):
         self._name = name
 
         if name is None:
             self._name = f"algorithm_{random_string(10)}"
 
         self._description = None
 
         if description is not None:
             self._description = description
 
+        self._context = context
+
+        if self.context is None:
+            self._context = {}
+
+        # Check if the context is a dictionary with only string,
+        # float or int values
+        for key, value in self.context.items():
+            if not isinstance(key, str) or \
+                    not isinstance(value, (str, float, int)):
+                raise OperationalException(
+                    "The context of the algorithm must be a dictionary with "
+                    "only string, float or int values."
+                )
+
         self._strategies = []
         self._tasks = []
         self.portfolio_service: PortfolioService
         self.position_service: PositionService
         self.order_service: OrderService
         self.market_service: MarketService
         self.configuration_service: ConfigurationService
@@ -105,14 +134,28 @@
         Function to get a config instance. This allows users when
         having access to the algorithm instance also to read the
         configs of the app.
         """
         return self.configuration_service.config
 
     @property
+    def description(self):
+        """
+        Function to get the description of the algorithm
+        """
+        return self._description
+
+    @property
+    def context(self):
+        """
+        Function to get the context of the algorithm
+        """
+        return self._context
+
+    @property
     def running(self) -> bool:
         """
         Returns True if the algorithm is running, False otherwise.
 
         The algorithm is considered to be running if has strategies
         scheduled to run in the strategy orchestrator service.
         """
@@ -358,17 +401,14 @@
                 "target_symbol": target_symbol,
                 "status": status,
                 "order_type": order_type,
                 "order_side": order_side
             }
         )
 
-    def get_order_fee(self, order_id) -> OrderFee:
-        return self.order_service.get_order_fee(order_id)
-
     def get_positions(
         self,
         market=None,
         identifier=None,
         amount_gt=None,
         amount_gte=None,
         amount_lt=None,
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 import shutil
 import threading
 from abc import abstractmethod
 from datetime import datetime
 from distutils.sysconfig import get_python_lib
 from time import sleep
-from typing import List, Optional, Tuple
+from typing import List, Optional
 
 from flask import Flask
 
 from investing_algorithm_framework.app.algorithm import Algorithm
 from investing_algorithm_framework.app.stateless import ActionHandler
 from investing_algorithm_framework.app.task import Task
 from investing_algorithm_framework.app.web import create_flask_app
 from investing_algorithm_framework.domain import DATABASE_NAME, TimeUnit, \
     DATABASE_DIRECTORY_PATH, RESOURCE_DIRECTORY, ENVIRONMENT, Environment, \
     SQLALCHEMY_DATABASE_URI, OperationalException, BACKTESTING_FLAG, \
     BACKTESTING_START_DATE, BACKTESTING_END_DATE, BacktestReport, \
     BACKTESTING_PENDING_ORDER_CHECK_INTERVAL, APP_MODE, MarketCredential, \
-    AppMode
+    AppMode, BacktestDateRange
 from investing_algorithm_framework.infrastructure import setup_sqlalchemy, \
     create_all_tables
 from investing_algorithm_framework.services import OrderBacktestService, \
     BacktestMarketDataSourceService, BacktestPortfolioService, \
     MarketDataSourceService, MarketCredentialService
 
 logger = logging.getLogger("investing_algorithm_framework")
@@ -315,15 +315,14 @@
 
         # Override the order service with the backtest order service
         market_data_source_service = self.container \
             .market_data_source_service()
         self.container.order_service.override(
             OrderBacktestService(
                 order_repository=self.container.order_repository(),
-                order_fee_repository=self.container.order_fee_repository(),
                 position_repository=self.container.position_repository(),
                 portfolio_repository=self.container.portfolio_repository(),
                 portfolio_configuration_service=self.container
                 .portfolio_configuration_service(),
                 portfolio_snapshot_service=self.container
                 .portfolio_snapshot_service(),
                 configuration_service=self.container.configuration_service(),
@@ -725,62 +724,66 @@
 
         if output_directory is None:
             output_directory = os.path.join(
                 self.config.get(RESOURCE_DIRECTORY),
                 "backtest_reports"
             )
 
-        backtest_report_writer_service.write_report_to_csv(
+        backtest_report_writer_service.write_report_to_json(
             report=report, output_directory=output_directory
         )
 
         return report
 
     def run_backtests(
         self,
         algorithms,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
-        date_ranges: Optional[Tuple[datetime, datetime]] = None,
+        date_ranges: Optional[List[BacktestDateRange]] = None,
         pending_order_check_interval=None,
         output_directory=None
     ) -> List[BacktestReport]:
         """
         Run a backtest for a set algorithm. This method should be called when
         running a backtest.
 
         :param algorithms: The algorithms to run backtests for (list of
         Algorithm instances)
         :param start_date: The start date of the backtest
         :param end_date: The end date of the backtest
         :param pending_order_check_interval: The interval at which to check
         :param date_ranges: The date ranges to run the backtests for (list of
-        tuples of start and end dates)
+        BacktestDateRange instances representing a start and end date)
         pending orders
         :param output_directory: The directory to write the backtest report to
         :return: List of BacktestReport intances
         """
         logger.info("Initializing backtests")
         reports = []
 
         if start_date is not None:
 
             if end_date is None:
                 end_date = datetime.utcnow()
 
-            date_ranges = [(start_date, end_date)]
+            date_ranges = [
+                BacktestDateRange(start_date=start_date, end_date=end_date)
+            ]
         else:
             if date_ranges is None:
                 raise OperationalException("No date ranges specified")
 
         market_data_sources = self._market_data_source_service\
             .get_market_data_sources()
 
         for date_range in date_ranges:
-            start_date, end_date = date_range
+            date_range: BacktestDateRange = date_range
+            start_date = date_range.start_date
+            end_date = date_range.end_date
             self._initialize_app_for_backtest(
                 backtest_start_date=start_date,
                 backtest_end_date=end_date,
                 pending_order_check_interval=pending_order_check_interval,
                 market_data_sources=market_data_sources
             )
 
@@ -800,24 +803,29 @@
                 # Run the backtest with the backtest_service
                 # and collect the report
                 report = backtest_service.run_backtest(
                     algorithm=algorithm,
                     start_date=start_date,
                     end_date=end_date
                 )
+
+                # Add date range name to report if present
+                if date_range.name is not None:
+                    report.date_range_name = date_range.name
+
                 backtest_report_writer_service = self.container \
                     .backtest_report_writer_service()
 
                 if output_directory is None:
                     output_directory = os.path.join(
                         self.config.get(RESOURCE_DIRECTORY),
                         "backtest_reports"
                     )
 
-                backtest_report_writer_service.write_report_to_csv(
+                backtest_report_writer_service.write_report_to_json(
                     report=report, output_directory=output_directory
                 )
                 reports.append(report)
 
         return reports
 
     def add_market_data_source(self, market_data_source):
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/create_app.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/create_app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/dependency_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dependency_injector import containers, providers
 
 from investing_algorithm_framework.app.algorithm import Algorithm
 from investing_algorithm_framework.infrastructure import SQLOrderRepository, \
     SQLPositionRepository, SQLPortfolioRepository, \
-    SQLOrderFeeRepository, SQLPortfolioSnapshotRepository, \
+    SQLPortfolioSnapshotRepository, \
     SQLPositionSnapshotRepository, PerformanceService, CCXTMarketService
 from investing_algorithm_framework.services import OrderService, \
     PositionService, PortfolioService, StrategyOrchestratorService, \
     PortfolioConfigurationService, MarketDataSourceService, BacktestService, \
     ConfigurationService, PortfolioSnapshotService, PositionSnapshotService, \
     MarketCredentialService, TradeService, BacktestReportWriterService, \
     PortfolioSyncService
@@ -29,15 +29,14 @@
     configuration_service = providers.ThreadSafeSingleton(
         ConfigurationService,
     )
     market_credential_service = providers.ThreadSafeSingleton(
         MarketCredentialService
     )
     order_repository = providers.Factory(SQLOrderRepository)
-    order_fee_repository = providers.Factory(SQLOrderFeeRepository)
     position_repository = providers.Factory(SQLPositionRepository)
     portfolio_repository = providers.Factory(SQLPortfolioRepository)
     position_snapshot_repository = providers.Factory(
         SQLPositionSnapshotRepository
     )
     portfolio_snapshot_repository = providers.Factory(
         SQLPortfolioSnapshotRepository
@@ -66,15 +65,14 @@
         portfolio_repository=portfolio_repository,
         position_repository=position_repository,
     )
     order_service = providers.Factory(
         OrderService,
         configuration_service=configuration_service,
         order_repository=order_repository,
-        order_fee_repository=order_fee_repository,
         portfolio_repository=portfolio_repository,
         position_repository=position_repository,
         market_service=market_service,
         market_credential_service=market_credential_service,
         portfolio_configuration_service=portfolio_configuration_service,
         portfolio_snapshot_service=portfolio_snapshot_service
     )
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 from .data_structures import PeekableQueue
 from .decimal_parsing import parse_decimal_to_string, parse_string_to_decimal
 from .exceptions import OperationalException, ApiException, \
     PermissionDeniedApiException, ImproperlyConfigured
 from .models import OrderStatus, OrderSide, OrderType, TimeInterval, \
     TimeUnit, TimeFrame, TradingTimeFrame, TradingDataType, \
     PortfolioConfiguration, Portfolio, Position, Order, TradeStatus, \
-    OrderFee, BacktestReport, PortfolioSnapshot, StrategyProfile, \
+    BacktestReport, PortfolioSnapshot, StrategyProfile, \
     BacktestPosition, Trade, MarketCredential, PositionSnapshot, \
-    BacktestReportsEvaluation, AppMode
+    BacktestReportsEvaluation, AppMode, BacktestDateRange
 from .services import TickerMarketDataSource, OrderBookMarketDataSource, \
     OHLCVMarketDataSource, BacktestMarketDataSource, MarketDataSource, \
     MarketService, MarketCredentialService, AbstractPortfolioSyncService, \
     RoundingService
 from .singleton import Singleton
 from .stateless_actions import StatelessActions
 from .strategy import Strategy
 from .utils import random_string, append_dict_as_row_to_csv, \
     add_column_headers_to_csv, get_total_amount_of_rows, \
+    load_backtest_report, \
     csv_to_list, StoppableThread, pretty_print_backtest_reports_evaluation, \
     pretty_print_backtest, load_csv_into_dict, load_backtest_reports
 
 __all__ = [
     'Config',
     "OrderStatus",
     "OrderSide",
@@ -66,15 +67,14 @@
     "StoppableThread",
     "Portfolio",
     "Position",
     "Order",
     "Strategy",
     "DATETIME_FORMAT",
     "StatelessActions",
-    "OrderFee",
     "parse_decimal_to_string",
     "parse_string_to_decimal",
     "BacktestReport",
     "pretty_print_backtest",
     "DATETIME_FORMAT_BACKTESTING",
     "BACKTESTING_FLAG",
     "BACKTESTING_INDEX_DATETIME",
@@ -108,8 +108,10 @@
     "load_backtest_reports",
     "SYMBOLS",
     "RESERVED_BALANCES",
     "AbstractPortfolioSyncService",
     "APP_MODE",
     "AppMode",
     "RoundingService",
+    "BacktestDateRange",
+    "load_backtest_report",
 ]
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/data_structures.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/data_structures.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/decimal_parsing.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/decimal_parsing.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .app_mode import AppMode
 from .backtesting import BacktestReport, BacktestPosition, \
-    BacktestReportsEvaluation
+    BacktestReportsEvaluation, BacktestDateRange
 from .market import MarketCredential
-from .order import OrderStatus, OrderSide, OrderType, Order, OrderFee
+from .order import OrderStatus, OrderSide, OrderType, Order
 from .portfolio import PortfolioConfiguration, Portfolio, PortfolioSnapshot
 from .position import Position, PositionSnapshot
 from .strategy_profile import StrategyProfile
 from .time_frame import TimeFrame
 from .time_interval import TimeInterval
 from .time_unit import TimeUnit
 from .trade import Trade, TradeStatus
@@ -22,19 +22,19 @@
     "TimeInterval",
     "TimeUnit",
     "TradingTimeFrame",
     "TradingDataType",
     "PortfolioConfiguration",
     "Position",
     "Portfolio",
-    "OrderFee",
     "BacktestReport",
     "PositionSnapshot",
     "PortfolioSnapshot",
     "StrategyProfile",
     "BacktestPosition",
     "Trade",
     "MarketCredential",
     "TradeStatus",
     "BacktestReportsEvaluation",
-    "AppMode"
+    "AppMode",
+    "BacktestDateRange"
 ]
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/app_mode.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/app_mode.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/backtesting/backtest_position.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,7 +100,21 @@
 
     def get_percentage_of_portfolio(self):
 
         if self._total_value_portfolio == 0:
             return 0.0
 
         return self.value / self._total_value_portfolio * 100
+
+    def to_dict(self):
+        return {
+            "symbol": self.symbol,
+            "amount": self.amount,
+            "cost": self.cost,
+            "price": self.price,
+            "value": self.value,
+            "growth": self.growth,
+            "growth_rate": self.growth_rate,
+            "amount_pending_buy": self.amount_pending_buy,
+            "amount_pending_sell": self.amount_pending_sell,
+            "percentage_of_portfolio": self.percentage_of_portfolio
+        }
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/backtesting/backtest_report.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 
 from investing_algorithm_framework.domain.models.base_model import BaseModel
 from investing_algorithm_framework.domain.models.time_unit import TimeUnit
+from investing_algorithm_framework.domain.constants import DATETIME_FORMAT
 
 
 class BacktestReport(BaseModel):
 
     def __init__(
         self,
         name=None,
@@ -14,15 +15,14 @@
         strategy_identifiers=None,
         initial_unallocated=0.0,
         number_of_runs=0,
         backtest_start_date_data=None,
         backtest_data_index_date=None,
         backtest_start_date=None,
         backtest_end_date=None,
-        backtest_index_date=None,
         trading_time_frame=None,
         trading_time_frame_start_date=None,
         symbols=None,
         market=None,
         number_of_days=0,
         number_of_orders=0,
         number_of_positions=0,
@@ -38,22 +38,23 @@
         growth_rate=0.0,
         growth=0.0,
         total_value=0.0,
         positions=None,
         average_trade_duration=0,
         average_trade_size=0.0,
         trades=None,
-        created_at: datetime = None
+        orders=None,
+        created_at: datetime = None,
+        context=None,
     ):
         self._name = name
         self._strategy_identifiers = strategy_identifiers
         self._backtest_start_date_data = backtest_start_date_data
         self._backtest_start_date = backtest_start_date
         self._backtest_end_date = backtest_end_date
-        self._backtest_index_date = backtest_index_date
         self._number_of_runs = number_of_runs
         self._trading_time_frame = trading_time_frame
         self._trading_time_frame_start_date = trading_time_frame_start_date
         self._symbols = symbols
         self._market = market
         self._number_of_days = number_of_days
         self._number_of_orders = number_of_orders
@@ -68,21 +69,23 @@
         self._growth = growth
         self._initial_unallocated = initial_unallocated
         self._trading_symbol = trading_symbol
         self._total_net_gain_percentage = total_net_gain_percentage
         self._total_net_gain = total_net_gain
         self._backtest_data_index_date = backtest_data_index_date
         self._total_value = total_value
-        self.positions = positions
+        self._positions = positions
+        self._orders = orders
         self._average_trade_duration = average_trade_duration
         self._average_trade_size = average_trade_size
         self._trades = trades
         self._created_at: datetime = created_at
         self._interval = interval
         self._time_unit = time_unit
+        self._context = context
 
     @property
     def name(self):
         return self._name
 
     @property
     def strategy_identifiers(self):
@@ -113,18 +116,14 @@
         return self._backtest_start_date
 
     @property
     def backtest_end_date(self):
         return self._backtest_end_date
 
     @property
-    def backtest_index_date(self):
-        return self._backtest_index_date
-
-    @property
     def trading_time_frame(self):
         return self._trading_time_frame
 
     @property
     def trading_time_frame_start_date(self):
         return self._trading_time_frame_start_date
 
@@ -156,18 +155,14 @@
     def backtest_start_date_data(self, value):
         self._backtest_start_date_data = value
 
     @backtest_end_date.setter
     def backtest_end_date(self, value):
         self._backtest_end_date = value
 
-    @backtest_index_date.setter
-    def backtest_index_date(self, value):
-        self._backtest_index_date = value
-
     @number_of_runs.setter
     def number_of_runs(self, value):
         self._number_of_runs = value
 
     @trading_time_frame.setter
     def trading_time_frame(self, value):
         self._trading_time_frame = value
@@ -313,14 +308,22 @@
         return self._positions
 
     @positions.setter
     def positions(self, value):
         self._positions = value
 
     @property
+    def orders(self):
+        return self._orders
+
+    @orders.setter
+    def orders(self, value):
+        self._orders = value
+
+    @property
     def average_trade_duration(self):
         return self._average_trade_duration
 
     @average_trade_duration.setter
     def average_trade_duration(self, value):
         self._average_trade_duration = value
 
@@ -345,14 +348,22 @@
         return self._interval
 
     @interval.setter
     def interval(self, value):
         self._interval = value
 
     @property
+    def context(self):
+        return self._context
+
+    @context.setter
+    def context(self, value):
+        self._context = value
+
+    @property
     def time_unit(self):
         return self._time_unit
 
     @time_unit.setter
     def time_unit(self, value):
         self._time_unit = value
 
@@ -368,28 +379,30 @@
             return 24 / self.interval
 
     def __repr__(self):
         return self.repr(
             name=self.name,
             start_date=self.backtest_start_date,
             end_date=self.backtest_end_date,
-            backtest_index_date=self.backtest_index_date,
             start_date_data=self.backtest_start_date_data,
         )
 
     def to_dict(self):
         """
         Convert the backtest report to a dictionary. So it can be
         saved to a file.
         """
         return {
             "name": self.name,
+            "context": self.context if self.context is not None else {},
             "strategy_identifiers": self.strategy_identifiers,
-            "backtest_start_date": self.backtest_start_date,
-            "backtest_end_date": self.backtest_end_date,
+            "backtest_start_date": self.backtest_start_date
+            .strftime(DATETIME_FORMAT),
+            "backtest_end_date": self.backtest_end_date
+            .strftime(DATETIME_FORMAT),
             "number_of_runs": self.number_of_runs,
             "symbols": self.symbols,
             "market": self.market,
             "number_of_days": self.number_of_days,
             "number_of_orders": self.number_of_orders,
             "number_of_positions": self.number_of_positions,
             "market_data_file": self.market_data_file,
@@ -400,18 +413,24 @@
             "total_cost": self.total_cost,
             "growth_rate": self.growth_rate,
             "growth": self.growth,
             "initial_unallocated": self.initial_unallocated,
             "trading_symbol": self.trading_symbol,
             "total_net_gain_percentage": self.total_net_gain_percentage,
             "total_net_gain": self.total_net_gain,
-            "backtest_data_index_date": self.backtest_data_index_date,
             "total_value": self.total_value,
             "average_trade_duration": self.average_trade_duration,
             "average_trade_size": self.average_trade_size,
+            "positions": [position.to_dict() for position in self.positions],
+            "trades": [trade.to_dict() for trade in self.trades],
+            "orders": [
+                order.to_dict(datetime_format=DATETIME_FORMAT)
+                for order in self.orders
+            ],
+            "created_at": self.created_at.strftime(DATETIME_FORMAT),
         }
 
     @staticmethod
     def from_dict(data):
         """
         Factory method to create a backtest report from a dictionary.
         """
@@ -434,12 +453,11 @@
             total_cost=float(data["total_cost"]),
             growth_rate=float(data["growth_rate"]),
             growth=float(data["growth"]),
             initial_unallocated=float(data["initial_unallocated"]),
             trading_symbol=data["trading_symbol"],
             total_net_gain_percentage=float(data["total_net_gain_percentage"]),
             total_net_gain=float(data["total_net_gain"]),
-            backtest_data_index_date=data["backtest_data_index_date"],
             total_value=float(data["total_value"]),
             average_trade_duration=data["average_trade_duration"],
             average_trade_size=float(data["average_trade_size"]),
         )
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/market/market_credential.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/market/market_credential.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 
 from dateutil.parser import parse
 
 from investing_algorithm_framework.domain.exceptions import \
     OperationalException
 from investing_algorithm_framework.domain.models.base_model import BaseModel
+from investing_algorithm_framework.domain.models.order.order_side import \
+    OrderSide
 from investing_algorithm_framework.domain.models.order.order_status import \
     OrderStatus
 from investing_algorithm_framework.domain.models.order.order_type import \
     OrderType
-from investing_algorithm_framework.domain.models.order.order_side import \
-    OrderSide
-from investing_algorithm_framework.domain.models.order.order_fee import \
-    OrderFee
 
 logger = logging.getLogger("investing_algorithm_framework")
 
 
 class Order(BaseModel):
-
+    """
+    Order model class to represent an order of the trading bot
+    """
     def __init__(
         self,
         order_type,
         order_side,
         status,
         amount,
         target_symbol=None,
@@ -36,18 +36,17 @@
         trade_closed_amount=None,
         external_id=None,
         filled=None,
         remaining=None,
         cost=None,
         fee=None,
         position_id=None,
-        stop_loss=None,
-        stop_loss_percentage=None,
-        trailing_stop_loss=None,
-        trailing_stop_loss_percentage=None,
+        order_fee=None,
+        order_fee_currency=None,
+        order_fee_rate=None
     ):
         if target_symbol is None:
             raise OperationalException("Target symbol is not specified")
 
         if trading_symbol is None:
             raise OperationalException("Trading symbol is not specified")
 
@@ -76,19 +75,18 @@
         self.trade_closed_amount = trade_closed_amount
         self.created_at = created_at
         self.updated_at = updated_at
         self.filled = filled
         self.remaining = remaining
         self.cost = cost
         self.fee = fee
-        self.stop_loss = stop_loss
-        self.stop_loss_percentage = stop_loss_percentage
-        self.trailing_stop_loss = trailing_stop_loss
-        self.trailing_stop_loss_percentage = trailing_stop_loss_percentage
         self._available_amount = self.filled
+        self.order_fee = order_fee
+        self.order_fee_currency = order_fee_currency
+        self.order_fee_rate = order_fee_rate
 
     def get_id(self):
         return self.id
 
     def get_external_id(self):
         return self.external_id
 
@@ -103,14 +101,32 @@
             return self.price
 
         return 0
 
     def set_price(self, price):
         self.price = price
 
+    def get_order_fee_currency(self):
+        return self.order_fee_currency
+
+    def set_order_fee_currency(self, order_fee_currency):
+        self.order_fee_currency = order_fee_currency
+
+    def get_order_fee_rate(self):
+        return self.order_fee_rate
+
+    def set_order_fee_rate(self, order_fee_rate):
+        self.order_fee_rate = order_fee_rate
+
+    def get_order_fee(self):
+        return self.order_fee
+
+    def set_order_fee(self, order_fee):
+        self.order_fee = order_fee
+
     def get_order_size(self):
         return self.order_side
 
     def get_status(self) -> OrderStatus:
         return self.status
 
     def set_status(self, status):
@@ -228,37 +244,48 @@
     def set_available_amount(self, available_amount):
         self._available_amount = available_amount
 
     @available_amount.setter
     def available_amount(self, available_amount):
         self.set_available_amount(available_amount)
 
-    def to_dict(self):
+    def to_dict(self, datetime_format=None):
+
+        if datetime_format is not None:
+            created_at = self.created_at.strftime(datetime_format) \
+                if self.created_at else None
+            updated_at = self.updated_at.strftime(datetime_format) \
+                if self.updated_at else None
+            trade_closed_at = self.trade_closed_at.strftime(datetime_format) \
+                if self.trade_closed_at else None
+        else:
+            created_at = self.created_at
+            updated_at = self.updated_at
+            trade_closed_at = self.trade_closed_at
+
         return {
             "external_id": self.external_id,
             "target_symbol": self.target_symbol,
             "trading_symbol": self.trading_symbol,
             "order_side": self.order_side,
             "order_type": self.order_type,
             "status": self.status,
             "price": self.price,
             "amount": self.amount,
             "net_gain": self.net_gain,
-            "trade_closed_at": self.trade_closed_at,
+            "trade_closed_at": trade_closed_at,
             "trade_closed_price": self.trade_closed_price,
-            "created_at": self.created_at,
-            "updated_at": self.updated_at,
+            "created_at": created_at,
+            "updated_at": updated_at,
             "filled": self.filled,
             "remaining": self.remaining,
             "cost": self.cost,
-            "fee": self.fee.to_dict() if self.fee is not None else None,
-            "stop_loss": self.stop_loss,
-            "stop_loss_percentage": self.stop_loss_percentage,
-            "trailing_stop_loss": self.trailing_stop_loss,
-            "trailing_stop_loss_percentage": self.trailing_stop_loss_percentage
+            "order_fee_currency": self.order_fee_currency,
+            "order_fee_rate": self.order_fee_rate,
+            "order_fee": self.order_fee,
         }
 
     @staticmethod
     def from_dict(data: dict):
         created_at = data.get("created_at", None)
         updated_at = data.get("updated_at", None)
         symbol = data.get("symbol", None)
@@ -286,35 +313,55 @@
             order_type=data.get("order_type", None),
             order_side=data.get("order_side", None),
             filled=data.get("filled", None),
             remaining=data.get("remaining", None),
             cost=data.get("cost", None),
             fee=data.get("fee", None),
             created_at=created_at,
-            updated_at=updated_at
+            updated_at=updated_at,
+            order_fee=data.get("order_fee", None),
+            order_fee_currency=data.get("order_fee_currency", None),
+            order_fee_rate=data.get("order_fee_rate", None),
         )
 
     @staticmethod
     def from_ccxt_order(ccxt_order):
+        """
+        Create an Order object from a ccxt order object
+        :param ccxt_order: ccxt order object
+        :return: Order object
+        """
         status = OrderStatus.from_value(ccxt_order["status"])
         target_symbol = ccxt_order.get("symbol").split("/")[0]
         trading_symbol = ccxt_order.get("symbol").split("/")[1]
+        ccxt_fee = ccxt_order.get("fee", None)
+        order_fee = None
+        order_fee_currency = None
+        order_fee_rate = None
+
+        if ccxt_fee is not None:
+            order_fee = ccxt_fee.get("cost", None)
+            order_fee_currency = ccxt_fee.get("currency", None)
+            order_fee_rate = ccxt_fee.get("rate", None)
+
         return Order(
             external_id=ccxt_order.get("id", None),
             target_symbol=target_symbol,
             trading_symbol=trading_symbol,
             price=ccxt_order.get("price", None),
             amount=ccxt_order.get("amount", None),
             status=status,
             order_type=ccxt_order.get("type", None),
             order_side=ccxt_order.get("side", None),
             filled=ccxt_order.get("filled", None),
             remaining=ccxt_order.get("remaining", None),
             cost=ccxt_order.get("cost", None),
-            fee=OrderFee.from_ccxt_fee(ccxt_order.get("fee", None)),
+            order_fee=order_fee,
+            order_fee_currency=order_fee_currency,
+            order_fee_rate=order_fee_rate,
             created_at=parse(ccxt_order.get("datetime", None))
         )
 
     def __repr__(self):
 
         if not hasattr(self, "id"):
             id_value = "ccxt external order"
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order_status.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/position/position_snapshot.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/strategy_profile.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/strategy_profile.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trade/trade.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trade/trade.py`

 * *Files 10% similar despite different names*

```diff
@@ -226,14 +226,31 @@
 
                 prices = filtered_df['Close'].to_numpy()
 
             highest_price = max(prices)
             stop_loss_price = highest_price * (1 - stop_loss_percentage / 100)
             return current_price <= stop_loss_price
 
+    def to_dict(self):
+        return {
+            "target_symbol": self.target_symbol,
+            "trading_symbol": self.trading_symbol,
+            "status": self.status,
+            "amount": self.amount,
+            "open_price": self.open_price,
+            "current_price": self.current_price,
+            "closed_price": self.closed_price,
+            "opened_at": self.opened_at.strftime(DATETIME_FORMAT)
+            if self.opened_at else None,
+            "closed_at": self.closed_at.strftime(DATETIME_FORMAT)
+            if self.closed_at else None,
+            "change": self.percentage_change,
+            "absolute_change": self.absolute_change,
+        }
+
     def __repr__(self):
         return self.repr(
             target_symbol=self.target_symbol,
             trading_symbol=self.trading_symbol,
             status=self.status,
             amount=self.amount,
             open_price=self.open_price,
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trade/trade_status.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trade/trade_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/market_credential_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/market_data_sources.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/market_data_sources.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/market_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/services/rounding_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/services/rounding_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .backtesting import pretty_print_backtest, \
+from .backtesting import pretty_print_backtest, load_backtest_report, \
     pretty_print_backtest_reports_evaluation, load_backtest_reports
 from .csv import get_total_amount_of_rows, append_dict_as_row_to_csv, \
     add_column_headers_to_csv, csv_to_list, load_csv_into_dict
 from .random import random_string
 from .stoppable_thread import StoppableThread
 from .synchronized import synchronized
 
@@ -13,9 +13,10 @@
     'get_total_amount_of_rows',
     'append_dict_as_row_to_csv',
     'add_column_headers_to_csv',
     'csv_to_list',
     'pretty_print_backtest',
     'pretty_print_backtest_reports_evaluation',
     'load_csv_into_dict',
+    'load_backtest_report',
     'load_backtest_reports',
 ]
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/backtesting.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/backtesting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import json
 from datetime import datetime
 from typing import List, Tuple
 
 from tabulate import tabulate
 
 from investing_algorithm_framework.domain import DATETIME_FORMAT
 from investing_algorithm_framework.domain.exceptions import \
@@ -458,14 +459,34 @@
         ]
         trades_table[f"Close price ({backtest_report.trading_symbol})"] = [
             trade.closed_price for trade in backtest_report.trades
         ]
         print(tabulate(trades_table, headers="keys", tablefmt="rounded_grid"))
 
 
+def load_backtest_report(file_path: str) -> BacktestReport:
+    """
+    Load a backtest report from a file.
+
+    param file_path: The file path
+    :return: The backtest report
+    """
+
+    if not os.path.isfile(file_path):
+        raise OperationalException("File does not exist")
+
+    if not file_path.endswith(".json"):
+        raise OperationalException("File is not a json file")
+
+    with open(file_path, 'r') as json_file:
+        data = json.load(json_file)
+
+    return BacktestReport.from_dict(data)
+
+
 def load_backtest_reports(folder_path: str) -> List[BacktestReport]:
     """
     Load backtest reports from a folder.
 
     param folder_path: The folder path
     :return: The backtest reports
     """
@@ -476,15 +497,14 @@
 
     list_of_files = os.listdir(folder_path)
 
     if not list_of_files:
         raise OperationalException(f"Folder {folder_path} is empty")
 
     for file in list_of_files:
-        if not file.endswith(".csv"):
+        if not file.endswith(".json"):
             continue
         file_path = os.path.join(folder_path, file)
-        data = load_csv_into_dict(file_path)
-        report = BacktestReport.from_dict(data)
+        report = load_backtest_report(file_path)
         backtest_reports.append(report)
 
     return backtest_reports
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from .database import setup_sqlalchemy, Session, \
     create_all_tables
-from .models import SQLPortfolio, SQLOrder, SQLPosition, SQLOrderFee, \
+from .models import SQLPortfolio, SQLOrder, SQLPosition, \
     SQLPortfolioSnapshot, SQLPositionSnapshot, \
     CCXTOHLCVBacktestMarketDataSource, CCXTOrderBookMarketDataSource, \
     CCXTTickerMarketDataSource, CCXTOHLCVMarketDataSource, \
     CSVOHLCVMarketDataSource, CSVTickerMarketDataSource
 from .repositories import SQLOrderRepository, SQLPositionRepository, \
-    SQLPortfolioRepository, SQLOrderFeeRepository, \
+    SQLPortfolioRepository, \
     SQLPortfolioSnapshotRepository, SQLPositionSnapshotRepository
 from .services import PerformanceService, CCXTMarketService
 
 __all__ = [
     "create_all_tables",
     "SQLPositionRepository",
     "SQLPortfolioRepository",
     "SQLOrderRepository",
-    "SQLOrderFeeRepository",
     "SQLPortfolioSnapshotRepository",
     "SQLPositionSnapshotRepository",
     "setup_sqlalchemy",
     "Session",
     "SQLPortfolio",
     "SQLOrder",
-    "SQLOrderFee",
     "SQLPosition",
     "PerformanceService",
     "SQLPortfolioSnapshot",
     "SQLPositionSnapshot",
     "CCXTOHLCVMarketDataSource",
     "CCXTOrderBookMarketDataSource",
     "CCXTTickerMarketDataSource",
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from .market_data_sources import CCXTOrderBookMarketDataSource, \
     CCXTTickerMarketDataSource, CCXTOHLCVMarketDataSource, \
     CCXTOHLCVBacktestMarketDataSource, CSVOHLCVMarketDataSource, \
     CSVTickerMarketDataSource
-from .order import SQLOrder, SQLOrderFee
+from .order import SQLOrder
 from .portfolio import SQLPortfolio, SQLPortfolioSnapshot
 from .position import SQLPosition, SQLPositionSnapshot
 
 __all__ = [
     "SQLOrder",
     "SQLPosition",
     "SQLPortfolio",
-    "SQLOrderFee",
     "SQLPositionSnapshot",
     "SQLPortfolioSnapshot",
     "CCXTOHLCVBacktestMarketDataSource",
     "CCXTOrderBookMarketDataSource",
     "CCXTTickerMarketDataSource",
     "CCXTOHLCVMarketDataSource",
     "CSVTickerMarketDataSource",
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from datetime import datetime
 
 from sqlalchemy import Column, Integer, String, DateTime, ForeignKey, Float
 from sqlalchemy.orm import relationship
 
 from investing_algorithm_framework.domain import OrderType, \
-    OrderSide, Order, OrderStatus, OrderFee
+    OrderSide, Order, OrderStatus
 from investing_algorithm_framework.infrastructure.database import SQLBaseModel
 from investing_algorithm_framework.infrastructure.models.model_extension \
     import SQLAlchemyModelExtension
 
 logger = logging.getLogger("investing_algorithm_framework")
 
 
@@ -31,20 +31,17 @@
     position = relationship("SQLPosition", back_populates="orders")
     created_at = Column(DateTime, default=datetime.utcnow)
     updated_at = Column(DateTime, default=datetime.utcnow)
     trade_closed_at = Column(DateTime, default=None)
     trade_closed_price = Column(Float, default=None)
     trade_closed_amount = Column(Float, default=None)
     net_gain = Column(Float, default=0)
-    fee = relationship(
-        "SQLOrderFee",
-        uselist=False,
-        back_populates="order",
-        cascade="all, delete"
-    )
+    order_fee = Column(Float, default=None)
+    order_fee_currency = Column(String)
+    order_fee_rate = Column(Float, default=None)
     _available_amount = None
 
     def update(self, data):
 
         if 'amount' in data and data['amount'] is not None:
             amount = data.pop('amount')
             self.amount = amount
@@ -97,29 +94,45 @@
             trade_closed_price=order.get_trade_closed_price(),
             trade_closed_amount=order.get_trade_closed_amount(),
             net_gain=order.get_net_gain(),
         )
 
     @staticmethod
     def from_ccxt_order(ccxt_order):
+        """
+        Create an Order object from a CCXT order object
+        :param ccxt_order: CCXT order object
+        """
         status = OrderStatus.from_value(ccxt_order["status"])
         target_symbol = ccxt_order.get("symbol").split("/")[0]
         trading_symbol = ccxt_order.get("symbol").split("/")[1]
+        ccxt_fee = ccxt_order.get("fee", None)
+        order_fee = None
+        order_fee_rate = None
+        order_fee_currency = None
+
+        if ccxt_fee is not None:
+            order_fee = ccxt_fee.get("cost", None)
+            order_fee_rate = ccxt_fee.get("rate", None)
+            order_fee_currency = ccxt_fee.get("currency", None)
+
         return Order(
             external_id=ccxt_order.get("id", None),
             target_symbol=target_symbol,
             trading_symbol=trading_symbol,
             price=ccxt_order.get("price", None),
             amount=ccxt_order.get("amount", None),
             status=status,
             order_type=ccxt_order.get("type", None),
             order_side=ccxt_order.get("side", None),
             filled=ccxt_order.get("filled", None),
             remaining=ccxt_order.get("remaining", None),
             cost=ccxt_order.get("cost", None),
-            fee=OrderFee.from_ccxt_fee(ccxt_order.get("fee", None)),
+            order_fee=order_fee,
+            order_fee_rate=order_fee_rate,
+            order_fee_currency=order_fee_currency,
             created_at=ccxt_order.get("datetime", None),
         )
 
     def __lt__(self, other):
         # Define the less-than comparison based on created_at attribute
         return self.created_at < other.created_at
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from sqlalchemy import Column, Integer, String, ForeignKey, Float
 from sqlalchemy.orm import relationship
 
-from investing_algorithm_framework.domain import OrderFee
+from investing_algorithm_framework.domain import PositionSnapshot
 from investing_algorithm_framework.infrastructure.database import SQLBaseModel
 from investing_algorithm_framework.infrastructure.models.model_extension \
     import SQLAlchemyModelExtension
 
 
-class SQLOrderFee(OrderFee, SQLBaseModel, SQLAlchemyModelExtension):
-    __tablename__ = "order_fees"
+class SQLPositionSnapshot(
+    SQLBaseModel, PositionSnapshot, SQLAlchemyModelExtension
+):
+    __tablename__ = "position_snapshots"
     id = Column(Integer, primary_key=True, unique=True)
-    currency = Column(String)
+    symbol = Column(String)
+    amount = Column(Float)
     cost = Column(Float)
-    rate = Column(Float)
-    order_id = Column(Integer, ForeignKey('orders.id'))
-    order = relationship("SQLOrder", back_populates="fee")
-
-    def __init__(self, currency, cost, rate, order_id):
-        super().__init__(currency, cost, rate)
-        self.order_id = order_id
+    portfolio_snapshot_id = Column(
+        Integer, ForeignKey('portfolio_snapshots.id')
+    )
+    portfolio_snapshot = relationship(
+        "SQLPortfolioSnapshot", back_populates="position_snapshots"
+    )
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import os
+import json
 
 from investing_algorithm_framework.domain import BacktestReport, \
     DATETIME_FORMAT_BACKTESTING
 
 
 class BacktestReportWriterService:
     """
@@ -17,26 +18,58 @@
     ) -> str:
         """
         Write a backtest report to a CSV file.
         """
 
         if not os.path.exists(output_directory):
             os.makedirs(output_directory)
+
+        csv_file_path = self.create_report_name(
+            report, output_directory, extension=".csv"
+        )
+        report_dict = report.to_dict()
+
+        with open(csv_file_path, 'w', newline='') as csv_file:
+            writer = csv.DictWriter(csv_file, fieldnames=report_dict.keys())
+            writer.writeheader()
+            writer.writerow(report_dict)
+
+        return csv_file_path
+
+    def write_report_to_json(
+        self, report: BacktestReport, output_directory: str
+    ):
+        if not os.path.exists(output_directory):
+            os.makedirs(output_directory)
         backtest_start_date = report.backtest_start_date\
             .strftime(DATETIME_FORMAT_BACKTESTING)
         backtest_end_date = report.backtest_end_date\
             .strftime(DATETIME_FORMAT_BACKTESTING)
         created_at = report.created_at.strftime(DATETIME_FORMAT_BACKTESTING)
-        csv_file_path = os.path.join(
+        json_file_path = os.path.join(
             output_directory,
             f"report_{report.name}_backtest_start_date_"
             f"{backtest_start_date}_backtest_end_date_"
-            f"{backtest_end_date}_created_at_{created_at}.csv"
+            f"{backtest_end_date}_created_at_{created_at}.json"
         )
         report_dict = report.to_dict()
+        # Convert dictionary to JSON
+        json_data = json.dumps(report_dict, indent=4)
 
-        with open(csv_file_path, 'w', newline='') as csv_file:
-            writer = csv.DictWriter(csv_file, fieldnames=report_dict.keys())
-            writer.writeheader()
-            writer.writerow(report_dict)
-
-        return csv_file_path
+        # Write JSON data to a .json file
+        with open(json_file_path, "w") as json_file:
+            json_file.write(json_data)
+
+    @staticmethod
+    def create_report_name(report, output_directory, extension=".json"):
+        backtest_start_date = report.backtest_start_date \
+            .strftime(DATETIME_FORMAT_BACKTESTING)
+        backtest_end_date = report.backtest_end_date \
+            .strftime(DATETIME_FORMAT_BACKTESTING)
+        created_at = report.created_at.strftime(DATETIME_FORMAT_BACKTESTING)
+        file_path = os.path.join(
+            output_directory,
+            f"report_{report.name}_backtest_start_date_"
+            f"{backtest_start_date}_backtest_end_date_"
+            f"{backtest_end_date}_created_at_{created_at}{extension}"
+        )
+        return file_path
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/backtesting/backtest_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/backtesting/backtest_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,14 @@
             if None in ids:
                 # Remove None from ids
                 ids = [x for x in ids if x is not None]
 
             backtest_profile = BacktestReport(
                 name=algorithm.name,
                 strategy_identifiers=ids,
-                backtest_index_date=start_date,
                 backtest_start_date=start_date,
                 backtest_end_date=end_date,
                 initial_unallocated=initial_unallocated,
                 trading_symbol=portfolio.trading_symbol,
                 created_at=datetime.utcnow(),
             )
             backtest_profile.number_of_runs = number_of_runs
@@ -273,14 +272,17 @@
                 self._performance_service\
                 .get_total_net_gain_percentage_of_backtest(
                     portfolio.id, backtest_profile
                 )
             positions = self._position_repository.get_all({
                 "portfolio": portfolio.id
             })
+            orders = self._order_service.get_all({
+                "portfolio": portfolio.id
+            })
             tickers = {}
 
             for position in positions:
 
                 if position.symbol != portfolio.trading_symbol:
                     ticker_symbol = \
                         f"{position.symbol}/{portfolio.trading_symbol}"
@@ -356,14 +358,15 @@
                                    f"/{portfolio.trading_symbol}",
                             market=portfolio.market
                         )
                     backtest_position.price = ticker["bid"]
                 backtest_positions.append(backtest_position)
             backtest_profile.positions = backtest_positions
             backtest_profile.trades = algorithm.get_trades()
+            backtest_profile.orders = orders
             return backtest_profile
 
     def set_backtest_market_data_sources(self, market_data_sources):
         self._backtest_market_data_sources = market_data_sources
 
     def get_backtest_market_data_sources(self):
         return self._backtest_market_data_sources
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/configuration_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/market_credential_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/order_service/order_backtest_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/order_service/order_backtest_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 
 
 class OrderBacktestService(OrderService):
 
     def __init__(
         self,
         order_repository,
-        order_fee_repository,
         position_repository,
         portfolio_repository,
         portfolio_configuration_service,
         portfolio_snapshot_service,
         configuration_service,
         market_data_source_service: BacktestMarketDataSourceService,
     ):
         super(OrderService, self).__init__(order_repository)
         self.order_repository = order_repository
-        self.order_fee_repository = order_fee_repository
         self.position_repository = position_repository
         self.portfolio_repository = portfolio_repository
         self.portfolio_configuration_service = portfolio_configuration_service
         self.portfolio_snapshot_service = portfolio_snapshot_service
         self.configuration_service = configuration_service
         self._market_data_source_service: BacktestMarketDataSourceService = \
             market_data_source_service
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/order_service/order_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/order_service/order_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,62 +14,51 @@
 
 class OrderService(RepositoryService):
 
     def __init__(
         self,
         configuration_service,
         order_repository,
-        order_fee_repository,
         market_service: MarketService,
         position_repository,
         portfolio_repository,
         portfolio_configuration_service,
         portfolio_snapshot_service,
         market_credential_service
     ):
         super(OrderService, self).__init__(order_repository)
         self.configuration_service = configuration_service
         self.order_repository = order_repository
-        self.order_fee_repository = order_fee_repository
         self.market_service: MarketService = market_service
         self.position_repository = position_repository
         self.portfolio_repository = portfolio_repository
         self.portfolio_configuration_service = portfolio_configuration_service
         self.portfolio_snapshot_service = portfolio_snapshot_service
         self.market_credential_service = market_credential_service
 
     def create(self, data, execute=True, validate=True, sync=True) -> Order:
         portfolio_id = data["portfolio_id"]
         portfolio = self.portfolio_repository.get(portfolio_id)
 
         if validate:
             self.validate_order(data, portfolio)
 
-        order_fee = None
-
-        if "fee" in data:
-            order_fee = data.pop("fee")
-
         del data["portfolio_id"]
         symbol = data["target_symbol"]
 
         if validate:
             self.validate_order(data, portfolio)
 
         position = self._create_position_if_not_exists(symbol, portfolio)
         data["position_id"] = position.id
         data["remaining"] = data["amount"]
         data["status"] = OrderStatus.CREATED.value
         order = self.order_repository.create(data)
         order_id = order.id
 
-        if order_fee:
-            order_fee["order_id"] = order_id
-            self.order_fee_repository.create(order_fee)
-
         if sync:
             if OrderSide.BUY.equals(order.get_order_side()):
                 self._sync_portfolio_with_created_buy_order(order)
             else:
                 self._sync_portfolio_with_created_sell_order(order)
 
         self.create_snapshot(portfolio.id, created_at=order.created_at)
@@ -88,28 +77,14 @@
                 "id": previous_order.position_id,
                 "symbol": previous_order.trading_symbol
             }
         )
         portfolio = self.portfolio_repository.get(
             trading_symbol_position.portfolio_id
         )
-
-        if "fee" in data:
-            order_fee_data = data.pop("fee")
-
-            if order_fee_data is not None:
-                if self.order_fee_repository.exists({"order_id": object_id}):
-                    order_fee = self.order_fee_repository\
-                        .find({"order_id": object_id})
-                    self.order_fee_repository\
-                        .update(order_fee.id, order_fee_data)
-                else:
-                    order_fee_data["order_id"] = object_id
-                    self.order_fee_repository.create(order_fee_data)
-
         new_order = self.order_repository.update(object_id, data)
         filled_difference = new_order.get_filled() \
             - previous_order.get_filled()
 
         if filled_difference:
 
             if OrderSide.BUY.equals(new_order.get_order_side()):
@@ -144,17 +119,14 @@
             created_at = data["updated_at"]
         else:
             created_at = datetime.now(tz=tzutc())
 
         self.create_snapshot(portfolio.id, created_at=created_at)
         return new_order
 
-    def get_order_fee(self, order_id):
-        return self.order_fee_repository.find({"order": order_id})
-
     def execute_order(self, order_id, portfolio):
         order = self.get(order_id)
 
         try:
             if OrderType.LIMIT.equals(order.get_order_type()):
 
                 if OrderSide.BUY.equals(order.get_order_side()):
```

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/position_snapshot_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/position_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/investing_algorithm_framework/services/trade_service/trade_service.py` & `investing_algorithm_framework-3.6.0/investing_algorithm_framework/services/trade_service/trade_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.2/pyproject.toml` & `investing_algorithm_framework-3.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investing-algorithm-framework"
-version = "v3.5.2"
+version = "v3.6.0"
 description = "A framework for creating trading bots"
 authors = ["MDUYN"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 wrapt = "^1.16.0"
```

### Comparing `investing_algorithm_framework-3.5.2/PKG-INFO` & `investing_algorithm_framework-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 3.5.2
+Version: 3.6.0
 Summary: A framework for creating trading bots
 Author: MDUYN
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.5.2
+Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.6.0
 Summary: A framework for creating trading bots Author: MDUYN Requires-Python:
 >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.9,<4.0.0) Requires-Dist: Flask-Migrate
 (>=2.6.0,<3.0.0) Requires-Dist: MarkupSafe (>=2.1.2,<3.0.0) Requires-Dist:
```

