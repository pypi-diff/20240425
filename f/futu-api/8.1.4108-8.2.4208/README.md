# Comparing `tmp/futu-api-8.1.4108.tar.gz` & `tmp/futu-api-8.2.4208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futu-api-8.1.4108.tar", last modified: Thu Feb 29 09:38:41 2024, max compression
+gzip compressed data, was "futu-api-8.2.4208.tar", last modified: Thu Apr 25 08:54:35 2024, max compression
```

## Comparing `futu-api-8.1.4108.tar` & `futu-api-8.2.4208.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:41.018836 futu-api-8.1.4108/
--rw-rw-rw-   0        0        0    11547 2023-08-10 06:34:41.000000 futu-api-8.1.4108/LICENSE
--rw-rw-rw-   0        0        0      252 2023-08-10 06:34:41.000000 futu-api-8.1.4108/MANIFEST.in
--rw-rw-rw-   0        0        0     8202 2024-02-29 09:38:41.017839 futu-api-8.1.4108/PKG-INFO
--rw-rw-rw-   0        0        0     7834 2023-08-10 06:34:41.000000 futu-api-8.1.4108/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:40.771498 futu-api-8.1.4108/futu/
--rw-rw-rw-   0        0        0       10 2024-02-21 12:07:36.000000 futu-api-8.1.4108/futu/VERSION.txt
--rw-rw-rw-   0        0        0     4710 2024-02-21 12:07:36.000000 futu-api-8.1.4108/futu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:40.795434 futu-api-8.1.4108/futu/common/
--rw-rw-rw-   0        0        0     2692 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/common/__init__.py
--rw-rw-rw-   0        0        0      805 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/callback_executor.py
--rw-rw-rw-   0        0        0     1152 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/common/comm_add_path.py
--rw-rw-rw-   0        0        0     5086 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/conn_mng.py
--rw-rw-rw-   0        0        0   132132 2023-12-20 07:18:34.000000 futu-api-8.1.4108/futu/common/constant.py
--rw-rw-rw-   0        0        0     1976 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/common/err.py
--rw-rw-rw-   0        0        0     9952 2024-02-21 12:07:36.000000 futu-api-8.1.4108/futu/common/ft_logger.py
--rw-rw-rw-   0        0        0     2975 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/handler_context.py
--rw-rw-rw-   0        0        0    23747 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/network_manager.py
--rw-rw-rw-   0        0        0    19957 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/open_context_base.py
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:40.958996 futu-api-8.1.4108/futu/common/pb/
--rw-rw-rw-   0        0        0    13481 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/pb/Common_pb2.py
--rw-rw-rw-   0        0        0    25388 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/GetDelayStatistics_pb2.py
--rw-rw-rw-   0        0        0    13767 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/GetGlobalState_pb2.py
--rw-rw-rw-   0        0        0    22019 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/GetUserInfo_pb2.py
--rw-rw-rw-   0        0        0    11166 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/InitConnect_pb2.py
--rw-rw-rw-   0        0        0     6626 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/KeepAlive_pb2.py
--rw-rw-rw-   0        0        0    30428 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Notify_pb2.py
--rw-rw-rw-   0        0        0   169999 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_Common_pb2.py
--rw-rw-rw-   0        0        0     7146 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetBasicQot_pb2.py
--rw-rw-rw-   0        0        0     8467 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetBroker_pb2.py
--rw-rw-rw-   0        0        0    11188 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetCapitalDistribution_pb2.py
--rw-rw-rw-   0        0        0    13400 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetCapitalFlow_pb2.py
--rw-rw-rw-   0        0        0    18959 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetCodeChange_pb2.py
--rw-rw-rw-   0        0        0    17426 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetFutureInfo_pb2.py
--rw-rw-rw-   0        0        0    16551 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py
--rw-rw-rw-   0        0        0    10865 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetHistoryKL_pb2.py
--rw-rw-rw-   0        0        0     9174 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetHoldingChangeList_pb2.py
--rw-rw-rw-   0        0        0    27810 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetIpoList_pb2.py
--rw-rw-rw-   0        0        0     8947 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetKL_pb2.py
--rw-rw-rw-   0        0        0     9295 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetMarketState_pb2.py
--rw-rw-rw-   0        0        0    22932 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetOptionChain_pb2.py
--rw-rw-rw-   0        0        0    10514 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py
--rw-rw-rw-   0        0        0    10711 2023-09-12 09:43:38.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetOrderBook_pb2.py
--rw-rw-rw-   0        0        0     9520 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetOwnerPlate_pb2.py
--rw-rw-rw-   0        0        0     8075 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetPlateSecurity_pb2.py
--rw-rw-rw-   0        0        0     7421 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetPlateSet_pb2.py
--rw-rw-rw-   0        0        0    13163 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetPriceReminder_pb2.py
--rw-rw-rw-   0        0        0     7817 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetRT_pb2.py
--rw-rw-rw-   0        0        0     8694 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetReference_pb2.py
--rw-rw-rw-   0        0        0     8850 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetRehab_pb2.py
--rw-rw-rw-   0        0        0    72558 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py
--rw-rw-rw-   0        0        0     8000 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetStaticInfo_pb2.py
--rw-rw-rw-   0        0        0     7839 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetSubInfo_pb2.py
--rw-rw-rw-   0        0        0    11266 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetSuspend_pb2.py
--rw-rw-rw-   0        0        0     8333 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetTicker_pb2.py
--rw-rw-rw-   0        0        0    10050 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py
--rw-rw-rw-   0        0        0     7188 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetUserSecurity_pb2.py
--rw-rw-rw-   0        0        0    40620 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_GetWarrant_pb2.py
--rw-rw-rw-   0        0        0     9055 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_ModifyUserSecurity_pb2.py
--rw-rw-rw-   0        0        0     8221 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_RegQotPush_pb2.py
--rw-rw-rw-   0        0        0    10669 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py
--rw-rw-rw-   0        0        0    11792 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_RequestHistoryKL_pb2.py
--rw-rw-rw-   0        0        0     7136 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_RequestRehab_pb2.py
--rw-rw-rw-   0        0        0    10445 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_RequestTradeDate_pb2.py
--rw-rw-rw-   0        0        0    11483 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_SetPriceReminder_pb2.py
--rw-rw-rw-   0        0        0    73998 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_StockFilter_pb2.py
--rw-rw-rw-   0        0        0     9648 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_Sub_pb2.py
--rw-rw-rw-   0        0        0     4867 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_UpdateBasicQot_pb2.py
--rw-rw-rw-   0        0        0     6226 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_UpdateBroker_pb2.py
--rw-rw-rw-   0        0        0     6377 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_UpdateKL_pb2.py
--rw-rw-rw-   0        0        0     8081 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_UpdateOrderBook_pb2.py
--rw-rw-rw-   0        0        0    10236 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_UpdatePriceReminder_pb2.py
--rw-rw-rw-   0        0        0     5611 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_UpdateRT_pb2.py
--rw-rw-rw-   0        0        0     5701 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Qot_UpdateTicker_pb2.py
--rw-rw-rw-   0        0        0     7294 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/TestCmd_pb2.py
--rw-rw-rw-   0        0        0    88287 2024-02-21 12:07:36.000000 futu-api-8.1.4108/futu/common/pb/Trd_Common_pb2.py
--rw-rw-rw-   0        0        0     7801 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetAccList_pb2.py
--rw-rw-rw-   0        0        0     8288 2023-09-12 09:43:39.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetFunds_pb2.py
--rw-rw-rw-   0        0        0     8515 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py
--rw-rw-rw-   0        0        0     8812 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetHistoryOrderList_pb2.py
--rw-rw-rw-   0        0        0    14671 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetMarginRatio_pb2.py
--rw-rw-rw-   0        0        0    10472 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py
--rw-rw-rw-   0        0        0     8724 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetOrderFillList_pb2.py
--rw-rw-rw-   0        0        0     9003 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetOrderList_pb2.py
--rw-rw-rw-   0        0        0     9550 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_GetPositionList_pb2.py
--rw-rw-rw-   0        0        0    12750 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_ModifyOrder_pb2.py
--rw-rw-rw-   0        0        0     5062 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_Notify_pb2.py
--rw-rw-rw-   0        0        0    13921 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_PlaceOrder_pb2.py
--rw-rw-rw-   0        0        0     8863 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_ReconfirmOrder_pb2.py
--rw-rw-rw-   0        0        0     6398 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_SubAccPush_pb2.py
--rw-rw-rw-   0        0        0     7225 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_UnlockTrade_pb2.py
--rw-rw-rw-   0        0        0     5361 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_UpdateOrderFill_pb2.py
--rw-rw-rw-   0        0        0     5259 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Trd_UpdateOrder_pb2.py
--rw-rw-rw-   0        0        0     6589 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/UsedQuota_pb2.py
--rw-rw-rw-   0        0        0     9329 2023-09-12 09:43:40.000000 futu-api-8.1.4108/futu/common/pb/Verification_pb2.py
--rw-rw-rw-   0        0        0       67 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/common/pb/__init__.py
--rwxrwxrwx   0        0        0      213 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/common/pb/build.bat
--rwxrwxrwx   0        0        0      130 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/common/pb/generate_python.bat
--rw-rw-rw-   0        0        0     4937 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/common/pbjson.py
--rw-rw-rw-   0        0        0     7788 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/sys_config.py
--rw-rw-rw-   0        0        0    26346 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/common/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:40.972959 futu-api-8.1.4108/futu/examples/
--rw-rw-rw-   0        0        0       27 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/examples/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/examples/get_mkt_snapshot_demo.py
--rw-rw-rw-   0        0        0     6608 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/examples/macd_strategy.py
--rw-rw-rw-   0        0        0    12064 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/examples/quote_and_trade_demo.py
--rw-rw-rw-   0        0        0     2866 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/examples/quote_push.py
--rw-rw-rw-   0        0        0     2151 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/examples/simple_filter_demo.py
--rw-rw-rw-   0        0        0     3711 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/examples/stocksell_demo.py
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:40.989913 futu-api-8.1.4108/futu/quote/
--rw-rw-rw-   0        0        0        0 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/quote/__init__.py
--rw-rw-rw-   0        0        0   128201 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/quote/open_quote_context.py
--rw-rw-rw-   0        0        0    17085 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/quote/quote_get_warrant.py
--rw-rw-rw-   0        0        0   132610 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/quote/quote_query.py
--rw-rw-rw-   0        0        0    13186 2023-09-22 07:20:53.000000 futu-api-8.1.4108/futu/quote/quote_response_handler.py
--rw-rw-rw-   0        0        0    31525 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/quote/quote_stockfilter_info.py
--rw-rw-rw-   0        0        0     5172 2023-09-18 06:15:46.000000 futu-api-8.1.4108/futu/quote/quote_tool.py
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:40.998890 futu-api-8.1.4108/futu/tools/
--rw-rw-rw-   0        0        0     7966 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/tools/Common.proto.json
--rw-rw-rw-   0        0        0        0 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/tools/__init__.py
--rw-rw-rw-   0        0        0      354 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/tools/auto_generate.py
--rw-rw-rw-   0        0        0    31193 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/tools/generate_code.py
--rw-rw-rw-   0        0        0     1976 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/tools/load_template.py
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:41.006868 futu-api-8.1.4108/futu/trade/
--rw-rw-rw-   0        0        0        0 2023-08-10 06:34:41.000000 futu-api-8.1.4108/futu/trade/__init__.py
--rw-rw-rw-   0        0        0    39980 2024-02-21 12:07:36.000000 futu-api-8.1.4108/futu/trade/open_trade_context.py
--rw-rw-rw-   0        0        0    36471 2024-02-21 12:07:36.000000 futu-api-8.1.4108/futu/trade/trade_query.py
--rw-rw-rw-   0        0        0     1793 2023-09-22 07:20:53.000000 futu-api-8.1.4108/futu/trade/trade_response_handler.py
-drwxrwxrwx   0        0        0        0 2024-02-29 09:38:41.015843 futu-api-8.1.4108/futu_api.egg-info/
--rw-rw-rw-   0        0        0     8202 2024-02-29 09:38:39.000000 futu-api-8.1.4108/futu_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4301 2024-02-29 09:38:40.000000 futu-api-8.1.4108/futu_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 09:38:39.000000 futu-api-8.1.4108/futu_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-02-29 09:38:39.000000 futu-api-8.1.4108/futu_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-02-29 09:38:39.000000 futu-api-8.1.4108/futu_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       61 2023-08-10 06:34:41.000000 futu-api-8.1.4108/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 09:38:41.018836 futu-api-8.1.4108/setup.cfg
--rw-rw-rw-   0        0        0     1788 2023-08-10 06:34:41.000000 futu-api-8.1.4108/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.951214 futu-api-8.2.4208/
+-rw-rw-rw-   0        0        0    11547 2023-08-10 06:34:41.000000 futu-api-8.2.4208/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-08-10 06:34:41.000000 futu-api-8.2.4208/MANIFEST.in
+-rw-rw-rw-   0        0        0     8202 2024-04-25 08:54:35.951214 futu-api-8.2.4208/PKG-INFO
+-rw-rw-rw-   0        0        0     7834 2023-08-10 06:34:41.000000 futu-api-8.2.4208/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.692905 futu-api-8.2.4208/futu/
+-rw-rw-rw-   0        0        0       10 2024-04-23 07:25:06.000000 futu-api-8.2.4208/futu/VERSION.txt
+-rw-rw-rw-   0        0        0     4710 2024-02-21 12:07:36.000000 futu-api-8.2.4208/futu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.717839 futu-api-8.2.4208/futu/common/
+-rw-rw-rw-   0        0        0     2692 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/common/__init__.py
+-rw-rw-rw-   0        0        0      805 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/common/callback_executor.py
+-rw-rw-rw-   0        0        0     1152 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/common/comm_add_path.py
+-rw-rw-rw-   0        0        0     5086 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/common/conn_mng.py
+-rw-rw-rw-   0        0        0   132539 2024-04-23 09:01:42.000000 futu-api-8.2.4208/futu/common/constant.py
+-rw-rw-rw-   0        0        0     1976 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/common/err.py
+-rw-rw-rw-   0        0        0     9952 2024-02-21 12:07:36.000000 futu-api-8.2.4208/futu/common/ft_logger.py
+-rw-rw-rw-   0        0        0     2975 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/common/handler_context.py
+-rw-rw-rw-   0        0        0    23747 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/common/network_manager.py
+-rw-rw-rw-   0        0        0    19957 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/common/open_context_base.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.890378 futu-api-8.2.4208/futu/common/pb/
+-rw-rw-rw-   0        0        0    13481 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/common/pb/Common_pb2.py
+-rw-rw-rw-   0        0        0    25388 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/GetDelayStatistics_pb2.py
+-rw-rw-rw-   0        0        0    13767 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/GetGlobalState_pb2.py
+-rw-rw-rw-   0        0        0    22019 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/GetUserInfo_pb2.py
+-rw-rw-rw-   0        0        0    11166 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/InitConnect_pb2.py
+-rw-rw-rw-   0        0        0     6626 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/KeepAlive_pb2.py
+-rw-rw-rw-   0        0        0    30428 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Notify_pb2.py
+-rw-rw-rw-   0        0        0   169999 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_Common_pb2.py
+-rw-rw-rw-   0        0        0     7146 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetBasicQot_pb2.py
+-rw-rw-rw-   0        0        0     8467 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetBroker_pb2.py
+-rw-rw-rw-   0        0        0    11188 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetCapitalDistribution_pb2.py
+-rw-rw-rw-   0        0        0    13400 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetCapitalFlow_pb2.py
+-rw-rw-rw-   0        0        0    18959 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetCodeChange_pb2.py
+-rw-rw-rw-   0        0        0    17426 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetFutureInfo_pb2.py
+-rw-rw-rw-   0        0        0    16551 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py
+-rw-rw-rw-   0        0        0    10865 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetHistoryKL_pb2.py
+-rw-rw-rw-   0        0        0     9174 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetHoldingChangeList_pb2.py
+-rw-rw-rw-   0        0        0    27810 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetIpoList_pb2.py
+-rw-rw-rw-   0        0        0     8947 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetKL_pb2.py
+-rw-rw-rw-   0        0        0     9295 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetMarketState_pb2.py
+-rw-rw-rw-   0        0        0    22932 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetOptionChain_pb2.py
+-rw-rw-rw-   0        0        0    10514 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py
+-rw-rw-rw-   0        0        0    10711 2023-09-12 09:43:38.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetOrderBook_pb2.py
+-rw-rw-rw-   0        0        0     9520 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetOwnerPlate_pb2.py
+-rw-rw-rw-   0        0        0     8075 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetPlateSecurity_pb2.py
+-rw-rw-rw-   0        0        0     7421 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetPlateSet_pb2.py
+-rw-rw-rw-   0        0        0    13163 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetPriceReminder_pb2.py
+-rw-rw-rw-   0        0        0     7817 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetRT_pb2.py
+-rw-rw-rw-   0        0        0     8694 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetReference_pb2.py
+-rw-rw-rw-   0        0        0     8850 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetRehab_pb2.py
+-rw-rw-rw-   0        0        0    72558 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py
+-rw-rw-rw-   0        0        0     8000 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetStaticInfo_pb2.py
+-rw-rw-rw-   0        0        0     7839 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetSubInfo_pb2.py
+-rw-rw-rw-   0        0        0    11266 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetSuspend_pb2.py
+-rw-rw-rw-   0        0        0     8333 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetTicker_pb2.py
+-rw-rw-rw-   0        0        0    10050 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py
+-rw-rw-rw-   0        0        0     7188 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetUserSecurity_pb2.py
+-rw-rw-rw-   0        0        0    40620 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_GetWarrant_pb2.py
+-rw-rw-rw-   0        0        0     9055 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_ModifyUserSecurity_pb2.py
+-rw-rw-rw-   0        0        0     8221 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_RegQotPush_pb2.py
+-rw-rw-rw-   0        0        0    10669 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py
+-rw-rw-rw-   0        0        0    11792 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_RequestHistoryKL_pb2.py
+-rw-rw-rw-   0        0        0     7136 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_RequestRehab_pb2.py
+-rw-rw-rw-   0        0        0    10445 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_RequestTradeDate_pb2.py
+-rw-rw-rw-   0        0        0    11483 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_SetPriceReminder_pb2.py
+-rw-rw-rw-   0        0        0    73998 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_StockFilter_pb2.py
+-rw-rw-rw-   0        0        0     9648 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_Sub_pb2.py
+-rw-rw-rw-   0        0        0     4867 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_UpdateBasicQot_pb2.py
+-rw-rw-rw-   0        0        0     6226 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_UpdateBroker_pb2.py
+-rw-rw-rw-   0        0        0     6377 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_UpdateKL_pb2.py
+-rw-rw-rw-   0        0        0     8081 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_UpdateOrderBook_pb2.py
+-rw-rw-rw-   0        0        0    10236 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_UpdatePriceReminder_pb2.py
+-rw-rw-rw-   0        0        0     5611 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_UpdateRT_pb2.py
+-rw-rw-rw-   0        0        0     5701 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Qot_UpdateTicker_pb2.py
+-rw-rw-rw-   0        0        0     7294 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/TestCmd_pb2.py
+-rw-rw-rw-   0        0        0    93961 2024-04-23 09:01:42.000000 futu-api-8.2.4208/futu/common/pb/Trd_Common_pb2.py
+-rw-rw-rw-   0        0        0     7801 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetAccList_pb2.py
+-rw-rw-rw-   0        0        0     8288 2023-09-12 09:43:39.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetFunds_pb2.py
+-rw-rw-rw-   0        0        0     8515 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py
+-rw-rw-rw-   0        0        0     8812 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetHistoryOrderList_pb2.py
+-rw-rw-rw-   0        0        0    14671 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetMarginRatio_pb2.py
+-rw-rw-rw-   0        0        0    11161 2024-04-23 07:25:06.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py
+-rw-rw-rw-   0        0        0     8239 2024-04-23 07:25:06.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetOrderFee_pb2.py
+-rw-rw-rw-   0        0        0     8724 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetOrderFillList_pb2.py
+-rw-rw-rw-   0        0        0     9003 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetOrderList_pb2.py
+-rw-rw-rw-   0        0        0     9550 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_GetPositionList_pb2.py
+-rw-rw-rw-   0        0        0    13899 2024-04-23 07:25:06.000000 futu-api-8.2.4208/futu/common/pb/Trd_ModifyOrder_pb2.py
+-rw-rw-rw-   0        0        0     5062 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_Notify_pb2.py
+-rw-rw-rw-   0        0        0    14672 2024-04-23 07:25:06.000000 futu-api-8.2.4208/futu/common/pb/Trd_PlaceOrder_pb2.py
+-rw-rw-rw-   0        0        0     8863 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_ReconfirmOrder_pb2.py
+-rw-rw-rw-   0        0        0     6398 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_SubAccPush_pb2.py
+-rw-rw-rw-   0        0        0     7225 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_UnlockTrade_pb2.py
+-rw-rw-rw-   0        0        0     5361 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_UpdateOrderFill_pb2.py
+-rw-rw-rw-   0        0        0     5259 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Trd_UpdateOrder_pb2.py
+-rw-rw-rw-   0        0        0     6589 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/UsedQuota_pb2.py
+-rw-rw-rw-   0        0        0     9329 2023-09-12 09:43:40.000000 futu-api-8.2.4208/futu/common/pb/Verification_pb2.py
+-rw-rw-rw-   0        0        0       67 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/common/pb/__init__.py
+-rwxrwxrwx   0        0        0      213 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/common/pb/build.bat
+-rwxrwxrwx   0        0        0      130 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/common/pb/generate_python.bat
+-rw-rw-rw-   0        0        0     4937 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/common/pbjson.py
+-rw-rw-rw-   0        0        0     7788 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/common/sys_config.py
+-rw-rw-rw-   0        0        0    26849 2024-04-23 07:25:06.000000 futu-api-8.2.4208/futu/common/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.906335 futu-api-8.2.4208/futu/examples/
+-rw-rw-rw-   0        0        0       27 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/examples/__init__.py
+-rw-rw-rw-   0        0        0     1785 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/examples/get_mkt_snapshot_demo.py
+-rw-rw-rw-   0        0        0     6608 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/examples/macd_strategy.py
+-rw-rw-rw-   0        0        0    12064 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/examples/quote_and_trade_demo.py
+-rw-rw-rw-   0        0        0     2866 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/examples/quote_push.py
+-rw-rw-rw-   0        0        0     2151 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/examples/simple_filter_demo.py
+-rw-rw-rw-   0        0        0     3711 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/examples/stocksell_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.922292 futu-api-8.2.4208/futu/quote/
+-rw-rw-rw-   0        0        0        0 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/quote/__init__.py
+-rw-rw-rw-   0        0        0   128201 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/quote/open_quote_context.py
+-rw-rw-rw-   0        0        0    17085 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/quote/quote_get_warrant.py
+-rw-rw-rw-   0        0        0   132610 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/quote/quote_query.py
+-rw-rw-rw-   0        0        0    13186 2023-09-22 07:20:53.000000 futu-api-8.2.4208/futu/quote/quote_response_handler.py
+-rw-rw-rw-   0        0        0    31525 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/quote/quote_stockfilter_info.py
+-rw-rw-rw-   0        0        0     5172 2023-09-18 06:15:46.000000 futu-api-8.2.4208/futu/quote/quote_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.933262 futu-api-8.2.4208/futu/tools/
+-rw-rw-rw-   0        0        0     7966 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/tools/Common.proto.json
+-rw-rw-rw-   0        0        0        0 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/tools/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/tools/auto_generate.py
+-rw-rw-rw-   0        0        0    31193 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/tools/generate_code.py
+-rw-rw-rw-   0        0        0     1976 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/tools/load_template.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.940244 futu-api-8.2.4208/futu/trade/
+-rw-rw-rw-   0        0        0        0 2023-08-10 06:34:41.000000 futu-api-8.2.4208/futu/trade/__init__.py
+-rw-rw-rw-   0        0        0    41300 2024-04-23 09:01:42.000000 futu-api-8.2.4208/futu/trade/open_trade_context.py
+-rw-rw-rw-   0        0        0    38362 2024-04-23 09:01:42.000000 futu-api-8.2.4208/futu/trade/trade_query.py
+-rw-rw-rw-   0        0        0     1793 2023-09-22 07:20:53.000000 futu-api-8.2.4208/futu/trade/trade_response_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:54:35.949219 futu-api-8.2.4208/futu_api.egg-info/
+-rw-rw-rw-   0        0        0     8202 2024-04-25 08:54:34.000000 futu-api-8.2.4208/futu_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2024-04-25 08:54:35.000000 futu-api-8.2.4208/futu_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:54:34.000000 futu-api-8.2.4208/futu_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-25 08:54:34.000000 futu-api-8.2.4208/futu_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-25 08:54:34.000000 futu-api-8.2.4208/futu_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       61 2023-08-10 06:34:41.000000 futu-api-8.2.4208/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:54:35.951214 futu-api-8.2.4208/setup.cfg
+-rw-rw-rw-   0        0        0     1788 2023-08-10 06:34:41.000000 futu-api-8.2.4208/setup.py
```

### Comparing `futu-api-8.1.4108/LICENSE` & `futu-api-8.2.4208/LICENSE`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/PKG-INFO` & `futu-api-8.2.4208/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futu-api
-Version: 8.1.4108
+Version: 8.2.4208
 Summary: Futu Quantitative Trading API
 Home-page: https://github.com/FutunnOpen/py-futu-api
 Author: Futu, Inc.
 Author-email: ftdev@futunn.com
 License: Apache License 2.0
 Keywords: Futu HK/US Stock Quant Trading API
 Platform: UNKNOWN
```

### Comparing `futu-api-8.1.4108/README.md` & `futu-api-8.2.4208/README.md`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/__init__.py` & `futu-api-8.2.4208/futu/__init__.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/__init__.py` & `futu-api-8.2.4208/futu/common/__init__.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/callback_executor.py` & `futu-api-8.2.4208/futu/common/callback_executor.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/comm_add_path.py` & `futu-api-8.2.4208/futu/common/comm_add_path.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/conn_mng.py` & `futu-api-8.2.4208/futu/common/conn_mng.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/constant.py` & `futu-api-8.2.4208/futu/common/constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     Trd_GetOrderFillList = 2211  # 获取成交列表
     Trd_UpdateOrderFill = 2218  # 成交通知(推送)
 
     Trd_GetHistoryOrderList = 2221  # 获取历史订单列表
     Trd_GetHistoryOrderFillList = 2222  # 获取历史成交列表
     Trd_GetMaxTrdQtys = 2111    # 查询最大买卖数量
     Trd_GetMarginRatio = 2223  # 获取融资融券数据
+    Trd_GetOrderFee = 2225  # 获取订单费用
 
     # 订阅数据
     Qot_Sub = 3001  # 订阅或者反订阅
     Qot_RegQotPush = 3002  # 注册推送
     Qot_GetSubInfo = 3003  # 获取订阅信息
     Qot_GetBasicQot = 3004  # 获取股票基本行情
     Qot_UpdateBasicQot = 3005  # 推送股票基本行情
@@ -1081,28 +1082,32 @@
     HKCC = "HKCC"  # 香港A股通市场
     FUTURES = "FUTURES"  # 期货市场
     FUTURES_SIMULATE_HK = "FUTURES_SIMULATE_HK"
     FUTURES_SIMULATE_US = "FUTURES_SIMULATE_US"
     FUTURES_SIMULATE_SG = "FUTURES_SIMULATE_SG"
     FUTURES_SIMULATE_JP = "FUTURES_SIMULATE_JP"
     # SG = "SG"
+    HKFUND = "HKFUND"
+    USFUND = "USFUND"
 
     def load_dic(self):
         return {
             self.NONE: Trd_Common_pb2.TrdMarket_Unknown,
             self.HK: Trd_Common_pb2.TrdMarket_HK,
             self.US: Trd_Common_pb2.TrdMarket_US,
             self.CN: Trd_Common_pb2.TrdMarket_CN,
             self.HKCC: Trd_Common_pb2.TrdMarket_HKCC,
             self.FUTURES: Trd_Common_pb2.TrdMarket_Futures,
             # self.SG: Trd_Common_pb2.TrdMarket_SG,
             self.FUTURES_SIMULATE_HK: Trd_Common_pb2.TrdMarket_Futures_Simulate_HK,
             self.FUTURES_SIMULATE_US: Trd_Common_pb2.TrdMarket_Futures_Simulate_US,
             self.FUTURES_SIMULATE_SG: Trd_Common_pb2.TrdMarket_Futures_Simulate_SG,
             self.FUTURES_SIMULATE_JP: Trd_Common_pb2.TrdMarket_Futures_Simulate_JP,
+            self.HKFUND: Trd_Common_pb2.TrdMarket_HK_Fund,
+            self.USFUND: Trd_Common_pb2.TrdMarket_US_Fund,
         }
 
 # 持仓方向
 class PositionSide(FtEnum):
     """
     持仓方向类型定义
     ..  py:class:: PositionSide
@@ -1401,15 +1406,21 @@
     (TrdMarket.HKCC, TrdEnv.REAL): True,
     (TrdMarket.HKCC, TrdEnv.SIMULATE): False,
 
     (TrdMarket.CN, TrdEnv.REAL): False,
     (TrdMarket.CN, TrdEnv.SIMULATE): True,
 
     (TrdMarket.FUTURES, TrdEnv.REAL): True,
-    (TrdMarket.FUTURES, TrdEnv.SIMULATE): True
+    (TrdMarket.FUTURES, TrdEnv.SIMULATE): True,
+
+    (TrdMarket.HKFUND, TrdEnv.REAL): True,
+    (TrdMarket.HKFUND, TrdEnv.SIMULATE): False,
+
+    (TrdMarket.USFUND, TrdEnv.REAL): True,
+    (TrdMarket.USFUND, TrdEnv.SIMULATE): False,
 }
 
 class TRADE(object):
     @staticmethod
     def check_mkt_envtype(trd_mkt, trd_env):
         if (trd_mkt, trd_env) in MKT_ENV_ENABLE_MAP:
             return MKT_ENV_ENABLE_MAP[trd_mkt, trd_env]
```

### Comparing `futu-api-8.1.4108/futu/common/err.py` & `futu-api-8.2.4208/futu/common/err.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/ft_logger.py` & `futu-api-8.2.4208/futu/common/ft_logger.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/handler_context.py` & `futu-api-8.2.4208/futu/common/handler_context.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/network_manager.py` & `futu-api-8.2.4208/futu/common/network_manager.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/open_context_base.py` & `futu-api-8.2.4208/futu/common/open_context_base.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Common_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/GetDelayStatistics_pb2.py` & `futu-api-8.2.4208/futu/common/pb/GetDelayStatistics_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/GetGlobalState_pb2.py` & `futu-api-8.2.4208/futu/common/pb/GetGlobalState_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/GetUserInfo_pb2.py` & `futu-api-8.2.4208/futu/common/pb/GetUserInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/InitConnect_pb2.py` & `futu-api-8.2.4208/futu/common/pb/InitConnect_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/KeepAlive_pb2.py` & `futu-api-8.2.4208/futu/common/pb/KeepAlive_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Notify_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Notify_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_Common_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetBasicQot_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetBasicQot_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetBroker_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetBroker_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetCapitalDistribution_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetCapitalDistribution_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetCapitalFlow_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetCapitalFlow_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetCodeChange_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetCodeChange_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetFutureInfo_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetFutureInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetHistoryKL_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetHistoryKL_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetHoldingChangeList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetHoldingChangeList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetIpoList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetIpoList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetKL_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetKL_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetMarketState_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetMarketState_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetOptionChain_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetOptionChain_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetOrderBook_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetOrderBook_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetOwnerPlate_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetOwnerPlate_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetPlateSecurity_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetPlateSecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetPlateSet_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetPlateSet_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetPriceReminder_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetPriceReminder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetRT_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetRT_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetReference_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetReference_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetRehab_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetRehab_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetStaticInfo_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetStaticInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetSubInfo_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetSubInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetSuspend_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetSuspend_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetTicker_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetTicker_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetUserSecurity_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetUserSecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_GetWarrant_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_GetWarrant_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_ModifyUserSecurity_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_ModifyUserSecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_RegQotPush_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_RegQotPush_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_RequestHistoryKL_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_RequestHistoryKL_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_RequestRehab_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_RequestRehab_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_RequestTradeDate_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_RequestTradeDate_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_SetPriceReminder_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_SetPriceReminder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_StockFilter_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_StockFilter_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_Sub_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_Sub_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_UpdateBasicQot_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_UpdateBasicQot_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_UpdateBroker_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_UpdateBroker_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_UpdateKL_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_UpdateKL_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_UpdateOrderBook_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_UpdateOrderBook_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_UpdatePriceReminder_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_UpdatePriceReminder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_UpdateRT_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_UpdateRT_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Qot_UpdateTicker_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Qot_UpdateTicker_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/TestCmd_pb2.py` & `futu-api-8.2.4208/futu/common/pb/TestCmd_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_Common_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_Common_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Common_pb2 as Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Trd_Common.proto',
   package='Trd_Common',
   syntax='proto2',
-  serialized_pb=_b('\n\x10Trd_Common.proto\x12\nTrd_Common\x1a\x0c\x43ommon.proto\"G\n\x0b\x41\x63\x63\x43\x61shInfo\x12\x10\n\x08\x63urrency\x18\x01 \x01(\x05\x12\x0c\n\x04\x63\x61sh\x18\x02 \x01(\x01\x12\x18\n\x10\x61vailableBalance\x18\x03 \x01(\x01\"=\n\tTrdHeader\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x11\n\ttrdMarket\x18\x03 \x02(\x05\"\xa2\x01\n\x06TrdAcc\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x19\n\x11trdMarketAuthList\x18\x03 \x03(\x05\x12\x0f\n\x07\x61\x63\x63Type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63\x61rdNum\x18\x05 \x01(\t\x12\x14\n\x0csecurityFirm\x18\x06 \x01(\x05\x12\x12\n\nsimAccType\x18\x07 \x01(\x05\x12\x12\n\nuniCardNum\x18\x08 \x01(\t\"\xf3\x04\n\x05\x46unds\x12\r\n\x05power\x18\x01 \x02(\x01\x12\x13\n\x0btotalAssets\x18\x02 \x02(\x01\x12\x0c\n\x04\x63\x61sh\x18\x03 \x02(\x01\x12\x11\n\tmarketVal\x18\x04 \x02(\x01\x12\x12\n\nfrozenCash\x18\x05 \x02(\x01\x12\x10\n\x08\x64\x65\x62tCash\x18\x06 \x02(\x01\x12\x19\n\x11\x61vlWithdrawalCash\x18\x07 \x02(\x01\x12\x10\n\x08\x63urrency\x18\x08 \x01(\x05\x12\x16\n\x0e\x61vailableFunds\x18\t \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\n \x01(\x01\x12\x12\n\nrealizedPL\x18\x0b \x01(\x01\x12\x11\n\triskLevel\x18\x0c \x01(\x05\x12\x15\n\rinitialMargin\x18\r \x01(\x01\x12\x19\n\x11maintenanceMargin\x18\x0e \x01(\x01\x12-\n\x0c\x63\x61shInfoList\x18\x0f \x03(\x0b\x32\x17.Trd_Common.AccCashInfo\x12\x15\n\rmaxPowerShort\x18\x10 \x01(\x01\x12\x14\n\x0cnetCashPower\x18\x11 \x01(\x01\x12\x0e\n\x06longMv\x18\x12 \x01(\x01\x12\x0f\n\x07shortMv\x18\x13 \x01(\x01\x12\x14\n\x0cpendingAsset\x18\x14 \x01(\x01\x12\x15\n\rmaxWithdrawal\x18\x15 \x01(\x01\x12\x12\n\nriskStatus\x18\x16 \x01(\x05\x12\x18\n\x10marginCallMargin\x18\x17 \x01(\x01\x12\r\n\x05isPdt\x18\x18 \x01(\x08\x12\x0e\n\x06pdtSeq\x18\x19 \x01(\t\x12\x15\n\rbeginningDTBP\x18\x1a \x01(\x01\x12\x15\n\rremainingDTBP\x18\x1b \x01(\x01\x12\x14\n\x0c\x64tCallAmount\x18\x1c \x01(\x01\x12\x10\n\x08\x64tStatus\x18\x1d \x01(\x05\"\x95\x03\n\x08Position\x12\x12\n\npositionID\x18\x01 \x02(\x04\x12\x14\n\x0cpositionSide\x18\x02 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x03 \x02(\t\x12\x0c\n\x04name\x18\x04 \x02(\t\x12\x0b\n\x03qty\x18\x05 \x02(\x01\x12\x12\n\ncanSellQty\x18\x06 \x02(\x01\x12\r\n\x05price\x18\x07 \x02(\x01\x12\x11\n\tcostPrice\x18\x08 \x01(\x01\x12\x0b\n\x03val\x18\t \x02(\x01\x12\r\n\x05plVal\x18\n \x02(\x01\x12\x0f\n\x07plRatio\x18\x0b \x01(\x01\x12\x11\n\tsecMarket\x18\x0c \x01(\x05\x12\x10\n\x08td_plVal\x18\x15 \x01(\x01\x12\x11\n\ttd_trdVal\x18\x16 \x01(\x01\x12\x11\n\ttd_buyVal\x18\x17 \x01(\x01\x12\x11\n\ttd_buyQty\x18\x18 \x01(\x01\x12\x12\n\ntd_sellVal\x18\x19 \x01(\x01\x12\x12\n\ntd_sellQty\x18\x1a \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\x1c \x01(\x01\x12\x12\n\nrealizedPL\x18\x1d \x01(\x01\x12\x10\n\x08\x63urrency\x18\x1e \x01(\x05\x12\x11\n\ttrdMarket\x18\x1f \x01(\x05\"\xf4\x03\n\x05Order\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x11\n\torderType\x18\x02 \x02(\x05\x12\x13\n\x0borderStatus\x18\x03 \x02(\x05\x12\x0f\n\x07orderID\x18\x04 \x02(\x04\x12\x11\n\torderIDEx\x18\x05 \x02(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x01(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x12\n\nupdateTime\x18\x0b \x02(\t\x12\x0f\n\x07\x66illQty\x18\x0c \x01(\x01\x12\x14\n\x0c\x66illAvgPrice\x18\r \x01(\x01\x12\x12\n\nlastErrMsg\x18\x0e \x01(\t\x12\x11\n\tsecMarket\x18\x0f \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x10 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x11 \x01(\x01\x12\x0e\n\x06remark\x18\x12 \x01(\t\x12\x13\n\x0btimeInForce\x18\x13 \x01(\x05\x12\x16\n\x0e\x66illOutsideRTH\x18\x14 \x01(\x08\x12\x10\n\x08\x61uxPrice\x18\x15 \x01(\x01\x12\x11\n\ttrailType\x18\x16 \x01(\x05\x12\x12\n\ntrailValue\x18\x17 \x01(\x01\x12\x13\n\x0btrailSpread\x18\x18 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x19 \x01(\x05\x12\x11\n\ttrdMarket\x18\x1a \x01(\x05\"\xb7\x02\n\tOrderFill\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x0e\n\x06\x66illID\x18\x02 \x02(\x04\x12\x10\n\x08\x66illIDEx\x18\x03 \x02(\t\x12\x0f\n\x07orderID\x18\x04 \x01(\x04\x12\x11\n\torderIDEx\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x02(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x17\n\x0f\x63ounterBrokerID\x18\x0b \x01(\x05\x12\x19\n\x11\x63ounterBrokerName\x18\x0c \x01(\t\x12\x11\n\tsecMarket\x18\r \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x0e \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x0f \x01(\x01\x12\x0e\n\x06status\x18\x10 \x01(\x05\"\xb1\x01\n\nMaxTrdQtys\x12\x12\n\nmaxCashBuy\x18\x01 \x02(\x01\x12\x1b\n\x13maxCashAndMarginBuy\x18\x02 \x01(\x01\x12\x17\n\x0fmaxPositionSell\x18\x03 \x02(\x01\x12\x14\n\x0cmaxSellShort\x18\x04 \x01(\x01\x12\x12\n\nmaxBuyBack\x18\x05 \x01(\x01\x12\x16\n\x0elongRequiredIM\x18\x06 \x01(\x01\x12\x17\n\x0fshortRequiredIM\x18\x07 \x01(\x01\"[\n\x13TrdFilterConditions\x12\x10\n\x08\x63odeList\x18\x01 \x03(\t\x12\x0e\n\x06idList\x18\x02 \x03(\x04\x12\x11\n\tbeginTime\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndTime\x18\x04 \x01(\t*.\n\x06TrdEnv\x12\x13\n\x0fTrdEnv_Simulate\x10\x00\x12\x0f\n\x0bTrdEnv_Real\x10\x01*X\n\x0bTrdCategory\x12\x17\n\x13TrdCategory_Unknown\x10\x00\x12\x18\n\x14TrdCategory_Security\x10\x01\x12\x16\n\x12TrdCategory_Future\x10\x02*\xa1\x02\n\tTrdMarket\x12\x15\n\x11TrdMarket_Unknown\x10\x00\x12\x10\n\x0cTrdMarket_HK\x10\x01\x12\x10\n\x0cTrdMarket_US\x10\x02\x12\x10\n\x0cTrdMarket_CN\x10\x03\x12\x12\n\x0eTrdMarket_HKCC\x10\x04\x12\x15\n\x11TrdMarket_Futures\x10\x05\x12\x10\n\x0cTrdMarket_SG\x10\x06\x12!\n\x1dTrdMarket_Futures_Simulate_HK\x10\n\x12!\n\x1dTrdMarket_Futures_Simulate_US\x10\x0b\x12!\n\x1dTrdMarket_Futures_Simulate_SG\x10\x0c\x12!\n\x1dTrdMarket_Futures_Simulate_JP\x10\r*\xac\x01\n\x0cTrdSecMarket\x12\x18\n\x14TrdSecMarket_Unknown\x10\x00\x12\x13\n\x0fTrdSecMarket_HK\x10\x01\x12\x13\n\x0fTrdSecMarket_US\x10\x02\x12\x16\n\x12TrdSecMarket_CN_SH\x10\x1f\x12\x16\n\x12TrdSecMarket_CN_SZ\x10 \x12\x13\n\x0fTrdSecMarket_SG\x10)\x12\x13\n\x0fTrdSecMarket_JP\x10\x33*m\n\x07TrdSide\x12\x13\n\x0fTrdSide_Unknown\x10\x00\x12\x0f\n\x0bTrdSide_Buy\x10\x01\x12\x10\n\x0cTrdSide_Sell\x10\x02\x12\x15\n\x11TrdSide_SellShort\x10\x03\x12\x13\n\x0fTrdSide_BuyBack\x10\x04*\xdb\x03\n\tOrderType\x12\x15\n\x11OrderType_Unknown\x10\x00\x12\x14\n\x10OrderType_Normal\x10\x01\x12\x14\n\x10OrderType_Market\x10\x02\x12\x1b\n\x17OrderType_AbsoluteLimit\x10\x05\x12\x15\n\x11OrderType_Auction\x10\x06\x12\x1a\n\x16OrderType_AuctionLimit\x10\x07\x12\x1a\n\x16OrderType_SpecialLimit\x10\x08\x12\x1e\n\x1aOrderType_SpecialLimit_All\x10\t\x12\x12\n\x0eOrderType_Stop\x10\n\x12\x17\n\x13OrderType_StopLimit\x10\x0b\x12\x1d\n\x19OrderType_MarketifTouched\x10\x0c\x12\x1c\n\x18OrderType_LimitifTouched\x10\r\x12\x1a\n\x16OrderType_TrailingStop\x10\x0e\x12\x1f\n\x1bOrderType_TrailingStopLimit\x10\x0f\x12\x12\n\x0eOrderType_TWAP\x10\x10\x12\x17\n\x13OrderType_TWAPLimit\x10\x11\x12\x12\n\x0eOrderType_VWAP\x10\x12\x12\x17\n\x13OrderType_VWAPLimit\x10\x13*M\n\tTrailType\x12\x15\n\x11TrailType_Unknown\x10\x00\x12\x13\n\x0fTrailType_Ratio\x10\x01\x12\x14\n\x10TrailType_Amount\x10\x02*\xfc\x03\n\x0bOrderStatus\x12\x1b\n\x17OrderStatus_Unsubmitted\x10\x00\x12 \n\x13OrderStatus_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x1d\n\x19OrderStatus_WaitingSubmit\x10\x01\x12\x1a\n\x16OrderStatus_Submitting\x10\x02\x12\x1c\n\x18OrderStatus_SubmitFailed\x10\x03\x12\x17\n\x13OrderStatus_TimeOut\x10\x04\x12\x19\n\x15OrderStatus_Submitted\x10\x05\x12\x1b\n\x17OrderStatus_Filled_Part\x10\n\x12\x1a\n\x16OrderStatus_Filled_All\x10\x0b\x12\x1f\n\x1bOrderStatus_Cancelling_Part\x10\x0c\x12\x1e\n\x1aOrderStatus_Cancelling_All\x10\r\x12\x1e\n\x1aOrderStatus_Cancelled_Part\x10\x0e\x12\x1d\n\x19OrderStatus_Cancelled_All\x10\x0f\x12\x16\n\x12OrderStatus_Failed\x10\x15\x12\x18\n\x14OrderStatus_Disabled\x10\x16\x12\x17\n\x13OrderStatus_Deleted\x10\x17\x12\x1d\n\x19OrderStatus_FillCancelled\x10\x18*e\n\x0fOrderFillStatus\x12\x16\n\x12OrderFillStatus_OK\x10\x00\x12\x1d\n\x19OrderFillStatus_Cancelled\x10\x01\x12\x1b\n\x17OrderFillStatus_Changed\x10\x02*`\n\x0cPositionSide\x12\x15\n\x11PositionSide_Long\x10\x00\x12!\n\x14PositionSide_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x16\n\x12PositionSide_Short\x10\x01*\xad\x01\n\rModifyOrderOp\x12\x19\n\x15ModifyOrderOp_Unknown\x10\x00\x12\x18\n\x14ModifyOrderOp_Normal\x10\x01\x12\x18\n\x14ModifyOrderOp_Cancel\x10\x02\x12\x19\n\x15ModifyOrderOp_Disable\x10\x03\x12\x18\n\x14ModifyOrderOp_Enable\x10\x04\x12\x18\n\x14ModifyOrderOp_Delete\x10\x05*P\n\nTrdAccType\x12\x16\n\x12TrdAccType_Unknown\x10\x00\x12\x13\n\x0fTrdAccType_Cash\x10\x01\x12\x15\n\x11TrdAccType_Margin\x10\x02*\x8c\x01\n\x08\x43urrency\x12\x14\n\x10\x43urrency_Unknown\x10\x00\x12\x10\n\x0c\x43urrency_HKD\x10\x01\x12\x10\n\x0c\x43urrency_USD\x10\x02\x12\x10\n\x0c\x43urrency_CNH\x10\x03\x12\x10\n\x0c\x43urrency_JPY\x10\x04\x12\x10\n\x0c\x43urrency_SGD\x10\x05\x12\x10\n\x0c\x43urrency_AUD\x10\x06*\xb6\x01\n\x0c\x43ltRiskLevel\x12!\n\x14\x43ltRiskLevel_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x43ltRiskLevel_Safe\x10\x00\x12\x18\n\x14\x43ltRiskLevel_Warning\x10\x01\x12\x17\n\x13\x43ltRiskLevel_Danger\x10\x02\x12\x1d\n\x19\x43ltRiskLevel_AbsoluteSafe\x10\x03\x12\x1a\n\x16\x43ltRiskLevel_OptDanger\x10\x04*7\n\x0bTimeInForce\x12\x13\n\x0fTimeInForce_DAY\x10\x00\x12\x13\n\x0fTimeInForce_GTC\x10\x01*\x95\x01\n\x0cSecurityFirm\x12\x18\n\x14SecurityFirm_Unknown\x10\x00\x12\x1f\n\x1bSecurityFirm_FutuSecurities\x10\x01\x12\x18\n\x14SecurityFirm_FutuInc\x10\x02\x12\x17\n\x13SecurityFirm_FutuSG\x10\x03\x12\x17\n\x13SecurityFirm_FutuAU\x10\x04*i\n\nSimAccType\x12\x16\n\x12SimAccType_Unknown\x10\x00\x12\x14\n\x10SimAccType_Stock\x10\x01\x12\x15\n\x11SimAccType_Option\x10\x02\x12\x16\n\x12SimAccType_Futures\x10\x03*\x94\x02\n\rCltRiskStatus\x12\x19\n\x15\x43ltRiskStatus_Unknown\x10\x00\x12\x18\n\x14\x43ltRiskStatus_Level1\x10\x01\x12\x18\n\x14\x43ltRiskStatus_Level2\x10\x02\x12\x18\n\x14\x43ltRiskStatus_Level3\x10\x03\x12\x18\n\x14\x43ltRiskStatus_Level4\x10\x04\x12\x18\n\x14\x43ltRiskStatus_Level5\x10\x05\x12\x18\n\x14\x43ltRiskStatus_Level6\x10\x06\x12\x18\n\x14\x43ltRiskStatus_Level7\x10\x07\x12\x18\n\x14\x43ltRiskStatus_Level8\x10\x08\x12\x18\n\x14\x43ltRiskStatus_Level9\x10\t*b\n\x08\x44TStatus\x12\x14\n\x10\x44TStatus_Unknown\x10\x00\x12\x16\n\x12\x44TStatus_Unlimited\x10\x01\x12\x13\n\x0f\x44TStatus_EMCall\x10\x02\x12\x13\n\x0f\x44TStatus_DTCall\x10\x03\x42@\n\x13\x63om.futu.openapi.pbZ)github.com/futuopen/ftapi4go/pb/trdcommon')
+  serialized_pb=_b('\n\x10Trd_Common.proto\x12\nTrd_Common\x1a\x0c\x43ommon.proto\"G\n\x0b\x41\x63\x63\x43\x61shInfo\x12\x10\n\x08\x63urrency\x18\x01 \x01(\x05\x12\x0c\n\x04\x63\x61sh\x18\x02 \x01(\x01\x12\x18\n\x10\x61vailableBalance\x18\x03 \x01(\x01\"=\n\tTrdHeader\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x11\n\ttrdMarket\x18\x03 \x02(\x05\"\xa2\x01\n\x06TrdAcc\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x19\n\x11trdMarketAuthList\x18\x03 \x03(\x05\x12\x0f\n\x07\x61\x63\x63Type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63\x61rdNum\x18\x05 \x01(\t\x12\x14\n\x0csecurityFirm\x18\x06 \x01(\x05\x12\x12\n\nsimAccType\x18\x07 \x01(\x05\x12\x12\n\nuniCardNum\x18\x08 \x01(\t\"\xb5\x05\n\x05\x46unds\x12\r\n\x05power\x18\x01 \x02(\x01\x12\x13\n\x0btotalAssets\x18\x02 \x02(\x01\x12\x0c\n\x04\x63\x61sh\x18\x03 \x02(\x01\x12\x11\n\tmarketVal\x18\x04 \x02(\x01\x12\x12\n\nfrozenCash\x18\x05 \x02(\x01\x12\x10\n\x08\x64\x65\x62tCash\x18\x06 \x02(\x01\x12\x19\n\x11\x61vlWithdrawalCash\x18\x07 \x02(\x01\x12\x10\n\x08\x63urrency\x18\x08 \x01(\x05\x12\x16\n\x0e\x61vailableFunds\x18\t \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\n \x01(\x01\x12\x12\n\nrealizedPL\x18\x0b \x01(\x01\x12\x11\n\triskLevel\x18\x0c \x01(\x05\x12\x15\n\rinitialMargin\x18\r \x01(\x01\x12\x19\n\x11maintenanceMargin\x18\x0e \x01(\x01\x12-\n\x0c\x63\x61shInfoList\x18\x0f \x03(\x0b\x32\x17.Trd_Common.AccCashInfo\x12\x15\n\rmaxPowerShort\x18\x10 \x01(\x01\x12\x14\n\x0cnetCashPower\x18\x11 \x01(\x01\x12\x0e\n\x06longMv\x18\x12 \x01(\x01\x12\x0f\n\x07shortMv\x18\x13 \x01(\x01\x12\x14\n\x0cpendingAsset\x18\x14 \x01(\x01\x12\x15\n\rmaxWithdrawal\x18\x15 \x01(\x01\x12\x12\n\nriskStatus\x18\x16 \x01(\x05\x12\x18\n\x10marginCallMargin\x18\x17 \x01(\x01\x12\r\n\x05isPdt\x18\x18 \x01(\x08\x12\x0e\n\x06pdtSeq\x18\x19 \x01(\t\x12\x15\n\rbeginningDTBP\x18\x1a \x01(\x01\x12\x15\n\rremainingDTBP\x18\x1b \x01(\x01\x12\x14\n\x0c\x64tCallAmount\x18\x1c \x01(\x01\x12\x10\n\x08\x64tStatus\x18\x1d \x01(\x05\x12\x18\n\x10securitiesAssets\x18\x1e \x01(\x01\x12\x12\n\nfundAssets\x18\x1f \x01(\x01\x12\x12\n\nbondAssets\x18  \x01(\x01\"\x95\x03\n\x08Position\x12\x12\n\npositionID\x18\x01 \x02(\x04\x12\x14\n\x0cpositionSide\x18\x02 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x03 \x02(\t\x12\x0c\n\x04name\x18\x04 \x02(\t\x12\x0b\n\x03qty\x18\x05 \x02(\x01\x12\x12\n\ncanSellQty\x18\x06 \x02(\x01\x12\r\n\x05price\x18\x07 \x02(\x01\x12\x11\n\tcostPrice\x18\x08 \x01(\x01\x12\x0b\n\x03val\x18\t \x02(\x01\x12\r\n\x05plVal\x18\n \x02(\x01\x12\x0f\n\x07plRatio\x18\x0b \x01(\x01\x12\x11\n\tsecMarket\x18\x0c \x01(\x05\x12\x10\n\x08td_plVal\x18\x15 \x01(\x01\x12\x11\n\ttd_trdVal\x18\x16 \x01(\x01\x12\x11\n\ttd_buyVal\x18\x17 \x01(\x01\x12\x11\n\ttd_buyQty\x18\x18 \x01(\x01\x12\x12\n\ntd_sellVal\x18\x19 \x01(\x01\x12\x12\n\ntd_sellQty\x18\x1a \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\x1c \x01(\x01\x12\x12\n\nrealizedPL\x18\x1d \x01(\x01\x12\x10\n\x08\x63urrency\x18\x1e \x01(\x05\x12\x11\n\ttrdMarket\x18\x1f \x01(\x05\"\xf4\x03\n\x05Order\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x11\n\torderType\x18\x02 \x02(\x05\x12\x13\n\x0borderStatus\x18\x03 \x02(\x05\x12\x0f\n\x07orderID\x18\x04 \x02(\x04\x12\x11\n\torderIDEx\x18\x05 \x02(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x01(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x12\n\nupdateTime\x18\x0b \x02(\t\x12\x0f\n\x07\x66illQty\x18\x0c \x01(\x01\x12\x14\n\x0c\x66illAvgPrice\x18\r \x01(\x01\x12\x12\n\nlastErrMsg\x18\x0e \x01(\t\x12\x11\n\tsecMarket\x18\x0f \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x10 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x11 \x01(\x01\x12\x0e\n\x06remark\x18\x12 \x01(\t\x12\x13\n\x0btimeInForce\x18\x13 \x01(\x05\x12\x16\n\x0e\x66illOutsideRTH\x18\x14 \x01(\x08\x12\x10\n\x08\x61uxPrice\x18\x15 \x01(\x01\x12\x11\n\ttrailType\x18\x16 \x01(\x05\x12\x12\n\ntrailValue\x18\x17 \x01(\x01\x12\x13\n\x0btrailSpread\x18\x18 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x19 \x01(\x05\x12\x11\n\ttrdMarket\x18\x1a \x01(\x05\",\n\x0cOrderFeeItem\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"[\n\x08OrderFee\x12\x11\n\torderIDEx\x18\x01 \x02(\t\x12\x11\n\tfeeAmount\x18\x02 \x01(\x01\x12)\n\x07\x66\x65\x65List\x18\x03 \x03(\x0b\x32\x18.Trd_Common.OrderFeeItem\"\xb7\x02\n\tOrderFill\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x0e\n\x06\x66illID\x18\x02 \x02(\x04\x12\x10\n\x08\x66illIDEx\x18\x03 \x02(\t\x12\x0f\n\x07orderID\x18\x04 \x01(\x04\x12\x11\n\torderIDEx\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x02(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x17\n\x0f\x63ounterBrokerID\x18\x0b \x01(\x05\x12\x19\n\x11\x63ounterBrokerName\x18\x0c \x01(\t\x12\x11\n\tsecMarket\x18\r \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x0e \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x0f \x01(\x01\x12\x0e\n\x06status\x18\x10 \x01(\x05\"\xb1\x01\n\nMaxTrdQtys\x12\x12\n\nmaxCashBuy\x18\x01 \x02(\x01\x12\x1b\n\x13maxCashAndMarginBuy\x18\x02 \x01(\x01\x12\x17\n\x0fmaxPositionSell\x18\x03 \x02(\x01\x12\x14\n\x0cmaxSellShort\x18\x04 \x01(\x01\x12\x12\n\nmaxBuyBack\x18\x05 \x01(\x01\x12\x16\n\x0elongRequiredIM\x18\x06 \x01(\x01\x12\x17\n\x0fshortRequiredIM\x18\x07 \x01(\x01\"r\n\x13TrdFilterConditions\x12\x10\n\x08\x63odeList\x18\x01 \x03(\t\x12\x0e\n\x06idList\x18\x02 \x03(\x04\x12\x11\n\tbeginTime\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndTime\x18\x04 \x01(\t\x12\x15\n\rorderIDExList\x18\x05 \x03(\t*.\n\x06TrdEnv\x12\x13\n\x0fTrdEnv_Simulate\x10\x00\x12\x0f\n\x0bTrdEnv_Real\x10\x01*X\n\x0bTrdCategory\x12\x17\n\x13TrdCategory_Unknown\x10\x00\x12\x18\n\x14TrdCategory_Security\x10\x01\x12\x16\n\x12TrdCategory_Future\x10\x02*\xcf\x02\n\tTrdMarket\x12\x15\n\x11TrdMarket_Unknown\x10\x00\x12\x10\n\x0cTrdMarket_HK\x10\x01\x12\x10\n\x0cTrdMarket_US\x10\x02\x12\x10\n\x0cTrdMarket_CN\x10\x03\x12\x12\n\x0eTrdMarket_HKCC\x10\x04\x12\x15\n\x11TrdMarket_Futures\x10\x05\x12\x10\n\x0cTrdMarket_SG\x10\x06\x12!\n\x1dTrdMarket_Futures_Simulate_HK\x10\n\x12!\n\x1dTrdMarket_Futures_Simulate_US\x10\x0b\x12!\n\x1dTrdMarket_Futures_Simulate_SG\x10\x0c\x12!\n\x1dTrdMarket_Futures_Simulate_JP\x10\r\x12\x15\n\x11TrdMarket_HK_Fund\x10q\x12\x15\n\x11TrdMarket_US_Fund\x10{*\xac\x01\n\x0cTrdSecMarket\x12\x18\n\x14TrdSecMarket_Unknown\x10\x00\x12\x13\n\x0fTrdSecMarket_HK\x10\x01\x12\x13\n\x0fTrdSecMarket_US\x10\x02\x12\x16\n\x12TrdSecMarket_CN_SH\x10\x1f\x12\x16\n\x12TrdSecMarket_CN_SZ\x10 \x12\x13\n\x0fTrdSecMarket_SG\x10)\x12\x13\n\x0fTrdSecMarket_JP\x10\x33*m\n\x07TrdSide\x12\x13\n\x0fTrdSide_Unknown\x10\x00\x12\x0f\n\x0bTrdSide_Buy\x10\x01\x12\x10\n\x0cTrdSide_Sell\x10\x02\x12\x15\n\x11TrdSide_SellShort\x10\x03\x12\x13\n\x0fTrdSide_BuyBack\x10\x04*\xdb\x03\n\tOrderType\x12\x15\n\x11OrderType_Unknown\x10\x00\x12\x14\n\x10OrderType_Normal\x10\x01\x12\x14\n\x10OrderType_Market\x10\x02\x12\x1b\n\x17OrderType_AbsoluteLimit\x10\x05\x12\x15\n\x11OrderType_Auction\x10\x06\x12\x1a\n\x16OrderType_AuctionLimit\x10\x07\x12\x1a\n\x16OrderType_SpecialLimit\x10\x08\x12\x1e\n\x1aOrderType_SpecialLimit_All\x10\t\x12\x12\n\x0eOrderType_Stop\x10\n\x12\x17\n\x13OrderType_StopLimit\x10\x0b\x12\x1d\n\x19OrderType_MarketifTouched\x10\x0c\x12\x1c\n\x18OrderType_LimitifTouched\x10\r\x12\x1a\n\x16OrderType_TrailingStop\x10\x0e\x12\x1f\n\x1bOrderType_TrailingStopLimit\x10\x0f\x12\x12\n\x0eOrderType_TWAP\x10\x10\x12\x17\n\x13OrderType_TWAPLimit\x10\x11\x12\x12\n\x0eOrderType_VWAP\x10\x12\x12\x17\n\x13OrderType_VWAPLimit\x10\x13*M\n\tTrailType\x12\x15\n\x11TrailType_Unknown\x10\x00\x12\x13\n\x0fTrailType_Ratio\x10\x01\x12\x14\n\x10TrailType_Amount\x10\x02*\xfc\x03\n\x0bOrderStatus\x12\x1b\n\x17OrderStatus_Unsubmitted\x10\x00\x12 \n\x13OrderStatus_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x1d\n\x19OrderStatus_WaitingSubmit\x10\x01\x12\x1a\n\x16OrderStatus_Submitting\x10\x02\x12\x1c\n\x18OrderStatus_SubmitFailed\x10\x03\x12\x17\n\x13OrderStatus_TimeOut\x10\x04\x12\x19\n\x15OrderStatus_Submitted\x10\x05\x12\x1b\n\x17OrderStatus_Filled_Part\x10\n\x12\x1a\n\x16OrderStatus_Filled_All\x10\x0b\x12\x1f\n\x1bOrderStatus_Cancelling_Part\x10\x0c\x12\x1e\n\x1aOrderStatus_Cancelling_All\x10\r\x12\x1e\n\x1aOrderStatus_Cancelled_Part\x10\x0e\x12\x1d\n\x19OrderStatus_Cancelled_All\x10\x0f\x12\x16\n\x12OrderStatus_Failed\x10\x15\x12\x18\n\x14OrderStatus_Disabled\x10\x16\x12\x17\n\x13OrderStatus_Deleted\x10\x17\x12\x1d\n\x19OrderStatus_FillCancelled\x10\x18*e\n\x0fOrderFillStatus\x12\x16\n\x12OrderFillStatus_OK\x10\x00\x12\x1d\n\x19OrderFillStatus_Cancelled\x10\x01\x12\x1b\n\x17OrderFillStatus_Changed\x10\x02*`\n\x0cPositionSide\x12\x15\n\x11PositionSide_Long\x10\x00\x12!\n\x14PositionSide_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x16\n\x12PositionSide_Short\x10\x01*\xad\x01\n\rModifyOrderOp\x12\x19\n\x15ModifyOrderOp_Unknown\x10\x00\x12\x18\n\x14ModifyOrderOp_Normal\x10\x01\x12\x18\n\x14ModifyOrderOp_Cancel\x10\x02\x12\x19\n\x15ModifyOrderOp_Disable\x10\x03\x12\x18\n\x14ModifyOrderOp_Enable\x10\x04\x12\x18\n\x14ModifyOrderOp_Delete\x10\x05*P\n\nTrdAccType\x12\x16\n\x12TrdAccType_Unknown\x10\x00\x12\x13\n\x0fTrdAccType_Cash\x10\x01\x12\x15\n\x11TrdAccType_Margin\x10\x02*\x8c\x01\n\x08\x43urrency\x12\x14\n\x10\x43urrency_Unknown\x10\x00\x12\x10\n\x0c\x43urrency_HKD\x10\x01\x12\x10\n\x0c\x43urrency_USD\x10\x02\x12\x10\n\x0c\x43urrency_CNH\x10\x03\x12\x10\n\x0c\x43urrency_JPY\x10\x04\x12\x10\n\x0c\x43urrency_SGD\x10\x05\x12\x10\n\x0c\x43urrency_AUD\x10\x06*\xb6\x01\n\x0c\x43ltRiskLevel\x12!\n\x14\x43ltRiskLevel_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x43ltRiskLevel_Safe\x10\x00\x12\x18\n\x14\x43ltRiskLevel_Warning\x10\x01\x12\x17\n\x13\x43ltRiskLevel_Danger\x10\x02\x12\x1d\n\x19\x43ltRiskLevel_AbsoluteSafe\x10\x03\x12\x1a\n\x16\x43ltRiskLevel_OptDanger\x10\x04*7\n\x0bTimeInForce\x12\x13\n\x0fTimeInForce_DAY\x10\x00\x12\x13\n\x0fTimeInForce_GTC\x10\x01*\x95\x01\n\x0cSecurityFirm\x12\x18\n\x14SecurityFirm_Unknown\x10\x00\x12\x1f\n\x1bSecurityFirm_FutuSecurities\x10\x01\x12\x18\n\x14SecurityFirm_FutuInc\x10\x02\x12\x17\n\x13SecurityFirm_FutuSG\x10\x03\x12\x17\n\x13SecurityFirm_FutuAU\x10\x04*i\n\nSimAccType\x12\x16\n\x12SimAccType_Unknown\x10\x00\x12\x14\n\x10SimAccType_Stock\x10\x01\x12\x15\n\x11SimAccType_Option\x10\x02\x12\x16\n\x12SimAccType_Futures\x10\x03*\x94\x02\n\rCltRiskStatus\x12\x19\n\x15\x43ltRiskStatus_Unknown\x10\x00\x12\x18\n\x14\x43ltRiskStatus_Level1\x10\x01\x12\x18\n\x14\x43ltRiskStatus_Level2\x10\x02\x12\x18\n\x14\x43ltRiskStatus_Level3\x10\x03\x12\x18\n\x14\x43ltRiskStatus_Level4\x10\x04\x12\x18\n\x14\x43ltRiskStatus_Level5\x10\x05\x12\x18\n\x14\x43ltRiskStatus_Level6\x10\x06\x12\x18\n\x14\x43ltRiskStatus_Level7\x10\x07\x12\x18\n\x14\x43ltRiskStatus_Level8\x10\x08\x12\x18\n\x14\x43ltRiskStatus_Level9\x10\t*b\n\x08\x44TStatus\x12\x14\n\x10\x44TStatus_Unknown\x10\x00\x12\x16\n\x12\x44TStatus_Unlimited\x10\x01\x12\x13\n\x0f\x44TStatus_EMCall\x10\x02\x12\x13\n\x0f\x44TStatus_DTCall\x10\x03\x42@\n\x13\x63om.futu.openapi.pbZ)github.com/futuopen/ftapi4go/pb/trdcommon')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,])
 
 _TRDENV = _descriptor.EnumDescriptor(
   name='TrdEnv',
   full_name='Trd_Common.TrdEnv',
   filename=None,
@@ -38,16 +38,16 @@
     _descriptor.EnumValueDescriptor(
       name='TrdEnv_Real', index=1, number=1,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=2475,
-  serialized_end=2521,
+  serialized_start=2703,
+  serialized_end=2749,
 )
 _sym_db.RegisterEnumDescriptor(_TRDENV)
 
 TrdEnv = enum_type_wrapper.EnumTypeWrapper(_TRDENV)
 _TRDCATEGORY = _descriptor.EnumDescriptor(
   name='TrdCategory',
   full_name='Trd_Common.TrdCategory',
@@ -65,16 +65,16 @@
     _descriptor.EnumValueDescriptor(
       name='TrdCategory_Future', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=2523,
-  serialized_end=2611,
+  serialized_start=2751,
+  serialized_end=2839,
 )
 _sym_db.RegisterEnumDescriptor(_TRDCATEGORY)
 
 TrdCategory = enum_type_wrapper.EnumTypeWrapper(_TRDCATEGORY)
 _TRDMARKET = _descriptor.EnumDescriptor(
   name='TrdMarket',
   full_name='Trd_Common.TrdMarket',
@@ -121,19 +121,27 @@
       name='TrdMarket_Futures_Simulate_SG', index=9, number=12,
       options=None,
       type=None),
     _descriptor.EnumValueDescriptor(
       name='TrdMarket_Futures_Simulate_JP', index=10, number=13,
       options=None,
       type=None),
+    _descriptor.EnumValueDescriptor(
+      name='TrdMarket_HK_Fund', index=11, number=113,
+      options=None,
+      type=None),
+    _descriptor.EnumValueDescriptor(
+      name='TrdMarket_US_Fund', index=12, number=123,
+      options=None,
+      type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=2614,
-  serialized_end=2903,
+  serialized_start=2842,
+  serialized_end=3177,
 )
 _sym_db.RegisterEnumDescriptor(_TRDMARKET)
 
 TrdMarket = enum_type_wrapper.EnumTypeWrapper(_TRDMARKET)
 _TRDSECMARKET = _descriptor.EnumDescriptor(
   name='TrdSecMarket',
   full_name='Trd_Common.TrdSecMarket',
@@ -167,16 +175,16 @@
     _descriptor.EnumValueDescriptor(
       name='TrdSecMarket_JP', index=6, number=51,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=2906,
-  serialized_end=3078,
+  serialized_start=3180,
+  serialized_end=3352,
 )
 _sym_db.RegisterEnumDescriptor(_TRDSECMARKET)
 
 TrdSecMarket = enum_type_wrapper.EnumTypeWrapper(_TRDSECMARKET)
 _TRDSIDE = _descriptor.EnumDescriptor(
   name='TrdSide',
   full_name='Trd_Common.TrdSide',
@@ -202,16 +210,16 @@
     _descriptor.EnumValueDescriptor(
       name='TrdSide_BuyBack', index=4, number=4,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=3080,
-  serialized_end=3189,
+  serialized_start=3354,
+  serialized_end=3463,
 )
 _sym_db.RegisterEnumDescriptor(_TRDSIDE)
 
 TrdSide = enum_type_wrapper.EnumTypeWrapper(_TRDSIDE)
 _ORDERTYPE = _descriptor.EnumDescriptor(
   name='OrderType',
   full_name='Trd_Common.OrderType',
@@ -289,16 +297,16 @@
     _descriptor.EnumValueDescriptor(
       name='OrderType_VWAPLimit', index=17, number=19,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=3192,
-  serialized_end=3667,
+  serialized_start=3466,
+  serialized_end=3941,
 )
 _sym_db.RegisterEnumDescriptor(_ORDERTYPE)
 
 OrderType = enum_type_wrapper.EnumTypeWrapper(_ORDERTYPE)
 _TRAILTYPE = _descriptor.EnumDescriptor(
   name='TrailType',
   full_name='Trd_Common.TrailType',
@@ -316,16 +324,16 @@
     _descriptor.EnumValueDescriptor(
       name='TrailType_Amount', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=3669,
-  serialized_end=3746,
+  serialized_start=3943,
+  serialized_end=4020,
 )
 _sym_db.RegisterEnumDescriptor(_TRAILTYPE)
 
 TrailType = enum_type_wrapper.EnumTypeWrapper(_TRAILTYPE)
 _ORDERSTATUS = _descriptor.EnumDescriptor(
   name='OrderStatus',
   full_name='Trd_Common.OrderStatus',
@@ -399,16 +407,16 @@
     _descriptor.EnumValueDescriptor(
       name='OrderStatus_FillCancelled', index=16, number=24,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=3749,
-  serialized_end=4257,
+  serialized_start=4023,
+  serialized_end=4531,
 )
 _sym_db.RegisterEnumDescriptor(_ORDERSTATUS)
 
 OrderStatus = enum_type_wrapper.EnumTypeWrapper(_ORDERSTATUS)
 _ORDERFILLSTATUS = _descriptor.EnumDescriptor(
   name='OrderFillStatus',
   full_name='Trd_Common.OrderFillStatus',
@@ -426,16 +434,16 @@
     _descriptor.EnumValueDescriptor(
       name='OrderFillStatus_Changed', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4259,
-  serialized_end=4360,
+  serialized_start=4533,
+  serialized_end=4634,
 )
 _sym_db.RegisterEnumDescriptor(_ORDERFILLSTATUS)
 
 OrderFillStatus = enum_type_wrapper.EnumTypeWrapper(_ORDERFILLSTATUS)
 _POSITIONSIDE = _descriptor.EnumDescriptor(
   name='PositionSide',
   full_name='Trd_Common.PositionSide',
@@ -453,16 +461,16 @@
     _descriptor.EnumValueDescriptor(
       name='PositionSide_Short', index=2, number=1,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4362,
-  serialized_end=4458,
+  serialized_start=4636,
+  serialized_end=4732,
 )
 _sym_db.RegisterEnumDescriptor(_POSITIONSIDE)
 
 PositionSide = enum_type_wrapper.EnumTypeWrapper(_POSITIONSIDE)
 _MODIFYORDEROP = _descriptor.EnumDescriptor(
   name='ModifyOrderOp',
   full_name='Trd_Common.ModifyOrderOp',
@@ -492,16 +500,16 @@
     _descriptor.EnumValueDescriptor(
       name='ModifyOrderOp_Delete', index=5, number=5,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4461,
-  serialized_end=4634,
+  serialized_start=4735,
+  serialized_end=4908,
 )
 _sym_db.RegisterEnumDescriptor(_MODIFYORDEROP)
 
 ModifyOrderOp = enum_type_wrapper.EnumTypeWrapper(_MODIFYORDEROP)
 _TRDACCTYPE = _descriptor.EnumDescriptor(
   name='TrdAccType',
   full_name='Trd_Common.TrdAccType',
@@ -519,16 +527,16 @@
     _descriptor.EnumValueDescriptor(
       name='TrdAccType_Margin', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4636,
-  serialized_end=4716,
+  serialized_start=4910,
+  serialized_end=4990,
 )
 _sym_db.RegisterEnumDescriptor(_TRDACCTYPE)
 
 TrdAccType = enum_type_wrapper.EnumTypeWrapper(_TRDACCTYPE)
 _CURRENCY = _descriptor.EnumDescriptor(
   name='Currency',
   full_name='Trd_Common.Currency',
@@ -562,16 +570,16 @@
     _descriptor.EnumValueDescriptor(
       name='Currency_AUD', index=6, number=6,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4719,
-  serialized_end=4859,
+  serialized_start=4993,
+  serialized_end=5133,
 )
 _sym_db.RegisterEnumDescriptor(_CURRENCY)
 
 Currency = enum_type_wrapper.EnumTypeWrapper(_CURRENCY)
 _CLTRISKLEVEL = _descriptor.EnumDescriptor(
   name='CltRiskLevel',
   full_name='Trd_Common.CltRiskLevel',
@@ -601,16 +609,16 @@
     _descriptor.EnumValueDescriptor(
       name='CltRiskLevel_OptDanger', index=5, number=4,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4862,
-  serialized_end=5044,
+  serialized_start=5136,
+  serialized_end=5318,
 )
 _sym_db.RegisterEnumDescriptor(_CLTRISKLEVEL)
 
 CltRiskLevel = enum_type_wrapper.EnumTypeWrapper(_CLTRISKLEVEL)
 _TIMEINFORCE = _descriptor.EnumDescriptor(
   name='TimeInForce',
   full_name='Trd_Common.TimeInForce',
@@ -624,16 +632,16 @@
     _descriptor.EnumValueDescriptor(
       name='TimeInForce_GTC', index=1, number=1,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5046,
-  serialized_end=5101,
+  serialized_start=5320,
+  serialized_end=5375,
 )
 _sym_db.RegisterEnumDescriptor(_TIMEINFORCE)
 
 TimeInForce = enum_type_wrapper.EnumTypeWrapper(_TIMEINFORCE)
 _SECURITYFIRM = _descriptor.EnumDescriptor(
   name='SecurityFirm',
   full_name='Trd_Common.SecurityFirm',
@@ -659,16 +667,16 @@
     _descriptor.EnumValueDescriptor(
       name='SecurityFirm_FutuAU', index=4, number=4,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5104,
-  serialized_end=5253,
+  serialized_start=5378,
+  serialized_end=5527,
 )
 _sym_db.RegisterEnumDescriptor(_SECURITYFIRM)
 
 SecurityFirm = enum_type_wrapper.EnumTypeWrapper(_SECURITYFIRM)
 _SIMACCTYPE = _descriptor.EnumDescriptor(
   name='SimAccType',
   full_name='Trd_Common.SimAccType',
@@ -690,16 +698,16 @@
     _descriptor.EnumValueDescriptor(
       name='SimAccType_Futures', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5255,
-  serialized_end=5360,
+  serialized_start=5529,
+  serialized_end=5634,
 )
 _sym_db.RegisterEnumDescriptor(_SIMACCTYPE)
 
 SimAccType = enum_type_wrapper.EnumTypeWrapper(_SIMACCTYPE)
 _CLTRISKSTATUS = _descriptor.EnumDescriptor(
   name='CltRiskStatus',
   full_name='Trd_Common.CltRiskStatus',
@@ -745,16 +753,16 @@
     _descriptor.EnumValueDescriptor(
       name='CltRiskStatus_Level9', index=9, number=9,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5363,
-  serialized_end=5639,
+  serialized_start=5637,
+  serialized_end=5913,
 )
 _sym_db.RegisterEnumDescriptor(_CLTRISKSTATUS)
 
 CltRiskStatus = enum_type_wrapper.EnumTypeWrapper(_CLTRISKSTATUS)
 _DTSTATUS = _descriptor.EnumDescriptor(
   name='DTStatus',
   full_name='Trd_Common.DTStatus',
@@ -776,16 +784,16 @@
     _descriptor.EnumValueDescriptor(
       name='DTStatus_DTCall', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5641,
-  serialized_end=5739,
+  serialized_start=5915,
+  serialized_end=6013,
 )
 _sym_db.RegisterEnumDescriptor(_DTSTATUS)
 
 DTStatus = enum_type_wrapper.EnumTypeWrapper(_DTSTATUS)
 TrdEnv_Simulate = 0
 TrdEnv_Real = 1
 TrdCategory_Unknown = 0
@@ -798,14 +806,16 @@
 TrdMarket_HKCC = 4
 TrdMarket_Futures = 5
 TrdMarket_SG = 6
 TrdMarket_Futures_Simulate_HK = 10
 TrdMarket_Futures_Simulate_US = 11
 TrdMarket_Futures_Simulate_SG = 12
 TrdMarket_Futures_Simulate_JP = 13
+TrdMarket_HK_Fund = 113
+TrdMarket_US_Fund = 123
 TrdSecMarket_Unknown = 0
 TrdSecMarket_HK = 1
 TrdSecMarket_US = 2
 TrdSecMarket_CN_SH = 31
 TrdSecMarket_CN_SZ = 32
 TrdSecMarket_SG = 41
 TrdSecMarket_JP = 51
@@ -1284,28 +1294,49 @@
     _descriptor.FieldDescriptor(
       name='dtStatus', full_name='Trd_Common.Funds.dtStatus', index=28,
       number=29, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='securitiesAssets', full_name='Trd_Common.Funds.securitiesAssets', index=29,
+      number=30, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='fundAssets', full_name='Trd_Common.Funds.fundAssets', index=30,
+      number=31, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='bondAssets', full_name='Trd_Common.Funds.bondAssets', index=31,
+      number=32, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=348,
-  serialized_end=975,
+  serialized_end=1041,
 )
 
 
 _POSITION = _descriptor.Descriptor(
   name='Position',
   full_name='Trd_Common.Position',
   filename=None,
@@ -1474,16 +1505,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=978,
-  serialized_end=1383,
+  serialized_start=1044,
+  serialized_end=1449,
 )
 
 
 _ORDER = _descriptor.Descriptor(
   name='Order',
   full_name='Trd_Common.Order',
   filename=None,
@@ -1680,16 +1711,99 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1386,
-  serialized_end=1886,
+  serialized_start=1452,
+  serialized_end=1952,
+)
+
+
+_ORDERFEEITEM = _descriptor.Descriptor(
+  name='OrderFeeItem',
+  full_name='Trd_Common.OrderFeeItem',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='title', full_name='Trd_Common.OrderFeeItem.title', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='Trd_Common.OrderFeeItem.value', index=1,
+      number=2, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1954,
+  serialized_end=1998,
+)
+
+
+_ORDERFEE = _descriptor.Descriptor(
+  name='OrderFee',
+  full_name='Trd_Common.OrderFee',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='orderIDEx', full_name='Trd_Common.OrderFee.orderIDEx', index=0,
+      number=1, type=9, cpp_type=9, label=2,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='feeAmount', full_name='Trd_Common.OrderFee.feeAmount', index=1,
+      number=2, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='feeList', full_name='Trd_Common.OrderFee.feeList', index=2,
+      number=3, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2000,
+  serialized_end=2091,
 )
 
 
 _ORDERFILL = _descriptor.Descriptor(
   name='OrderFill',
   full_name='Trd_Common.OrderFill',
   filename=None,
@@ -1816,16 +1930,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1889,
-  serialized_end=2200,
+  serialized_start=2094,
+  serialized_end=2405,
 )
 
 
 _MAXTRDQTYS = _descriptor.Descriptor(
   name='MaxTrdQtys',
   full_name='Trd_Common.MaxTrdQtys',
   filename=None,
@@ -1889,16 +2003,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2203,
-  serialized_end=2380,
+  serialized_start=2408,
+  serialized_end=2585,
 )
 
 
 _TRDFILTERCONDITIONS = _descriptor.Descriptor(
   name='TrdFilterConditions',
   full_name='Trd_Common.TrdFilterConditions',
   filename=None,
@@ -1929,37 +2043,47 @@
     _descriptor.FieldDescriptor(
       name='endTime', full_name='Trd_Common.TrdFilterConditions.endTime', index=3,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderIDExList', full_name='Trd_Common.TrdFilterConditions.orderIDExList', index=4,
+      number=5, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2382,
-  serialized_end=2473,
+  serialized_start=2587,
+  serialized_end=2701,
 )
 
 _FUNDS.fields_by_name['cashInfoList'].message_type = _ACCCASHINFO
+_ORDERFEE.fields_by_name['feeList'].message_type = _ORDERFEEITEM
 DESCRIPTOR.message_types_by_name['AccCashInfo'] = _ACCCASHINFO
 DESCRIPTOR.message_types_by_name['TrdHeader'] = _TRDHEADER
 DESCRIPTOR.message_types_by_name['TrdAcc'] = _TRDACC
 DESCRIPTOR.message_types_by_name['Funds'] = _FUNDS
 DESCRIPTOR.message_types_by_name['Position'] = _POSITION
 DESCRIPTOR.message_types_by_name['Order'] = _ORDER
+DESCRIPTOR.message_types_by_name['OrderFeeItem'] = _ORDERFEEITEM
+DESCRIPTOR.message_types_by_name['OrderFee'] = _ORDERFEE
 DESCRIPTOR.message_types_by_name['OrderFill'] = _ORDERFILL
 DESCRIPTOR.message_types_by_name['MaxTrdQtys'] = _MAXTRDQTYS
 DESCRIPTOR.message_types_by_name['TrdFilterConditions'] = _TRDFILTERCONDITIONS
 DESCRIPTOR.enum_types_by_name['TrdEnv'] = _TRDENV
 DESCRIPTOR.enum_types_by_name['TrdCategory'] = _TRDCATEGORY
 DESCRIPTOR.enum_types_by_name['TrdMarket'] = _TRDMARKET
 DESCRIPTOR.enum_types_by_name['TrdSecMarket'] = _TRDSECMARKET
@@ -2018,14 +2142,28 @@
 Order = _reflection.GeneratedProtocolMessageType('Order', (_message.Message,), dict(
   DESCRIPTOR = _ORDER,
   __module__ = 'Trd_Common_pb2'
   # @@protoc_insertion_point(class_scope:Trd_Common.Order)
   ))
 _sym_db.RegisterMessage(Order)
 
+OrderFeeItem = _reflection.GeneratedProtocolMessageType('OrderFeeItem', (_message.Message,), dict(
+  DESCRIPTOR = _ORDERFEEITEM,
+  __module__ = 'Trd_Common_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_Common.OrderFeeItem)
+  ))
+_sym_db.RegisterMessage(OrderFeeItem)
+
+OrderFee = _reflection.GeneratedProtocolMessageType('OrderFee', (_message.Message,), dict(
+  DESCRIPTOR = _ORDERFEE,
+  __module__ = 'Trd_Common_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_Common.OrderFee)
+  ))
+_sym_db.RegisterMessage(OrderFee)
+
 OrderFill = _reflection.GeneratedProtocolMessageType('OrderFill', (_message.Message,), dict(
   DESCRIPTOR = _ORDERFILL,
   __module__ = 'Trd_Common_pb2'
   # @@protoc_insertion_point(class_scope:Trd_Common.OrderFill)
   ))
 _sym_db.RegisterMessage(OrderFill)
```

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetAccList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetAccList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetFunds_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetFunds_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetHistoryOrderList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetHistoryOrderList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetMarginRatio_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetMarginRatio_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,273 +1,280 @@
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: Trd_GetMaxTrdQtys.proto
-
-import sys
-_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf import descriptor_pb2
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-import Common_pb2 as Common__pb2
-import Trd_Common_pb2 as Trd__Common__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='Trd_GetMaxTrdQtys.proto',
-  package='Trd_GetMaxTrdQtys',
-  syntax='proto2',
-  serialized_pb=_b('\n\x17Trd_GetMaxTrdQtys.proto\x12\x11Trd_GetMaxTrdQtys\x1a\x0c\x43ommon.proto\x1a\x10Trd_Common.proto\"\xb1\x01\n\x03\x43\x32S\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x11\n\torderType\x18\x02 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x03 \x02(\t\x12\r\n\x05price\x18\x04 \x02(\x01\x12\x0f\n\x07orderID\x18\x05 \x01(\x04\x12\x13\n\x0b\x61\x64justPrice\x18\x06 \x01(\x08\x12\x1a\n\x12\x61\x64justSideAndLimit\x18\x07 \x01(\x01\x12\x11\n\tsecMarket\x18\x08 \x01(\x05\"X\n\x03S2C\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12*\n\nmaxTrdQtys\x18\x02 \x01(\x0b\x32\x16.Trd_Common.MaxTrdQtys\".\n\x07Request\x12#\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x16.Trd_GetMaxTrdQtys.C2S\"g\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12#\n\x03s2c\x18\x04 \x01(\x0b\x32\x16.Trd_GetMaxTrdQtys.S2CBG\n\x13\x63om.futu.openapi.pbZ0github.com/futuopen/ftapi4go/pb/trdgetmaxtrdqtys')
-  ,
-  dependencies=[Common__pb2.DESCRIPTOR,Trd__Common__pb2.DESCRIPTOR,])
-
-
-
-
-_C2S = _descriptor.Descriptor(
-  name='C2S',
-  full_name='Trd_GetMaxTrdQtys.C2S',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='header', full_name='Trd_GetMaxTrdQtys.C2S.header', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='orderType', full_name='Trd_GetMaxTrdQtys.C2S.orderType', index=1,
-      number=2, type=5, cpp_type=1, label=2,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='code', full_name='Trd_GetMaxTrdQtys.C2S.code', index=2,
-      number=3, type=9, cpp_type=9, label=2,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='price', full_name='Trd_GetMaxTrdQtys.C2S.price', index=3,
-      number=4, type=1, cpp_type=5, label=2,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='orderID', full_name='Trd_GetMaxTrdQtys.C2S.orderID', index=4,
-      number=5, type=4, cpp_type=4, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='adjustPrice', full_name='Trd_GetMaxTrdQtys.C2S.adjustPrice', index=5,
-      number=6, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='adjustSideAndLimit', full_name='Trd_GetMaxTrdQtys.C2S.adjustSideAndLimit', index=6,
-      number=7, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='secMarket', full_name='Trd_GetMaxTrdQtys.C2S.secMarket', index=7,
-      number=8, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=79,
-  serialized_end=256,
-)
-
-
-_S2C = _descriptor.Descriptor(
-  name='S2C',
-  full_name='Trd_GetMaxTrdQtys.S2C',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='header', full_name='Trd_GetMaxTrdQtys.S2C.header', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='maxTrdQtys', full_name='Trd_GetMaxTrdQtys.S2C.maxTrdQtys', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=258,
-  serialized_end=346,
-)
-
-
-_REQUEST = _descriptor.Descriptor(
-  name='Request',
-  full_name='Trd_GetMaxTrdQtys.Request',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='c2s', full_name='Trd_GetMaxTrdQtys.Request.c2s', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=348,
-  serialized_end=394,
-)
-
-
-_RESPONSE = _descriptor.Descriptor(
-  name='Response',
-  full_name='Trd_GetMaxTrdQtys.Response',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='retType', full_name='Trd_GetMaxTrdQtys.Response.retType', index=0,
-      number=1, type=5, cpp_type=1, label=2,
-      has_default_value=True, default_value=-400,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='retMsg', full_name='Trd_GetMaxTrdQtys.Response.retMsg', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='errCode', full_name='Trd_GetMaxTrdQtys.Response.errCode', index=2,
-      number=3, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='s2c', full_name='Trd_GetMaxTrdQtys.Response.s2c', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=396,
-  serialized_end=499,
-)
-
-_C2S.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
-_S2C.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
-_S2C.fields_by_name['maxTrdQtys'].message_type = Trd__Common__pb2._MAXTRDQTYS
-_REQUEST.fields_by_name['c2s'].message_type = _C2S
-_RESPONSE.fields_by_name['s2c'].message_type = _S2C
-DESCRIPTOR.message_types_by_name['C2S'] = _C2S
-DESCRIPTOR.message_types_by_name['S2C'] = _S2C
-DESCRIPTOR.message_types_by_name['Request'] = _REQUEST
-DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-C2S = _reflection.GeneratedProtocolMessageType('C2S', (_message.Message,), dict(
-  DESCRIPTOR = _C2S,
-  __module__ = 'Trd_GetMaxTrdQtys_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.C2S)
-  ))
-_sym_db.RegisterMessage(C2S)
-
-S2C = _reflection.GeneratedProtocolMessageType('S2C', (_message.Message,), dict(
-  DESCRIPTOR = _S2C,
-  __module__ = 'Trd_GetMaxTrdQtys_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.S2C)
-  ))
-_sym_db.RegisterMessage(S2C)
-
-Request = _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), dict(
-  DESCRIPTOR = _REQUEST,
-  __module__ = 'Trd_GetMaxTrdQtys_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.Request)
-  ))
-_sym_db.RegisterMessage(Request)
-
-Response = _reflection.GeneratedProtocolMessageType('Response', (_message.Message,), dict(
-  DESCRIPTOR = _RESPONSE,
-  __module__ = 'Trd_GetMaxTrdQtys_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.Response)
-  ))
-_sym_db.RegisterMessage(Response)
-
-
-DESCRIPTOR.has_options = True
-DESCRIPTOR._options = _descriptor._ParseOptions(descriptor_pb2.FileOptions(), _b('\n\023com.futu.openapi.pbZ0github.com/futuopen/ftapi4go/pb/trdgetmaxtrdqtys'))
-# @@protoc_insertion_point(module_scope)
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: Trd_GetMaxTrdQtys.proto
+
+import sys
+_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf import descriptor_pb2
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+import Common_pb2 as Common__pb2
+import Trd_Common_pb2 as Trd__Common__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='Trd_GetMaxTrdQtys.proto',
+  package='Trd_GetMaxTrdQtys',
+  syntax='proto2',
+  serialized_pb=_b('\n\x17Trd_GetMaxTrdQtys.proto\x12\x11Trd_GetMaxTrdQtys\x1a\x0c\x43ommon.proto\x1a\x10Trd_Common.proto\"\xc4\x01\n\x03\x43\x32S\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x11\n\torderType\x18\x02 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x03 \x02(\t\x12\r\n\x05price\x18\x04 \x02(\x01\x12\x0f\n\x07orderID\x18\x05 \x01(\x04\x12\x13\n\x0b\x61\x64justPrice\x18\x06 \x01(\x08\x12\x1a\n\x12\x61\x64justSideAndLimit\x18\x07 \x01(\x01\x12\x11\n\tsecMarket\x18\x08 \x01(\x05\x12\x11\n\torderIDEx\x18\t \x01(\t\"X\n\x03S2C\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12*\n\nmaxTrdQtys\x18\x02 \x01(\x0b\x32\x16.Trd_Common.MaxTrdQtys\".\n\x07Request\x12#\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x16.Trd_GetMaxTrdQtys.C2S\"g\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12#\n\x03s2c\x18\x04 \x01(\x0b\x32\x16.Trd_GetMaxTrdQtys.S2CBG\n\x13\x63om.futu.openapi.pbZ0github.com/futuopen/ftapi4go/pb/trdgetmaxtrdqtys')
+  ,
+  dependencies=[Common__pb2.DESCRIPTOR,Trd__Common__pb2.DESCRIPTOR,])
+
+
+
+
+_C2S = _descriptor.Descriptor(
+  name='C2S',
+  full_name='Trd_GetMaxTrdQtys.C2S',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='header', full_name='Trd_GetMaxTrdQtys.C2S.header', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderType', full_name='Trd_GetMaxTrdQtys.C2S.orderType', index=1,
+      number=2, type=5, cpp_type=1, label=2,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='code', full_name='Trd_GetMaxTrdQtys.C2S.code', index=2,
+      number=3, type=9, cpp_type=9, label=2,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='price', full_name='Trd_GetMaxTrdQtys.C2S.price', index=3,
+      number=4, type=1, cpp_type=5, label=2,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderID', full_name='Trd_GetMaxTrdQtys.C2S.orderID', index=4,
+      number=5, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='adjustPrice', full_name='Trd_GetMaxTrdQtys.C2S.adjustPrice', index=5,
+      number=6, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='adjustSideAndLimit', full_name='Trd_GetMaxTrdQtys.C2S.adjustSideAndLimit', index=6,
+      number=7, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='secMarket', full_name='Trd_GetMaxTrdQtys.C2S.secMarket', index=7,
+      number=8, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderIDEx', full_name='Trd_GetMaxTrdQtys.C2S.orderIDEx', index=8,
+      number=9, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=79,
+  serialized_end=275,
+)
+
+
+_S2C = _descriptor.Descriptor(
+  name='S2C',
+  full_name='Trd_GetMaxTrdQtys.S2C',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='header', full_name='Trd_GetMaxTrdQtys.S2C.header', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='maxTrdQtys', full_name='Trd_GetMaxTrdQtys.S2C.maxTrdQtys', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=277,
+  serialized_end=365,
+)
+
+
+_REQUEST = _descriptor.Descriptor(
+  name='Request',
+  full_name='Trd_GetMaxTrdQtys.Request',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='c2s', full_name='Trd_GetMaxTrdQtys.Request.c2s', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=367,
+  serialized_end=413,
+)
+
+
+_RESPONSE = _descriptor.Descriptor(
+  name='Response',
+  full_name='Trd_GetMaxTrdQtys.Response',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='retType', full_name='Trd_GetMaxTrdQtys.Response.retType', index=0,
+      number=1, type=5, cpp_type=1, label=2,
+      has_default_value=True, default_value=-400,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='retMsg', full_name='Trd_GetMaxTrdQtys.Response.retMsg', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='errCode', full_name='Trd_GetMaxTrdQtys.Response.errCode', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='s2c', full_name='Trd_GetMaxTrdQtys.Response.s2c', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=415,
+  serialized_end=518,
+)
+
+_C2S.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
+_S2C.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
+_S2C.fields_by_name['maxTrdQtys'].message_type = Trd__Common__pb2._MAXTRDQTYS
+_REQUEST.fields_by_name['c2s'].message_type = _C2S
+_RESPONSE.fields_by_name['s2c'].message_type = _S2C
+DESCRIPTOR.message_types_by_name['C2S'] = _C2S
+DESCRIPTOR.message_types_by_name['S2C'] = _S2C
+DESCRIPTOR.message_types_by_name['Request'] = _REQUEST
+DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+C2S = _reflection.GeneratedProtocolMessageType('C2S', (_message.Message,), dict(
+  DESCRIPTOR = _C2S,
+  __module__ = 'Trd_GetMaxTrdQtys_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.C2S)
+  ))
+_sym_db.RegisterMessage(C2S)
+
+S2C = _reflection.GeneratedProtocolMessageType('S2C', (_message.Message,), dict(
+  DESCRIPTOR = _S2C,
+  __module__ = 'Trd_GetMaxTrdQtys_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.S2C)
+  ))
+_sym_db.RegisterMessage(S2C)
+
+Request = _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), dict(
+  DESCRIPTOR = _REQUEST,
+  __module__ = 'Trd_GetMaxTrdQtys_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.Request)
+  ))
+_sym_db.RegisterMessage(Request)
+
+Response = _reflection.GeneratedProtocolMessageType('Response', (_message.Message,), dict(
+  DESCRIPTOR = _RESPONSE,
+  __module__ = 'Trd_GetMaxTrdQtys_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_GetMaxTrdQtys.Response)
+  ))
+_sym_db.RegisterMessage(Response)
+
+
+DESCRIPTOR.has_options = True
+DESCRIPTOR._options = _descriptor._ParseOptions(descriptor_pb2.FileOptions(), _b('\n\023com.futu.openapi.pbZ0github.com/futuopen/ftapi4go/pb/trdgetmaxtrdqtys'))
+# @@protoc_insertion_point(module_scope)
```

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetOrderFillList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetOrderFillList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetOrderList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetOrderList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_GetPositionList_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_GetPositionList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_ModifyOrder_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_ModifyOrder_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,315 +1,329 @@
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: Trd_ModifyOrder.proto
-
-import sys
-_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf import descriptor_pb2
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-import Common_pb2 as Common__pb2
-import Trd_Common_pb2 as Trd__Common__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='Trd_ModifyOrder.proto',
-  package='Trd_ModifyOrder',
-  syntax='proto2',
-  serialized_pb=_b('\n\x15Trd_ModifyOrder.proto\x12\x0fTrd_ModifyOrder\x1a\x0c\x43ommon.proto\x1a\x10Trd_Common.proto\"\xb6\x02\n\x03\x43\x32S\x12\"\n\x08packetID\x18\x01 \x02(\x0b\x32\x10.Common.PacketID\x12%\n\x06header\x18\x02 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07orderID\x18\x03 \x02(\x04\x12\x15\n\rmodifyOrderOp\x18\x04 \x02(\x05\x12\x0e\n\x06\x66orAll\x18\x05 \x01(\x08\x12\x11\n\ttrdMarket\x18\x06 \x01(\x05\x12\x0b\n\x03qty\x18\x08 \x01(\x01\x12\r\n\x05price\x18\t \x01(\x01\x12\x13\n\x0b\x61\x64justPrice\x18\n \x01(\x08\x12\x1a\n\x12\x61\x64justSideAndLimit\x18\x0b \x01(\x01\x12\x10\n\x08\x61uxPrice\x18\x0c \x01(\x01\x12\x11\n\ttrailType\x18\r \x01(\x05\x12\x12\n\ntrailValue\x18\x0e \x01(\x01\x12\x13\n\x0btrailSpread\x18\x0f \x01(\x01\"=\n\x03S2C\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07orderID\x18\x02 \x02(\x04\",\n\x07Request\x12!\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x14.Trd_ModifyOrder.C2S\"e\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12!\n\x03s2c\x18\x04 \x01(\x0b\x32\x14.Trd_ModifyOrder.S2CBE\n\x13\x63om.futu.openapi.pbZ.github.com/futuopen/ftapi4go/pb/trdmodifyorder')
-  ,
-  dependencies=[Common__pb2.DESCRIPTOR,Trd__Common__pb2.DESCRIPTOR,])
-
-
-
-
-_C2S = _descriptor.Descriptor(
-  name='C2S',
-  full_name='Trd_ModifyOrder.C2S',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='packetID', full_name='Trd_ModifyOrder.C2S.packetID', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='header', full_name='Trd_ModifyOrder.C2S.header', index=1,
-      number=2, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='orderID', full_name='Trd_ModifyOrder.C2S.orderID', index=2,
-      number=3, type=4, cpp_type=4, label=2,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='modifyOrderOp', full_name='Trd_ModifyOrder.C2S.modifyOrderOp', index=3,
-      number=4, type=5, cpp_type=1, label=2,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='forAll', full_name='Trd_ModifyOrder.C2S.forAll', index=4,
-      number=5, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trdMarket', full_name='Trd_ModifyOrder.C2S.trdMarket', index=5,
-      number=6, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='qty', full_name='Trd_ModifyOrder.C2S.qty', index=6,
-      number=8, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='price', full_name='Trd_ModifyOrder.C2S.price', index=7,
-      number=9, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='adjustPrice', full_name='Trd_ModifyOrder.C2S.adjustPrice', index=8,
-      number=10, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='adjustSideAndLimit', full_name='Trd_ModifyOrder.C2S.adjustSideAndLimit', index=9,
-      number=11, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='auxPrice', full_name='Trd_ModifyOrder.C2S.auxPrice', index=10,
-      number=12, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trailType', full_name='Trd_ModifyOrder.C2S.trailType', index=11,
-      number=13, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trailValue', full_name='Trd_ModifyOrder.C2S.trailValue', index=12,
-      number=14, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trailSpread', full_name='Trd_ModifyOrder.C2S.trailSpread', index=13,
-      number=15, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=75,
-  serialized_end=385,
-)
-
-
-_S2C = _descriptor.Descriptor(
-  name='S2C',
-  full_name='Trd_ModifyOrder.S2C',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='header', full_name='Trd_ModifyOrder.S2C.header', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='orderID', full_name='Trd_ModifyOrder.S2C.orderID', index=1,
-      number=2, type=4, cpp_type=4, label=2,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=387,
-  serialized_end=448,
-)
-
-
-_REQUEST = _descriptor.Descriptor(
-  name='Request',
-  full_name='Trd_ModifyOrder.Request',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='c2s', full_name='Trd_ModifyOrder.Request.c2s', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=450,
-  serialized_end=494,
-)
-
-
-_RESPONSE = _descriptor.Descriptor(
-  name='Response',
-  full_name='Trd_ModifyOrder.Response',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='retType', full_name='Trd_ModifyOrder.Response.retType', index=0,
-      number=1, type=5, cpp_type=1, label=2,
-      has_default_value=True, default_value=-400,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='retMsg', full_name='Trd_ModifyOrder.Response.retMsg', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='errCode', full_name='Trd_ModifyOrder.Response.errCode', index=2,
-      number=3, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='s2c', full_name='Trd_ModifyOrder.Response.s2c', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=496,
-  serialized_end=597,
-)
-
-_C2S.fields_by_name['packetID'].message_type = Common__pb2._PACKETID
-_C2S.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
-_S2C.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
-_REQUEST.fields_by_name['c2s'].message_type = _C2S
-_RESPONSE.fields_by_name['s2c'].message_type = _S2C
-DESCRIPTOR.message_types_by_name['C2S'] = _C2S
-DESCRIPTOR.message_types_by_name['S2C'] = _S2C
-DESCRIPTOR.message_types_by_name['Request'] = _REQUEST
-DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-C2S = _reflection.GeneratedProtocolMessageType('C2S', (_message.Message,), dict(
-  DESCRIPTOR = _C2S,
-  __module__ = 'Trd_ModifyOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.C2S)
-  ))
-_sym_db.RegisterMessage(C2S)
-
-S2C = _reflection.GeneratedProtocolMessageType('S2C', (_message.Message,), dict(
-  DESCRIPTOR = _S2C,
-  __module__ = 'Trd_ModifyOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.S2C)
-  ))
-_sym_db.RegisterMessage(S2C)
-
-Request = _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), dict(
-  DESCRIPTOR = _REQUEST,
-  __module__ = 'Trd_ModifyOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.Request)
-  ))
-_sym_db.RegisterMessage(Request)
-
-Response = _reflection.GeneratedProtocolMessageType('Response', (_message.Message,), dict(
-  DESCRIPTOR = _RESPONSE,
-  __module__ = 'Trd_ModifyOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.Response)
-  ))
-_sym_db.RegisterMessage(Response)
-
-
-DESCRIPTOR.has_options = True
-DESCRIPTOR._options = _descriptor._ParseOptions(descriptor_pb2.FileOptions(), _b('\n\023com.futu.openapi.pbZ.github.com/futuopen/ftapi4go/pb/trdmodifyorder'))
-# @@protoc_insertion_point(module_scope)
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: Trd_ModifyOrder.proto
+
+import sys
+_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf import descriptor_pb2
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+import Common_pb2 as Common__pb2
+import Trd_Common_pb2 as Trd__Common__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='Trd_ModifyOrder.proto',
+  package='Trd_ModifyOrder',
+  syntax='proto2',
+  serialized_pb=_b('\n\x15Trd_ModifyOrder.proto\x12\x0fTrd_ModifyOrder\x1a\x0c\x43ommon.proto\x1a\x10Trd_Common.proto\"\xc9\x02\n\x03\x43\x32S\x12\"\n\x08packetID\x18\x01 \x02(\x0b\x32\x10.Common.PacketID\x12%\n\x06header\x18\x02 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07orderID\x18\x03 \x02(\x04\x12\x15\n\rmodifyOrderOp\x18\x04 \x02(\x05\x12\x0e\n\x06\x66orAll\x18\x05 \x01(\x08\x12\x11\n\ttrdMarket\x18\x06 \x01(\x05\x12\x0b\n\x03qty\x18\x08 \x01(\x01\x12\r\n\x05price\x18\t \x01(\x01\x12\x13\n\x0b\x61\x64justPrice\x18\n \x01(\x08\x12\x1a\n\x12\x61\x64justSideAndLimit\x18\x0b \x01(\x01\x12\x10\n\x08\x61uxPrice\x18\x0c \x01(\x01\x12\x11\n\ttrailType\x18\r \x01(\x05\x12\x12\n\ntrailValue\x18\x0e \x01(\x01\x12\x13\n\x0btrailSpread\x18\x0f \x01(\x01\x12\x11\n\torderIDEx\x18\x10 \x01(\t\"P\n\x03S2C\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07orderID\x18\x02 \x02(\x04\x12\x11\n\torderIDEx\x18\x03 \x01(\t\",\n\x07Request\x12!\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x14.Trd_ModifyOrder.C2S\"e\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12!\n\x03s2c\x18\x04 \x01(\x0b\x32\x14.Trd_ModifyOrder.S2CBE\n\x13\x63om.futu.openapi.pbZ.github.com/futuopen/ftapi4go/pb/trdmodifyorder')
+  ,
+  dependencies=[Common__pb2.DESCRIPTOR,Trd__Common__pb2.DESCRIPTOR,])
+
+
+
+
+_C2S = _descriptor.Descriptor(
+  name='C2S',
+  full_name='Trd_ModifyOrder.C2S',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='packetID', full_name='Trd_ModifyOrder.C2S.packetID', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='header', full_name='Trd_ModifyOrder.C2S.header', index=1,
+      number=2, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderID', full_name='Trd_ModifyOrder.C2S.orderID', index=2,
+      number=3, type=4, cpp_type=4, label=2,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='modifyOrderOp', full_name='Trd_ModifyOrder.C2S.modifyOrderOp', index=3,
+      number=4, type=5, cpp_type=1, label=2,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='forAll', full_name='Trd_ModifyOrder.C2S.forAll', index=4,
+      number=5, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trdMarket', full_name='Trd_ModifyOrder.C2S.trdMarket', index=5,
+      number=6, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='qty', full_name='Trd_ModifyOrder.C2S.qty', index=6,
+      number=8, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='price', full_name='Trd_ModifyOrder.C2S.price', index=7,
+      number=9, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='adjustPrice', full_name='Trd_ModifyOrder.C2S.adjustPrice', index=8,
+      number=10, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='adjustSideAndLimit', full_name='Trd_ModifyOrder.C2S.adjustSideAndLimit', index=9,
+      number=11, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='auxPrice', full_name='Trd_ModifyOrder.C2S.auxPrice', index=10,
+      number=12, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trailType', full_name='Trd_ModifyOrder.C2S.trailType', index=11,
+      number=13, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trailValue', full_name='Trd_ModifyOrder.C2S.trailValue', index=12,
+      number=14, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trailSpread', full_name='Trd_ModifyOrder.C2S.trailSpread', index=13,
+      number=15, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderIDEx', full_name='Trd_ModifyOrder.C2S.orderIDEx', index=14,
+      number=16, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=75,
+  serialized_end=404,
+)
+
+
+_S2C = _descriptor.Descriptor(
+  name='S2C',
+  full_name='Trd_ModifyOrder.S2C',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='header', full_name='Trd_ModifyOrder.S2C.header', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderID', full_name='Trd_ModifyOrder.S2C.orderID', index=1,
+      number=2, type=4, cpp_type=4, label=2,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderIDEx', full_name='Trd_ModifyOrder.S2C.orderIDEx', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=406,
+  serialized_end=486,
+)
+
+
+_REQUEST = _descriptor.Descriptor(
+  name='Request',
+  full_name='Trd_ModifyOrder.Request',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='c2s', full_name='Trd_ModifyOrder.Request.c2s', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=488,
+  serialized_end=532,
+)
+
+
+_RESPONSE = _descriptor.Descriptor(
+  name='Response',
+  full_name='Trd_ModifyOrder.Response',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='retType', full_name='Trd_ModifyOrder.Response.retType', index=0,
+      number=1, type=5, cpp_type=1, label=2,
+      has_default_value=True, default_value=-400,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='retMsg', full_name='Trd_ModifyOrder.Response.retMsg', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='errCode', full_name='Trd_ModifyOrder.Response.errCode', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='s2c', full_name='Trd_ModifyOrder.Response.s2c', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=534,
+  serialized_end=635,
+)
+
+_C2S.fields_by_name['packetID'].message_type = Common__pb2._PACKETID
+_C2S.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
+_S2C.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
+_REQUEST.fields_by_name['c2s'].message_type = _C2S
+_RESPONSE.fields_by_name['s2c'].message_type = _S2C
+DESCRIPTOR.message_types_by_name['C2S'] = _C2S
+DESCRIPTOR.message_types_by_name['S2C'] = _S2C
+DESCRIPTOR.message_types_by_name['Request'] = _REQUEST
+DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+C2S = _reflection.GeneratedProtocolMessageType('C2S', (_message.Message,), dict(
+  DESCRIPTOR = _C2S,
+  __module__ = 'Trd_ModifyOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.C2S)
+  ))
+_sym_db.RegisterMessage(C2S)
+
+S2C = _reflection.GeneratedProtocolMessageType('S2C', (_message.Message,), dict(
+  DESCRIPTOR = _S2C,
+  __module__ = 'Trd_ModifyOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.S2C)
+  ))
+_sym_db.RegisterMessage(S2C)
+
+Request = _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), dict(
+  DESCRIPTOR = _REQUEST,
+  __module__ = 'Trd_ModifyOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.Request)
+  ))
+_sym_db.RegisterMessage(Request)
+
+Response = _reflection.GeneratedProtocolMessageType('Response', (_message.Message,), dict(
+  DESCRIPTOR = _RESPONSE,
+  __module__ = 'Trd_ModifyOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_ModifyOrder.Response)
+  ))
+_sym_db.RegisterMessage(Response)
+
+
+DESCRIPTOR.has_options = True
+DESCRIPTOR._options = _descriptor._ParseOptions(descriptor_pb2.FileOptions(), _b('\n\023com.futu.openapi.pbZ.github.com/futuopen/ftapi4go/pb/trdmodifyorder'))
+# @@protoc_insertion_point(module_scope)
```

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_Notify_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_Notify_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_PlaceOrder_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_PlaceOrder_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,336 +1,343 @@
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: Trd_PlaceOrder.proto
-
-import sys
-_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf import descriptor_pb2
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-import Common_pb2 as Common__pb2
-import Trd_Common_pb2 as Trd__Common__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='Trd_PlaceOrder.proto',
-  package='Trd_PlaceOrder',
-  syntax='proto2',
-  serialized_pb=_b('\n\x14Trd_PlaceOrder.proto\x12\x0eTrd_PlaceOrder\x1a\x0c\x43ommon.proto\x1a\x10Trd_Common.proto\"\xed\x02\n\x03\x43\x32S\x12\"\n\x08packetID\x18\x01 \x02(\x0b\x32\x10.Common.PacketID\x12%\n\x06header\x18\x02 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07trdSide\x18\x03 \x02(\x05\x12\x11\n\torderType\x18\x04 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x05 \x02(\t\x12\x0b\n\x03qty\x18\x06 \x02(\x01\x12\r\n\x05price\x18\x07 \x01(\x01\x12\x13\n\x0b\x61\x64justPrice\x18\x08 \x01(\x08\x12\x1a\n\x12\x61\x64justSideAndLimit\x18\t \x01(\x01\x12\x11\n\tsecMarket\x18\n \x01(\x05\x12\x0e\n\x06remark\x18\x0b \x01(\t\x12\x13\n\x0btimeInForce\x18\x0c \x01(\x05\x12\x16\n\x0e\x66illOutsideRTH\x18\r \x01(\x08\x12\x10\n\x08\x61uxPrice\x18\x0e \x01(\x01\x12\x11\n\ttrailType\x18\x0f \x01(\x05\x12\x12\n\ntrailValue\x18\x10 \x01(\x01\x12\x13\n\x0btrailSpread\x18\x11 \x01(\x01\"=\n\x03S2C\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07orderID\x18\x02 \x01(\x04\"+\n\x07Request\x12 \n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x13.Trd_PlaceOrder.C2S\"d\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12 \n\x03s2c\x18\x04 \x01(\x0b\x32\x13.Trd_PlaceOrder.S2CBD\n\x13\x63om.futu.openapi.pbZ-github.com/futuopen/ftapi4go/pb/trdplaceorder')
-  ,
-  dependencies=[Common__pb2.DESCRIPTOR,Trd__Common__pb2.DESCRIPTOR,])
-
-
-
-
-_C2S = _descriptor.Descriptor(
-  name='C2S',
-  full_name='Trd_PlaceOrder.C2S',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='packetID', full_name='Trd_PlaceOrder.C2S.packetID', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='header', full_name='Trd_PlaceOrder.C2S.header', index=1,
-      number=2, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trdSide', full_name='Trd_PlaceOrder.C2S.trdSide', index=2,
-      number=3, type=5, cpp_type=1, label=2,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='orderType', full_name='Trd_PlaceOrder.C2S.orderType', index=3,
-      number=4, type=5, cpp_type=1, label=2,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='code', full_name='Trd_PlaceOrder.C2S.code', index=4,
-      number=5, type=9, cpp_type=9, label=2,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='qty', full_name='Trd_PlaceOrder.C2S.qty', index=5,
-      number=6, type=1, cpp_type=5, label=2,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='price', full_name='Trd_PlaceOrder.C2S.price', index=6,
-      number=7, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='adjustPrice', full_name='Trd_PlaceOrder.C2S.adjustPrice', index=7,
-      number=8, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='adjustSideAndLimit', full_name='Trd_PlaceOrder.C2S.adjustSideAndLimit', index=8,
-      number=9, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='secMarket', full_name='Trd_PlaceOrder.C2S.secMarket', index=9,
-      number=10, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='remark', full_name='Trd_PlaceOrder.C2S.remark', index=10,
-      number=11, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='timeInForce', full_name='Trd_PlaceOrder.C2S.timeInForce', index=11,
-      number=12, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='fillOutsideRTH', full_name='Trd_PlaceOrder.C2S.fillOutsideRTH', index=12,
-      number=13, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='auxPrice', full_name='Trd_PlaceOrder.C2S.auxPrice', index=13,
-      number=14, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trailType', full_name='Trd_PlaceOrder.C2S.trailType', index=14,
-      number=15, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trailValue', full_name='Trd_PlaceOrder.C2S.trailValue', index=15,
-      number=16, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='trailSpread', full_name='Trd_PlaceOrder.C2S.trailSpread', index=16,
-      number=17, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=73,
-  serialized_end=438,
-)
-
-
-_S2C = _descriptor.Descriptor(
-  name='S2C',
-  full_name='Trd_PlaceOrder.S2C',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='header', full_name='Trd_PlaceOrder.S2C.header', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='orderID', full_name='Trd_PlaceOrder.S2C.orderID', index=1,
-      number=2, type=4, cpp_type=4, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=440,
-  serialized_end=501,
-)
-
-
-_REQUEST = _descriptor.Descriptor(
-  name='Request',
-  full_name='Trd_PlaceOrder.Request',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='c2s', full_name='Trd_PlaceOrder.Request.c2s', index=0,
-      number=1, type=11, cpp_type=10, label=2,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=503,
-  serialized_end=546,
-)
-
-
-_RESPONSE = _descriptor.Descriptor(
-  name='Response',
-  full_name='Trd_PlaceOrder.Response',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='retType', full_name='Trd_PlaceOrder.Response.retType', index=0,
-      number=1, type=5, cpp_type=1, label=2,
-      has_default_value=True, default_value=-400,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='retMsg', full_name='Trd_PlaceOrder.Response.retMsg', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='errCode', full_name='Trd_PlaceOrder.Response.errCode', index=2,
-      number=3, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='s2c', full_name='Trd_PlaceOrder.Response.s2c', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=548,
-  serialized_end=648,
-)
-
-_C2S.fields_by_name['packetID'].message_type = Common__pb2._PACKETID
-_C2S.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
-_S2C.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
-_REQUEST.fields_by_name['c2s'].message_type = _C2S
-_RESPONSE.fields_by_name['s2c'].message_type = _S2C
-DESCRIPTOR.message_types_by_name['C2S'] = _C2S
-DESCRIPTOR.message_types_by_name['S2C'] = _S2C
-DESCRIPTOR.message_types_by_name['Request'] = _REQUEST
-DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-C2S = _reflection.GeneratedProtocolMessageType('C2S', (_message.Message,), dict(
-  DESCRIPTOR = _C2S,
-  __module__ = 'Trd_PlaceOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.C2S)
-  ))
-_sym_db.RegisterMessage(C2S)
-
-S2C = _reflection.GeneratedProtocolMessageType('S2C', (_message.Message,), dict(
-  DESCRIPTOR = _S2C,
-  __module__ = 'Trd_PlaceOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.S2C)
-  ))
-_sym_db.RegisterMessage(S2C)
-
-Request = _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), dict(
-  DESCRIPTOR = _REQUEST,
-  __module__ = 'Trd_PlaceOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.Request)
-  ))
-_sym_db.RegisterMessage(Request)
-
-Response = _reflection.GeneratedProtocolMessageType('Response', (_message.Message,), dict(
-  DESCRIPTOR = _RESPONSE,
-  __module__ = 'Trd_PlaceOrder_pb2'
-  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.Response)
-  ))
-_sym_db.RegisterMessage(Response)
-
-
-DESCRIPTOR.has_options = True
-DESCRIPTOR._options = _descriptor._ParseOptions(descriptor_pb2.FileOptions(), _b('\n\023com.futu.openapi.pbZ-github.com/futuopen/ftapi4go/pb/trdplaceorder'))
-# @@protoc_insertion_point(module_scope)
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: Trd_PlaceOrder.proto
+
+import sys
+_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf import descriptor_pb2
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+import Common_pb2 as Common__pb2
+import Trd_Common_pb2 as Trd__Common__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='Trd_PlaceOrder.proto',
+  package='Trd_PlaceOrder',
+  syntax='proto2',
+  serialized_pb=_b('\n\x14Trd_PlaceOrder.proto\x12\x0eTrd_PlaceOrder\x1a\x0c\x43ommon.proto\x1a\x10Trd_Common.proto\"\xed\x02\n\x03\x43\x32S\x12\"\n\x08packetID\x18\x01 \x02(\x0b\x32\x10.Common.PacketID\x12%\n\x06header\x18\x02 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07trdSide\x18\x03 \x02(\x05\x12\x11\n\torderType\x18\x04 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x05 \x02(\t\x12\x0b\n\x03qty\x18\x06 \x02(\x01\x12\r\n\x05price\x18\x07 \x01(\x01\x12\x13\n\x0b\x61\x64justPrice\x18\x08 \x01(\x08\x12\x1a\n\x12\x61\x64justSideAndLimit\x18\t \x01(\x01\x12\x11\n\tsecMarket\x18\n \x01(\x05\x12\x0e\n\x06remark\x18\x0b \x01(\t\x12\x13\n\x0btimeInForce\x18\x0c \x01(\x05\x12\x16\n\x0e\x66illOutsideRTH\x18\r \x01(\x08\x12\x10\n\x08\x61uxPrice\x18\x0e \x01(\x01\x12\x11\n\ttrailType\x18\x0f \x01(\x05\x12\x12\n\ntrailValue\x18\x10 \x01(\x01\x12\x13\n\x0btrailSpread\x18\x11 \x01(\x01\"P\n\x03S2C\x12%\n\x06header\x18\x01 \x02(\x0b\x32\x15.Trd_Common.TrdHeader\x12\x0f\n\x07orderID\x18\x02 \x01(\x04\x12\x11\n\torderIDEx\x18\x03 \x01(\t\"+\n\x07Request\x12 \n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x13.Trd_PlaceOrder.C2S\"d\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12 \n\x03s2c\x18\x04 \x01(\x0b\x32\x13.Trd_PlaceOrder.S2CBD\n\x13\x63om.futu.openapi.pbZ-github.com/futuopen/ftapi4go/pb/trdplaceorder')
+  ,
+  dependencies=[Common__pb2.DESCRIPTOR,Trd__Common__pb2.DESCRIPTOR,])
+
+
+
+
+_C2S = _descriptor.Descriptor(
+  name='C2S',
+  full_name='Trd_PlaceOrder.C2S',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='packetID', full_name='Trd_PlaceOrder.C2S.packetID', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='header', full_name='Trd_PlaceOrder.C2S.header', index=1,
+      number=2, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trdSide', full_name='Trd_PlaceOrder.C2S.trdSide', index=2,
+      number=3, type=5, cpp_type=1, label=2,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderType', full_name='Trd_PlaceOrder.C2S.orderType', index=3,
+      number=4, type=5, cpp_type=1, label=2,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='code', full_name='Trd_PlaceOrder.C2S.code', index=4,
+      number=5, type=9, cpp_type=9, label=2,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='qty', full_name='Trd_PlaceOrder.C2S.qty', index=5,
+      number=6, type=1, cpp_type=5, label=2,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='price', full_name='Trd_PlaceOrder.C2S.price', index=6,
+      number=7, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='adjustPrice', full_name='Trd_PlaceOrder.C2S.adjustPrice', index=7,
+      number=8, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='adjustSideAndLimit', full_name='Trd_PlaceOrder.C2S.adjustSideAndLimit', index=8,
+      number=9, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='secMarket', full_name='Trd_PlaceOrder.C2S.secMarket', index=9,
+      number=10, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='remark', full_name='Trd_PlaceOrder.C2S.remark', index=10,
+      number=11, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='timeInForce', full_name='Trd_PlaceOrder.C2S.timeInForce', index=11,
+      number=12, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='fillOutsideRTH', full_name='Trd_PlaceOrder.C2S.fillOutsideRTH', index=12,
+      number=13, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='auxPrice', full_name='Trd_PlaceOrder.C2S.auxPrice', index=13,
+      number=14, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trailType', full_name='Trd_PlaceOrder.C2S.trailType', index=14,
+      number=15, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trailValue', full_name='Trd_PlaceOrder.C2S.trailValue', index=15,
+      number=16, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='trailSpread', full_name='Trd_PlaceOrder.C2S.trailSpread', index=16,
+      number=17, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=73,
+  serialized_end=438,
+)
+
+
+_S2C = _descriptor.Descriptor(
+  name='S2C',
+  full_name='Trd_PlaceOrder.S2C',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='header', full_name='Trd_PlaceOrder.S2C.header', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderID', full_name='Trd_PlaceOrder.S2C.orderID', index=1,
+      number=2, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderIDEx', full_name='Trd_PlaceOrder.S2C.orderIDEx', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=440,
+  serialized_end=520,
+)
+
+
+_REQUEST = _descriptor.Descriptor(
+  name='Request',
+  full_name='Trd_PlaceOrder.Request',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='c2s', full_name='Trd_PlaceOrder.Request.c2s', index=0,
+      number=1, type=11, cpp_type=10, label=2,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=522,
+  serialized_end=565,
+)
+
+
+_RESPONSE = _descriptor.Descriptor(
+  name='Response',
+  full_name='Trd_PlaceOrder.Response',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='retType', full_name='Trd_PlaceOrder.Response.retType', index=0,
+      number=1, type=5, cpp_type=1, label=2,
+      has_default_value=True, default_value=-400,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='retMsg', full_name='Trd_PlaceOrder.Response.retMsg', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='errCode', full_name='Trd_PlaceOrder.Response.errCode', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='s2c', full_name='Trd_PlaceOrder.Response.s2c', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=567,
+  serialized_end=667,
+)
+
+_C2S.fields_by_name['packetID'].message_type = Common__pb2._PACKETID
+_C2S.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
+_S2C.fields_by_name['header'].message_type = Trd__Common__pb2._TRDHEADER
+_REQUEST.fields_by_name['c2s'].message_type = _C2S
+_RESPONSE.fields_by_name['s2c'].message_type = _S2C
+DESCRIPTOR.message_types_by_name['C2S'] = _C2S
+DESCRIPTOR.message_types_by_name['S2C'] = _S2C
+DESCRIPTOR.message_types_by_name['Request'] = _REQUEST
+DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+C2S = _reflection.GeneratedProtocolMessageType('C2S', (_message.Message,), dict(
+  DESCRIPTOR = _C2S,
+  __module__ = 'Trd_PlaceOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.C2S)
+  ))
+_sym_db.RegisterMessage(C2S)
+
+S2C = _reflection.GeneratedProtocolMessageType('S2C', (_message.Message,), dict(
+  DESCRIPTOR = _S2C,
+  __module__ = 'Trd_PlaceOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.S2C)
+  ))
+_sym_db.RegisterMessage(S2C)
+
+Request = _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), dict(
+  DESCRIPTOR = _REQUEST,
+  __module__ = 'Trd_PlaceOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.Request)
+  ))
+_sym_db.RegisterMessage(Request)
+
+Response = _reflection.GeneratedProtocolMessageType('Response', (_message.Message,), dict(
+  DESCRIPTOR = _RESPONSE,
+  __module__ = 'Trd_PlaceOrder_pb2'
+  # @@protoc_insertion_point(class_scope:Trd_PlaceOrder.Response)
+  ))
+_sym_db.RegisterMessage(Response)
+
+
+DESCRIPTOR.has_options = True
+DESCRIPTOR._options = _descriptor._ParseOptions(descriptor_pb2.FileOptions(), _b('\n\023com.futu.openapi.pbZ-github.com/futuopen/ftapi4go/pb/trdplaceorder'))
+# @@protoc_insertion_point(module_scope)
```

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_ReconfirmOrder_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_ReconfirmOrder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_SubAccPush_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_SubAccPush_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_UnlockTrade_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_UnlockTrade_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_UpdateOrderFill_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_UpdateOrderFill_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Trd_UpdateOrder_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Trd_UpdateOrder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/UsedQuota_pb2.py` & `futu-api-8.2.4208/futu/common/pb/UsedQuota_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pb/Verification_pb2.py` & `futu-api-8.2.4208/futu/common/pb/Verification_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/pbjson.py` & `futu-api-8.2.4208/futu/common/pbjson.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/sys_config.py` & `futu-api-8.2.4208/futu/common/sys_config.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/common/utils.py` & `futu-api-8.2.4208/futu/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 ProtoInfo = collections.namedtuple('ProtoInfo', ['proto_id', 'serial_no'])
 
 
 def get_message_head_len():
     return calcsize(MESSAGE_HEAD_FMT)
 
 
+def is_valid_date(date_str):
+    try:
+        datetime.strptime(date_str, "%Y-%m-%d")
+        return True
+    except ValueError:
+        return False
+
+
 def check_date_str_format(s, default_time="00:00:00"):
     """Check the format of date string"""
     try:
         str_fmt = s
         if ":" not in s:
             str_fmt = '{} {}'.format(s, default_time)
 
@@ -38,15 +46,15 @@
     ret_code, ret_data = check_date_str_format(date_str, default_time)
     if ret_code != RET_OK:
         return ret_code, ret_data
 
     return RET_OK, ret_data.strftime("%Y-%m-%d %H:%M:%S")
 
 
-def normalize_start_end_date(start, end, delta_days=0, default_time_start="00:00:00", default_time_end="23:59:59", prefer_end_now=True):
+def normalize_start_end_date(start, end, delta_days=0, default_time_start="00:00:00", default_time_end="23:59:59", prefer_end_now=True, only_date=False):
     """
 
     :param start:
     :param end:
     :param delta_days:
     :param default_time_start:
     :param default_time_end:
@@ -97,16 +105,20 @@
             dt_now = datetime.now()
             dt_start = datetime(year=dt_now.year, month=dt_now.month, day=dt_now.day, hour=hour_start, minute=min_start,
                               second=sec_start)
             dt_tmp = dt_start + delta
             dt_end = datetime(year=dt_tmp.year, month=dt_tmp.month, day=dt_tmp.day, hour=hour_end, minute=min_end,
                                 second=sec_end)
 
-    start = dt_start.strftime("%Y-%m-%d %H:%M:%S")
-    end = dt_end.strftime("%Y-%m-%d %H:%M:%S")
+    if only_date:
+        start = dt_start.strftime("%Y-%m-%d")
+        end = dt_end.strftime("%Y-%m-%d")
+    else:
+        start = dt_start.strftime("%Y-%m-%d %H:%M:%S")
+        end = dt_end.strftime("%Y-%m-%d %H:%M:%S")
 
     return RET_OK, '', start, end
 
 
 def is_str(s):
     if IS_PY2:
         return isinstance(s, str) or isinstance(s, unicode)
@@ -332,14 +344,18 @@
         from  .pb.Trd_UpdateOrderFill_pb2 import Response
         ProtobufMap.created_protobuf_map[ProtoId.Trd_UpdateOrderFill] = Response()
 
         """ Trd_GetHistoryOrderList = 2221  # 获取历史订单列表 """
         from .pb.Trd_GetHistoryOrderList_pb2 import Response
         ProtobufMap.created_protobuf_map[ProtoId.Trd_GetHistoryOrderList] = Response()
 
+        """ Trd_GetOrderFee = 2225  # 获取订单费用 """
+        from .pb.Trd_GetOrderFee_pb2 import Response
+        ProtobufMap.created_protobuf_map[ProtoId.Trd_GetOrderFee] = Response()
+
         """ Trd_GetHistoryOrderFillList = 2222  # 获取历史成交列表 """
         from .pb.Trd_GetHistoryOrderFillList_pb2 import Response
         ProtobufMap.created_protobuf_map[ProtoId.Trd_GetHistoryOrderFillList] = Response()
 
         """ Qot_GetReference = 2223  获取正股相关股票，暂时只有窝轮"""
         from .pb.Trd_GetMarginRatio_pb2 import Response
         ProtobufMap.created_protobuf_map[ProtoId.Trd_GetMarginRatio] = Response()
```

### Comparing `futu-api-8.1.4108/futu/examples/get_mkt_snapshot_demo.py` & `futu-api-8.2.4208/futu/examples/get_mkt_snapshot_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/examples/macd_strategy.py` & `futu-api-8.2.4208/futu/examples/macd_strategy.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/examples/quote_and_trade_demo.py` & `futu-api-8.2.4208/futu/examples/quote_and_trade_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/examples/quote_push.py` & `futu-api-8.2.4208/futu/examples/quote_push.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/examples/simple_filter_demo.py` & `futu-api-8.2.4208/futu/examples/simple_filter_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/examples/stocksell_demo.py` & `futu-api-8.2.4208/futu/examples/stocksell_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/quote/open_quote_context.py` & `futu-api-8.2.4208/futu/quote/open_quote_context.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/quote/quote_get_warrant.py` & `futu-api-8.2.4208/futu/quote/quote_get_warrant.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/quote/quote_query.py` & `futu-api-8.2.4208/futu/quote/quote_query.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/quote/quote_response_handler.py` & `futu-api-8.2.4208/futu/quote/quote_response_handler.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/quote/quote_stockfilter_info.py` & `futu-api-8.2.4208/futu/quote/quote_stockfilter_info.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/quote/quote_tool.py` & `futu-api-8.2.4208/futu/quote/quote_tool.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/tools/Common.proto.json` & `futu-api-8.2.4208/futu/tools/Common.proto.json`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/tools/generate_code.py` & `futu-api-8.2.4208/futu/tools/generate_code.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/tools/load_template.py` & `futu-api-8.2.4208/futu/tools/load_template.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu/trade/open_trade_context.py` & `futu-api-8.2.4208/futu/trade/open_trade_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,28 +80,30 @@
         if ret_code != RET_OK:
             return RET_ERROR, msg
 
         # 记录当前市场的帐号列表
         self.__last_acc_list = []
         for record in acc_list:
             trdMkt_list = record["trdMarket_list"]
-            if self.__trd_mkt == TrdMarket.NONE or self.__trd_mkt in trdMkt_list or self.is_futures_market_sim(trdMkt_list):
+            if (self.__trd_mkt == TrdMarket.NONE or
+                    self.__trd_mkt in trdMkt_list or
+                    self.is_futures_market_sim(trdMkt_list)):
                 if record['trd_env'] == TrdEnv.SIMULATE or record['security_firm'] == NoneDataValue or record['security_firm'] == self.__security_firm:
                     trd_marketauth = []
                     for item in record["trdmarket_auth"]:
                         trd_marketauth.append(TrdMarket.to_string2(item))
                     self.__last_acc_list.append({
                         "trd_env": record["trd_env"],
                         "acc_id": record["acc_id"],
                         "acc_type": record["acc_type"],
                         "uni_card_num": record["uni_card_num"],
                         "card_num": record["card_num"],
                         "security_firm": record["security_firm"],
                         "sim_acc_type": record["sim_acc_type"],
-                        "trdmarket_auth" : trd_marketauth})
+                        "trdmarket_auth": trd_marketauth})
 
         col_list = ["acc_id", "trd_env", "acc_type", "uni_card_num", "card_num", "security_firm", "sim_acc_type", "trdmarket_auth"]
 
         acc_table = pd.DataFrame(copy(self.__last_acc_list), columns=col_list)
 
         return RET_OK, acc_table
 
@@ -303,15 +305,16 @@
         }
 
         ret_code, msg, accinfo_list = query_processor(**kargs)
         if ret_code != RET_OK:
             return RET_ERROR, msg
 
         col_list = [
-            'power', 'max_power_short', 'net_cash_power', 'total_assets', 'cash', 'market_val', 'long_mv', 'short_mv',
+            'power', 'max_power_short', 'net_cash_power', 'total_assets', 'securities_assets', 'fund_assets',
+            'bond_assets', 'cash', 'market_val', 'long_mv', 'short_mv',
             'pending_asset', 'interest_charged_amount', 'frozen_cash', 'avl_withdrawal_cash', 'max_withdrawal', 'currency',
             'available_funds', 'unrealized_pl', 'realized_pl', 'risk_level', 'risk_status', 'initial_margin',
             'margin_call_margin', 'maintenance_margin', 'hk_cash', 'hk_avl_withdrawal_cash', 'us_cash',
             'us_avl_withdrawal_cash', 'cn_cash', 'cn_avl_withdrawal_cash', 'jp_cash', 'jp_avl_withdrawal_cash',
             'sg_cash', 'sg_avl_withdrawal_cash', 'au_cash', 'au_avl_withdrawal_cash', 'is_pdt', 'pdt_seq', 'beginning_dtbp', 'remaining_dtbp',
             'dt_call_amount', 'dt_status'
         ]
@@ -496,16 +499,16 @@
         if ret_code != RET_OK:
             return RET_ERROR, msg
 
         return RET_OK, order_list
 
     def place_order(self, price, qty, code, trd_side, order_type=OrderType.NORMAL,
                     adjust_limit=0, trd_env=TrdEnv.REAL, acc_id=0, acc_index=0, remark=None,
-                    time_in_force=TimeInForce.DAY, fill_outside_rth=False, aux_price = None,
-                    trail_type = None ,trail_value = None ,trail_spread = None):
+                    time_in_force=TimeInForce.DAY, fill_outside_rth=False, aux_price=None,
+                    trail_type=None, trail_value=None, trail_spread=None):
         """
         place order
         use  set_handle(HKTradeOrderHandlerBase) to recv order push !
         """
         # ret, msg = self._check_trd_env(trd_env)
         # if ret != RET_OK:
         #     return ret, msg
@@ -564,15 +567,15 @@
         if ret_code != RET_OK:
             return RET_ERROR, msg
 
         order_item = {'trd_env': trd_env, 'order_id': order_id}
 
         # 保持跟v2.0兼容， 增加必要的订单字段
         for x in range(3):
-            ret_code, ret_data = self._order_list_query_impl(order_id=order_id,status_filter_list=[],
+            ret_code, ret_data = self._order_list_query_impl(order_id=order_id, status_filter_list=[],
                                             code="", start="", end="", trd_env=trd_env, acc_id=acc_id,
                                                              refresh_cache=False, trd_mkt=acc_auth_list[0])
             if ret_code == RET_OK and len(ret_data) > 0:
                 order_item = ret_data[0]
                 order_item['trd_env'] = trd_env
                 break
 
@@ -757,14 +760,49 @@
             "time_in_force", "fill_outside_rth", "aux_price", "trail_type", "trail_value",
             "trail_spread", "currency",
         ]
         order_list_table = pd.DataFrame(order_list, columns=col_list)
 
         return RET_OK, order_list_table
 
+    def order_fee_query(self, order_id_list=[], trd_env=TrdEnv.REAL, acc_id=0, acc_index=0):
+        ret, msg = self._check_trd_env(trd_env)
+        if ret != RET_OK:
+            return ret, msg
+
+        ret, msg, acc_id, acc_auth_list = self._check_acc_id_and_acc_index(trd_env, acc_id, acc_index)
+        if ret != RET_OK:
+            return ret, msg
+
+        if order_id_list is not None and not isinstance(order_id_list, list):
+            return RET_ERROR, 'order_id_list type error'
+
+        query_processor = self._get_sync_query_processor(
+            OrderFeeQuery.pack_req,
+            OrderFeeQuery.unpack_rsp)
+
+        kargs = {
+            'order_id_list': order_id_list,
+            'trd_mkt': acc_auth_list[0],
+            'trd_env': trd_env,
+            'acc_id': acc_id,
+            'conn_id': self.get_sync_conn_id()
+        }
+
+        ret_code, msg, order_fee_list = query_processor(**kargs)
+        if ret_code != RET_OK:
+            return RET_ERROR, msg
+
+        col_list = [
+            "order_id", "fee_amount", "fee_details",
+        ]
+        order_fee_list_table = pd.DataFrame(order_fee_list, columns=col_list)
+
+        return RET_OK, order_fee_list_table
+
     def history_deal_list_query(self, code='', start='', end='', trd_env=TrdEnv.REAL, acc_id=0, acc_index=0):
 
         ret, msg = self._check_trd_env(trd_env)
         if ret != RET_OK:
             return ret, msg
 
         ret, msg, acc_id, acc_auth_list = self._check_acc_id_and_acc_index(trd_env, acc_id, acc_index)
```

### Comparing `futu-api-8.1.4108/futu/trade/trade_query.py` & `futu-api-8.2.4208/futu/trade/trade_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,17 @@
 
         raw_funds = rsp_pb.s2c.funds
         accinfo_list = [{
             'power': raw_funds.power,
             'max_power_short': raw_funds.maxPowerShort if raw_funds.HasField('maxPowerShort') else NoneDataValue,
             'net_cash_power': raw_funds.netCashPower if raw_funds.HasField('netCashPower') else NoneDataValue,
             'total_assets': raw_funds.totalAssets,
+            'securities_assets': raw_funds.securitiesAssets if raw_funds.HasField('securitiesAssets') else NoneDataValue,
+            'fund_assets': raw_funds.fundAssets if raw_funds.HasField('fundAssets') else NoneDataValue,
+            'bond_assets': raw_funds.bondAssets if raw_funds.HasField('bondAssets') else NoneDataValue,
             'cash': raw_funds.cash,
             'market_val': raw_funds.marketVal,
             'long_mv': raw_funds.longMv if raw_funds.HasField('longMv') else NoneDataValue,
             'short_mv': raw_funds.shortMv if raw_funds.HasField('shortMv') else NoneDataValue,
             'pending_asset': raw_funds.pendingAsset if raw_funds.HasField('pendingAsset') else NoneDataValue,
             'interest_charged_amount': raw_funds.debtCash if raw_funds.HasField('debtCash') else NoneDataValue,
             'frozen_cash': raw_funds.frozenCash,
@@ -274,15 +277,15 @@
         _, req.c2s.header.trdEnv = TrdEnv.to_number(trd_env)
         req.c2s.header.accID = acc_id
         _, req.c2s.header.trdMarket = TrdMarket.to_number(trd_mkt)
 
         if code:
             req.c2s.filterConditions.codeList.append(code)
         if order_id:
-            req.c2s.filterConditions.idList.append(int(order_id))
+            req.c2s.filterConditions.orderIDExList.append(order_id)
 
         if start:
             req.c2s.filterConditions.beginTime = start
         if end:
             req.c2s.filterConditions.endTime = end
         if refresh_cache:
             req.c2s.refreshCache = refresh_cache
@@ -299,15 +302,15 @@
     def parse_order(cls, rsp_pb, order):
         order_dict = {
             "code": merge_trd_mkt_stock_str(order.secMarket, order.code),
             "stock_name": order.name,
             "trd_side": TrdSide.to_string2(order.trdSide) if order.HasField('trdSide') else 'N/A',# 初始化枚举类型
             "order_type": OrderType.to_string2(order.orderType) if order.HasField('orderType') else 'N/A',# 初始化枚举类型
             "order_status": OrderStatus.to_string2(order.orderStatus) if order.HasField('orderStatus') else 'N/A',# 初始化枚举类型
-            "order_id": str(order.orderID),
+            "order_id": str(order.orderIDEx),
             "qty": order.qty,
             "price": order.price,
             "create_time": order.createTime,
             "updated_time": order.updateTime,
             "dealt_qty": order.fillQty,
             "dealt_avg_price": order.fillAvgPrice,
             "last_err_msg": order.lastErrMsg,
@@ -391,15 +394,15 @@
 
     @classmethod
     def unpack_rsp(cls, rsp_pb):
         """Convert from PLS response to user response"""
         if rsp_pb.retType != RET_OK:
             return RET_ERROR, rsp_pb.retMsg, None
 
-        order_id = str(rsp_pb.s2c.orderID)
+        order_id = str(rsp_pb.s2c.orderIDEx)
 
         return RET_OK, "", order_id
 
 
 class ModifyOrder:
     """modify order class"""
     def __init__(self):
@@ -416,15 +419,17 @@
         req.c2s.packetID.serialNo = serial_no
         req.c2s.packetID.connID = conn_id
 
         _, req.c2s.header.trdEnv = TrdEnv.to_number(trd_env)
         req.c2s.header.accID = acc_id
         _, req.c2s.header.trdMarket = TrdMarket.to_number(trd_mkt)
 
-        req.c2s.orderID = int(order_id)
+        # orderID不使用了，但是required字段必须传值
+        req.c2s.orderID = 0
+        req.c2s.orderIDEx = order_id
         _, req.c2s.modifyOrderOp = ModifyOrderOp.to_number(modify_order_op)
         req.c2s.forAll = False
 
         if modify_order_op == ModifyOrderOp.NORMAL:
             req.c2s.qty = qty
             req.c2s.price = price
             req.c2s.adjustPrice = adjust_limit != 0
@@ -442,15 +447,15 @@
 
     @classmethod
     def unpack_rsp(cls, rsp_pb):
         """Convert from PLS response to user response"""
         if rsp_pb.retType != RET_OK:
             return RET_ERROR, rsp_pb.retMsg, None
 
-        order_id = str(rsp_pb.s2c.orderID)
+        order_id = str(rsp_pb.s2c.orderIDEx)
         modify_order_list = [{
             'trd_env': TrdEnv.to_string2(rsp_pb.s2c.header.trdEnv) if rsp_pb.s2c.header.HasField('trdEnv') else 'N/A',# 初始化枚举类型
             'order_id': order_id
         }]
 
         return RET_OK, "", modify_order_list
 
@@ -511,15 +516,15 @@
 
     @classmethod
     def parse_deal(cls, rsp_pb, deal):
         deal_dict = {
             "code": merge_trd_mkt_stock_str(deal.secMarket, deal.code),
             "stock_name": deal.name,
             "deal_id": deal.fillID,
-            "order_id": str(deal.orderID) if deal.HasField('orderID') else NoneDataValue,
+            "order_id": str(deal.orderIDEx) if deal.HasField('orderIDEx') else NoneDataValue,
             "qty": deal.qty,
             "price": deal.price,
             "trd_side": TrdSide.to_string2(deal.trdSide) if deal.HasField('trdSide') else 'N/A',# 初始化枚举类型
             "create_time": deal.createTime,
             "counter_broker_id": deal.counterBrokerID if deal.HasField('counterBrokerID') else NoneDataValue,
             "counter_broker_name": deal.counterBrokerName if deal.HasField('counterBrokerName') else NoneDataValue,
             "status": DealStatus.to_string2(deal.status) if deal.HasField("status") else NoneDataValue
@@ -577,15 +582,15 @@
         raw_order_list = rsp_pb.s2c.orderList
         order_list = [{
                       "code": merge_trd_mkt_stock_str(order.secMarket, order.code),
                       "stock_name": order.name,
                       "trd_side": TrdSide.to_string2(order.trdSide) if order.HasField('trdSide') else 'N/A',# 初始化枚举类型
                       "order_type": OrderType.to_string2(order.orderType) if order.HasField('orderType') else 'N/A',# 初始化枚举类型
                       "order_status": OrderStatus.to_string2(order.orderStatus) if order.HasField('orderStatus') else 'N/A',# 初始化枚举类型
-                      "order_id": str(order.orderID),
+                      "order_id": str(order.orderIDEx),
                       "qty": order.qty,
                       "price": order.price,
                       "create_time": order.createTime,
                       "updated_time": order.updateTime,
                       "dealt_qty": order.fillQty,
                       "dealt_avg_price": order.fillAvgPrice,
                       "last_err_msg": order.lastErrMsg,
@@ -597,14 +602,59 @@
                       "trail_value": order.trailValue if order.HasField("trailValue") else 'N/A',
                       "trail_spread": order.trailSpread if order.HasField("trailSpread") else 'N/A',
                       "currency": Currency.to_string2(order.currency) if order.HasField('currency') else NoneDataValue,
                       } for order in raw_order_list]
         return RET_OK, "", order_list
 
 
+class OrderFeeQuery:
+    """Class for querying order fee"""
+
+    def __init__(self):
+        pass
+
+    @classmethod
+    def pack_req(cls, order_id_list, trd_env, acc_id, trd_mkt, conn_id):
+
+        from ..common.pb.Trd_GetOrderFee_pb2 import Request
+        req = Request()
+        _, req.c2s.header.trdEnv = TrdEnv.to_number(trd_env)
+        req.c2s.header.accID = acc_id
+        _, req.c2s.header.trdMarket = TrdMarket.to_number(trd_mkt)
+
+        if order_id_list:
+            for order_id in order_id_list:
+                req.c2s.orderIdExList.append(str(order_id))
+
+        return pack_pb_req(req, ProtoId.Trd_GetOrderFee, conn_id)
+
+    @classmethod
+    def get_fee_details(cls, order_fee):
+        fee_details = []
+        for fee_item in order_fee.feeList:
+            fee_details.append((str(fee_item.title), fee_item.value))
+        return fee_details
+
+    @classmethod
+    def unpack_rsp(cls, rsp_pb):
+
+        if rsp_pb.retType != RET_OK:
+            return RET_ERROR, rsp_pb.retMsg, None
+
+        none_data = 'N/A'
+        raw_order_fee_list = rsp_pb.s2c.orderFeeList
+
+        order_fee_list = [{
+            "order_id": str(order_fee.orderIDEx),
+            "fee_amount": order_fee.feeAmount if order_fee.HasField('feeAmount') else none_data,
+            "fee_details": cls.get_fee_details(order_fee),
+        } for order_fee in raw_order_fee_list]
+        return RET_OK, "", order_fee_list
+
+
 class HistoryDealListQuery:
     """Class for """
 
     def __init__(self):
         pass
 
     @classmethod
@@ -631,15 +681,15 @@
             return RET_ERROR, rsp_pb.retMsg, None
 
         raw_deal_list = rsp_pb.s2c.orderFillList
         deal_list = [{
                     "code": merge_trd_mkt_stock_str(deal.secMarket, deal.code),
                     "stock_name": deal.name,
                     "deal_id": deal.fillID,
-                    "order_id": str(deal.orderID) if deal.HasField('orderID') else "",
+                    "order_id": str(deal.orderIDEx) if deal.HasField('orderIDEx') else "",
                     "qty": deal.qty,
                     "price": deal.price,
                     "trd_side": TrdSide.to_string2(deal.trdSide) if deal.HasField('trdSide') else 'N/A',# 初始化枚举类型
                     "create_time": deal.createTime,
                     "counter_broker_id": deal.counterBrokerID if deal.HasField('counterBrokerID') else "",
                     "counter_broker_name": deal.counterBrokerName,
                     "status": DealStatus.to_string2(deal.status) if deal.HasField('status') else 'N/A'# 初始化枚举类型
@@ -696,15 +746,15 @@
         req.c2s.header.accID = acc_id
         _, req.c2s.header.trdMarket = TrdMarket.to_number(trd_mkt)
 
         _, req.c2s.orderType = OrderType.to_number(order_type)
         req.c2s.code = code
         req.c2s.price = price
         if order_id is not None:
-            req.c2s.orderID = int(order_id)
+            req.c2s.orderIDEx = order_id
         if adjust_limit == 0:
             req.c2s.adjustPrice = False
         else:
             req.c2s.adjustPrice = True
             req.c2s.adjustSideAndLimit = adjust_limit
 
         r, proto_qot_mkt = Market.to_number(sec_mkt_str)
```

### Comparing `futu-api-8.1.4108/futu/trade/trade_response_handler.py` & `futu-api-8.2.4208/futu/trade/trade_response_handler.py`

 * *Files identical despite different names*

### Comparing `futu-api-8.1.4108/futu_api.egg-info/PKG-INFO` & `futu-api-8.2.4208/futu_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futu-api
-Version: 8.1.4108
+Version: 8.2.4208
 Summary: Futu Quantitative Trading API
 Home-page: https://github.com/FutunnOpen/py-futu-api
 Author: Futu, Inc.
 Author-email: ftdev@futunn.com
 License: Apache License 2.0
 Keywords: Futu HK/US Stock Quant Trading API
 Platform: UNKNOWN
```

### Comparing `futu-api-8.1.4108/futu_api.egg-info/SOURCES.txt` & `futu-api-8.2.4208/futu_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 futu/common/pb/Trd_Common_pb2.py
 futu/common/pb/Trd_GetAccList_pb2.py
 futu/common/pb/Trd_GetFunds_pb2.py
 futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py
 futu/common/pb/Trd_GetHistoryOrderList_pb2.py
 futu/common/pb/Trd_GetMarginRatio_pb2.py
 futu/common/pb/Trd_GetMaxTrdQtys_pb2.py
+futu/common/pb/Trd_GetOrderFee_pb2.py
 futu/common/pb/Trd_GetOrderFillList_pb2.py
 futu/common/pb/Trd_GetOrderList_pb2.py
 futu/common/pb/Trd_GetPositionList_pb2.py
 futu/common/pb/Trd_ModifyOrder_pb2.py
 futu/common/pb/Trd_Notify_pb2.py
 futu/common/pb/Trd_PlaceOrder_pb2.py
 futu/common/pb/Trd_ReconfirmOrder_pb2.py
```

### Comparing `futu-api-8.1.4108/setup.py` & `futu-api-8.2.4208/setup.py`

 * *Files identical despite different names*

