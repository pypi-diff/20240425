# Comparing `tmp/openbb_nightly-4.1.7.dev202404230010.tar.gz` & `tmp/openbb_nightly-4.1.7.dev202404240009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.7.dev202404230010.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.7.dev202404240009.tar", max compression
```

## Comparing `openbb_nightly-4.1.7.dev202404230010.tar` & `openbb_nightly-4.1.7.dev202404240009.tar`

### file list

```diff
@@ -1,791 +1,792 @@
--rw-r--r--   0        0        0     6818 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/README.md
--rw-r--r--   0        0        0       19 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1972 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0       34 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0       30 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7189 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0       30 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    18672 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2563 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5938 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2705 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2964 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8326 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2238 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      966 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2247 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0       29 2024-04-23 00:10:04.635662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0       38 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      302 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       99 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      551 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      252 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      458 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0     1908 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/api_settings.py
--rw-r--r--   0        0        0     1035 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      398 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3875 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      502 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2233 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1054 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/field.py
--rw-r--r--   0        0        0      694 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      474 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     5669 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9094 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1477 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      536 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0      801 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/python_settings.py
--rw-r--r--   0        0        0       37 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0      130 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     4044 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    21268 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    23086 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2627 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10402 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3511 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3064 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0       30 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7595 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2024 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1582 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1948 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    65939 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3077 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     2224 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5986 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2396 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2581 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     8142 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0     1377 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/available_indicators.py
--rw-r--r--   0        0        0      630 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-04-23 00:10:04.639662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1288 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     3722 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/country_profile.py
--rw-r--r--   0        0        0     1591 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      423 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1886 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/economic_indicators.py
--rw-r--r--   0        0        0     1750 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      888 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      939 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     2390 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6200 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-04-23 00:10:04.643662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3083 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3474 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     5013 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9699 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.647662 openbb_nightly-4.1.7.dev202404230010/core/openbb_core/py.typed
--rw-r--r--   0        0        0       34 2024-04-23 00:10:04.651662 openbb_nightly-4.1.7.dev202404230010/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-23 00:10:04.651662 openbb_nightly-4.1.7.dev202404230010/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0       31 2024-04-23 00:10:04.651662 openbb_nightly-4.1.7.dev202404230010/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-23 00:10:04.651662 openbb_nightly-4.1.7.dev202404230010/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0       34 2024-04-23 00:10:04.651662 openbb_nightly-4.1.7.dev202404230010/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3848 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0       37 2024-04-23 00:10:04.655662 openbb_nightly-4.1.7.dev202404230010/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4117 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0       32 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0    11799 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2336 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5816 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3493 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     3832 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3787 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6392 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.659662 openbb_nightly-4.1.7.dev202404230010/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4097 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0       29 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8654 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14268 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1378 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10942 2024-04-23 00:10:04.663662 openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0       35 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16738 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    19706 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/relative_rotation.py
--rw-r--r--   0        0        0    64220 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0    19798 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    40926 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0       28 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-04-23 00:10:04.667662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-04-23 00:10:04.687662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17442 2024-04-23 00:10:04.687662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-04-23 00:10:04.687662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0       42 2024-04-23 00:10:04.687662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     8068 2024-04-23 00:10:04.687662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2554 2024-04-23 00:10:04.687662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58532 2024-04-23 00:10:04.687662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228579 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0       30 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7185 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12381 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0       25 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
--rw-r--r--   0        0        0     8555 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    19572 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3300 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5697 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6877 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3547 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    25006 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1437 2024-04-23 00:10:04.711662 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   717892 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2246 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0    26843 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0       32 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/__init__.py
--rw-r--r--   0        0        0      603 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/colors.py
--rw-r--r--   0        0        0     3462 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0     3491 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0    20295 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
--rw-r--r--   0        0        0     2493 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0    16657 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
--rw-r--r--   0        0        0     1440 2024-04-23 00:10:04.715663 openbb_nightly-4.1.7.dev202404230010/openbb/__init__.py
--rw-r--r--   0        0        0  1211662 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/assets/reference.json
--rw-r--r--   0        0        0     2813 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/__extensions__.py
--rw-r--r--   0        0        0       50 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/__init__.py
--rw-r--r--   0        0        0     3299 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/crypto.py
--rw-r--r--   0        0        0     6468 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    11706 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/currency.py
--rw-r--r--   0        0        0     6360 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12047 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    65529 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/economy.py
--rw-r--r--   0        0        0    12355 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27548 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity.py
--rw-r--r--   0        0        0    18353 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2807 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    25823 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    40717 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   167585 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30431 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26606 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3504 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    75407 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/etf.py
--rw-r--r--   0        0        0     4538 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    19470 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7001 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26229 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    10857 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11744 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/index.py
--rw-r--r--   0        0        0    15304 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/regulators.py
--rw-r--r--   0        0        0    16380 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/package/regulators_sec.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.719663 openbb_nightly-4.1.7.dev202404230010/openbb/py.typed
--rw-r--r--   0        0        0     1106 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12452 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      877 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    17979 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9801 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-04-23 00:10:04.723662 openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      779 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     1779 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-04-23 00:10:04.727663 openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      895 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-04-23 00:10:04.731663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-04-23 00:10:04.735663 openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      805 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/__init__.py
--rw-r--r--   0        0        0       21 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/models/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/models/available_indicators.py
--rw-r--r--   0        0        0    12504 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/models/country_profile.py
--rw-r--r--   0        0        0    18643 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/models/economic_indicators.py
--rw-r--r--   0        0        0       24 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/__init__.py
--rw-r--r--   0        0        0    22209 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/helpers.py
--rw-r--r--   0        0        0    24368 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/indicator_countries.json
--rw-r--r--   0        0        0     5244 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
--rw-r--r--   0        0        0    66758 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/multipliers.json
--rw-r--r--   0        0        0    87109 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/scales.json
--rw-r--r--   0        0        0    73815 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
--rw-r--r--   0        0        0    90624 2024-04-23 00:10:04.783663 openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/units.json
--rw-r--r--   0        0        0      716 2024-04-23 00:10:04.787663 openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-04-23 00:10:04.787663 openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-04-23 00:10:04.787663 openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-04-23 00:10:04.787663 openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      538 2024-04-23 00:10:04.795663 openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-23 00:10:04.795663 openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-04-23 00:10:04.795663 openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-04-23 00:10:04.795663 openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5553 2024-04-23 00:10:04.795663 openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1005 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9573 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.851663 openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     8255 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6076 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5308 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-04-23 00:10:04.855663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6768 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2780 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5050 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2270 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3938 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     6297 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3521 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3270 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.859663 openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     3126 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6656 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-04-23 00:10:04.879663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-04-23 00:10:04.883663 openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      988 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5269 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     5393 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3273 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2376 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7327 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8417 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9694 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5090 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3357 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8901 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-04-23 00:10:04.887663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6513 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2560 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-04-23 00:10:04.891663 openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     1840 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6330 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5157 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-04-23 00:10:04.899663 openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      981 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2100 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6283 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6255 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7150 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-04-23 00:10:04.907663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     6142 2024-04-23 00:10:04.911663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3734 2024-04-23 00:10:04.911663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-04-23 00:10:04.911663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.911663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-04-23 00:10:04.911663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-04-23 00:10:04.911663 openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1562 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8328 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2615 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13896 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7434 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:04.927663 openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      512 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      677 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1120 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-23 00:10:05.019664 openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3319 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5162 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4647 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8843 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5455 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12451 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10325 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5986 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-04-23 00:10:05.031664 openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1241 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6582 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9222 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10325 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-23 00:10:05.131664 openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      440 2024-04-23 00:10:05.135664 openbb_nightly-4.1.7.dev202404230010/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4606 2024-04-23 00:10:05.135664 openbb_nightly-4.1.7.dev202404230010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-04-23 00:10:05.135664 openbb_nightly-4.1.7.dev202404230010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3719 2024-04-23 00:10:05.135664 openbb_nightly-4.1.7.dev202404230010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1044 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4232 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     2036 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5858 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10102 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4230 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6552 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-04-23 00:10:05.139664 openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     7005 2024-04-23 00:10:14.335693 openbb_nightly-4.1.7.dev202404230010/pyproject.toml
--rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202404230010/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/README.md
+-rw-r--r--   0        0        0       19 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7189 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    18672 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1908 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/api_settings.py
+-rw-r--r--   0        0        0     1035 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3875 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      502 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2233 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1054 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/field.py
+-rw-r--r--   0        0        0      694 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      474 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     5669 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9094 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1477 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0      801 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/python_settings.py
+-rw-r--r--   0        0        0       37 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     4044 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-04-24 00:09:20.109956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    21268 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23086 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10402 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3511 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7595 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2024 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1948 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    65939 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2224 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1368 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2581 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     8142 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0     1377 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/available_indicators.py
+-rw-r--r--   0        0        0      630 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1246 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     3722 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/country_profile.py
+-rw-r--r--   0        0        0     1591 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      423 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1886 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/economic_indicators.py
+-rw-r--r--   0        0        0     1750 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-04-24 00:09:20.113956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      912 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      939 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     2390 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3083 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3474 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-04-24 00:09:20.117956 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9699 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.121955 openbb_nightly-4.1.7.dev202404240009/core/openbb_core/py.typed
+-rw-r--r--   0        0        0       34 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0       31 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3848 2024-04-24 00:09:20.125956 openbb_nightly-4.1.7.dev202404240009/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0       32 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0    11799 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.129956 openbb_nightly-4.1.7.dev202404240009/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6392 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-04-24 00:09:20.133956 openbb_nightly-4.1.7.dev202404240009/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0       29 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0       35 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    64220 2024-04-24 00:09:20.137956 openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0    19798 2024-04-24 00:09:20.141955 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-04-24 00:09:20.141955 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    40926 2024-04-24 00:09:20.141955 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-04-24 00:09:20.141955 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-04-24 00:09:20.141955 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-04-24 00:09:20.157956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17442 2024-04-24 00:09:20.157956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-04-24 00:09:20.157956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-04-24 00:09:20.157956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     8068 2024-04-24 00:09:20.157956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-04-24 00:09:20.157956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58532 2024-04-24 00:09:20.157956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228579 2024-04-24 00:09:20.181956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-04-24 00:09:20.181956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12381 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0       25 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
+-rw-r--r--   0        0        0     8555 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    19572 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3300 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5697 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6877 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3547 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    25006 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-04-24 00:09:20.185956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0    26843 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0       32 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/colors.py
+-rw-r--r--   0        0        0     3462 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0     3491 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0    20295 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
+-rw-r--r--   0        0        0     2493 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0    16657 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
+-rw-r--r--   0        0        0     1440 2024-04-24 00:09:20.189956 openbb_nightly-4.1.7.dev202404240009/openbb/__init__.py
+-rw-r--r--   0        0        0  1214504 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2813 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0       50 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/__init__.py
+-rw-r--r--   0        0        0     3299 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6468 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    13823 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/currency.py
+-rw-r--r--   0        0        0     6360 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12047 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    65529 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/economy.py
+-rw-r--r--   0        0        0    12355 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27558 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity.py
+-rw-r--r--   0        0        0    18353 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2807 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    25823 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    40717 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   163982 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30431 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26606 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3710 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    75407 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/etf.py
+-rw-r--r--   0        0        0     4538 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    19470 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7001 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26229 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    10857 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11744 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/index.py
+-rw-r--r--   0        0        0    15304 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/regulators.py
+-rw-r--r--   0        0        0    16379 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/package/regulators_sec.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.193956 openbb_nightly-4.1.7.dev202404240009/openbb/py.typed
+-rw-r--r--   0        0        0     1106 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12452 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      877 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    17979 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9801 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-24 00:09:20.197955 openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     1779 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4725 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     5698 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-04-24 00:09:20.201956 openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      895 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-04-24 00:09:20.205956 openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      805 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/models/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/models/available_indicators.py
+-rw-r--r--   0        0        0    12504 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/models/country_profile.py
+-rw-r--r--   0        0        0    18643 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/models/economic_indicators.py
+-rw-r--r--   0        0        0       24 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/__init__.py
+-rw-r--r--   0        0        0    22209 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/helpers.py
+-rw-r--r--   0        0        0    24368 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/indicator_countries.json
+-rw-r--r--   0        0        0     5244 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
+-rw-r--r--   0        0        0    66758 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/multipliers.json
+-rw-r--r--   0        0        0    87109 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/scales.json
+-rw-r--r--   0        0        0    73815 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
+-rw-r--r--   0        0        0    90624 2024-04-24 00:09:20.257956 openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/units.json
+-rw-r--r--   0        0        0      716 2024-04-24 00:09:20.265956 openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-04-24 00:09:20.265956 openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-04-24 00:09:20.265956 openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3510 2024-04-24 00:09:20.265956 openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      538 2024-04-24 00:09:20.281956 openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-04-24 00:09:20.281956 openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-04-24 00:09:20.281956 openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-04-24 00:09:20.281956 openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-04-24 00:09:20.281956 openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1005 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9573 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     8255 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-24 00:09:20.353956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6076 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5308 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6768 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2780 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5050 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3521 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3270 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.357956 openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     3126 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-04-24 00:09:20.377956 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6338 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6656 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-04-24 00:09:20.381955 openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      988 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5269 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     5393 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22983 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     3273 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-04-24 00:09:20.385956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     8675 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2376 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7327 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8417 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9694 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5090 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3357 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6513 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     2560 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-04-24 00:09:20.389956 openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     1840 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5157 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-04-24 00:09:20.401955 openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      981 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-04-24 00:09:20.405956 openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2247 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     6961 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6283 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6255 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6125 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     9753 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/currency_snapshots.py
+-rw-r--r--   0        0        0     7150 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6142 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-04-24 00:09:20.409956 openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1562 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1658 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0    10150 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     3154 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2681 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    38596 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2766 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2051 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2900 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3498 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1796 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    15490 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7587 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.425956 openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      512 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1120 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3651 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5295 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4662 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5323 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-24 00:09:20.517956 openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3319 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5162 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4647 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8843 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5455 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12451 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10325 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5986 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5133 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-04-24 00:09:20.529955 openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1241 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6582 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9222 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-24 00:09:20.629956 openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      440 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1044 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-04-24 00:09:20.633956 openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4232 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     2036 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5858 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10102 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4230 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-04-24 00:09:20.637956 openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     7005 2024-04-24 00:09:33.757954 openbb_nightly-4.1.7.dev202404240009/pyproject.toml
+-rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202404240009/PKG-INFO
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/README.md` & `openbb_nightly-4.1.7.dev202404240009/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/app_loader.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/app_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/command_runner.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/logging_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/utils/expired_files.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/abstract/singleton.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/abstract/singleton.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/api_settings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/api_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/credentials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/field.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/field.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/hub/hub_session.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/obbject.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/preferences.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/profile.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/python_settings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/python_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/provider_interface.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/query.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/router.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/system_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/service/user_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/package_builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/utils/filters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/app/version.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/env.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/available_indicators.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class CotSearchQueryParams(QueryParams):
     """Commitment of Traders Reports Search Query."""
 
     query: str = Field(description="Search query.", default="")
     use_cache: Optional[bool] = Field(
         default=True,
-        description="Whether or not to use cache. If True, cache will store for seven days.",
+        description="Whether or not to use cache.",
     )
 
 
 class CotSearchData(Data):
     """Commitment of Traders Reports Search Data."""
 
     code: str = Field(description="CFTC Code of the report.")
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/country_profile.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
 class EquitySearchData(Data):
     """Equity Search Data."""
 
     symbol: Optional[str] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
     )
-    name: str = Field(description="Name of the company.")
+    name: Optional[str] = Field(default=None, description="Name of the company.")
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/standard_models/world_news.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/core/openbb_core/provider/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/currency/openbb_currency/currency_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/economy/openbb_economy/economy_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/index/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/relative_rotation.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.7.dev202404240009/extensions/technical/openbb_technical/technical_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/charting_router.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/charting_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/table.html` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/colors.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/colors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/utils/generic_charts.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py` & `openbb_nightly-4.1.7.dev202404240009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/assets/reference.json` & `openbb_nightly-4.1.7.dev202404240009/openbb/assets/reference.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999595198893572%*

 * *Differences: {"'paths'": "{'/currency/snapshots': {'parameters': {'standard': {0: {'description': 'The base "*

 * *            "currency symbol. Multiple items allowed for provider(s): fmp, polygon.'}, 3: {'type': "*

 * *            '"Literal[\'fmp\', \'polygon\']"}}, \'polygon\': []}, \'returns\': {\'OBBject\': {1: '*

 * *            '{\'type\': "Optional[Literal[\'fmp\', \'polygon\']]"}}}, \'data\': {\'polygon\': '*

 * *            "[OrderedDict([('name', 'vwap'), ('type', 'float'), ('description', 'The "*

 * *            "volume-weighted ave […]*

```diff
@@ -843,14 +843,156 @@
                         "default": null,
                         "description": "The timestamp of the last rate.",
                         "name": "last_rate_timestamp",
                         "optional": true,
                         "type": "datetime"
                     }
                 ],
+                "polygon": [
+                    {
+                        "default": null,
+                        "description": "The volume-weighted average price.",
+                        "name": "vwap",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The change in price from the previous day.",
+                        "name": "change",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The percentage change in price from the previous day.",
+                        "name": "change_percent",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The previous day's opening price.",
+                        "name": "prev_open",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The previous day's high price.",
+                        "name": "prev_high",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The previous day's low price.",
+                        "name": "prev_low",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The previous day's volume.",
+                        "name": "prev_volume",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The previous day's VWAP.",
+                        "name": "prev_vwap",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The current bid price.",
+                        "name": "bid",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The current ask price.",
+                        "name": "ask",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The open price from the most recent minute bar.",
+                        "name": "minute_open",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The high price from the most recent minute bar.",
+                        "name": "minute_high",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The low price from the most recent minute bar.",
+                        "name": "minute_low",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The close price from the most recent minute bar.",
+                        "name": "minute_close",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The volume from the most recent minute bar.",
+                        "name": "minute_volume",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The VWAP from the most recent minute bar.",
+                        "name": "minute_vwap",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The number of transactions in the most recent minute bar.",
+                        "name": "minute_transactions",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The timestamp of the last quote.",
+                        "name": "quote_timestamp",
+                        "optional": true,
+                        "type": "datetime"
+                    },
+                    {
+                        "default": null,
+                        "description": "The timestamp for the start of the most recent minute bar.",
+                        "name": "minute_timestamp",
+                        "optional": true,
+                        "type": "datetime"
+                    },
+                    {
+                        "default": "",
+                        "description": "The last time the data was updated.",
+                        "name": "last_updated",
+                        "optional": false,
+                        "type": "datetime"
+                    }
+                ],
                 "standard": [
                     {
                         "default": "",
                         "description": "The base, or domestic, currency.",
                         "name": "base_currency",
                         "optional": false,
                         "type": "str"
@@ -918,18 +1060,19 @@
                 "message": null
             },
             "description": "Snapshots of currency exchange rates from an indirect or direct perspective of a base currency.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.currency.snapshots(provider='fmp')\n# Get exchange rates from USD and XAU to EUR, JPY, and GBP using 'fmp' as provider.\nobb.currency.snapshots(provider='fmp', base='USD,XAU', counter_currencies='EUR,JPY,GBP', quote_type='indirect')\n```\n\n",
             "model": "CurrencySnapshots",
             "parameters": {
                 "fmp": [],
+                "polygon": [],
                 "standard": [
                     {
                         "default": "usd",
-                        "description": "The base currency symbol. Multiple items allowed for provider(s): fmp.",
+                        "description": "The base currency symbol. Multiple items allowed for provider(s): fmp, polygon.",
                         "name": "base",
                         "optional": true,
                         "type": "Union[str, List[str]]"
                     },
                     {
                         "default": "indirect",
                         "description": "Whether the quote is direct or indirect. Selecting 'direct' will return the exchange rate as the amount of domestic currency required to buy one unit of the foreign currency. Selecting 'indirect' (default) will return the exchange rate as the amount of foreign currency required to buy one unit of the domestic currency.",
@@ -945,29 +1088,29 @@
                         "type": "Union[List[str], str]"
                     },
                     {
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
-                        "type": "Literal['fmp']"
+                        "type": "Literal['fmp', 'polygon']"
                     }
                 ]
             },
             "returns": {
                 "OBBject": [
                     {
                         "description": "Serializable results.",
                         "name": "results",
                         "type": "List[CurrencySnapshots]"
                     },
                     {
                         "description": "Provider name.",
                         "name": "provider",
-                        "type": "Optional[Literal['fmp']]"
+                        "type": "Optional[Literal['fmp', 'polygon']]"
                     },
                     {
                         "description": "List of warnings.",
                         "name": "warnings",
                         "type": "Optional[List[Warning_]]"
                     },
                     {
@@ -10830,15 +10973,15 @@
                         "type": "date"
                     },
                     {
                         "default": null,
                         "description": "The SEC Act number.",
                         "name": "act",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The SEC Item numbers.",
                         "name": "items",
                         "optional": true,
                         "type": "Union[str, float]"
@@ -10858,50 +11001,50 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The accession number.",
                         "name": "accession_number",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The file number.",
                         "name": "file_number",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The film number.",
                         "name": "film_number",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "Whether the filing is an inline XBRL filing.",
                         "name": "is_inline_xbrl",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "Whether the filing is an XBRL filing.",
                         "name": "is_xbrl",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The size of the filing.",
                         "name": "size",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The URL to the complete filing submission.",
                         "name": "complete_submission_url",
                         "optional": true,
                         "type": "str"
@@ -11000,22 +11143,15 @@
                 ],
                 "sec": [
                     {
                         "default": null,
                         "description": "Lookup filings by Central Index Key (CIK) instead of by symbol.",
                         "name": "cik",
                         "optional": true,
-                        "type": "Union[int, str]"
-                    },
-                    {
-                        "default": null,
-                        "description": "Type of the SEC filing form.",
-                        "name": "type",
-                        "optional": true,
-                        "type": "Literal['1', '1-A', '1-A POS', '1-A-W', '1-E', '1-E AD', '1-K', '1-SA', '1-U', '1-Z', '1-Z-W', '10-12B', '10-12G', '10-D', '10-K', '10-KT', '10-Q', '10-QT', '11-K', '11-KT', '13F-HR', '13F-NT', '13FCONP', '144', '15-12B', '15-12G', '15-15D', '15F-12B', '15F-12G', '15F-15D', '18-12B', '18-K', '19B-4E', '2-A', '2-AF', '2-E', '20-F', '20FR12B', '20FR12G', '24F-2NT', '25', '25-NSE', '253G1', '253G2', '253G3', '253G4', '3', '305B2', '34-12H', '4', '40-17F1', '40-17F2', '40-17G', '40-17GCS', '40-202A', '40-203A', '40-206A', '40-24B2', '40-33', '40-6B', '40-8B25', '40-8F-2', '40-APP', '40-F', '40-OIP', '40FR12B', '40FR12G', '424A', '424B1', '424B2', '424B3', '424B4', '424B5', '424B7', '424B8', '424H', '425', '485APOS', '485BPOS', '485BXT', '486APOS', '486BPOS', '486BXT', '487', '497', '497AD', '497H2', '497J', '497K', '497VPI', '497VPU', '5', '6-K', '6B NTC', '6B ORDR', '8-A12B', '8-A12G', '8-K', '8-K12B', '8-K12G3', '8-K15D5', '8-M', '8F-2 NTC', '8F-2 ORDR', '9-M', 'ABS-15G', 'ABS-EE', 'ADN-MTL', 'ADV-E', 'ADV-H-C', 'ADV-H-T', 'ADV-NR', 'ANNLRPT', 'APP NTC', 'APP ORDR', 'APP WD', 'APP WDG', 'ARS', 'ATS-N', 'ATS-N-C', 'ATS-N/UA', 'AW', 'AW WD', 'C', 'C-AR', 'C-AR-W', 'C-TR', 'C-TR-W', 'C-U', 'C-U-W', 'C-W', 'CB', 'CERT', 'CERTARCA', 'CERTBATS', 'CERTCBO', 'CERTNAS', 'CERTNYS', 'CERTPAC', 'CFPORTAL', 'CFPORTAL-W', 'CORRESP', 'CT ORDER', 'D', 'DEF 14A', 'DEF 14C', 'DEFA14A', 'DEFA14C', 'DEFC14A', 'DEFC14C', 'DEFM14A', 'DEFM14C', 'DEFN14A', 'DEFR14A', 'DEFR14C', 'DEL AM', 'DFAN14A', 'DFRN14A', 'DOS', 'DOSLTR', 'DRS', 'DRSLTR', 'DSTRBRPT', 'EFFECT', 'F-1', 'F-10', 'F-10EF', 'F-10POS', 'F-1MEF', 'F-3', 'F-3ASR', 'F-3D', 'F-3DPOS', 'F-3MEF', 'F-4', 'F-4 POS', 'F-4MEF', 'F-6', 'F-6 POS', 'F-6EF', 'F-7', 'F-7 POS', 'F-8', 'F-8 POS', 'F-80', 'F-80POS', 'F-9', 'F-9 POS', 'F-N', 'F-X', 'FOCUSN', 'FWP', 'G-405', 'G-405N', 'G-FIN', 'G-FINW', 'IRANNOTICE', 'MA', 'MA-A', 'MA-I', 'MA-W', 'MSD', 'MSDCO', 'MSDW', 'N-1', 'N-14', 'N-14 8C', 'N-14MEF', 'N-18F1', 'N-1A', 'N-2', 'N-2 POSASR', 'N-23C-2', 'N-23C3A', 'N-23C3B', 'N-23C3C', 'N-2ASR', 'N-2MEF', 'N-30B-2', 'N-30D', 'N-4', 'N-5', 'N-54A', 'N-54C', 'N-6', 'N-6F', 'N-8A', 'N-8B-2', 'N-8F', 'N-8F NTC', 'N-8F ORDR', 'N-CEN', 'N-CR', 'N-CSR', 'N-CSRS', 'N-MFP', 'N-MFP1', 'N-MFP2', 'N-PX', 'N-Q', 'N-VP', 'N-VPFS', 'NO ACT', 'NPORT-EX', 'NPORT-NP', 'NPORT-P', 'NRSRO-CE', 'NRSRO-UPD', 'NSAR-A', 'NSAR-AT', 'NSAR-B', 'NSAR-BT', 'NSAR-U', 'NT 10-D', 'NT 10-K', 'NT 10-Q', 'NT 11-K', 'NT 20-F', 'NT N-CEN', 'NT N-MFP', 'NT N-MFP1', 'NT N-MFP2', 'NT NPORT-EX', 'NT NPORT-P', 'NT-NCEN', 'NT-NCSR', 'NT-NSAR', 'NTFNCEN', 'NTFNCSR', 'NTFNSAR', 'NTN 10D', 'NTN 10K', 'NTN 10Q', 'NTN 20F', 'OIP NTC', 'OIP ORDR', 'POS 8C', 'POS AM', 'POS AMI', 'POS EX', 'POS462B', 'POS462C', 'POSASR', 'PRE 14A', 'PRE 14C', 'PREC14A', 'PREC14C', 'PREM14A', 'PREM14C', 'PREN14A', 'PRER14A', 'PRER14C', 'PRRN14A', 'PX14A6G', 'PX14A6N', 'QRTLYRPT', 'QUALIF', 'REG-NR', 'REVOKED', 'RW', 'RW WD', 'S-1', 'S-11', 'S-11MEF', 'S-1MEF', 'S-20', 'S-3', 'S-3ASR', 'S-3D', 'S-3DPOS', 'S-3MEF', 'S-4', 'S-4 POS', 'S-4EF', 'S-4MEF', 'S-6', 'S-8', 'S-8 POS', 'S-B', 'S-BMEF', 'SBSE', 'SBSE-A', 'SBSE-BD', 'SBSE-C', 'SBSE-W', 'SC 13D', 'SC 13E1', 'SC 13E3', 'SC 13G', 'SC 14D9', 'SC 14F1', 'SC 14N', 'SC TO-C', 'SC TO-I', 'SC TO-T', 'SC13E4F', 'SC14D1F', 'SC14D9C', 'SC14D9F', 'SD', 'SDR', 'SE', 'SEC ACTION', 'SEC STAFF ACTION', 'SEC STAFF LETTER', 'SF-1', 'SF-3', 'SL', 'SP 15D2', 'STOP ORDER', 'SUPPL', 'T-3', 'TA-1', 'TA-2', 'TA-W', 'TACO', 'TH', 'TTW', 'UNDER', 'UPLOAD', 'WDL-REQ', 'X-17A-5']"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": true,
                         "description": "Whether or not to use cache. If True, cache will store for one day.",
                         "name": "use_cache",
                         "optional": true,
                         "type": "bool"
@@ -20253,18 +20389,18 @@
                         "default": null,
                         "description": "Symbol representing the entity requested in the data.",
                         "name": "symbol",
                         "optional": true,
                         "type": "str"
                     },
                     {
-                        "default": "",
+                        "default": null,
                         "description": "Name of the company.",
                         "name": "name",
-                        "optional": false,
+                        "optional": true,
                         "type": "str"
                     }
                 ]
             },
             "deprecated": {
                 "flag": null,
                 "message": null
@@ -20425,14 +20561,21 @@
                     },
                     {
                         "default": 0,
                         "description": "Skip N number of reports from current. A value of 1 will skip the most recent report.",
                         "name": "skip_reports",
                         "optional": true,
                         "type": "int"
+                    },
+                    {
+                        "default": true,
+                        "description": "Whether or not to use cache for the request, default is True. Each reporting period is a separate URL, new reports will be added to the cache.",
+                        "name": "use_cache",
+                        "optional": true,
+                        "type": "bool"
                     }
                 ],
                 "standard": [
                     {
                         "default": "",
                         "description": "Symbol to get data for.",
                         "name": "symbol",
@@ -21630,15 +21773,15 @@
                         "description": "The delta of the option.",
                         "name": "delta",
                         "optional": true,
                         "type": "Union[str, float]"
                     },
                     {
                         "default": null,
-                        "description": "The type of rate for reveivable portion of the swap.",
+                        "description": "The type of rate for receivable portion of the swap.",
                         "name": "rate_type_rec",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The receive currency of the swap.",
@@ -21651,53 +21794,53 @@
                         "description": "The upfront amount received of the swap.",
                         "name": "upfront_receive",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "default": null,
-                        "description": "The floating rate index for reveivable portion of the swap.",
+                        "description": "The floating rate index for receivable portion of the swap.",
                         "name": "floating_rate_index_rec",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The floating rate spread for reveivable portion of the swap.",
                         "name": "floating_rate_spread_rec",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "default": null,
-                        "description": "The rate tenor for reveivable portion of the swap.",
+                        "description": "The rate tenor for receivable portion of the swap.",
                         "name": "rate_tenor_rec",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
-                        "description": "The rate tenor unit for reveivable portion of the swap.",
+                        "description": "The rate tenor unit for receivable portion of the swap.",
                         "name": "rate_tenor_unit_rec",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
-                        "description": "The reset date for reveivable portion of the swap.",
+                        "description": "The reset date for receivable portion of the swap.",
                         "name": "reset_date_rec",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
-                        "description": "The reset date unit for reveivable portion of the swap.",
+                        "description": "The reset date unit for receivable portion of the swap.",
                         "name": "reset_date_unit_rec",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The type of rate for payment portion of the swap.",
                         "name": "rate_type_pmnt",
                         "optional": true,
                         "type": "str"
@@ -21738,29 +21881,29 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The rate tenor unit for payment portion of the swap.",
                         "name": "rate_tenor_unit_pmnt",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The reset date for payment portion of the swap.",
                         "name": "reset_date_pmnt",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The reset date unit for payment portion of the swap.",
                         "name": "reset_date_unit_pmnt",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The type of repo.",
                         "name": "repo_type",
                         "optional": true,
                         "type": "str"
@@ -27253,15 +27396,23 @@
                 "flag": null,
                 "message": null
             },
             "description": "Map a ticker symbol to a CIK number.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.regulators.sec.cik_map(symbol='MSFT', provider='sec')\n```\n\n",
             "model": "CikMap",
             "parameters": {
-                "sec": [],
+                "sec": [
+                    {
+                        "default": true,
+                        "description": "Whether or not to use cache for the request, default is True.",
+                        "name": "use_cache",
+                        "optional": true,
+                        "type": "bool"
+                    }
+                ],
                 "standard": [
                     {
                         "default": "",
                         "description": "Symbol to get data for.",
                         "name": "symbol",
                         "optional": false,
                         "type": "str"
@@ -27316,15 +27467,15 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "Central Index Key (CIK)",
                         "name": "cik",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     }
                 ],
                 "standard": []
             },
             "deprecated": {
                 "flag": null,
                 "message": null
@@ -27340,15 +27491,15 @@
                         "description": "Search query.",
                         "name": "query",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": true,
-                        "description": "Whether or not to use cache. If True, cache will store for seven days.",
+                        "description": "Whether or not to use cache.",
                         "name": "use_cache",
                         "optional": true,
                         "type": "bool"
                     },
                     {
                         "default": "sec",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'sec' if there is no default.",
@@ -27514,15 +27665,15 @@
                         "description": "Search query.",
                         "name": "query",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": true,
-                        "description": "Whether or not to use cache. If True, cache will store for seven days.",
+                        "description": "Whether or not to use cache.",
                         "name": "use_cache",
                         "optional": true,
                         "type": "bool"
                     },
                     {
                         "default": "sec",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'sec' if there is no default.",
@@ -27604,15 +27755,15 @@
                         "description": "Search query.",
                         "name": "query",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": true,
-                        "description": "Whether or not to use cache. If True, cache will store for seven days.",
+                        "description": "Whether or not to use cache.",
                         "name": "use_cache",
                         "optional": true,
                         "type": "bool"
                     },
                     {
                         "default": "sec",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'sec' if there is no default.",
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/__extensions__.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/crypto.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/crypto_price.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/crypto_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/currency.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/currency.py`

 * *Files 12% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     @exception_handler
     @validate
     def snapshots(
         self,
         base: Annotated[
             Union[str, List[str]],
             OpenBBField(
-                description="The base currency symbol. Multiple comma separated items allowed for provider(s): fmp."
+                description="The base currency symbol. Multiple comma separated items allowed for provider(s): fmp, polygon."
             ),
         ] = "usd",
         quote_type: Annotated[
             Literal["direct", "indirect"],
             OpenBBField(
                 description="Whether the quote is direct or indirect. Selecting 'direct' will return the exchange rate as the amount of domestic currency required to buy one unit of the foreign currency. Selecting 'indirect' (default) will return the exchange rate as the amount of foreign currency required to buy one unit of the domestic currency."
             ),
@@ -166,42 +166,42 @@
         counter_currencies: Annotated[
             Union[List[str], str, None],
             OpenBBField(
                 description="An optional list of counter currency symbols to filter for. None returns all."
             ),
         ] = None,
         provider: Annotated[
-            Optional[Literal["fmp"]],
+            Optional[Literal["fmp", "polygon"]],
             OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Snapshots of currency exchange rates from an indirect or direct perspective of a base currency.
 
         Parameters
         ----------
         base : Union[str, List[str]]
-            The base currency symbol. Multiple comma separated items allowed for provider(s): fmp.
+            The base currency symbol. Multiple comma separated items allowed for provider(s): fmp, polygon.
         quote_type : Literal['direct', 'indirect']
             Whether the quote is direct or indirect. Selecting 'direct' will return the exchange rate as the amount of domestic currency required to buy one unit of the foreign currency. Selecting 'indirect' (default) will return the exchange rate as the amount of foreign currency required to buy one unit of the domestic currency.
         counter_currencies : Union[List[str], str, None]
             An optional list of counter currency symbols to filter for. None returns all.
-        provider : Optional[Literal['fmp']]
+        provider : Optional[Literal['fmp', 'polygon']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
         -------
         OBBject
             results : List[CurrencySnapshots]
                 Serializable results.
-            provider : Optional[Literal['fmp']]
+            provider : Optional[Literal['fmp', 'polygon']]
                 Provider name.
             warnings : Optional[List[Warning_]]
                 List of warnings.
             chart : Optional[Chart]
                 Chart object.
             extra : Dict[str, Any]
                 Extra info.
@@ -223,27 +223,64 @@
         close : Optional[float]
             The close price.
         volume : Optional[int]
             The trading volume.
         prev_close : Optional[float]
             The previous close price.
         change : Optional[float]
-            The change in the price from the previous close. (provider: fmp)
+            The change in the price from the previous close. (provider: fmp, polygon)
         change_percent : Optional[float]
-            The change in the price from the previous close, as a normalized percent. (provider: fmp)
+            The change in the price from the previous close, as a normalized percent. (provider: fmp);
+            The percentage change in price from the previous day. (provider: polygon)
         ma50 : Optional[float]
             The 50-day moving average. (provider: fmp)
         ma200 : Optional[float]
             The 200-day moving average. (provider: fmp)
         year_high : Optional[float]
             The 52-week high. (provider: fmp)
         year_low : Optional[float]
             The 52-week low. (provider: fmp)
         last_rate_timestamp : Optional[datetime]
             The timestamp of the last rate. (provider: fmp)
+        vwap : Optional[float]
+            The volume-weighted average price. (provider: polygon)
+        prev_open : Optional[float]
+            The previous day's opening price. (provider: polygon)
+        prev_high : Optional[float]
+            The previous day's high price. (provider: polygon)
+        prev_low : Optional[float]
+            The previous day's low price. (provider: polygon)
+        prev_volume : Optional[float]
+            The previous day's volume. (provider: polygon)
+        prev_vwap : Optional[float]
+            The previous day's VWAP. (provider: polygon)
+        bid : Optional[float]
+            The current bid price. (provider: polygon)
+        ask : Optional[float]
+            The current ask price. (provider: polygon)
+        minute_open : Optional[float]
+            The open price from the most recent minute bar. (provider: polygon)
+        minute_high : Optional[float]
+            The high price from the most recent minute bar. (provider: polygon)
+        minute_low : Optional[float]
+            The low price from the most recent minute bar. (provider: polygon)
+        minute_close : Optional[float]
+            The close price from the most recent minute bar. (provider: polygon)
+        minute_volume : Optional[float]
+            The volume from the most recent minute bar. (provider: polygon)
+        minute_vwap : Optional[float]
+            The VWAP from the most recent minute bar. (provider: polygon)
+        minute_transactions : Optional[float]
+            The number of transactions in the most recent minute bar. (provider: polygon)
+        quote_timestamp : Optional[datetime]
+            The timestamp of the last quote. (provider: polygon)
+        minute_timestamp : Optional[datetime]
+            The timestamp for the start of the most recent minute bar. (provider: polygon)
+        last_updated : Optional[datetime]
+            The last time the data was updated. (provider: polygon)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.currency.snapshots(provider='fmp')
         >>> # Get exchange rates from USD and XAU to EUR, JPY, and GBP using 'fmp' as provider.
         >>> obb.currency.snapshots(provider='fmp', base='USD,XAU', counter_currencies='EUR,JPY,GBP', quote_type='indirect')
@@ -252,19 +289,19 @@
         return self._run(
             "/currency/snapshots",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/currency/snapshots",
-                        ("fmp",),
+                        ("fmp", "polygon"),
                     )
                 },
                 standard_params={
                     "base": base,
                     "quote_type": quote_type,
                     "counter_currencies": counter_currencies,
                 },
                 extra_params=kwargs,
-                info={"base": {"multiple_items_allowed": ["fmp"]}},
+                info={"base": {"multiple_items_allowed": ["fmp", "polygon"]}},
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/currency_price.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/currency_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/derivatives.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/derivatives_options.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/economy.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/economy.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,15 +620,15 @@
             extra : Dict[str, Any]
                 Extra info.
 
         EquitySearch
         ------------
         symbol : Optional[str]
             Symbol representing the entity requested in the data.
-        name : str
+        name : Optional[str]
             Name of the company.
         cik : Optional[str]
             ;
             Central Index Key (provider: sec)
         lei : Optional[str]
             The Legal Entity Identifier (LEI) of the company. (provider: intrinio)
         intrinio_id : Optional[str]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_compare.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_fundamental.py`

 * *Files 8% similar despite different names*

```diff
@@ -1193,18 +1193,16 @@
             no default.
         start_date : Optional[datetime.date]
             Start date of the data, in YYYY-MM-DD format. (provider: intrinio)
         end_date : Optional[datetime.date]
             End date of the data, in YYYY-MM-DD format. (provider: intrinio)
         thea_enabled : Optional[bool]
             Return filings that have been read by Intrinio's Thea NLP. (provider: intrinio)
-        cik : Optional[Union[int, str]]
+        cik : Optional[Union[str, int]]
             Lookup filings by Central Index Key (CIK) instead of by symbol. (provider: sec)
-        type : Optional[Literal['1', '1-A', '1-A POS', '1-A-W', '1-E', '1-E AD', '1-K', '1-SA', '1-U', '1-Z', '1-Z-W', '10-12B', '10-12G', '10-D', '10-K', '10-KT', '10-Q', '10-QT', '11-K', '11-KT', '13F-HR', '13F-NT', '13FCONP', '144', '15-12B', '15-12G', '15-15D', '15F-12B', '15F-12G', '15F-15D', '18-12B', '18-K', '19B-4E', '2-A', '2-AF', '2-E', '20-F', '20FR12B', '20FR12G', '24F-2NT', '25', '25-NSE', '253G1', '253G2', '253G3', '253G4', '3', '305B2', '34-12H', '4', '40-17F1', '40-17F2', '40-17G', '40-17GCS', '40-202A', '40-203A', '40-206A', '40-24B2', '40-33', '40-6B', '40-8B25', '40-8F-2', '40-APP', '40-F', '40-OIP', '40FR12B', '40FR12G', '424A', '424B1', '424B2', '424B3', '424B4', '424B5', '424B7', '424B8', '424H', '425', '485APOS', '485BPOS', '485BXT', '486APOS', '486BPOS', '486BXT', '487', '497', '497AD', '497H2', '497J', '497K', '497VPI', '497VPU', '5', '6-K', '6B NTC', '6B ORDR', '8-A12B', '8-A12G', '8-K', '8-K12B', '8-K12G3', '8-K15D5', '8-M', '8F-2 NTC', '8F-2 ORDR', '9-M', 'ABS-15G', 'ABS-EE', 'ADN-MTL', 'ADV-E', 'ADV-H-C', 'ADV-H-T', 'ADV-NR', 'ANNLRPT', 'APP NTC', 'APP ORDR', 'APP WD', 'APP WDG', 'ARS', 'ATS-N', 'ATS-N-C', 'ATS-N/UA', 'AW', 'AW WD', 'C', 'C-AR', 'C-AR-W', 'C-TR', 'C-TR-W', 'C-U', 'C-U-W', 'C-W', 'CB', 'CERT', 'CERTARCA', 'CERTBATS', 'CERTCBO', 'CERTNAS', 'CERTNYS', 'CERTPAC', 'CFPORTAL', 'CFPORTAL-W', 'CORRESP', 'CT ORDER', 'D', 'DEF 14A', 'DEF 14C', 'DEFA14A', 'DEFA14C', 'DEFC14A', 'DEFC14C', 'DEFM14A', 'DEFM14C', 'DEFN14A', 'DEFR14A', 'DEFR14C', 'DEL AM', 'DFAN14A', 'DFRN14A', 'DOS', 'DOSLTR', 'DRS', 'DRSLTR', 'DSTRBRPT', 'EFFECT', 'F-1', 'F-10', 'F-10EF', 'F-10POS', 'F-1MEF', 'F-3', 'F-3ASR', 'F-3D', 'F-3DPOS', 'F-3MEF', 'F-4', 'F-4 POS', 'F-4MEF', 'F-6', 'F-6 POS', 'F-6EF', 'F-7', 'F-7 POS', 'F-8', 'F-8 POS', 'F-80', 'F-80POS', 'F-9', 'F-9 POS', 'F-N', 'F-X', 'FOCUSN', 'FWP', 'G-405', 'G-405N', 'G-FIN', 'G-FINW', 'IRANNOTICE', 'MA', 'MA-A', 'MA-I', 'MA-W', 'MSD', 'MSDCO', 'MSDW', 'N-1', 'N-14', 'N-14 8C', 'N-14MEF', 'N-18F1', 'N-1A', 'N-2', 'N-2 POSASR', 'N-23C-2', 'N-23C3A', 'N-23C3B', 'N-23C3C', 'N-2ASR', 'N-2MEF', 'N-30B-2', 'N-30D', 'N-4', 'N-5', 'N-54A', 'N-54C', 'N-6', 'N-6F', 'N-8A', 'N-8B-2', 'N-8F', 'N-8F NTC', 'N-8F ORDR', 'N-CEN', 'N-CR', 'N-CSR', 'N-CSRS', 'N-MFP', 'N-MFP1', 'N-MFP2', 'N-PX', 'N-Q', 'N-VP', 'N-VPFS', 'NO ACT', 'NPORT-EX', 'NPORT-NP', 'NPORT-P', 'NRSRO-CE', 'NRSRO-UPD', 'NSAR-A', 'NSAR-AT', 'NSAR-B', 'NSAR-BT', 'NSAR-U', 'NT 10-D', 'NT 10-K', 'NT 10-Q', 'NT 11-K', 'NT 20-F', 'NT N-CEN', 'NT N-MFP', 'NT N-MFP1', 'NT N-MFP2', 'NT NPORT-EX', 'NT NPORT-P', 'NT-NCEN', 'NT-NCSR', 'NT-NSAR', 'NTFNCEN', 'NTFNCSR', 'NTFNSAR', 'NTN 10D', 'NTN 10K', 'NTN 10Q', 'NTN 20F', 'OIP NTC', 'OIP ORDR', 'POS 8C', 'POS AM', 'POS AMI', 'POS EX', 'POS462B', 'POS462C', 'POSASR', 'PRE 14A', 'PRE 14C', 'PREC14A', 'PREC14C', 'PREM14A', 'PREM14C', 'PREN14A', 'PRER14A', 'PRER14C', 'PRRN14A', 'PX14A6G', 'PX14A6N', 'QRTLYRPT', 'QUALIF', 'REG-NR', 'REVOKED', 'RW', 'RW WD', 'S-1', 'S-11', 'S-11MEF', 'S-1MEF', 'S-20', 'S-3', 'S-3ASR', 'S-3D', 'S-3DPOS', 'S-3MEF', 'S-4', 'S-4 POS', 'S-4EF', 'S-4MEF', 'S-6', 'S-8', 'S-8 POS', 'S-B', 'S-BMEF', 'SBSE', 'SBSE-A', 'SBSE-BD', 'SBSE-C', 'SBSE-W', 'SC 13D', 'SC 13E1', 'SC 13E3', 'SC 13G', 'SC 14D9', 'SC 14F1', 'SC 14N', 'SC TO-C', 'SC TO-I', 'SC TO-T', 'SC13E4F', 'SC14D1F', 'SC14D9C', 'SC14D9F', 'SD', 'SDR', 'SE', 'SEC ACTION', 'SEC STAFF ACTION', 'SEC STAFF LETTER', 'SF-1', 'SF-3', 'SL', 'SP 15D2', 'STOP ORDER', 'SUPPL', 'T-3', 'TA-1', 'TA-2', 'TA-W', 'TACO', 'TH', 'TTW', 'UNDER', 'UPLOAD', 'WDL-REQ', 'X-17A-5']]
-            Type of the SEC filing form. (provider: sec)
         use_cache : bool
             Whether or not to use cache.  If True, cache will store for one day. (provider: sec)
 
         Returns
         -------
         OBBject
             results : List[CompanyFilings]
@@ -1244,33 +1242,33 @@
             URL for the XBRL filing for the report. (provider: intrinio)
         industry_group : Optional[str]
             Industry group of the company. (provider: intrinio)
         industry_category : Optional[str]
             Industry category of the company. (provider: intrinio)
         report_date : Optional[date]
             The date of the filing. (provider: sec)
-        act : Optional[Union[int, str]]
+        act : Optional[Union[str, int]]
             The SEC Act number. (provider: sec)
         items : Optional[Union[str, float]]
             The SEC Item numbers. (provider: sec)
         primary_doc_description : Optional[str]
             The description of the primary document. (provider: sec)
         primary_doc : Optional[str]
             The filename of the primary document. (provider: sec)
-        accession_number : Optional[Union[int, str]]
+        accession_number : Optional[Union[str, int]]
             The accession number. (provider: sec)
-        file_number : Optional[Union[int, str]]
+        file_number : Optional[Union[str, int]]
             The file number. (provider: sec)
-        film_number : Optional[Union[int, str]]
+        film_number : Optional[Union[str, int]]
             The film number. (provider: sec)
-        is_inline_xbrl : Optional[Union[int, str]]
+        is_inline_xbrl : Optional[Union[str, int]]
             Whether the filing is an inline XBRL filing. (provider: sec)
-        is_xbrl : Optional[Union[int, str]]
+        is_xbrl : Optional[Union[str, int]]
             Whether the filing is an XBRL filing. (provider: sec)
-        size : Optional[Union[int, str]]
+        size : Optional[Union[str, int]]
             The size of the filing. (provider: sec)
         complete_submission_url : Optional[str]
             The URL to the complete filing submission. (provider: sec)
         filing_detail_url : Optional[str]
             The URL to the filing details. (provider: sec)
 
         Examples
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_price.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/equity_shorts.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,16 @@
                 Limit the number of reports to parse, from most recent.
                 Approximately 24 reports per year, going back to 2009.
                  (provider: sec)
         skip_reports : Optional[int]
 
                 Skip N number of reports from current. A value of 1 will skip the most recent report.
                  (provider: sec)
+        use_cache : Optional[bool]
+            Whether or not to use cache for the request, default is True. Each reporting period is a separate URL, new reports will be added to the cache. (provider: sec)
 
         Returns
         -------
         OBBject
             results : List[EquityFTD]
                 Serializable results.
             provider : Optional[Literal['sec']]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/etf.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/etf.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,48 +523,48 @@
         exercise_currency : Optional[str]
             The currency of the option exercise price. (provider: sec)
         shares_per_contract : Optional[float]
             The number of shares per contract. (provider: sec)
         delta : Optional[Union[str, float]]
             The delta of the option. (provider: sec)
         rate_type_rec : Optional[str]
-            The type of rate for reveivable portion of the swap. (provider: sec)
+            The type of rate for receivable portion of the swap. (provider: sec)
         receive_currency : Optional[str]
             The receive currency of the swap. (provider: sec)
         upfront_receive : Optional[float]
             The upfront amount received of the swap. (provider: sec)
         floating_rate_index_rec : Optional[str]
-            The floating rate index for reveivable portion of the swap. (provider: sec)
+            The floating rate index for receivable portion of the swap. (provider: sec)
         floating_rate_spread_rec : Optional[float]
             The floating rate spread for reveivable portion of the swap. (provider: sec)
         rate_tenor_rec : Optional[str]
-            The rate tenor for reveivable portion of the swap. (provider: sec)
-        rate_tenor_unit_rec : Optional[Union[int, str]]
-            The rate tenor unit for reveivable portion of the swap. (provider: sec)
+            The rate tenor for receivable portion of the swap. (provider: sec)
+        rate_tenor_unit_rec : Optional[Union[str, int]]
+            The rate tenor unit for receivable portion of the swap. (provider: sec)
         reset_date_rec : Optional[str]
-            The reset date for reveivable portion of the swap. (provider: sec)
-        reset_date_unit_rec : Optional[Union[int, str]]
-            The reset date unit for reveivable portion of the swap. (provider: sec)
+            The reset date for receivable portion of the swap. (provider: sec)
+        reset_date_unit_rec : Optional[Union[str, int]]
+            The reset date unit for receivable portion of the swap. (provider: sec)
         rate_type_pmnt : Optional[str]
             The type of rate for payment portion of the swap. (provider: sec)
         payment_currency : Optional[str]
             The payment currency of the swap. (provider: sec)
         upfront_payment : Optional[float]
             The upfront amount received of the swap. (provider: sec)
         floating_rate_index_pmnt : Optional[str]
             The floating rate index for payment portion of the swap. (provider: sec)
         floating_rate_spread_pmnt : Optional[float]
             The floating rate spread for payment portion of the swap. (provider: sec)
         rate_tenor_pmnt : Optional[str]
             The rate tenor for payment portion of the swap. (provider: sec)
-        rate_tenor_unit_pmnt : Optional[Union[int, str]]
+        rate_tenor_unit_pmnt : Optional[Union[str, int]]
             The rate tenor unit for payment portion of the swap. (provider: sec)
         reset_date_pmnt : Optional[str]
             The reset date for payment portion of the swap. (provider: sec)
-        reset_date_unit_pmnt : Optional[Union[int, str]]
+        reset_date_unit_pmnt : Optional[Union[str, int]]
             The reset date unit for payment portion of the swap. (provider: sec)
         repo_type : Optional[str]
             The type of repo. (provider: sec)
         is_cleared : Optional[str]
             If the repo is cleared. (provider: sec)
         is_tri_party : Optional[str]
             If the repo is tri party. (provider: sec)
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_corporate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/index.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/index.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/news.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/openbb/package/regulators_sec.py` & `openbb_nightly-4.1.7.dev202404240009/openbb/package/regulators_sec.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         ----------
         symbol : str
             Symbol to get data for.
         provider : Optional[Literal['sec']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'sec' if there is
             no default.
+        use_cache : Optional[bool]
+            Whether or not to use cache for the request, default is True. (provider: sec)
 
         Returns
         -------
         OBBject
             results : CikMap
                 Serializable results.
             provider : Optional[Literal['sec']]
@@ -111,15 +113,15 @@
         """Search SEC-regulated institutions by name and return a list of results with CIK numbers.
 
         Parameters
         ----------
         query : str
             Search query.
         use_cache : Optional[bool]
-            Whether or not to use cache. If True, cache will store for seven days.
+            Whether or not to use cache.
         provider : Optional[Literal['sec']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'sec' if there is
             no default.
 
         Returns
         -------
@@ -135,15 +137,15 @@
             extra : Dict[str, Any]
                 Extra info.
 
         InstitutionsSearch
         ------------------
         name : Optional[str]
             The name of the institution. (provider: sec)
-        cik : Optional[Union[int, str]]
+        cik : Optional[Union[str, int]]
             Central Index Key (CIK) (provider: sec)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.regulators.sec.institutions_search(provider='sec')
         >>> obb.regulators.sec.institutions_search(query='blackstone real estate', provider='sec')
@@ -258,15 +260,15 @@
         """Use tool for navigating the directory of SEC XML schema files by year.
 
         Parameters
         ----------
         query : str
             Search query.
         use_cache : Optional[bool]
-            Whether or not to use cache. If True, cache will store for seven days.
+            Whether or not to use cache.
         provider : Optional[Literal['sec']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'sec' if there is
             no default.
         url : Optional[str]
             Enter an optional URL path to fetch the next level. (provider: sec)
 
@@ -353,15 +355,15 @@
         """Search for Industry Titles, Reporting Office, and SIC Codes. An empty query string returns all results.
 
         Parameters
         ----------
         query : str
             Search query.
         use_cache : Optional[bool]
-            Whether or not to use cache. If True, cache will store for seven days.
+            Whether or not to use cache.
         provider : Optional[Literal['sec']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'sec' if there is
             no default.
 
         Returns
         -------
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.7.dev202404240009/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/models/available_indicators.py` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/models/country_profile.py` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/models/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/indicator_countries.json` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/indicator_countries.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/indicators_descriptions.json` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/multipliers.json` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/multipliers.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/scales.json` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/scales.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/econdb/openbb_econdb/utils/units.json` & `openbb_nightly-4.1.7.dev202404240009/providers/econdb/openbb_econdb/utils/units.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finra/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.7.dev202404240009/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.7.dev202404240009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/search_attributes.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.7.dev202404240009/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.7.dev202404240009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from openbb_core.provider.abstract.provider import Provider
 from openbb_polygon.models.balance_sheet import PolygonBalanceSheetFetcher
 from openbb_polygon.models.cash_flow import PolygonCashFlowStatementFetcher
 from openbb_polygon.models.company_news import PolygonCompanyNewsFetcher
 from openbb_polygon.models.crypto_historical import PolygonCryptoHistoricalFetcher
 from openbb_polygon.models.currency_historical import PolygonCurrencyHistoricalFetcher
 from openbb_polygon.models.currency_pairs import PolygonCurrencyPairsFetcher
+from openbb_polygon.models.currency_snapshots import PolygonCurrencySnapshotsFetcher
 from openbb_polygon.models.equity_historical import PolygonEquityHistoricalFetcher
 from openbb_polygon.models.equity_nbbo import PolygonEquityNBBOFetcher
 from openbb_polygon.models.income_statement import PolygonIncomeStatementFetcher
 from openbb_polygon.models.index_historical import (
     PolygonIndexHistoricalFetcher,
 )
 from openbb_polygon.models.market_snapshots import PolygonMarketSnapshotsFetcher
@@ -25,14 +26,15 @@
     fetcher_dict={
         "BalanceSheet": PolygonBalanceSheetFetcher,
         "CashFlowStatement": PolygonCashFlowStatementFetcher,
         "CompanyNews": PolygonCompanyNewsFetcher,
         "CryptoHistorical": PolygonCryptoHistoricalFetcher,
         "CurrencyHistorical": PolygonCurrencyHistoricalFetcher,
         "CurrencyPairs": PolygonCurrencyPairsFetcher,
+        "CurrencySnapshots": PolygonCurrencySnapshotsFetcher,
         "EquityHistorical": PolygonEquityHistoricalFetcher,
         "EquityNBBO": PolygonEquityNBBOFetcher,
         "EtfHistorical": PolygonEquityHistoricalFetcher,
         "IncomeStatement": PolygonIncomeStatementFetcher,
         "IndexHistorical": PolygonIndexHistoricalFetcher,
         "MarketIndices": PolygonIndexHistoricalFetcher,
         "MarketSnapshots": PolygonMarketSnapshotsFetcher,
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/cik_map.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """SEC CIK Mapping Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cik_map import CikMapData, CikMapQueryParams
 from openbb_sec.utils.helpers import symbol_map
+from pydantic import Field
 
 
 class SecCikMapQueryParams(CikMapQueryParams):
     """SEC CIK Mapping Query.
 
     Source: https://sec.gov/
     """
 
+    use_cache: Optional[bool] = Field(
+        default=True,
+        description="Whether or not to use cache for the request, default is True.",
+    )
+
 
 class SecCikMapData(CikMapData):
     """SEC CIK Mapping Data."""
 
 
 class SecCikMapFetcher(
     Fetcher[
@@ -28,21 +36,21 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecCikMapQueryParams:
         """Transform the query."""
         return SecCikMapQueryParams(**params)
 
     @staticmethod
-    def extract_data(
-        query: SecCikMapQueryParams,  # pylint: disable=W0613:unused-argument
+    async def aextract_data(
+        query: SecCikMapQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the SEC endpoint."""
-        results = {"cik": symbol_map(query.symbol)}
+        results = {"cik": await symbol_map(query.symbol, query.use_cache)}
         if not results:
             return {"Error": "Symbol not found."}
         return results
 
     @staticmethod
     def transform_data(
         query: SecCikMapQueryParams, data: Dict, **kwargs: Any
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,240 +1,288 @@
-"""SEC Company Filings Model."""
+"""Tradier Equity Quote Model."""
+
+# pylint: disable = unused-argument
 
-# pylint: skip-file
 from datetime import (
     date as dateType,
     datetime,
 )
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Literal, Optional
 
-import pandas as pd
-import requests
+from dateutil.parser import parse
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.company_filings import (
-    CompanyFilingsData,
-    CompanyFilingsQueryParams,
+from openbb_core.provider.standard_models.equity_quote import (
+    EquityQuoteData,
+    EquityQuoteQueryParams,
 )
-from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
-from openbb_sec.utils.definitions import FORM_TYPES, HEADERS
-from openbb_sec.utils.helpers import sec_session_company_filings, symbol_map
-from pydantic import Field, field_validator
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
+from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
+from pydantic import Field, field_validator, model_validator
+from pytz import timezone
+
+
+class TradierEquityQuoteQueryParams(EquityQuoteQueryParams):
+    """Tradier Equity Quote Query."""
 
+    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
-class SecCompanyFilingsQueryParams(CompanyFilingsQueryParams):
-    """SEC Company Filings Query.
 
-    Source: https://sec.gov/
-    """
+class TradierEquityQuoteData(EquityQuoteData):
+    """Tradier Equity Quote Data."""
+
+    __alias_dict__ = {
+        "name": "description",
+        "exchange": "exch",
+        "asset_type": "type",
+        "bid_exchange": "bidexch",
+        "bid_size": "bidsize",
+        "ask_size": "asksize",
+        "ask_exchange": "askexch",
+        "last_price": "last",
+        "last_timestamp": "trade_date",
+        "prev_close": "prevclose",
+        "year_high": "week_52_high",
+        "year_low": "week_52_low",
+        "volume_avg": "average_volume",
+        "change_percent": "change_percentage",
+        "root_symbol": "root_symbols",
+        "orats_final_iv": "smv_vol",
+        "greeks_timestamp": "updated_at",
+        "bid_timestamp": "bid_date",
+        "ask_timestamp": "ask_date",
+    }
 
-    symbol: Optional[str] = Field(
-        description=QUERY_DESCRIPTIONS.get("symbol", ""),
+    last_volume: Optional[int] = Field(
         default=None,
+        description="The last trade volume.",
     )
-    cik: Optional[Union[str, int]] = Field(
-        description="Lookup filings by Central Index Key (CIK) instead of by symbol.",
+    volume_avg: Optional[int] = Field(
         default=None,
+        description="The average daily trading volume.",
     )
-    type: Optional[FORM_TYPES] = Field(
-        description="Type of the SEC filing form.",
+    bid_timestamp: Optional[datetime] = Field(
         default=None,
-        alias="form_type",
+        description="Timestamp of the bid price.",
     )
-    use_cache: bool = Field(
-        description="Whether or not to use cache.  If True, cache will store for one day.",
-        default=True,
+    ask_timestamp: Optional[datetime] = Field(
+        default=None,
+        description="Timestamp of the ask price.",
     )
-
-
-class SecCompanyFilingsData(CompanyFilingsData):
-    """SEC Company Filings Data."""
-
-    __alias_dict__ = {
-        "filing_date": "filingDate",
-        "accepted_date": "acceptanceDateTime",
-        "filing_url": "filingDetailUrl",
-        "report_url": "primaryDocumentUrl",
-        "report_type": "form",
-    }
-
-    report_date: Optional[dateType] = Field(
-        description="The date of the filing.",
+    greeks_timestamp: Optional[datetime] = Field(
+        default=None,
+        description="Timestamp of the greeks data.",
+    )
+    underlying: Optional[str] = Field(
+        default=None,
+        description="The underlying symbol for the option.",
+    )
+    root_symbol: Optional[str] = Field(
+        default=None,
+        description="The root symbol for the option.",
+    )
+    option_type: Optional[Literal["call", "put"]] = Field(
+        default=None,
+        description="Type of option - call or put.",
+    )
+    contract_size: Optional[int] = Field(
+        default=None,
+        description="The number of shares in a standard contract.",
+    )
+    expiration_type: Optional[str] = Field(
+        default=None,
+        description="The expiration type of the option - i.e, standard, weekly, etc.",
+    )
+    expiration_date: Optional[dateType] = Field(
         default=None,
-        alias="reportDate",
+        description="The expiration date of the option.",
     )
-    act: Optional[Union[str, int]] = Field(
-        description="The SEC Act number.", default=None
+    strike: Optional[float] = Field(
+        default=None,
+        description="The strike price of the option.",
     )
-    items: Optional[Union[str, float]] = Field(
-        description="The SEC Item numbers.", default=None
+    open_interest: Optional[int] = Field(
+        default=None,
+        description="The number of open contracts for the option.",
     )
-    primary_doc_description: Optional[str] = Field(
-        description="The description of the primary document.",
+    bid_iv: Optional[float] = Field(
         default=None,
-        alias="primaryDocDescription",
+        description="Implied volatility of the bid price.",
     )
-    primary_doc: Optional[str] = Field(
-        description="The filename of the primary document.",
+    ask_iv: Optional[float] = Field(
         default=None,
-        alias="primaryDocument",
+        description="Implied volatility of the ask price.",
     )
-    accession_number: Optional[Union[str, int]] = Field(
-        description="The accession number.",
+    mid_iv: Optional[float] = Field(
         default=None,
-        alias="accessionNumber",
+        description="Mid-point implied volatility of the option.",
     )
-    file_number: Optional[Union[str, int]] = Field(
-        description="The file number.",
+    orats_final_iv: Optional[float] = Field(
         default=None,
-        alias="fileNumber",
+        description="ORATS final implied volatility of the option.",
     )
-    film_number: Optional[Union[str, int]] = Field(
-        description="The film number.",
+    delta: Optional[float] = Field(
         default=None,
-        alias="filmNumber",
+        description="Delta of the option.",
     )
-    is_inline_xbrl: Optional[Union[str, int]] = Field(
-        description="Whether the filing is an inline XBRL filing.",
+    gamma: Optional[float] = Field(
         default=None,
-        alias="isInlineXBRL",
+        description="Gamma of the option.",
     )
-    is_xbrl: Optional[Union[str, int]] = Field(
-        description="Whether the filing is an XBRL filing.",
+    theta: Optional[float] = Field(
         default=None,
-        alias="isXBRL",
+        description="Theta of the option.",
     )
-    size: Optional[Union[str, int]] = Field(
-        description="The size of the filing.", default=None
+    vega: Optional[float] = Field(
+        default=None,
+        description="Vega of the option.",
     )
-    complete_submission_url: Optional[str] = Field(
-        description="The URL to the complete filing submission.",
+    rho: Optional[float] = Field(
         default=None,
-        alias="completeSubmissionUrl",
+        description="Rho of the option.",
     )
-    filing_detail_url: Optional[str] = Field(
-        description="The URL to the filing details.",
+    phi: Optional[float] = Field(
         default=None,
-        alias="filingDetailUrl",
+        description="Phi of the option.",
     )
 
-    @field_validator("report_date", mode="before", check_fields=False)
-    def validate_report_date(cls, v: Optional[Union[str, dateType]]):
-        """Validate report_date."""
-        if isinstance(v, dateType):
+    @field_validator(
+        "last_timestamp",
+        "ask_timestamp",
+        "bid_timestamp",
+        "greeks_timestamp",
+        mode="before",
+        check_fields=False,
+    )
+    @classmethod
+    def validate_dates(cls, v):
+        """Validate the dates."""
+        if v != 0 and v is not None and isinstance(v, int):
+            v = int(v) / 1000  # milliseconds to seconds
+            v = safe_fromtimestamp(v)
+            v = v.replace(microsecond=0)
+            v = v.astimezone(timezone("America/New_York"))
+            return v
+        if v is not None and isinstance(v, str):
+            v = parse(v)
+            v = v.replace(microsecond=0, tzinfo=timezone("UTC"))
+            v = v.astimezone(timezone("America/New_York"))
             return v
-        v = v if v != "" else None
+        return None
+
+    @field_validator("change_percent", mode="before", check_fields=False)
+    @classmethod
+    def normalize_percent(cls, v):
+        """Normalize the percentage."""
+        return float(v) / 100 if v else None
+
+    @model_validator(mode="before")
+    @classmethod
+    def replace_zero(cls, values):
+        """Check for zero values and replace with None."""
         return (
-            datetime.strptime(v, "%Y-%m-%d").date()
-            if v and isinstance(v, str)
-            else None
+            {k: None if (v == 0 or str(v) == "0") else v for k, v in values.items()}
+            if isinstance(values, dict)
+            else values
         )
 
 
-class SecCompanyFilingsFetcher(
-    Fetcher[SecCompanyFilingsQueryParams, List[SecCompanyFilingsData]]
+class TradierEquityQuoteFetcher(
+    Fetcher[TradierEquityQuoteQueryParams, List[TradierEquityQuoteData]]
 ):
-    """Transform the query, extract and transform the data from the SEC endpoints."""
+    """Tradier Equity Quote Fetcher."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> SecCompanyFilingsQueryParams:
-        """Transform query params."""
-        return SecCompanyFilingsQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> TradierEquityQuoteQueryParams:
+        """Transform the query."""
+        return TradierEquityQuoteQueryParams(**params)
 
     @staticmethod
-    def extract_data(
-        query: SecCompanyFilingsQueryParams,  # pylint: disable=unused-argument
+    async def aextract_data(
+        query: TradierEquityQuoteQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Extract the data from the SEC endpoint."""
-        filings = pd.DataFrame()
-
-        if query.symbol and not query.cik:
-            query.cik = symbol_map(query.symbol.lower(), use_cache=query.use_cache)
-            if not query.cik:
-                return []
-        if query.cik is None:
-            return []
-
-        # The leading 0s need to be inserted but are typically removed from the data to store as an integer.
-        if len(query.cik) != 10:  # type: ignore
-            cik_: str = ""
-            temp = 10 - len(query.cik)  # type: ignore
-            for i in range(temp):
-                cik_ = cik_ + "0"
-            query.cik = cik_ + str(query.cik)  # type: ignore
-
-        url = f"https://data.sec.gov/submissions/CIK{query.cik}.json"
-        r = (
-            requests.get(url, headers=HEADERS, timeout=5)
-            if query.use_cache is False
-            else sec_session_company_filings.get(url, headers=HEADERS, timeout=5)
-        )
-        if r.status_code == 200:
-            data = r.json()
-            filings = pd.DataFrame.from_records(data["filings"]["recent"])
-            if len(filings) >= 1000:
-                new_urls = pd.DataFrame(data["filings"]["files"])
-                for i in new_urls.index:
-                    new_cik: str = data["filings"]["files"][i]["name"]
-                    new_url: str = "https://data.sec.gov/submissions/" + new_cik
-                    r_ = (
-                        requests.get(new_url, headers=HEADERS, timeout=5)
-                        if query.use_cache is False
-                        else sec_session_company_filings.get(
-                            new_url, headers=HEADERS, timeout=5
-                        )
-                    )
-                    if r_.status_code == 200:
-                        data_ = r_.json()
-                        additional_data = pd.DataFrame.from_records(data_)
-                        filings = pd.concat([filings, additional_data], axis=0)
-        cols = [
-            "reportDate",
-            "filingDate",
-            "acceptanceDateTime",
-            "act",
-            "form",
-            "items",
-            "primaryDocDescription",
-            "primaryDocument",
-            "accessionNumber",
-            "fileNumber",
-            "filmNumber",
-            "isInlineXBRL",
-            "isXBRL",
-            "size",
-        ]
-        filings = (
-            pd.DataFrame(filings, columns=cols)
-            .fillna(value="N/A")
-            .replace("N/A", None)
-            .astype(str)
-        )
-        filings = filings.sort_values(by=["reportDate", "filingDate"], ascending=False)
-        base_url = f"https://www.sec.gov/Archives/edgar/data/{query.cik}/"
-        filings["primaryDocumentUrl"] = (
-            base_url
-            + filings["accessionNumber"].str.replace("-", "")
-            + "/"
-            + filings["primaryDocument"]
-        )
-        filings["completeSubmissionUrl"] = (
-            base_url + filings["accessionNumber"] + ".txt"
+        """Return the raw data from the Tradier endpoint."""
+        api_key = credentials.get("tradier_api_key") if credentials else ""
+        sandbox = True
+
+        if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
+            raise ValueError(
+                "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
+            )
+
+        if api_key:
+            sandbox = (
+                credentials.get("tradier_account_type") == "sandbox"
+                if credentials
+                else False
+            )
+
+        BASE_URL = (
+            "https://api.tradier.com/"
+            if sandbox is False
+            else "https://sandbox.tradier.com/"
         )
-        filings["filingDetailUrl"] = (
-            base_url + filings["accessionNumber"] + "-index.htm"
-        )
-        if "type" in query.model_dump() and query.type is not None:
-            filings = filings[filings["form"] == query.type]
-
-        if "limit" in query.model_dump():
-            filings = filings.head(query.limit) if query.limit != 0 else filings
+        HEADERS = {
+            "Authorization": f"Bearer {api_key}",
+            "Accept": "application/json",
+        }
+        url = f"{BASE_URL}v1/markets/quotes?symbols={query.symbol}&greeks=true"
+
+        response = await amake_request(url, headers=HEADERS)
+
+        if response.get("quotes"):  # type: ignore
+            data = response["quotes"].get("quote")  # type: ignore
+            if len(data) > 0:
+                return data if isinstance(data, list) else [data]
 
-        return filings.to_dict("records")
+        raise EmptyDataError("No results found.")
 
     @staticmethod
     def transform_data(
-        query: SecCompanyFilingsQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[SecCompanyFilingsData]:
-        """Transform the data."""
-        return [SecCompanyFilingsData.model_validate(d) for d in data]
+        query: TradierEquityQuoteQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
+    ) -> List[TradierEquityQuoteData]:
+        """Transform and validate the data."""
+        results: List[TradierEquityQuoteData] = []
+
+        for d in data:
+
+            d["exch"] = (
+                OPTIONS_EXCHANGES.get(d["exch"])
+                if d.get("type") in ["option", "index"]
+                else STOCK_EXCHANGES.get(d["exch"])
+            )
+            d["askexch"] = (
+                OPTIONS_EXCHANGES.get(d["askexch"])
+                if d.get("type") in ["option", "index"]
+                else STOCK_EXCHANGES.get(d["askexch"])
+            )
+            d["bidexch"] = (
+                OPTIONS_EXCHANGES.get(d["bidexch"])
+                if d.get("type") in ["option", "index"]
+                else STOCK_EXCHANGES.get(d["bidexch"])
+            )
+
+            if "greeks" in d:
+                # Flatten the nested greeks dictionary
+                greeks = d.pop("greeks")
+                if greeks is not None:
+                    d.update(**greeks)
+
+            if (
+                d.get("root_symbols") == d.get("symbol")
+                and d.get("root_symbols") is not None
+            ):
+                _ = d.pop("root_symbols")
+
+            if (
+                d.get("root_symbol") == d.get("underlying")
+                and d.get("root_symbol") is not None
+            ):
+                _ = d.pop("root_symbol")
+
+            results.append(TradierEquityQuoteData.model_validate(d))
+
+        return results
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,95 @@
-"""SEC Equity FTD Model."""
+"""Yahoo Finance ETF Historical Price Model."""
 
-import concurrent.futures
+from datetime import datetime
 from typing import Any, Dict, List, Optional
 
+from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.equity_ftd import (
-    EquityFtdData,
-    EquityFtdQueryParams,
+from openbb_core.provider.standard_models.etf_historical import (
+    EtfHistoricalData,
+    EtfHistoricalQueryParams,
 )
-from openbb_sec.utils.helpers import download_zip_file, get_ftd_urls
-from pydantic import Field
+from openbb_core.provider.utils.errors import EmptyDataError
+from pandas import Timestamp
+from pydantic import Field, field_validator
 
+from ..utils.helpers import yf_download
 
-class SecEquityFtdQueryParams(EquityFtdQueryParams):
-    """SEC Equity FTD Query.
 
-    Source: https://sec.gov/
+class YFinanceEtfHistoricalQueryParams(EtfHistoricalQueryParams):
+    """Yahoo Finance ETF Historical Price Query.
+
+    Source: https://finance.yahoo.com/
     """
 
-    limit: Optional[int] = Field(
-        description="""
-        Limit the number of reports to parse, from most recent.
-        Approximately 24 reports per year, going back to 2009.
-        """,
-        default=24,
-    )
-    skip_reports: Optional[int] = Field(
-        description="""
-        Skip N number of reports from current. A value of 1 will skip the most recent report.
-        """,
-        default=0,
-    )
 
+class YFinanceEtfHistoricalData(EtfHistoricalData):
+    """Yahoo Finance ETF Historical Price Data."""
+
+    __alias_dict__ = {
+        "adj_close": "adj close",
+    }
+
+    adj_close: Optional[float] = Field(
+        default=None,
+        description="The adjusted closing price of the ETF.",
+    )
 
-class SecEquityFtdData(EquityFtdData):
-    """SEC Equity FTD Data."""
+    @field_validator("date", mode="before", check_fields=False)
+    def date_validate(cls, v):  # pylint: disable=E0213
+        """Return formatted datetime."""
+        if isinstance(v, Timestamp):
+            return v.to_pydatetime()
+        return v
 
 
-class SecEquityFtdFetcher(
+class YFinanceEtfHistoricalFetcher(
     Fetcher[
-        SecEquityFtdQueryParams,
-        List[SecEquityFtdData],
+        YFinanceEtfHistoricalQueryParams,
+        List[YFinanceEtfHistoricalData],
     ]
 ):
-    """Transform the query, extract and transform the data from the SEC endpoints."""
+    """Transform the query, extract and transform the data from the Yahoo Finance endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> SecEquityFtdQueryParams:
-        """Transform query params."""
-        return SecEquityFtdQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> YFinanceEtfHistoricalQueryParams:
+        """Transform the query."""
+        transformed_params = params
+        now = datetime.now().date()
 
+        if params.get("start_date") is None:
+            transformed_params["start_date"] = now - relativedelta(years=1)
+
+        if params.get("end_date") is None:
+            transformed_params["end_date"] = now
+
+        return YFinanceEtfHistoricalQueryParams(**params)
+
+    # pylint: disable=unused-argument
     @staticmethod
     def extract_data(
-        query: SecEquityFtdQueryParams,  # pylint: disable=unused-argument
+        query: YFinanceEtfHistoricalQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Extract the data from the SEC website."""
-        results = []
-        limit = query.limit if query.limit is not None and query.limit > 0 else 0
-        symbol = query.symbol.upper()
-
-        urls_data = get_ftd_urls()
-        urls = list(urls_data.values())
-        if limit > 0:
-            urls = (
-                urls[:limit]
-                if not query.skip_reports
-                else urls[query.skip_reports : limit + query.skip_reports]  # noqa: E203
-            )
-
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            executor.map(
-                lambda url: results.extend(download_zip_file(url, symbol)), urls
-            )
+        """Return the raw data from the Yahoo Finance endpoint."""
+        data = yf_download(
+            symbol=query.symbol,
+            start_date=query.start_date,
+            end_date=query.end_date,
+            keep_adjusted=True,
+        )
 
-        results = sorted(results, key=lambda d: d["date"], reverse=True)
+        if data.empty:
+            raise EmptyDataError()
 
-        return results
+        return data.to_dict("records")
 
     @staticmethod
     def transform_data(
-        query: SecEquityFtdQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[SecEquityFtdData]:
+        query: YFinanceEtfHistoricalQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
+    ) -> List[YFinanceEtfHistoricalData]:
         """Transform the data to the standard format."""
-        return [SecEquityFtdData.model_validate(d) for d in data]
+        return [YFinanceEtfHistoricalData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/equity_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """SEC Equity Search Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_search import (
     EquitySearchData,
     EquitySearchQueryParams,
 )
@@ -26,15 +28,14 @@
         description="Whether to direct the search to the list of mutual funds and ETFs.",
     )
 
 
 class SecEquitySearchData(EquitySearchData):
     """SEC Equity Search Data."""
 
-    name: Optional[str] = Field(default=None)
     cik: str = Field(description="Central Index Key")
 
 
 class SecEquitySearchFetcher(
     Fetcher[
         SecEquitySearchQueryParams,
         List[SecEquitySearchData],
@@ -44,33 +45,33 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecEquitySearchQueryParams:
         """Transform the query."""
         return SecEquitySearchQueryParams(**params)
 
     @staticmethod
-    def extract_data(
-        query: SecEquitySearchQueryParams,  # pylint: disable=unused-argument
+    async def aextract_data(
+        query: SecEquitySearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
         results = DataFrame()
 
         if query.is_fund is True:
-            companies = get_mf_and_etf_map(use_cache=query.use_cache).astype(str)
+            companies = await get_mf_and_etf_map(use_cache=query.use_cache)
             results = companies[
                 companies["cik"].str.contains(query.query, case=False)
                 | companies["seriesId"].str.contains(query.query, case=False)
                 | companies["classId"].str.contains(query.query, case=False)
                 | companies["symbol"].str.contains(query.query, case=False)
             ]
 
         if query.is_fund is False:
-            companies = get_all_companies(use_cache=query.use_cache)
+            companies = await get_all_companies(use_cache=query.use_cache)
 
             results = companies[
                 companies["name"].str.contains(query.query, case=False)
                 | companies["symbol"].str.contains(query.query, case=False)
                 | companies["cik"].str.contains(query.query, case=False)
             ]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """SEC ETF Holings Model."""
 
 # pylint: disable =[unused-argument,too-many-locals,too-many-branches]
 
-import warnings
 from datetime import date as dateType
 from typing import Any, Dict, List, Optional, Union
+from warnings import warn
 
 import pandas as pd
-import requests
 import xmltodict
+from aiohttp_client_cache import SQLiteBackend
+from aiohttp_client_cache.session import CachedSession
+from openbb_core.app.utils import get_user_cache_directory
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_holdings import (
     EtfHoldingsData,
     EtfHoldingsQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
-from openbb_sec.utils.helpers import HEADERS, get_nport_candidates, sec_session_etf
-from pydantic import Field, model_validator
-
-_warn = warnings.warn
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_sec.utils.helpers import HEADERS, get_nport_candidates
+from pandas.tseries.offsets import MonthEnd
+from pydantic import Field, field_validator, model_validator
 
 
 class SecEtfHoldingsQueryParams(EtfHoldingsQueryParams):
     """SEC ETF Holdings Query.
 
     Source: https://www.sec.gov/Archives/edgar/data/
     """
@@ -53,14 +57,15 @@
     balance: Optional[float] = Field(
         description="The balance of the holding.", default=None
     )
     weight: Optional[float] = Field(
         description="The weight of the holding in ETF in %.",
         alias="pctVal",
         default=None,
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     value: Optional[float] = Field(
         description="The value of the holding in USD.", alias="valUSD", default=None
     )
     payoff_profile: Optional[str] = Field(
         description="The payoff profile of the holding.",
         alias="payoffProfile",
@@ -126,15 +131,17 @@
         description="The type of coupon for the debt security.", default=None
     )
     rate_type: Optional[str] = Field(
         description="The type of rate for the debt security, floating or fixed.",
         default=None,
     )
     annualized_return: Optional[float] = Field(
-        description="The annualized return on the debt security.", default=None
+        description="The annualized return on the debt security.",
+        default=None,
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     is_default: Optional[str] = Field(
         description="If the debt security is defaulted.", default=None
     )
     in_arrears: Optional[str] = Field(
         description="If the debt security is in arrears.", default=None
     )
@@ -167,42 +174,42 @@
     shares_per_contract: Optional[float] = Field(
         description="The number of shares per contract.", default=None
     )
     delta: Optional[Union[str, float]] = Field(
         description="The delta of the option.", default=None
     )
     rate_type_rec: Optional[str] = Field(
-        description="The type of rate for reveivable portion of the swap.", default=None
+        description="The type of rate for receivable portion of the swap.", default=None
     )
     receive_currency: Optional[str] = Field(
         description="The receive currency of the swap.", default=None
     )
     upfront_receive: Optional[float] = Field(
         description="The upfront amount received of the swap.", default=None
     )
     floating_rate_index_rec: Optional[str] = Field(
-        description="The floating rate index for reveivable portion of the swap.",
+        description="The floating rate index for receivable portion of the swap.",
         default=None,
     )
     floating_rate_spread_rec: Optional[float] = Field(
         description="The floating rate spread for reveivable portion of the swap.",
         default=None,
     )
     rate_tenor_rec: Optional[str] = Field(
-        description="The rate tenor for reveivable portion of the swap.", default=None
+        description="The rate tenor for receivable portion of the swap.", default=None
     )
     rate_tenor_unit_rec: Optional[Union[str, int]] = Field(
-        description="The rate tenor unit for reveivable portion of the swap.",
+        description="The rate tenor unit for receivable portion of the swap.",
         default=None,
     )
     reset_date_rec: Optional[str] = Field(
-        description="The reset date for reveivable portion of the swap.", default=None
+        description="The reset date for receivable portion of the swap.", default=None
     )
     reset_date_unit_rec: Optional[Union[str, int]] = Field(
-        description="The reset date unit for reveivable portion of the swap.",
+        description="The reset date unit for receivable portion of the swap.",
         default=None,
     )
     rate_type_pmnt: Optional[str] = Field(
         description="The type of rate for payment portion of the swap.", default=None
     )
     payment_currency: Optional[str] = Field(
         description="The payment currency of the swap.", default=None
@@ -280,14 +287,20 @@
     notional_currency: Optional[str] = Field(
         description="The currency of the derivative's notional amount.", default=None
     )
     unrealized_gain: Optional[float] = Field(
         description="The unrealized gain or loss on the derivative.", default=None
     )
 
+    @field_validator("weight", "annualized_return", mode="before", check_fields=False)
+    @classmethod
+    def normalize_percent(cls, v):
+        """Normalize the percent values."""
+        return float(v) / 100 if v else None
+
     @model_validator(mode="before")
     @classmethod
     def replace_zero(cls, values):
         """Check for zero values and replace with None."""
         return (
             {k: None if v == 0 else v for k, v in values.items()}
             if isinstance(values, dict)
@@ -305,69 +318,81 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecEtfHoldingsQueryParams:
         """Transform the query."""
         params["symbol"] = params["symbol"].upper()
         return SecEtfHoldingsQueryParams(**params)
 
-    # pylint: disable=unused-argument
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecEtfHoldingsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the SEC endpoint."""
-        filing_candidates = pd.DataFrame.from_records(
-            get_nport_candidates(symbol=query.symbol, use_cache=query.use_cache)
+        filings = await get_nport_candidates(
+            symbol=query.symbol, use_cache=query.use_cache
         )
+        filing_candidates = pd.DataFrame.from_records(filings)
         if filing_candidates.empty:
             raise ValueError(f"No N-Port records found for {query.symbol}.")
-        dates = filing_candidates["period_ending"].to_list()
+        dates = filing_candidates.period_ending.to_list()
         new_date: str = ""
         if query.date is not None:
             date = query.date
             # Gets the URL for the nearest date to the requested date.
             __dates = pd.Series(pd.to_datetime(dates))
             __date = pd.to_datetime(date)
             __nearest = pd.DataFrame(__dates - __date)
             __nearest_date = abs(__nearest[0].astype("int64")).idxmin()
             new_date = __dates[__nearest_date].strftime("%Y-%m-%d")
             date = new_date if new_date else date
-            _warn(f"Closest filing date to, {query.date}, is the period ending: {date}")
+            warn(f"Closest filing date to, {query.date}, is the period ending: {date}")
             filing_url = filing_candidates[filing_candidates["period_ending"] == date][
                 "primary_doc"
             ].values[0]
         else:
             filing_url = filing_candidates["primary_doc"].values[0]
-            period_ending = filing_candidates["period_ending"].values[0]
-            _warn(f"The latest filing is for the period ending: {period_ending}")
-        _warn(f"Source Document: {filing_url}")
-        r = (
-            sec_session_etf.get(filing_url, headers=HEADERS, timeout=5)
-            if query.use_cache
-            else requests.get(filing_url, headers=HEADERS, timeout=5)
-        )
-        if r.status_code != 200:
-            raise RuntimeError(f"Request failed with status code {r.status_code}")
-        response = xmltodict.parse(r.content)
 
-        return response
+        async def callback(response, session):
+            """Response callback for the request."""
+            return await response.read()
+
+        if query.use_cache is True:
+            cache_dir = f"{get_user_cache_directory()}/http/sec_etf"
+            async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
+                try:
+                    response = await amake_request(
+                        filing_url, headers=HEADERS, session=session, response_callback=callback  # type: ignore
+                    )
+                finally:
+                    await session.close()
+        else:
+            response = await amake_request(
+                filing_url, headers=HEADERS, response_callback=callback  # type: ignore
+            )
+        results = xmltodict.parse(response)
+
+        return results
 
     # pylint: disable=too-many-statements
     @staticmethod
     def transform_data(  # noqa: PLR0912
         query: SecEtfHoldingsQueryParams,
         data: Dict,
         **kwargs: Any,
-    ) -> List[SecEtfHoldingsData]:
+    ) -> AnnotatedResult[List[SecEtfHoldingsData]]:
         """Transform the data."""
+
+        if not data:
+            raise EmptyDataError(f"No data was returned for the symbol, {query.symbol}")
         results = []
 
         response = data
+
         # Parse the response if it is a NPORT-P filing.
         if (
             "edgarSubmission" in response
             and "formData" in response["edgarSubmission"]
             and response["edgarSubmission"]["headerData"]["submissionType"] == "NPORT-P"
             and "invstOrSecs" in response["edgarSubmission"]["formData"]
             and "invstOrSec" in response["edgarSubmission"]["formData"]["invstOrSecs"]
@@ -702,9 +727,115 @@
             df["pctVal"] = df["pctVal"].astype(float)
             results = (
                 df.fillna("N/A")
                 .replace("N/A", None)
                 .sort_values(by="pctVal", ascending=False)
                 .to_dict(orient="records")
             )
-
-        return [SecEtfHoldingsData.model_validate(d) for d in results]
+        # Extract additional information from the form that doesn't belong in the holdings table.
+        metadata = {}
+        try:
+            gen_info = response["edgarSubmission"]["formData"].get("genInfo", {})  # type: ignore
+            if gen_info:
+                metadata["fund_name"] = gen_info.get("seriesName")
+                metadata["series_id"] = gen_info.get("seriesId")
+                metadata["lei"] = gen_info.get("seriesLei")
+                metadata["period_ending"] = gen_info.get("repPdDate")
+                metadata["fiscal_year_end"] = gen_info.get("repPdEnd")
+                current_month = pd.to_datetime(metadata["period_ending"])
+                month_1 = (current_month - MonthEnd(2)).date().strftime("%Y-%m-%d")
+                month_2 = (current_month - MonthEnd(1)).date().strftime("%Y-%m-%d")
+                month_3 = current_month.strftime("%Y-%m-%d")
+            fund_info = response["edgarSubmission"]["formData"].get("fundInfo", {})  # type: ignore
+            if fund_info:
+                metadata["total_assets"] = float(fund_info.pop("totAssets", None))
+                metadata["total_liabilities"] = float(fund_info.pop("totLiabs", None))
+                metadata["net_assets"] = float(fund_info.pop("netAssets", None))
+                metadata["cash_and_equivalents"] = fund_info.pop(
+                    "cshNotRptdInCorD", None
+                )
+                return_info = fund_info["returnInfo"]["monthlyTotReturns"].get(
+                    "monthlyTotReturn", {}
+                )
+                returns = {
+                    month_1: float(return_info.get("@rtn1")) / 100,
+                    month_2: float(return_info.get("@rtn2")) / 100,
+                    month_3: float(return_info.get("@rtn3")) / 100,
+                }
+                metadata["returns"] = returns
+                flow = {
+                    month_1: {
+                        "creation": float(fund_info["mon1Flow"].get("@sales", None)),
+                        "redemption": float(
+                            fund_info["mon1Flow"].get("@redemption", None)
+                        ),
+                    },
+                    month_2: {
+                        "creation": float(fund_info["mon2Flow"].get("@sales", None)),
+                        "redemption": float(
+                            fund_info["mon2Flow"].get("@redemption", None)
+                        ),
+                    },
+                    month_3: {
+                        "creation": float(fund_info["mon3Flow"].get("@sales")),
+                        "redemption": float(
+                            fund_info["mon3Flow"].get("@redemption", None)
+                        ),
+                    },
+                }
+                metadata["flow"] = flow
+                gains = {
+                    month_1: {
+                        "realized": float(
+                            fund_info["returnInfo"]["othMon1"].get(
+                                "@netRealizedGain", None
+                            )
+                        ),
+                        "unrealized": float(
+                            fund_info["returnInfo"]["othMon1"].get(
+                                "@netUnrealizedAppr", None
+                            )
+                        ),
+                    },
+                    month_2: {
+                        "realized": float(
+                            fund_info["returnInfo"]["othMon2"].get(
+                                "@netRealizedGain", None
+                            )
+                        ),
+                        "unrealized": float(
+                            fund_info["returnInfo"]["othMon2"].get(
+                                "@netUnrealizedAppr", None
+                            )
+                        ),
+                    },
+                    month_3: {
+                        "realized": float(
+                            fund_info["returnInfo"]["othMon3"].get(
+                                "@netRealizedGain", None
+                            )
+                        ),
+                        "unrealized": float(
+                            fund_info["returnInfo"]["othMon3"].get(
+                                "@netUnrealizedAppr", None
+                            )
+                        ),
+                    },
+                }
+                metadata["gains"] = gains
+                _borrowers = fund_info["borrowers"].get("borrower", [])
+                if _borrowers:
+                    borrowers = [
+                        {
+                            "name": d["@name"],
+                            "lei": d["@lei"],
+                            "value": float(d["@aggrVal"]),
+                        }
+                        for d in _borrowers
+                    ]
+                    metadata["borrowers"] = borrowers
+        except Exception as e:  # pylint: disable=W0718
+            warn(f"Error extracting metadata: {e}")
+        return AnnotatedResult(
+            result=[SecEtfHoldingsData.model_validate(d) for d in results],
+            metadata=metadata,
+        )
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,17 +52,17 @@
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
         symbol = query.symbol
         urls = []
         cik = symbol.isnumeric()
         filings = (
-            parse_13f.get_13f_candidates(symbol=symbol)
+            await parse_13f.get_13f_candidates(symbol=symbol)
             if cik is False
-            else parse_13f.get_13f_candidates(cik=symbol)
+            else await parse_13f.get_13f_candidates(cik=symbol)
         )
         if query.limit and query.date is None:
             urls = filings.iloc[: query.limit].to_list()
         if query.date is not None:
             date = parse_13f.date_to_quarter_end(query.date.strftime("%Y-%m-%d"))
             urls = [filings.loc[date]]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """SEC Institutions Search Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cot_search import CotSearchQueryParams
 from openbb_sec.utils.helpers import get_all_ciks
 from pydantic import Field
@@ -36,26 +38,24 @@
     """Transform the query, extract and transform the data from the SEC endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecInstitutionsSearchQueryParams:
         """Transform the query."""
         return SecInstitutionsSearchQueryParams(**params)
 
-    # pylint: disable=unused-argument
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecInstitutionsSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
-        institutions = get_all_ciks(use_cache=query.use_cache)
+        institutions = await get_all_ciks(use_cache=query.use_cache)
         hp = institutions["Institution"].str.contains(query.query, case=False)
         return institutions[hp].astype(str).to_dict("records")
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: SecInstitutionsSearchQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecInstitutionsSearchData]:
         """Transform the data to the standard format."""
         return [SecInstitutionsSearchData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """SEC Litigation RSS Feed Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
-import requests
 import xmltodict
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_sec.utils.definitions import SEC_HEADERS
+from openbb_core.provider.utils.helpers import make_request
+from openbb_sec.utils.definitions import HEADERS
 from pydantic import Field
 
 
 class SecRssLitigationQueryParams(QueryParams):
     """SEC Litigation RSS Feed Query.
 
     Source: https://sec.gov/
@@ -45,15 +47,15 @@
         query: SecRssLitigationQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
         results = []
         url = "https://www.sec.gov/rss/litigation/litreleases.xml"
-        r = requests.get(url, headers=SEC_HEADERS, timeout=5)
+        r = make_request(url, headers=HEADERS)
 
         if r.status_code == 200:
             data = xmltodict.parse(r.content)
             cols = ["title", "link", "summary", "date", "id"]
             feed = pd.DataFrame.from_records(data["rss"]["channel"]["item"])[
                 ["title", "link", "description", "pubDate", "dc:creator"]
             ]
@@ -69,10 +71,12 @@
                 )
 
             results = feed.reset_index().to_dict(orient="records")
 
         return results
 
     @staticmethod
-    def transform_data(data: List[Dict], **kwargs: Any) -> List[SecRssLitigationData]:
+    def transform_data(
+        query: SecRssLitigationQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[SecRssLitigationData]:
         """Transform the data to the standard format."""
         return [SecRssLitigationData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/sic_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """SEC Standard Industrial Classification Code (SIC) Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
-import requests
+from aiohttp_client_cache import SQLiteBackend
+from aiohttp_client_cache.session import CachedSession
+from openbb_core.app.utils import get_user_cache_directory
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cot_search import CotSearchQueryParams
-from openbb_sec.utils.helpers import SEC_HEADERS, sec_session_companies
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_sec.utils.helpers import SEC_HEADERS, sec_callback
 from pydantic import Field
 
 
 class SecSicSearchQueryParams(CotSearchQueryParams):
     """SEC Standard Industrial Classification Code (SIC) Query.
 
     Source: https://sec.gov/
@@ -33,57 +38,61 @@
     Fetcher[
         SecSicSearchQueryParams,
         List[SecSicSearchData],
     ]
 ):
     """Transform the query, extract and transform the data from the SEC endpoints."""
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_query(
         params: Dict[str, Any], **kwargs: Any
     ) -> SecSicSearchQueryParams:
         """Transform the query."""
         return SecSicSearchQueryParams(**params)
 
-    # pylint: disable=unused-argument
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecSicSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract data from the SEC website table."""
         data = pd.DataFrame()
         results: List[Dict] = []
         url = (
             "https://www.sec.gov/corpfin/"
             "division-of-corporation-finance-standard-industrial-classification-sic-code-list"
         )
-        r = (
-            sec_session_companies.get(url, timeout=5, headers=SEC_HEADERS)
-            if query.use_cache is True
-            else requests.get(url, timeout=5, headers=SEC_HEADERS)
-        )
-
-        if r.status_code == 200:
-            data = pd.read_html(r.content.decode())[0].astype(str)
-            if len(data) == 0:
-                return results
-            if query:
-                data = data[
-                    data["SIC Code"].str.contains(query.query, case=False)
-                    | data["Office"].str.contains(query.query, case=False)
-                    | data["Industry Title"].str.contains(query.query, case=False)
-                ]
-            data["SIC Code"] = data["SIC Code"].astype(int)
+        if query.use_cache is True:
+            cache_dir = f"{get_user_cache_directory()}/http/sec_sic"
+            async with CachedSession(
+                cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 30)
+            ) as session:
+                try:
+                    response = await amake_request(
+                        url, headers=SEC_HEADERS, session=session, response_callback=sec_callback  # type: ignore
+                    )
+                finally:
+                    await session.close()
+        else:
+            response = await amake_request(url, headers=SEC_HEADERS, response_callback=sec_callback)  # type: ignore
+
+        data = pd.read_html(response)[0].astype(str)
+        if len(data) == 0:
+            return results
+        if query:
+            data = data[
+                data["SIC Code"].str.contains(query.query, case=False)
+                | data["Office"].str.contains(query.query, case=False)
+                | data["Industry Title"].str.contains(query.query, case=False)
+            ]
+        data["SIC Code"] = data["SIC Code"].astype(int)
         results = data.to_dict("records")
 
         return results
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: SecSicSearchQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecSicSearchData]:
         """Transform the data."""
         return [SecSicSearchData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """SEC Symbol Mapping Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, Optional
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.symbol_map import SymbolMapQueryParams
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 from openbb_sec.utils.helpers import cik_map
 from pydantic import Field
 
-# pylint: disable=unused-argument
-
 
 class SecSymbolMapQueryParams(SymbolMapQueryParams):
     """SEC Symbol Mapping Query.
 
     Source: https://sec.gov/
     """
 
@@ -35,23 +35,25 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecSymbolMapQueryParams:
         """Transform the query."""
         return SecSymbolMapQueryParams(**params)
 
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecSymbolMapQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the SEC endpoint."""
         if not query.query.isdigit():
             raise ValueError("Query is required and must be a valid CIK.")
-        return {"symbol": cik_map(int(query.query))}
+        symbol = await cik_map(int(query.query), query.use_cache)
+        response = {"symbol": symbol}
+        return response
 
     @staticmethod
     def transform_data(
         query: SecSymbolMapQueryParams, data: Dict, **kwargs: Any
     ) -> SecSymbolMapData:
         """Transform the data to the standard format."""
         return SecSymbolMapData.model_validate(data)
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,161 +1,177 @@
 """SEC Helpers module."""
 
-# pylint: skip-file
+# pylint: disable =unused-argument
+
 from datetime import timedelta
 from io import BytesIO
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 from zipfile import ZipFile
 
 import pandas as pd
 import requests
 import requests_cache
+from aiohttp_client_cache import SQLiteBackend
+from aiohttp_client_cache.session import CachedSession
 from openbb_core.app.utils import get_user_cache_directory
+from openbb_core.provider.utils.helpers import amake_request, make_request
 from openbb_sec.utils.definitions import HEADERS, QUARTERS, SEC_HEADERS, TAXONOMIES
 
-cache_dir = get_user_cache_directory()
-
-sec_session_companies = requests_cache.CachedSession(
-    f"{cache_dir}/http/sec_companies", expire_after=timedelta(days=2)
-)
-sec_session_frames = requests_cache.CachedSession(
-    f"{cache_dir}/http/sec_frames", expire_after=timedelta(days=2)
-)
-sec_session_ftd = requests_cache.CachedSession(f"{cache_dir}/http/sec_ftd")
-
-sec_session_etf = requests_cache.CachedSession(f"{cache_dir}/http/sec_etf")
 
-sec_session_company_filings = requests_cache.CachedSession(
-    f"{cache_dir}/http/sec_company_filings", expire_after=timedelta(days=1)
-)
+async def sec_callback(response, session):
+    """Response callback for SEC requests."""
+    content_type = response.headers.get("Content-Type", "")
+    if "application/json" in content_type:
+        return await response.json()
+    if "text/html" in content_type:
+        return await response.text(encoding="latin-1")
+    return await response.text()
 
 
-def get_all_companies(use_cache: bool = True) -> pd.DataFrame:
+async def get_all_companies(use_cache: bool = True) -> pd.DataFrame:
     """Get all company names, tickers, and CIK numbers registered with the SEC.
 
     Companies are sorted by market cap.
 
     Returns
     -------
     pd.DataFrame: Pandas DataFrame with columns for Symbol, Company Name, and CIK Number.
 
     Example
     -------
     >>> tickers = get_all_companies()
     """
     url = "https://www.sec.gov/files/company_tickers.json"
 
-    r = (
-        sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
-        if use_cache is True
-        else requests.get(url, headers=SEC_HEADERS, timeout=5)
-    )
-    df = pd.DataFrame(r.json()).transpose()
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_companies"
+        async with CachedSession(
+            cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
+        ) as session:
+            try:
+                response = await amake_request(url, headers=SEC_HEADERS, session=session)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, headers=SEC_HEADERS)  # type: ignore
+
+    df = pd.DataFrame(response).transpose()
     cols = ["cik", "symbol", "name"]
     df.columns = cols
     return df.astype(str)
 
 
-def get_all_ciks(use_cache: bool = True) -> pd.DataFrame:
+async def get_all_ciks(use_cache: bool = True) -> pd.DataFrame:
     """Get a list of entity names and their CIK number."""
-    HEADERS = {
-        "User-Agent": "my real company name definitelynot@fakecompany.com",
-        "Accept-Encoding": "gzip, deflate",
-        "Host": "www.sec.gov",
-    }
     url = "https://www.sec.gov/Archives/edgar/cik-lookup-data.txt"
-    r = (
-        sec_session_companies.get(url, headers=HEADERS, timeout=5)
-        if use_cache is True
-        else requests.get(url, headers=HEADERS, timeout=5)
-    )
-    data = r.text
-    lines = data.split("\n")
+
+    async def callback(response, session):
+        """Response callback for CIK lookup data."""
+        return await response.text(encoding="latin-1")
+
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_ciks"
+        async with CachedSession(
+            cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
+        ) as session:
+            try:
+                response = await amake_request(url, headers=SEC_HEADERS, session=session, response_callback=callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, headers=SEC_HEADERS, response_callback=callback)  # type: ignore
+    data = response
+    lines = data.split("\n")  # type: ignore
     data_list = []
     delimiter = ":"
     for line in lines:
         row = line.split(delimiter)
         data_list.append(row)
     df = pd.DataFrame(data_list)
     df = df.iloc[:, 0:2]
     cols = ["Institution", "CIK Number"]
     df.columns = cols
     df = df.dropna()
 
-    return df
+    return df.astype(str)
 
 
-def get_mf_and_etf_map(use_cache: bool = True) -> pd.DataFrame:
+async def get_mf_and_etf_map(use_cache: bool = True) -> pd.DataFrame:
     """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbols = pd.DataFrame()
 
     url = "https://www.sec.gov/files/company_tickers_mf.json"
-    r = (
-        sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
-        if use_cache is True
-        else requests.get(url, headers=SEC_HEADERS, timeout=5)
-    )
-    if r.status_code == 200:
-        symbols = pd.DataFrame(data=r.json()["data"], columns=r.json()["fields"])
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_mf_etf_map"
+        async with CachedSession(
+            cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
+        ) as session:
+            try:
+                response = await amake_request(url, headers=SEC_HEADERS, session=session, response_callback=sec_callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, headers=SEC_HEADERS, response_callback=sec_callback)  # type: ignore
 
-    return symbols
+    symbols = pd.DataFrame(data=response["data"], columns=response["fields"])  # type: ignore
 
+    return symbols.astype(str)
 
-def search_institutions(keyword: str, use_cache: bool = True) -> pd.DataFrame:
+
+async def search_institutions(keyword: str, use_cache: bool = True) -> pd.DataFrame:
     """Search for an institution by name.  It is case-insensitive."""
-    institutions = get_all_ciks(use_cache=use_cache)
+    institutions = await get_all_ciks(use_cache=use_cache)
     hp = institutions["Institution"].str.contains(keyword, case=False)
-    return institutions[hp].astype(str)
+    return institutions[hp]
 
 
-def symbol_map(symbol: str, use_cache: bool = True) -> str:
+async def symbol_map(symbol: str, use_cache: bool = True) -> str:
     """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbol = symbol.upper().replace(".", "-")
-    symbols = get_all_companies(use_cache=use_cache)
+    symbols = await get_all_companies(use_cache=use_cache)
 
     if symbol not in symbols["symbol"].to_list():
-        symbols = get_mf_and_etf_map(use_cache=use_cache).astype(str)
+        symbols = await get_mf_and_etf_map(use_cache=use_cache)
         if symbol not in symbols["symbol"].to_list():
             return ""
-
     cik = symbols[symbols["symbol"] == symbol]["cik"].iloc[0]
     cik_: str = ""
     temp = 10 - len(cik)
-    for i in range(temp):
+    for i in range(temp):  # pylint: disable=W0612
         cik_ = cik_ + "0"
 
     return str(cik_ + cik)
 
 
-def cik_map(cik: int, use_cache: bool = True) -> str:
+async def cik_map(cik: Union[str, int], use_cache: bool = True) -> str:
     """Convert a CIK number to a ticker symbol.  Enter CIK as an integer with no leading zeros.
 
     Function is not meant for funds.
 
     Parameters
     ----------
     cik : int
         The CIK number to convert to a ticker symbol.
 
     Returns
     -------
     str: The ticker symbol associated with the CIK number.
     """
-    _cik = str(cik)
+    _cik = str(cik) if isinstance(cik, int) else cik.lstrip("0")
     symbol = ""
-    companies = get_all_companies(use_cache=use_cache).astype(str)
+    companies = await get_all_companies(use_cache=use_cache)
     if _cik in companies["cik"].to_list():
         symbol = companies[companies["cik"] == _cik]["symbol"].iloc[0]
     else:
-        return f"Error: CIK, {cik}, does not have a unique ticker."
+        return f"Error: CIK, {_cik}, does not have a unique ticker."
 
     return symbol
 
 
-def get_frame(
+def get_frame(  # pylint: disable =too-many-arguments
     year: int,
     quarter: Optional[QUARTERS] = None,
     taxonomy: TAXONOMIES = "us-gaap",
     units: str = "USD",
     fact: str = "Revenues",
     instantaneous: bool = False,
     use_cache: bool = True,
@@ -192,15 +208,17 @@
     NetIncomeLoss
 
     Facts where units are, "shares":
     WeightedAverageNumberOfDilutedSharesOutstanding
     """
     if fact in ["WeightedAverageNumberOfDilutedSharesOutstanding"]:
         units = "shares"
-
+    sec_session_frames = requests_cache.CachedSession(
+        f"{get_user_cache_directory()}/http/sec_frames", expire_after=timedelta(days=2)
+    )
     url = f"https://data.sec.gov/api/xbrl/frames/{taxonomy}/{fact}/{units}/CY{year}"
 
     if quarter:
         url = url + f"Q{quarter}"
 
     if instantaneous:
         url = url + "I"
@@ -228,88 +246,101 @@
     }
 
     results = {"metadata": metadata, "data": data}
 
     return results
 
 
-def get_schema_filelist(query: str = "", url: str = "") -> List:
+def get_schema_filelist(query: str = "", url: str = "", use_cache: bool = True) -> List:
     """Get a list of schema files from the SEC website."""
     results: List = []
     url = url if url else f"https://xbrl.fasb.org/us-gaap/{query}"
     _url = url
     _url = url + "/" if query else _url
-    r = sec_session_companies.get(_url, headers=HEADERS, timeout=5)
-
-    if r.status_code != 200:
-        raise RuntimeError(f"Request failed with status code {r.status_code}")
-
-    data = pd.read_html(r.content.decode())[0]["Name"].dropna()
+    response = make_request(_url)
+    data = pd.read_html(response.content)[0]["Name"].dropna()
     if len(data) > 0:
         data.iloc[0] = url if not query else url + "/"
         results = data.to_list()
 
     return results
 
 
-def download_zip_file(url, symbol: Optional[str] = None) -> List[Dict]:
+async def download_zip_file(
+    url, symbol: Optional[str] = None, use_cache: bool = True
+) -> List[Dict]:
     """Download a list of files from URLs."""
     results = pd.DataFrame()
-    r = sec_session_ftd.get(url, timeout=5, headers=HEADERS)
-    if r.status_code == 200:
-        try:
-            data = pd.read_csv(BytesIO(r.content), compression="zip", sep="|")
-            results = data.iloc[:-2]
-        except ValueError:
-            zip_file = ZipFile(BytesIO(r.content))
-            file_list = [d.filename for d in zip_file.infolist()]
-            for item in file_list:
+
+    async def callback(response, session):
+        """Response callback for ZIP file downloads."""
+        return await response.read()
+
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_ftd"
+        async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
+            try:
+                response = await amake_request(url, session=session, headers=HEADERS, response_callback=callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, response_callback=callback)  # type: ignore
+
+    try:
+        data = pd.read_csv(BytesIO(response), compression="zip", sep="|")  # type: ignore
+        results = data.iloc[:-2]
+    except ValueError:
+        zip_file = ZipFile(BytesIO(response))  # type: ignore
+        file_list = [d.filename for d in zip_file.infolist()]
+        for item in file_list:
+            with zip_file.open(item) as _item:
                 _file = pd.read_csv(
-                    zip_file.open(item),
+                    _item,
                     encoding="ISO-8859-1",
                     sep="|",
                     low_memory=False,
                     on_bad_lines="skip",
                 )
                 results = pd.concat([results, _file.iloc[:-2]])
-        if "SETTLEMENT DATE" in results.columns:
-            results = results.rename(
-                columns={
-                    "SETTLEMENT DATE": "date",
-                    "SYMBOL": "symbol",
-                    "CUSIP": "cusip",
-                    "QUANTITY (FAILS)": "quantity",
-                    "PRICE": "price",
-                    "DESCRIPTION": "description",
-                }
-            )
-            if symbol is not None:
-                results = results[results["symbol"] == symbol]
-            results["date"] = pd.to_datetime(results["date"], format="%Y%m%d").dt.date
-            results["price"] = results["price"].mask(
-                results["price"].str.contains(r"^\d+(?:\.\d+)?$", regex=True)
-                == False,  # noqa
-                None,
+
+    if "SETTLEMENT DATE" in results.columns:
+        results = results.rename(
+            columns={
+                "SETTLEMENT DATE": "date",
+                "SYMBOL": "symbol",
+                "CUSIP": "cusip",
+                "QUANTITY (FAILS)": "quantity",
+                "PRICE": "price",
+                "DESCRIPTION": "description",
+            }
+        )
+        if symbol is not None:
+            results = results[results["symbol"] == symbol]
+        results["date"] = pd.to_datetime(results["date"], format="%Y%m%d").dt.date
+        results["price"] = results["price"].mask(
+            results["price"].str.contains(  # pylint: disable=C0121
+                r"^\d+(?:\.\d+)?$", regex=True
             )
-            results["price"] = results["price"].astype(float)
+            == False,  # noqa
+            None,
+        )
+        results["price"] = results["price"].astype(float)
 
     return results.reset_index(drop=True).to_dict("records")
 
 
-def get_ftd_urls() -> Dict:
+async def get_ftd_urls() -> Dict:
     """Get Fails-to-Deliver Data URLs."""
     results = {}
     position = None
     key = "title"
     value = "Fails-to-Deliver Data"
 
-    r = requests.get("https://www.sec.gov/data.json", timeout=5, headers=SEC_HEADERS)
-    if r.status_code != 200:
-        raise RuntimeError(f"Request failed with status code {str(r.status_code)}")
-    data = r.json()["dataset"]
+    r = await amake_request("https://www.sec.gov/data.json", headers=SEC_HEADERS)
+    data = r.get("dataset", {})  # type: ignore
 
     for index, d in enumerate(data):
         if key in d and d[key] == value:
             position = index
             break
     if position is not None:
         fails = data[position]["distribution"]
@@ -319,15 +350,15 @@
         ftd_urls = pd.Series(index=dates, data=urls)
         ftd_urls.index = ftd_urls.index.str.replace("_", "")
         results = ftd_urls.to_dict()
 
     return results
 
 
-def get_series_id(
+async def get_series_id(
     symbol: Optional[str] = None, cik: Optional[str] = None, use_cache: bool = True
 ):
     """Map the fund to the series and class IDs for validating the correct filing.
 
     For an exact match, use a symbol.
     """
     symbol = symbol if symbol else ""
@@ -335,77 +366,69 @@
 
     results = pd.DataFrame()
     if not symbol and not cik:
         raise ValueError("Either symbol or cik must be provided.")
 
     target = symbol if symbol else cik
     choice = "cik" if not symbol else "symbol"
-    funds = get_mf_and_etf_map(use_cache=use_cache).astype(str)
+    funds = await get_mf_and_etf_map(use_cache=use_cache)
 
     results = funds[
         funds["cik"].str.contains(target, case=False)
         | funds["seriesId"].str.contains(target, case=False)
         | funds["classId"].str.contains(target, case=False)
         | funds["symbol"].str.contains(target, case=False)
     ]
 
     if len(results) > 0:
         results = results[results[choice if not symbol else choice] == target]
 
         return results
 
 
-def get_nport_candidates(symbol: str, use_cache: bool = True) -> List[Dict]:
+async def get_nport_candidates(symbol: str, use_cache: bool = True) -> List[Dict]:
     """Get a list of all NPORT-P filings for a given fund's symbol."""
     results = []
-    _series_id = get_series_id(symbol, use_cache=use_cache)
+    _series_id = await get_series_id(symbol, use_cache=use_cache)
     try:
         series_id = (
-            symbol_map(symbol, use_cache)
+            await symbol_map(symbol, use_cache)
             if _series_id is None or len(_series_id) == 0
             else _series_id["seriesId"].iloc[0]
         )
-    except IndexError:
-        raise ValueError("Fund not found for, the symbol: " + symbol)
+    except IndexError as e:
+        raise ValueError("Fund not found for, the symbol: " + symbol) from e
     if series_id == "" or series_id is None:
         raise ValueError("Fund not found for, the symbol: " + symbol)
 
     url = f"https://efts.sec.gov/LATEST/search-index?q={series_id}&dateRange=all&forms=NPORT-P"
 
-    def request_data(url: str = url, use_cache: bool = use_cache):
-        r = (
-            sec_session_companies.get(url, timeout=5, headers=HEADERS)
-            if use_cache is True
-            else requests.get(url, headers=HEADERS, timeout=5)
-        )
-        return r
-
-    r = request_data(url, use_cache=use_cache)
-
-    if r.status_code != 200:
-        if r.status_code == 500:
-            r = request_data()
-            if r.status_code != 200:
-                raise RuntimeError(
-                    f"Request failed with status code {str(r.status_code)}"
-                )
-        if r.status_code not in (200, 500):
-            raise RuntimeError(f"Request failed with status code {str(r.status_code)}")
-    r_json = r.json()
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_etf"
+        async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
+            try:
+                response = await amake_request(url, session=session, headers=HEADERS, response_callback=sec_callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, response_callback=sec_callback)  # type: ignore
 
-    if "hits" in r_json and len(r_json["hits"]["hits"]) > 0:
-        hits = r_json["hits"]["hits"]
+    if "hits" in response and len(response["hits"].get("hits")) > 0:  # type: ignore
+        hits = response["hits"]["hits"]  # type: ignore
         results = [
             {
                 "name": d["_source"]["display_names"][0],
                 "cik": d["_source"]["ciks"][0],
                 "file_date": d["_source"]["file_date"],
                 "period_ending": d["_source"]["period_ending"],
                 "form_type": d["_source"]["form"],
-                "primary_doc": f"https://www.sec.gov/Archives/edgar/data/{int(d['_source']['ciks'][0])}/{d['_id'].replace('-', '').replace(':', '/')}",  # noqa
+                "primary_doc": (
+                    f"https://www.sec.gov/Archives/edgar/data/{int(d['_source']['ciks'][0])}"  # noqa
+                    + f"/{d['_id'].replace('-', '').replace(':', '/')}"  # noqa
+                ),
             }
             for d in hits
         ]
     return (
         sorted(results, key=lambda d: d["file_date"], reverse=True)
         if len(results) > 0
         else results
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,37 +15,40 @@
     return (
         (to_datetime(date).to_period("Q").to_timestamp("D") + offsets.QuarterEnd())
         .date()
         .strftime("%Y-%m-%d")
     )
 
 
-def get_13f_candidates(symbol: Optional[str] = None, cik: Optional[str] = None):
+async def get_13f_candidates(symbol: Optional[str] = None, cik: Optional[str] = None):
     """Get the 13F-HR filings for a given symbol or CIK."""
     fetcher = SecCompanyFilingsFetcher()
     params: Dict[str, Any] = {}
     if cik is not None:
         params["cik"] = str(cik)
     if symbol is not None:
         params["symbol"] = symbol
     if cik is None and symbol is None:
         raise ValueError("Either symbol or cik must be provided.")
 
     params["use_cache"] = False
     params["form_type"] = "13F-HR"
-    query = fetcher.transform_query(params)
-    filings = fetcher.extract_data(query, {})
+    filings = await fetcher.fetch_data(params, {})
+    filings = [d.model_dump() for d in filings]
     if len(filings) == 0:
         raise ValueError(f"No 13F-HR filings found for {symbol if symbol else cik}.")
 
     # Filings before June 30, 2013 are non-structured and are not supported by downstream parsers.
+    up_to = to_datetime("2013-06-30").date()  # pylint: disable=unused-variable # noqa
     return (
         DataFrame(data=filings)
-        .query("`reportDate` >= '2013-06-30'")
-        .set_index("reportDate")["completeSubmissionUrl"]
+        .query("`report_date` >= @up_to")
+        .set_index("report_date")["complete_submission_url"]
+        .fillna("N/A")
+        .replace("N/A", None)
     )
 
 
 async def complete_submission_callback(response, _):
     """Use callback function for processing the response object."""
     if response.status == 200:
         return await response.text()
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202404240009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.7.dev202404240009/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,128 @@
-"""Tradier Equity Quote Model."""
+"""Tradier Options Chains Model."""
 
 # pylint: disable = unused-argument
 
-from datetime import (
-    date as dateType,
-    datetime,
-)
-from typing import Any, Dict, List, Literal, Optional
+import asyncio
+from datetime import datetime
+from typing import Any, Dict, List, Optional
 
 from dateutil.parser import parse
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.equity_quote import (
-    EquityQuoteData,
-    EquityQuoteQueryParams,
+from openbb_core.provider.standard_models.options_chains import (
+    OptionsChainsData,
+    OptionsChainsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
-class TradierEquityQuoteQueryParams(EquityQuoteQueryParams):
-    """Tradier Equity Quote Query."""
+class TradierOptionsChainsQueryParams(OptionsChainsQueryParams):
+    """Tradier Options Chains Query.
+
+    Source: https://documentation.tradier.com/brokerage-api/markets/get-options-chains
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    Greeks/IV data is updated once per hour.
+    This data is calculated using the ORATS APIs and is supplied directly from them.
+    """
 
 
-class TradierEquityQuoteData(EquityQuoteData):
-    """Tradier Equity Quote Data."""
+class TradierOptionsChainsData(OptionsChainsData):
+    """Tradier Options Chains Data."""
 
     __alias_dict__ = {
-        "name": "description",
-        "exchange": "exch",
-        "asset_type": "type",
-        "bid_exchange": "bidexch",
+        "expiration": "expiration_date",
+        "contract_symbol": "symbol",
+        "last_trade_price": "last",
         "bid_size": "bidsize",
         "ask_size": "asksize",
-        "ask_exchange": "askexch",
-        "last_price": "last",
-        "last_timestamp": "trade_date",
-        "prev_close": "prevclose",
-        "year_high": "week_52_high",
-        "year_low": "week_52_low",
-        "volume_avg": "average_volume",
         "change_percent": "change_percentage",
-        "root_symbol": "root_symbols",
         "orats_final_iv": "smv_vol",
+        "implied_volatility": "mid_iv",
         "greeks_timestamp": "updated_at",
-        "bid_timestamp": "bid_date",
+        "prev_close": "prevclose",
+        "year_high": "week_52_high",
+        "year_low": "week_52_low",
+        "last_trade_timestamp": "trade_date",
+        "last_trade_volume": "last_volume",
+        "ask_exchange": "askexch",
         "ask_timestamp": "ask_date",
+        "bid_exchange": "bidexch",
+        "bid_timestamp": "bid_date",
     }
 
-    last_volume: Optional[int] = Field(
+    phi: Optional[float] = Field(
         default=None,
-        description="The last trade volume.",
+        description="Phi of the option. The sensitivity of the option relative to dividend yield.",
     )
-    volume_avg: Optional[int] = Field(
+    bid_iv: Optional[float] = Field(
         default=None,
-        description="The average daily trading volume.",
+        description="Implied volatility of the bid price.",
     )
-    bid_timestamp: Optional[datetime] = Field(
+    ask_iv: Optional[float] = Field(
         default=None,
-        description="Timestamp of the bid price.",
+        description="Implied volatility of the ask price.",
     )
-    ask_timestamp: Optional[datetime] = Field(
+    orats_final_iv: Optional[float] = Field(
         default=None,
-        description="Timestamp of the ask price.",
+        description="ORATS final implied volatility of the option, updated once per hour.",
     )
-    greeks_timestamp: Optional[datetime] = Field(
+    year_high: Optional[float] = Field(
         default=None,
-        description="Timestamp of the greeks data.",
+        description="52-week high price of the option.",
     )
-    underlying: Optional[str] = Field(
+    year_low: Optional[float] = Field(
         default=None,
-        description="The underlying symbol for the option.",
+        description="52-week low price of the option.",
     )
-    root_symbol: Optional[str] = Field(
+    last_trade_volume: Optional[int] = Field(
         default=None,
-        description="The root symbol for the option.",
+        description="Volume of the last trade.",
     )
-    option_type: Optional[Literal["call", "put"]] = Field(
+    dte: Optional[int] = Field(
         default=None,
-        description="Type of option - call or put.",
+        description="Days to expiration.",
     )
     contract_size: Optional[int] = Field(
         default=None,
-        description="The number of shares in a standard contract.",
-    )
-    expiration_type: Optional[str] = Field(
-        default=None,
-        description="The expiration type of the option - i.e, standard, weekly, etc.",
-    )
-    expiration_date: Optional[dateType] = Field(
-        default=None,
-        description="The expiration date of the option.",
-    )
-    strike: Optional[float] = Field(
-        default=None,
-        description="The strike price of the option.",
-    )
-    open_interest: Optional[int] = Field(
-        default=None,
-        description="The number of open contracts for the option.",
-    )
-    bid_iv: Optional[float] = Field(
-        default=None,
-        description="Implied volatility of the bid price.",
-    )
-    ask_iv: Optional[float] = Field(
-        default=None,
-        description="Implied volatility of the ask price.",
-    )
-    mid_iv: Optional[float] = Field(
-        default=None,
-        description="Mid-point implied volatility of the option.",
-    )
-    orats_final_iv: Optional[float] = Field(
-        default=None,
-        description="ORATS final implied volatility of the option.",
+        description="Size of the contract.",
     )
-    delta: Optional[float] = Field(
+    bid_exchange: Optional[str] = Field(
         default=None,
-        description="Delta of the option.",
+        description="Exchange of the bid price.",
     )
-    gamma: Optional[float] = Field(
+    bid_timestamp: Optional[datetime] = Field(
         default=None,
-        description="Gamma of the option.",
+        description="Timestamp of the bid price.",
     )
-    theta: Optional[float] = Field(
+    ask_exchange: Optional[str] = Field(
         default=None,
-        description="Theta of the option.",
+        description="Exchange of the ask price.",
     )
-    vega: Optional[float] = Field(
+    ask_timestamp: Optional[datetime] = Field(
         default=None,
-        description="Vega of the option.",
+        description="Timestamp of the ask price.",
     )
-    rho: Optional[float] = Field(
+    greeks_timestamp: Optional[datetime] = Field(
         default=None,
-        description="Rho of the option.",
+        description="Timestamp of the last greeks update."
+        + " Greeks/IV data is updated once per hour.",
     )
-    phi: Optional[float] = Field(
-        default=None,
-        description="Phi of the option.",
+    last_trade_timestamp: Optional[datetime] = Field(
+        default=None, description="Timestamp of the last trade."
     )
 
     @field_validator(
-        "last_timestamp",
+        "last_trade_timestamp",
+        "greeks_timestamp",
         "ask_timestamp",
         "bid_timestamp",
-        "greeks_timestamp",
         mode="before",
         check_fields=False,
     )
     @classmethod
     def validate_dates(cls, v):
         """Validate the dates."""
         if v != 0 and v is not None and isinstance(v, int):
@@ -171,38 +140,53 @@
 
     @field_validator("change_percent", mode="before", check_fields=False)
     @classmethod
     def normalize_percent(cls, v):
         """Normalize the percentage."""
         return float(v) / 100 if v else None
 
+    @field_validator("bid_exchange", "ask_exchange", mode="before", check_fields=False)
+    @classmethod
+    def map_exchange(cls, v):
+        """Map the exchange from a code to a name."""
+        if v:
+            return (
+                OPTIONS_EXCHANGES.get(v, v)
+                if v in OPTIONS_EXCHANGES
+                else STOCK_EXCHANGES.get(v, v)
+            )
+        return None
+
     @model_validator(mode="before")
     @classmethod
     def replace_zero(cls, values):
         """Check for zero values and replace with None."""
         return (
-            {k: None if (v == 0 or str(v) == "0") else v for k, v in values.items()}
+            {
+                k: None if (v == 0 or str(v) == "0") and k != "dte" else v
+                for k, v in values.items()
+            }
             if isinstance(values, dict)
             else values
         )
 
 
-class TradierEquityQuoteFetcher(
-    Fetcher[TradierEquityQuoteQueryParams, List[TradierEquityQuoteData]]
+class TradierOptionsChainsFetcher(
+    Fetcher[TradierOptionsChainsQueryParams, List[TradierOptionsChainsData]]
 ):
-    """Tradier Equity Quote Fetcher."""
+    """Tradier Options Chains Fetcher."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> TradierEquityQuoteQueryParams:
-        """Transform the query."""
-        return TradierEquityQuoteQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> TradierOptionsChainsQueryParams:
+        """Transform the query parameters."""
+        return TradierOptionsChainsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: TradierEquityQuoteQueryParams,
+        query: TradierOptionsChainsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Tradier endpoint."""
         api_key = credentials.get("tradier_api_key") if credentials else ""
         sandbox = True
 
@@ -215,74 +199,92 @@
             sandbox = (
                 credentials.get("tradier_account_type") == "sandbox"
                 if credentials
                 else False
             )
 
         BASE_URL = (
-            "https://api.tradier.com/"
+            "https://api.tradier.com/v1/markets/options/"
             if sandbox is False
-            else "https://sandbox.tradier.com/"
+            else "https://sandbox.tradier.com/v1/markets/options/"
         )
+
         HEADERS = {
             "Authorization": f"Bearer {api_key}",
             "Accept": "application/json",
         }
-        url = f"{BASE_URL}v1/markets/quotes?symbols={query.symbol}&greeks=true"
-
-        response = await amake_request(url, headers=HEADERS)
 
-        if response.get("quotes"):  # type: ignore
-            data = response["quotes"].get("quote")  # type: ignore
-            if len(data) > 0:
-                return data if isinstance(data, list) else [data]
-
-        raise EmptyDataError("No results found.")
+        # Get the expiration dates for the symbol so we can gather the chains data.
+        async def get_expirations(symbol):
+            """Get the expiration dates for the given symbol."""
+            url = (
+                f"{BASE_URL}expirations?symbol={symbol}&includeAllRoots=true"
+                "&strikes=false&contractSize=false&expirationType=false"
+            )
+            response = await amake_request(url, headers=HEADERS)
+            if response.get("expirations") and isinstance(response["expirations"].get("date"), list):  # type: ignore
+                expirations = response["expirations"].get("date")  # type: ignore
+                return expirations if expirations else []
+
+        expirations = await get_expirations(query.symbol)
+        if expirations == []:
+            raise ValueError(f"No expiration dates found for {query.symbol}")
+
+        results = []
+
+        async def get_one(url):
+            """Get the chain for a single expiration."""
+            chain = await amake_request(url, headers=HEADERS)
+            if chain.get("options") and isinstance(chain["options"].get("option", []), list):  # type: ignore
+                data = chain["options"]["option"]  # type: ignore
+                for d in data.copy():
+                    # Remove any strikes returned without data.
+                    keys = ["volume", "open_interest", "last", "bid", "ask"]
+                    if all(d.get(key) in [0, "0", None] for key in keys):
+                        data.remove(d)
+                        continue
+                    # Flatten the nested greeks dictionary
+                    greeks = d.pop("greeks")
+                    if greeks is not None:
+                        d.update(**greeks)
+                    # Pop fields that are duplicate information or not of interest.
+                    to_pop = [
+                        "root_symbol",
+                        "exch",
+                        "type",
+                        "expiration_type",
+                        "underlying",
+                        "description",
+                        "average_volume",
+                    ]
+                    _ = [d.pop(key) for key in to_pop if key in d]
+                    # Add the DTE field to the data for easier filtering later.
+                    d["dte"] = (
+                        datetime.strptime(d["expiration_date"], "%Y-%m-%d").date()
+                        - datetime.now().date()
+                    ).days
+
+                results.extend(data)
+
+        urls = [
+            f"{BASE_URL}chains?symbol={query.symbol}&expiration={expiration}&greeks=true"
+            for expiration in expirations  # type: ignore
+        ]
+
+        tasks = [get_one(url) for url in urls]
+
+        await asyncio.gather(*tasks)
+
+        if not results:
+            raise EmptyDataError(f"No options chains data found for {query.symbol}.")
+        return sorted(
+            results, key=lambda x: [x["expiration_date"], x["strike"], x["symbol"]]
+        )
 
     @staticmethod
     def transform_data(
-        query: TradierEquityQuoteQueryParams,
+        query: TradierOptionsChainsQueryParams,
         data: List[Dict],
         **kwargs: Any,
-    ) -> List[TradierEquityQuoteData]:
+    ) -> List[TradierOptionsChainsData]:
         """Transform and validate the data."""
-        results: List[TradierEquityQuoteData] = []
-
-        for d in data:
-
-            d["exch"] = (
-                OPTIONS_EXCHANGES.get(d["exch"])
-                if d.get("type") in ["option", "index"]
-                else STOCK_EXCHANGES.get(d["exch"])
-            )
-            d["askexch"] = (
-                OPTIONS_EXCHANGES.get(d["askexch"])
-                if d.get("type") in ["option", "index"]
-                else STOCK_EXCHANGES.get(d["askexch"])
-            )
-            d["bidexch"] = (
-                OPTIONS_EXCHANGES.get(d["bidexch"])
-                if d.get("type") in ["option", "index"]
-                else STOCK_EXCHANGES.get(d["bidexch"])
-            )
-
-            if "greeks" in d:
-                # Flatten the nested greeks dictionary
-                greeks = d.pop("greeks")
-                if greeks is not None:
-                    d.update(**greeks)
-
-            if (
-                d.get("root_symbols") == d.get("symbol")
-                and d.get("root_symbols") is not None
-            ):
-                _ = d.pop("root_symbols")
-
-            if (
-                d.get("root_symbol") == d.get("underlying")
-                and d.get("root_symbol") is not None
-            ):
-                _ = d.pop("root_symbol")
-
-            results.append(TradierEquityQuoteData.model_validate(d))
-
-        return results
+        return [TradierOptionsChainsData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.7.dev202404240009/providers/sec/openbb_sec/models/company_filings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,290 +1,289 @@
-"""Tradier Options Chains Model."""
+"""SEC Company Filings Model."""
 
-# pylint: disable = unused-argument
+# pylint: disable=unused-argument
 
-import asyncio
-from datetime import datetime
-from typing import Any, Dict, List, Optional
+from datetime import (
+    date as dateType,
+    datetime,
+)
+from typing import Any, Dict, List, Optional, Union
 
-from dateutil.parser import parse
+from aiohttp_client_cache import SQLiteBackend
+from aiohttp_client_cache.session import CachedSession
+from openbb_core.app.utils import get_user_cache_directory
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.options_chains import (
-    OptionsChainsData,
-    OptionsChainsQueryParams,
+from openbb_core.provider.standard_models.company_filings import (
+    CompanyFilingsData,
+    CompanyFilingsQueryParams,
 )
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
-from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
-from pydantic import Field, field_validator, model_validator
-from pytz import timezone
-
+from openbb_core.provider.utils.helpers import amake_request, amake_requests
+from openbb_sec.utils.definitions import FORM_TYPES, HEADERS
+from openbb_sec.utils.helpers import symbol_map
+from pandas import DataFrame
+from pydantic import Field, field_validator
 
-class TradierOptionsChainsQueryParams(OptionsChainsQueryParams):
-    """Tradier Options Chains Query.
 
-    Source: https://documentation.tradier.com/brokerage-api/markets/get-options-chains
+class SecCompanyFilingsQueryParams(CompanyFilingsQueryParams):
+    """SEC Company Filings Query.
 
-    Greeks/IV data is updated once per hour.
-    This data is calculated using the ORATS APIs and is supplied directly from them.
+    Source: https://sec.gov/
     """
 
+    symbol: Optional[str] = Field(
+        description=QUERY_DESCRIPTIONS.get("symbol", ""),
+        default=None,
+    )
+    cik: Optional[Union[str, int]] = Field(
+        description="Lookup filings by Central Index Key (CIK) instead of by symbol.",
+        default=None,
+    )
+    form_type: Union[None, FORM_TYPES] = Field(
+        description="Type of the SEC filing form.",
+        default=None,
+    )
+    use_cache: bool = Field(
+        description="Whether or not to use cache.  If True, cache will store for one day.",
+        default=True,
+    )
+
 
-class TradierOptionsChainsData(OptionsChainsData):
-    """Tradier Options Chains Data."""
+class SecCompanyFilingsData(CompanyFilingsData):
+    """SEC Company Filings Data."""
 
     __alias_dict__ = {
-        "expiration": "expiration_date",
-        "contract_symbol": "symbol",
-        "last_trade_price": "last",
-        "bid_size": "bidsize",
-        "ask_size": "asksize",
-        "change_percent": "change_percentage",
-        "orats_final_iv": "smv_vol",
-        "implied_volatility": "mid_iv",
-        "greeks_timestamp": "updated_at",
-        "prev_close": "prevclose",
-        "year_high": "week_52_high",
-        "year_low": "week_52_low",
-        "last_trade_timestamp": "trade_date",
-        "last_trade_volume": "last_volume",
-        "ask_exchange": "askexch",
-        "ask_timestamp": "ask_date",
-        "bid_exchange": "bidexch",
-        "bid_timestamp": "bid_date",
+        "filing_date": "filingDate",
+        "accepted_date": "acceptanceDateTime",
+        "filing_url": "filingDetailUrl",
+        "report_url": "primaryDocumentUrl",
+        "report_type": "form",
     }
 
-    phi: Optional[float] = Field(
+    report_date: Optional[dateType] = Field(
+        description="The date of the filing.",
         default=None,
-        description="Phi of the option. The sensitivity of the option relative to dividend yield.",
+        alias="reportDate",
     )
-    bid_iv: Optional[float] = Field(
-        default=None,
-        description="Implied volatility of the bid price.",
+    act: Optional[Union[str, int]] = Field(
+        description="The SEC Act number.", default=None
     )
-    ask_iv: Optional[float] = Field(
-        default=None,
-        description="Implied volatility of the ask price.",
+    items: Optional[Union[str, float]] = Field(
+        description="The SEC Item numbers.", default=None
     )
-    orats_final_iv: Optional[float] = Field(
+    primary_doc_description: Optional[str] = Field(
+        description="The description of the primary document.",
         default=None,
-        description="ORATS final implied volatility of the option, updated once per hour.",
+        alias="primaryDocDescription",
     )
-    year_high: Optional[float] = Field(
+    primary_doc: Optional[str] = Field(
+        description="The filename of the primary document.",
         default=None,
-        description="52-week high price of the option.",
+        alias="primaryDocument",
     )
-    year_low: Optional[float] = Field(
+    accession_number: Optional[Union[str, int]] = Field(
+        description="The accession number.",
         default=None,
-        description="52-week low price of the option.",
+        alias="accessionNumber",
     )
-    last_trade_volume: Optional[int] = Field(
+    file_number: Optional[Union[str, int]] = Field(
+        description="The file number.",
         default=None,
-        description="Volume of the last trade.",
+        alias="fileNumber",
     )
-    dte: Optional[int] = Field(
+    film_number: Optional[Union[str, int]] = Field(
+        description="The film number.",
         default=None,
-        description="Days to expiration.",
+        alias="filmNumber",
     )
-    contract_size: Optional[int] = Field(
+    is_inline_xbrl: Optional[Union[str, int]] = Field(
+        description="Whether the filing is an inline XBRL filing.",
         default=None,
-        description="Size of the contract.",
+        alias="isInlineXBRL",
     )
-    bid_exchange: Optional[str] = Field(
+    is_xbrl: Optional[Union[str, int]] = Field(
+        description="Whether the filing is an XBRL filing.",
         default=None,
-        description="Exchange of the bid price.",
+        alias="isXBRL",
     )
-    bid_timestamp: Optional[datetime] = Field(
-        default=None,
-        description="Timestamp of the bid price.",
-    )
-    ask_exchange: Optional[str] = Field(
-        default=None,
-        description="Exchange of the ask price.",
+    size: Optional[Union[str, int]] = Field(
+        description="The size of the filing.", default=None
     )
-    ask_timestamp: Optional[datetime] = Field(
+    complete_submission_url: Optional[str] = Field(
+        description="The URL to the complete filing submission.",
         default=None,
-        description="Timestamp of the ask price.",
+        alias="completeSubmissionUrl",
     )
-    greeks_timestamp: Optional[datetime] = Field(
+    filing_detail_url: Optional[str] = Field(
+        description="The URL to the filing details.",
         default=None,
-        description="Timestamp of the last greeks update."
-        + " Greeks/IV data is updated once per hour.",
-    )
-    last_trade_timestamp: Optional[datetime] = Field(
-        default=None, description="Timestamp of the last trade."
+        alias="filingDetailUrl",
     )
 
-    @field_validator(
-        "last_trade_timestamp",
-        "greeks_timestamp",
-        "ask_timestamp",
-        "bid_timestamp",
-        mode="before",
-        check_fields=False,
-    )
+    @field_validator("report_date", mode="before", check_fields=False)
     @classmethod
-    def validate_dates(cls, v):
-        """Validate the dates."""
-        if v != 0 and v is not None and isinstance(v, int):
-            v = int(v) / 1000  # milliseconds to seconds
-            v = safe_fromtimestamp(v)
-            v = v.replace(microsecond=0)
-            v = v.astimezone(timezone("America/New_York"))
-            return v
-        if v is not None and isinstance(v, str):
-            v = parse(v)
-            v = v.replace(microsecond=0, tzinfo=timezone("UTC"))
-            v = v.astimezone(timezone("America/New_York"))
+    def validate_report_date(cls, v: Optional[Union[str, dateType]]):
+        """Validate report_date."""
+        if isinstance(v, dateType):
             return v
-        return None
-
-    @field_validator("change_percent", mode="before", check_fields=False)
-    @classmethod
-    def normalize_percent(cls, v):
-        """Normalize the percentage."""
-        return float(v) / 100 if v else None
-
-    @field_validator("bid_exchange", "ask_exchange", mode="before", check_fields=False)
-    @classmethod
-    def map_exchange(cls, v):
-        """Map the exchange from a code to a name."""
-        if v:
-            return (
-                OPTIONS_EXCHANGES.get(v, v)
-                if v in OPTIONS_EXCHANGES
-                else STOCK_EXCHANGES.get(v, v)
-            )
-        return None
-
-    @model_validator(mode="before")
-    @classmethod
-    def replace_zero(cls, values):
-        """Check for zero values and replace with None."""
+        v = v if v != "" else None
         return (
-            {
-                k: None if (v == 0 or str(v) == "0") and k != "dte" else v
-                for k, v in values.items()
-            }
-            if isinstance(values, dict)
-            else values
+            datetime.strptime(v, "%Y-%m-%d").date()
+            if v and isinstance(v, str)
+            else None
         )
 
 
-class TradierOptionsChainsFetcher(
-    Fetcher[TradierOptionsChainsQueryParams, List[TradierOptionsChainsData]]
+class SecCompanyFilingsFetcher(
+    Fetcher[SecCompanyFilingsQueryParams, List[SecCompanyFilingsData]]
 ):
-    """Tradier Options Chains Fetcher."""
+    """Transform the query, extract and transform the data from the SEC endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> TradierOptionsChainsQueryParams:
-        """Transform the query parameters."""
-        return TradierOptionsChainsQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> SecCompanyFilingsQueryParams:
+        """Transform query params."""
+        return SecCompanyFilingsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: TradierOptionsChainsQueryParams,
+        query: SecCompanyFilingsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Return the raw data from the Tradier endpoint."""
-        api_key = credentials.get("tradier_api_key") if credentials else ""
-        sandbox = True
-
-        if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
-            raise ValueError(
-                "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
+        """Extract the data from the SEC endpoint."""
+        filings = DataFrame()
+
+        if query.symbol and not query.cik:
+            query.cik = await symbol_map(
+                query.symbol.lower(), use_cache=query.use_cache
             )
+            if not query.cik:
+                raise ValueError(f"CIK not found for symbol {query.symbol}")
+        if query.cik is None:
+            raise ValueError("Error: CIK or symbol must be provided.")
+
+        # The leading 0s need to be inserted but are typically removed from the data to store as an integer.
+        if len(query.cik) != 10:  # type: ignore
+            cik_: str = ""
+            temp = 10 - len(query.cik)  # type: ignore
+            for i in range(temp):
+                cik_ = cik_ + "0"
+            query.cik = cik_ + str(query.cik)  # type: ignore
+
+        url = f"https://data.sec.gov/submissions/CIK{query.cik}.json"
+
+        if query.use_cache is True:
+            cache_dir = f"{get_user_cache_directory()}/http/sec_company_filings"
+            async with CachedSession(
+                cache=SQLiteBackend(cache_dir, expire_after=3600 * 24)
+            ) as session:
+                try:
+                    data = await amake_request(url, headers=HEADERS, session=session)  # type: ignore
+                finally:
+                    await session.close()
+        else:
+            data = await amake_request(url, headers=HEADERS)  # type: ignore
+
+        # This seems to work for the data structure.
+        filings = (
+            DataFrame.from_records(data["filings"].get("recent"))  # type: ignore
+            if "filings" in data
+            else DataFrame()
+        )
+        results = filings.to_dict("records")
 
-        if api_key:
-            sandbox = (
-                credentials.get("tradier_account_type") == "sandbox"
-                if credentials
-                else False
+        # If there are lots of filings, there will be custom pagination.
+        if (
+            (query.limit and len(filings) >= 1000)
+            or query.form_type is not None
+            or query.limit == 0
+        ):
+
+            async def callback(response, session):
+                """Response callback for excess company filings."""
+                result = await response.json()
+                if result:
+                    new_data = DataFrame.from_records(result)
+                    results.extend(new_data.to_dict("records"))
+
+            urls = []
+            new_urls = (
+                DataFrame(data["filings"].get("files"))  # type: ignore
+                if "filings" in data
+                else DataFrame()
             )
+            for i in new_urls.index:
+                new_cik: str = data["filings"]["files"][i]["name"]  # type: ignore
+                new_url: str = "https://data.sec.gov/submissions/" + new_cik
+                urls.append(new_url)
+            if query.use_cache is True:
+                cache_dir = f"{get_user_cache_directory()}/http/sec_company_filings"
+                async with CachedSession(
+                    cache=SQLiteBackend(cache_dir, expire_after=3600 * 24)
+                ) as session:
+                    try:
+                        await amake_requests(urls, headers=HEADERS, session=session, response_callback=callback)  # type: ignore
+                    finally:
+                        await session.close()
+            else:
+                await amake_requests(urls, headers=HEADERS, response_callback=callback)  # type: ignore
 
-        BASE_URL = (
-            "https://api.tradier.com/v1/markets/options/"
-            if sandbox is False
-            else "https://sandbox.tradier.com/v1/markets/options/"
-        )
+        return results
 
-        HEADERS = {
-            "Authorization": f"Bearer {api_key}",
-            "Accept": "application/json",
-        }
-
-        # Get the expiration dates for the symbol so we can gather the chains data.
-        async def get_expirations(symbol):
-            """Get the expiration dates for the given symbol."""
-            url = (
-                f"{BASE_URL}expirations?symbol={symbol}&includeAllRoots=true"
-                "&strikes=false&contractSize=false&expirationType=false"
+    @staticmethod
+    def transform_data(
+        query: SecCompanyFilingsQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[SecCompanyFilingsData]:
+        """Transform the data."""
+        if not data:
+            raise EmptyDataError(
+                f"No filings found for CIK {query.cik}, or symbol {query.symbol}"
             )
-            response = await amake_request(url, headers=HEADERS)
-            if response.get("expirations") and isinstance(response["expirations"].get("date"), list):  # type: ignore
-                expirations = response["expirations"].get("date")  # type: ignore
-                return expirations if expirations else []
-
-        expirations = await get_expirations(query.symbol)
-        if expirations == []:
-            raise ValueError(f"No expiration dates found for {query.symbol}")
-
-        results = []
-
-        async def get_one(url):
-            """Get the chain for a single expiration."""
-            chain = await amake_request(url, headers=HEADERS)
-            if chain.get("options") and isinstance(chain["options"].get("option", []), list):  # type: ignore
-                data = chain["options"]["option"]  # type: ignore
-                for d in data.copy():
-                    # Remove any strikes returned without data.
-                    keys = ["volume", "open_interest", "last", "bid", "ask"]
-                    if all(d.get(key) in [0, "0", None] for key in keys):
-                        data.remove(d)
-                        continue
-                    # Flatten the nested greeks dictionary
-                    greeks = d.pop("greeks")
-                    if greeks is not None:
-                        d.update(**greeks)
-                    # Pop fields that are duplicate information or not of interest.
-                    to_pop = [
-                        "root_symbol",
-                        "exch",
-                        "type",
-                        "expiration_type",
-                        "underlying",
-                        "description",
-                        "average_volume",
-                    ]
-                    _ = [d.pop(key) for key in to_pop if key in d]
-                    # Add the DTE field to the data for easier filtering later.
-                    d["dte"] = (
-                        datetime.strptime(d["expiration_date"], "%Y-%m-%d").date()
-                        - datetime.now().date()
-                    ).days
-
-                results.extend(data)
-
-        urls = [
-            f"{BASE_URL}chains?symbol={query.symbol}&expiration={expiration}&greeks=true"
-            for expiration in expirations  # type: ignore
+        cols = [
+            "reportDate",
+            "filingDate",
+            "acceptanceDateTime",
+            "act",
+            "form",
+            "items",
+            "primaryDocDescription",
+            "primaryDocument",
+            "accessionNumber",
+            "fileNumber",
+            "filmNumber",
+            "isInlineXBRL",
+            "isXBRL",
+            "size",
         ]
+        filings = (
+            DataFrame(data, columns=cols)
+            .fillna(value="N/A")
+            .replace("N/A", None)
+            .astype(str)
+        )
+        filings = filings.sort_values(by=["reportDate", "filingDate"], ascending=False)
+        base_url = f"https://www.sec.gov/Archives/edgar/data/{query.cik}/"
+        filings["primaryDocumentUrl"] = (
+            base_url
+            + filings["accessionNumber"].str.replace("-", "")
+            + "/"
+            + filings["primaryDocument"]
+        )
+        filings["completeSubmissionUrl"] = (
+            base_url + filings["accessionNumber"] + ".txt"
+        )
+        filings["filingDetailUrl"] = (
+            base_url + filings["accessionNumber"] + "-index.htm"
+        )
+        if query.form_type:
+            filings = filings[filings["form"] == query.form_type]
 
-        tasks = [get_one(url) for url in urls]
-
-        await asyncio.gather(*tasks)
+        if query.limit:
+            filings = filings.head(query.limit) if query.limit != 0 else filings
 
-        if not results:
-            raise EmptyDataError(f"No options chains data found for {query.symbol}.")
-        return sorted(
-            results, key=lambda x: [x["expiration_date"], x["strike"], x["symbol"]]
-        )
+        if len(filings) == 0:
+            raise EmptyDataError("No filings were found using the filters provided.")
 
-    @staticmethod
-    def transform_data(
-        query: TradierOptionsChainsQueryParams,
-        data: List[Dict],
-        **kwargs: Any,
-    ) -> List[TradierOptionsChainsData]:
-        """Transform and validate the data."""
-        return [TradierOptionsChainsData.model_validate(d) for d in data]
+        return [
+            SecCompanyFilingsData.model_validate(d) for d in filings.to_dict("records")
+        ]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Trading Economics Economic Calendar Model."""
 
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional, Union
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.economic_calendar import (
     EconomicCalendarData,
     EconomicCalendarQueryParams,
 )
 from openbb_core.provider.utils.helpers import ClientResponse, amake_request, check_item
@@ -27,14 +28,15 @@
     "labour",
     "markets",
     "money",
     "prices",
     "trade",
     "business",
 ]
+TE_COUNTRY_LIMIT = 28
 
 
 class TEEconomicCalendarQueryParams(EconomicCalendarQueryParams):
     """Trading Economics Economic Calendar Query.
 
     Source: https://docs.tradingeconomics.com/economic_calendar/
     """
@@ -44,23 +46,32 @@
     # TODO: Probably want to figure out the list we can use.
     country: Optional[str] = Field(default=None, description="Country of the event.")
     importance: Optional[IMPORTANCE] = Field(
         default=None, description="Importance of the event."
     )
     group: Optional[GROUPS] = Field(default=None, description="Grouping of events")
 
+    _number_of_countries: int = 0
+
     @field_validator("country", mode="before", check_fields=False)
     @classmethod
     def validate_country(cls, c: str):  # pylint: disable=E0213
         """Validate country."""
         result = []
         values = c.replace(" ", "_").split(",")
         for v in values:
             check_item(v.lower(), COUNTRIES)
             result.append(v.lower())
+
+        cls._number_of_countries = len(result)
+        if cls._number_of_countries >= TE_COUNTRY_LIMIT:
+            warn(
+                f"Trading Economics API tend to fail if the number of countries is above {TE_COUNTRY_LIMIT}."
+            )
+
         return ",".join(result)
 
     @field_validator("importance")
     @classmethod
     def importance_to_number(cls, v):
         """Convert importance to number."""
         string_to_value = {"Low": 1, "Medium": 2, "High": 3}
@@ -126,18 +137,22 @@
                 "No url generated. Check combination of input parameters."
             )
         url = f"{url}{api_key}"
 
         async def callback(response: ClientResponse, _: Any) -> Union[dict, List[dict]]:
             """Return the response."""
             if response.status != 200:
-                raise RuntimeError(f"Error in TE request -> {await response.text()}")
+                raise RuntimeError(
+                    f"Error in TE request: \n{await response.text()}"
+                    f"\nInfo -> TE API tend to fail if the number of countries is above {TE_COUNTRY_LIMIT}."
+                )
             return await response.json()
 
         return await amake_request(url, response_callback=callback, **kwargs)
 
+    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: TEEconomicCalendarQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[TEEconomicCalendarData]:
         """Return the transformed data."""
         return [TEEconomicCalendarData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.7.dev202404240009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,74 @@
-"""Yahoo Finance ETF Historical Price Model."""
+"""YFinance Key Executives Model."""
 
-from datetime import datetime
+# pylint: disable=unused-argument
 from typing import Any, Dict, List, Optional
 
-from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.etf_historical import (
-    EtfHistoricalData,
-    EtfHistoricalQueryParams,
+from openbb_core.provider.standard_models.key_executives import (
+    KeyExecutivesData,
+    KeyExecutivesQueryParams,
 )
-from openbb_core.provider.utils.errors import EmptyDataError
-from pandas import Timestamp
-from pydantic import Field, field_validator
+from pydantic import Field
+from yfinance import Ticker
 
-from ..utils.helpers import yf_download
 
+class YFinanceKeyExecutivesQueryParams(KeyExecutivesQueryParams):
+    """YFinance Key Executives Query."""
 
-class YFinanceEtfHistoricalQueryParams(EtfHistoricalQueryParams):
-    """Yahoo Finance ETF Historical Price Query.
 
-    Source: https://finance.yahoo.com/
-    """
-
-
-class YFinanceEtfHistoricalData(EtfHistoricalData):
-    """Yahoo Finance ETF Historical Price Data."""
+class YFinanceKeyExecutivesData(KeyExecutivesData):
+    """YFinance Key Executives Data."""
 
     __alias_dict__ = {
-        "adj_close": "adj close",
+        "year_born": "yearBorn",
+        "fiscal_year": "fiscalYear",
+        "pay": "totalPay",
+        "exercised_value": "exercisedValue",
+        "unexercised_value": "unexercisedValue",
     }
 
-    adj_close: Optional[float] = Field(
+    exercised_value: Optional[int] = Field(
         default=None,
-        description="The adjusted closing price of the ETF.",
+        description="Value of shares exercised.",
+    )
+    unexercised_value: Optional[int] = Field(
+        default=None,
+        description="Value of shares not exercised.",
     )
-
-    @field_validator("date", mode="before", check_fields=False)
-    def date_validate(cls, v):  # pylint: disable=E0213
-        """Return formatted datetime."""
-        if isinstance(v, Timestamp):
-            return v.to_pydatetime()
-        return v
 
 
-class YFinanceEtfHistoricalFetcher(
-    Fetcher[
-        YFinanceEtfHistoricalQueryParams,
-        List[YFinanceEtfHistoricalData],
-    ]
+class YFinanceKeyExecutivesFetcher(
+    Fetcher[YFinanceKeyExecutivesQueryParams, List[YFinanceKeyExecutivesData]]
 ):
-    """Transform the query, extract and transform the data from the Yahoo Finance endpoints."""
+    """YFinance Key Executives Fetcher."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> YFinanceEtfHistoricalQueryParams:
+    def transform_query(params: Dict[str, Any]) -> YFinanceKeyExecutivesQueryParams:
         """Transform the query."""
-        transformed_params = params
-        now = datetime.now().date()
+        return YFinanceKeyExecutivesQueryParams(**params)
 
-        if params.get("start_date") is None:
-            transformed_params["start_date"] = now - relativedelta(years=1)
-
-        if params.get("end_date") is None:
-            transformed_params["end_date"] = now
-
-        return YFinanceEtfHistoricalQueryParams(**params)
-
-    # pylint: disable=unused-argument
     @staticmethod
     def extract_data(
-        query: YFinanceEtfHistoricalQueryParams,
+        query: YFinanceKeyExecutivesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Return the raw data from the Yahoo Finance endpoint."""
-        data = yf_download(
-            symbol=query.symbol,
-            start_date=query.start_date,
-            end_date=query.end_date,
-            keep_adjusted=True,
-        )
-
-        if data.empty:
-            raise EmptyDataError()
-
-        return data.to_dict("records")
+        """Extract the raw data from YFinance."""
+        try:
+            ticker = Ticker(query.symbol).get_info()
+        except Exception as e:
+            raise RuntimeError(f"Error getting data for {query.symbol}: {e}") from e
+        if ticker.get("companyOfficers") is None:
+            raise ValueError(f"No executive data found for {query.symbol}")
+        officers_data = ticker.get("companyOfficers", [])
+        [d.pop("maxAge") for d in officers_data]  # pylint: disable=W0106
+        return officers_data
 
     @staticmethod
     def transform_data(
-        query: YFinanceEtfHistoricalQueryParams,
+        query: YFinanceKeyExecutivesQueryParams,
         data: List[Dict],
         **kwargs: Any,
-    ) -> List[YFinanceEtfHistoricalData]:
-        """Transform the data to the standard format."""
-        return [YFinanceEtfHistoricalData.model_validate(d) for d in data]
+    ) -> List[YFinanceKeyExecutivesData]:
+        """Transform the data."""
+        return [YFinanceKeyExecutivesData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.7.dev202404240009/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202404230010/pyproject.toml` & `openbb_nightly-4.1.7.dev202404240009/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.7.dev202404230010"
+version = "4.1.7.dev202404240009"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
```

### Comparing `openbb_nightly-4.1.7.dev202404230010/PKG-INFO` & `openbb_nightly-4.1.7.dev202404240009/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.7.dev202404230010
+Version: 4.1.7.dev202404240009
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

